# Tool-Calling — Worked Example (Neuron Kernel)

Concrete traces for the tool layer described in [`oneri.md`](oneri.md) §2.
Extended thinking is **on** so the reasoning is visible; the only roles on the
wire are `user` and `assistant` (a tool result is a `user` message carrying a
`tool_result` block — there is no separate "tool" role).

Every example below is built on evidence from the 21 site reviews:

| Example | Fixes the gap observed in |
|---|---|
| A · Natural-language search + commute | 16 Beercocks: 515 results, filters only, free sentence → "Couldn't find the address" |
| B · Country-aware stamp duty | 06 Property Connections: English SDLT shown on a Scottish property |
| C · Grounding & handoff | 01 Kinetic: title says 2 beds, material info says 3 — the model must not pick one |

---

## 0 · Request envelope

```json
{
  "model": "claude-opus-5",
  "max_tokens": 8000,
  "thinking": { "type": "adaptive", "display": "summarized" },
  "output_config": { "effort": "medium" },
  "system": [
    {
      "type": "text",
      "text": "You are the property assistant for Beercocks (tenant_id: beercocks). Rules:\n1. Never state a fact about a property unless it came back from a tool in this conversation. No prices, no bedroom counts, no distances from memory.\n2. Always name the source field or tool for every factual claim.\n3. If a field is missing, contradictory, or the question needs a human, say so and hand off. Do not guess.\n4. Stamp duty is country-dependent: England/NI = SDLT, Scotland = LBTT, Wales = LTT. Read the country from the property record, never assume.\n5. Valuation output is an explanation, not advice: describe what drives the estimate and state that an in-person appraisal is required.",
      "cache_control": { "type": "ephemeral" }
    }
  ],
  "tools": [ /* see §1 */ ],
  "messages": [ /* see §2 */ ]
}
```

The system block and the tool list are the stable prefix, so they carry the
cache breakpoint; the volatile per-user query goes after it.

---

## 1 · Tool definitions

Four of the ten tools from the contract in `oneri.md` — enough to run the
traces below. `strict: true` guarantees the arguments validate exactly, which
is what makes NL search regression-testable.

```json
[
  {
    "name": "search_properties",
    "description": "Search the tenant's live listings. This is the ONLY way to find properties; never answer from memory. Returns matching listings with id, price, bedrooms, type, postcode. If a search returns 0 results, relax the single tightest numeric criterion by ~10% and search again, then tell the user exactly what you relaxed.",
    "strict": true,
    "input_schema": {
      "type": "object",
      "properties": {
        "location":       { "type": "string", "description": "Town, area or postcode district as written by the user, e.g. 'Hessle' or 'HU13'" },
        "transaction":    { "type": "string", "enum": ["sale", "rent"] },
        "min_bedrooms":   { "type": "integer" },
        "max_price":      { "type": "integer", "description": "GBP, whole pounds" },
        "property_types": { "type": "array", "items": { "type": "string", "enum": ["detached", "semi-detached", "terraced", "flat", "bungalow"] } },
        "must_have":      { "type": "array", "items": { "type": "string", "enum": ["garden", "garage", "parking", "chain-free", "new-build"] } },
        "sort":           { "type": "string", "enum": ["relevance", "price_asc", "price_desc", "newest"] }
      },
      "required": ["location", "transaction"],
      "additionalProperties": false
    }
  },
  {
    "name": "get_property",
    "description": "Full record for one listing: description, features, EPC, floor plan, material information, country. Every answer about a specific property must be grounded in this record.",
    "strict": true,
    "input_schema": {
      "type": "object",
      "properties": { "property_id": { "type": "string" } },
      "required": ["property_id"],
      "additionalProperties": false
    }
  },
  {
    "name": "get_commute",
    "description": "Real travel time between a property and a destination. Use this instead of the radius filter whenever the user names a place they need to reach.",
    "strict": true,
    "input_schema": {
      "type": "object",
      "properties": {
        "property_id":  { "type": "string" },
        "destination":  { "type": "string", "description": "Free-text destination, e.g. 'Hull Royal Infirmary'" },
        "mode":         { "type": "string", "enum": ["driving", "transit", "cycling", "walking"] },
        "arrive_by":    { "type": "string", "description": "Local time, HH:MM, for peak-hour accuracy" }
      },
      "required": ["property_id", "destination", "mode"],
      "additionalProperties": false
    }
  },
  {
    "name": "calc_stamp_duty",
    "description": "Country-aware purchase tax. Pass the country from the property record: England/Northern Ireland = SDLT, Scotland = LBTT, Wales = LTT. Never compute the tax yourself.",
    "strict": true,
    "input_schema": {
      "type": "object",
      "properties": {
        "price":        { "type": "integer" },
        "country":      { "type": "string", "enum": ["england", "northern-ireland", "scotland", "wales"] },
        "buyer_status": { "type": "string", "enum": ["first-time", "home-mover", "additional-property"] }
      },
      "required": ["price", "country", "buyer_status"],
      "additionalProperties": false
    }
  },
  {
    "name": "handoff_to_agent",
    "description": "Hand the conversation to a human negotiator. Use whenever the answer is not in the listing record, the record contradicts itself, or the user asks for advice rather than information. This is the default when unsure.",
    "strict": true,
    "input_schema": {
      "type": "object",
      "properties": {
        "reason":         { "type": "string" },
        "context":        { "type": "string", "description": "What the user asked and what was already established" },
        "property_id":    { "type": "string" },
        "urgency":        { "type": "string", "enum": ["normal", "high"] }
      },
      "required": ["reason", "context"],
      "additionalProperties": false
    }
  },
  {
    "name": "flag_data_issue",
    "description": "Report a contradiction or gap in a listing record to the branch's data-quality queue. Fire this in addition to answering — it is not a substitute for handing off.",
    "strict": true,
    "input_schema": {
      "type": "object",
      "properties": {
        "property_id": { "type": "string" },
        "field":       { "type": "string" },
        "issue":       { "type": "string" }
      },
      "required": ["property_id", "field", "issue"],
      "additionalProperties": false
    }
  }
]
```

---

## 2 · Example A — natural-language search, empty result, commute

Today this sentence returns *"Couldn't find the address"* on 16 Beercocks.

### Turn 1 — `user`

```json
{
  "role": "user",
  "content": "Looking for a 3 bed semi in Hessle with a garden, up to £250k. I start at Hull Royal Infirmary at 8am so the drive matters."
}
```

### Turn 2 — `assistant`

```json
{
  "role": "assistant",
  "content": [
    {
      "type": "thinking",
      "thinking": "One sentence, five constraints: location Hessle, 3 bedrooms, semi-detached, garden, max £250,000 — plus a commute requirement to Hull Royal Infirmary arriving 08:00 by car. The commute is not a search filter; it is a per-property lookup, so it has to wait until I have candidate ids. Search first, commute second. I must not estimate the drive myself and I must not guess what is on the market — both have to come from tools.",
      "signature": "ErUBCkYIBRgCKkD…"
    },
    {
      "type": "text",
      "text": "Let me search Hessle first, then check the drive for whatever comes back."
    },
    {
      "type": "tool_use",
      "id": "toolu_01A7Hs3",
      "name": "search_properties",
      "input": {
        "location": "Hessle",
        "transaction": "sale",
        "min_bedrooms": 3,
        "max_price": 250000,
        "property_types": ["semi-detached"],
        "must_have": ["garden"],
        "sort": "relevance"
      }
    }
  ]
}
```

### Turn 3 — `user` (tool result)

```json
{
  "role": "user",
  "content": [
    {
      "type": "tool_result",
      "tool_use_id": "toolu_01A7Hs3",
      "content": "{\"total\": 0, \"results\": [], \"applied_filters\": {\"location\": \"Hessle\", \"min_bedrooms\": 3, \"max_price\": 250000, \"property_types\": [\"semi-detached\"], \"must_have\": [\"garden\"]}}"
    }
  ]
}
```

### Turn 4 — `assistant`

```json
{
  "role": "assistant",
  "content": [
    {
      "type": "thinking",
      "thinking": "Zero results. The wrong move is to show nothing, and the worse move is to invent a listing. Which constraint is tightest? Bedrooms and 'semi-detached' are categorical — dropping them changes what the user asked for. Price is the one numeric knob, so raise £250k to £275k (+10%) and keep everything else identical. I will state the relaxation explicitly in the final answer so the user is never shown results they did not ask for without knowing why.",
      "signature": "ErUBCkYIBRgCKkD…"
    },
    {
      "type": "tool_use",
      "id": "toolu_02Kq9Lm",
      "name": "search_properties",
      "input": {
        "location": "Hessle",
        "transaction": "sale",
        "min_bedrooms": 3,
        "max_price": 275000,
        "property_types": ["semi-detached"],
        "must_have": ["garden"],
        "sort": "price_asc"
      }
    }
  ]
}
```

### Turn 5 — `user` (tool result)

```json
{
  "role": "user",
  "content": [
    {
      "type": "tool_result",
      "tool_use_id": "toolu_02Kq9Lm",
      "content": "{\"total\": 2, \"results\": [{\"id\": \"bcx-4471\", \"address\": \"Southfield, Hessle HU13\", \"price\": 259950, \"bedrooms\": 3, \"type\": \"semi-detached\", \"features\": [\"rear garden\", \"driveway\"], \"country\": \"england\"}, {\"id\": \"bcx-4508\", \"address\": \"Tranby Lane, Hessle HU13\", \"price\": 272500, \"bedrooms\": 3, \"type\": \"semi-detached\", \"features\": [\"south-facing garden\", \"garage\"], \"country\": \"england\"}]}"
    }
  ]
}
```

### Turn 6 — `assistant` (parallel tool use)

Two `tool_use` blocks in **one** assistant message — the client executes them
concurrently and must return **both** results in a **single** `user` message.

```json
{
  "role": "assistant",
  "content": [
    {
      "type": "thinking",
      "thinking": "Two candidates, both England, both with a garden. Now the part the current site cannot do at all: the actual drive. Both commute lookups are independent, so I issue them in the same turn rather than serially. Arrive-by 08:00 matters — an off-peak number would be misleading for a hospital shift start.",
      "signature": "ErUBCkYIBRgCKkD…"
    },
    {
      "type": "tool_use",
      "id": "toolu_03Rt2Pv",
      "name": "get_commute",
      "input": { "property_id": "bcx-4471", "destination": "Hull Royal Infirmary", "mode": "driving", "arrive_by": "08:00" }
    },
    {
      "type": "tool_use",
      "id": "toolu_04Wn8Cd",
      "name": "get_commute",
      "input": { "property_id": "bcx-4508", "destination": "Hull Royal Infirmary", "mode": "driving", "arrive_by": "08:00" }
    }
  ]
}
```

### Turn 7 — `user` (both results, one message)

```json
{
  "role": "user",
  "content": [
    {
      "type": "tool_result",
      "tool_use_id": "toolu_03Rt2Pv",
      "content": "{\"property_id\": \"bcx-4471\", \"destination\": \"Hull Royal Infirmary\", \"mode\": \"driving\", \"distance_miles\": 4.8, \"duration_min_offpeak\": 13, \"duration_min_peak_arrive_0800\": 24, \"route\": \"A1105 / Anlaby Road\"}"
    },
    {
      "type": "tool_result",
      "tool_use_id": "toolu_04Wn8Cd",
      "content": "{\"property_id\": \"bcx-4508\", \"destination\": \"Hull Royal Infirmary\", \"mode\": \"driving\", \"distance_miles\": 6.1, \"duration_min_offpeak\": 16, \"duration_min_peak_arrive_0800\": 31, \"route\": \"A164 / A63\"}"
    }
  ]
}
```

### Turn 8 — `assistant` (final)

```json
{
  "role": "assistant",
  "content": [
    {
      "type": "thinking",
      "thinking": "Everything I am about to say is now sourced: prices and features from search_properties, drive times from get_commute. Two things must be explicit — that I widened the budget, and that 24 and 31 minutes are peak figures for an 08:00 arrival, not the off-peak numbers a map would show. No recommendation on which to buy; that is the negotiator's job.",
      "signature": "ErUBCkYIBRgCKkD…"
    },
    {
      "type": "text",
      "text": "Nothing in Hessle matched all of it under £250,000, so I widened the budget to £275,000 and kept everything else the same — 3 bedrooms, semi-detached, garden:\n\n**Southfield, Hessle HU13 — £259,950**\nRear garden, driveway. Drive to Hull Royal Infirmary: 4.8 miles, about **24 minutes** arriving at 8am (13 off-peak), via Anlaby Road.\n\n**Tranby Lane, Hessle HU13 — £272,500**\nSouth-facing garden, garage. Drive: 6.1 miles, about **31 minutes** arriving at 8am (16 off-peak), via the A164/A63.\n\nBoth times are peak-hour estimates for an 08:00 arrival, not off-peak. Want me to hold the budget at £250,000 and widen the area to Anlaby and Kirk Ella instead, or book a viewing on either of these?"
    }
  ]
}
```

**What this replaces:** free-sentence input parsed into validated JSON instead
of `Couldn't find the address`; an empty result answered with a stated
relaxation instead of a dead end; and a real 08:00 drive time instead of the
radius filter.

---

## 3 · Example B — country-aware stamp duty

Site 06 shows English SDLT on a Scottish property. The tool signature makes
that class of bug unreachable: `country` is required and comes from the record.

### Turn 1 — `user`

```json
{ "role": "user", "content": "What's the stamp duty on the Edinburgh flat at £310,000? It'd be our first place." }
```

### Turn 2 — `assistant`

```json
{
  "role": "assistant",
  "content": [
    {
      "type": "thinking",
      "thinking": "'Edinburgh' in the user's sentence is a hint, not a source. The country must come from the listing record, so get_property first, calc_stamp_duty second — I cannot fill in the required 'country' argument honestly until the record answers it. And I never compute the bands myself: Scotland is LBTT with its own first-time-buyer relief, and hardcoding that is exactly how site 06 ended up quoting the wrong tax.",
      "signature": "ErUBCkYIBRgCKkD…"
    },
    {
      "type": "tool_use",
      "id": "toolu_05Ed1Nb",
      "name": "get_property",
      "input": { "property_id": "pc-2210" }
    }
  ]
}
```

### Turn 3 — `user` (tool result)

```json
{
  "role": "user",
  "content": [
    {
      "type": "tool_result",
      "tool_use_id": "toolu_05Ed1Nb",
      "content": "{\"id\": \"pc-2210\", \"address\": \"Leith Walk, Edinburgh EH6\", \"price\": 310000, \"bedrooms\": 2, \"type\": \"flat\", \"tenure\": \"leasehold\", \"country\": \"scotland\", \"epc\": {\"current\": \"C\", \"potential\": \"B\"}}"
    }
  ]
}
```

### Turn 4 — `assistant`

```json
{
  "role": "assistant",
  "content": [
    {
      "type": "thinking",
      "thinking": "country = scotland, confirmed from the record. So LBTT, not SDLT, and first-time buyer status from the user's own words.",
      "signature": "ErUBCkYIBRgCKkD…"
    },
    {
      "type": "tool_use",
      "id": "toolu_06Lb4Tx",
      "name": "calc_stamp_duty",
      "input": { "price": 310000, "country": "scotland", "buyer_status": "first-time" }
    }
  ]
}
```

### Turn 5 — `user` (tool result)

```json
{
  "role": "user",
  "content": [
    {
      "type": "tool_result",
      "tool_use_id": "toolu_06Lb4Tx",
      "content": "{\"tax\": \"LBTT\", \"jurisdiction\": \"scotland\", \"total_due\": 3100, \"first_time_buyer_relief_applied\": true, \"bands\": [{\"range\": \"£0–£175,000\", \"rate\": \"0% (FTB relief)\", \"due\": 0}, {\"range\": \"£175,000–£250,000\", \"rate\": \"2%\", \"due\": 1500}, {\"range\": \"£250,000–£310,000\", \"rate\": \"5%\", \"due\": 3000}], \"note\": \"Illustration only. Confirm with your solicitor.\"}"
    }
  ]
}
```

### Turn 6 — `assistant` (final)

```json
{
  "role": "assistant",
  "content": [
    {
      "type": "text",
      "text": "That one is in Scotland, so it's **LBTT**, not English stamp duty — and as first-time buyers you get the relief:\n\n- £0–£175,000 — 0% (first-time buyer relief) → £0\n- £175,000–£250,000 — 2% → £1,500\n- £250,000–£310,000 — 5% → £3,000\n\n**Total: £3,100.**\n\nThis is an illustration to budget against, not a formal calculation — your solicitor confirms the final figure at offer stage."
    }
  ]
}
```

Note the shape of the fix: the model is not trusted to *know* the tax regime,
only to *route* to the right one — and the schema will not let it route without
reading the record.

---

## 4 · Example C — grounding limit and handoff

01 Kinetic has a listing whose title says 2 bedrooms and whose material
information says 3. This is what the model must do with it.

### Turn 1 — `user`

```json
{ "role": "user", "content": "Is the Marlborough Avenue house 2 or 3 bedrooms, and has the boiler been replaced recently?" }
```

### Turn 2 — `assistant`

```json
{
  "role": "assistant",
  "content": [
    {
      "type": "thinking",
      "thinking": "Two questions. Both need the record — pull it before saying anything.",
      "signature": "ErUBCkYIBRgCKkD…"
    },
    {
      "type": "tool_use",
      "id": "toolu_07Mv6Kj",
      "name": "get_property",
      "input": { "property_id": "kin-1180" }
    }
  ]
}
```

### Turn 3 — `user` (tool result)

```json
{
  "role": "user",
  "content": [
    {
      "type": "tool_result",
      "tool_use_id": "toolu_07Mv6Kj",
      "content": "{\"id\": \"kin-1180\", \"address\": \"Marlborough Avenue, Hull HU5\", \"title\": \"2 Bedroom Terraced House\", \"price\": 168000, \"material_information\": {\"bedrooms\": 3, \"council_tax_band\": \"A\", \"tenure\": \"freehold\"}, \"description\": \"…generous first floor accommodation…\", \"heating\": null, \"country\": \"england\"}"
    }
  ]
}
```

### Turn 4 — `assistant` (parallel: flag + handoff)

```json
{
  "role": "assistant",
  "content": [
    {
      "type": "thinking",
      "thinking": "The record contradicts itself: title says 2 bedrooms, material information says 3. Picking either one would be a misdescription, and material information is the legally weightier field, which makes guessing worse, not safer. So: flag the contradiction to the data-quality queue AND hand off to a human — the flag fixes the listing, the handoff answers this buyer. The boiler question is separate: 'heating' is null, meaning the record has no answer, not that there is no boiler. Absence of data is never a negative answer.",
      "signature": "ErUBCkYIBRgCKkD…"
    },
    {
      "type": "tool_use",
      "id": "toolu_08Fg3Qz",
      "name": "flag_data_issue",
      "input": {
        "property_id": "kin-1180",
        "field": "bedrooms",
        "issue": "Title says '2 Bedroom Terraced House'; material_information.bedrooms = 3. Contradiction is buyer-visible and was raised in a live chat."
      }
    },
    {
      "type": "tool_use",
      "id": "toolu_09Hy7Rw",
      "name": "handoff_to_agent",
      "input": {
        "reason": "Contradictory bedroom count in the listing record, plus a heating question the record does not cover.",
        "context": "Buyer asked whether kin-1180 (Marlborough Avenue) is 2 or 3 bedrooms and whether the boiler was replaced recently. Title and material information disagree; the heating field is empty.",
        "property_id": "kin-1180",
        "urgency": "normal"
      }
    }
  ]
}
```

### Turn 5 — `user` (both results)

```json
{
  "role": "user",
  "content": [
    { "type": "tool_result", "tool_use_id": "toolu_08Fg3Qz", "content": "{\"status\": \"queued\", \"ticket\": \"dq-8842\", \"branch\": \"hull\"}" },
    { "type": "tool_result", "tool_use_id": "toolu_09Hy7Rw", "content": "{\"status\": \"assigned\", \"agent\": \"Hull sales team\", \"callback_window\": \"today, before 17:30\"}" }
  ]
}
```

### Turn 6 — `assistant` (final)

```json
{
  "role": "assistant",
  "content": [
    {
      "type": "text",
      "text": "I'd rather not guess on either of those.\n\n**Bedrooms:** the listing is inconsistent — the title says 2 bedrooms, the material information section says 3. I've flagged it for correction rather than pick one.\n\n**Boiler:** the heating details aren't recorded on this listing, so I have nothing to answer from. That's a gap in the record, not a 'no'.\n\nThe Hull team has both questions and will come back to you before 17:30 today. Anything else about the property I can check in the meantime?"
    }
  ]
}
```

---

## 5 · Why this shape

| Property | How it is achieved |
|---|---|
| **Hallucination surface is small** | The model chooses *which* tool and *what* arguments; it never supplies facts. Every price, drive time and tax figure in the traces above came back from a tool call. |
| **It is testable** | The output of turn 2 in Example A is JSON, not prose. A golden set of ~200 real queries from the 21 sites turns every prompt change into a regression run — compare emitted arguments, not free text. |
| **Bug classes become unreachable** | `calc_stamp_duty` cannot be called without `country`, and `country` only exists on the record. The site-06 bug has nowhere to live. |
| **Missing data has a defined behaviour** | `null` field → `handoff_to_agent`, contradiction → `flag_data_issue` + handoff. "I don't know" is a designed output, not a failure. |
| **Every turn is training data** | Each trace, plus whatever the negotiator corrects afterwards, is a labelled example. This is where the fine-tune dataset in `oneri.md` §5 comes from. |

**Wire-format reminders**

- Thinking blocks are echoed back **unchanged** (signature included) on every
  follow-up request in the same conversation; strip them and the model loses
  its own reasoning chain.
- Multiple `tool_use` blocks in one assistant message must be answered by
  **one** user message containing **all** the `tool_result` blocks. Splitting
  them across messages quietly teaches the model to stop calling tools in
  parallel.
- A failed tool returns a `tool_result` with `"is_error": true` — it is still
  returned, never dropped.
- `tool_use_id` must match the `id` of the block it answers, exactly.
