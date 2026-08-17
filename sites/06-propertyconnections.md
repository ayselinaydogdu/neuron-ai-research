# 06 · propertyconnections.uk.com

**URL:** https://propertyconnections.uk.com/
**Group / Grup:** B

---

## English

This site is reviewed independently by 4 people across 4 rounds.

| Round | Reviewer | Status |
|---|---|---|
| 1 | Ayselin | Done |
| 2 | Görkem | Done |
| 3 | Berkay | Not done |
| 4 | Yasemin | Done |

> Fill in only your own round block; don't edit anyone else's.
> Write short, concrete sentences (not "yes/no" — say what it is).
> What to check: ../checklist.md · Terms: ../info/ai-feature-glossary.md

### Round 1 — Ayselin

## Search

- Traditional filter-based search is available (price, bedrooms, property type, etc.).
- Natural Language Search is not available. Queries such as "3 bedroom house under £300k near schools" are not supported.
- Smart query interpretation (e.g., typo correction, synonym recognition, or AI-assisted result refinement) is not available.
- Saved searches or property alerts are not available.

## Property Details

- Property descriptions are detailed but lengthy; an AI-generated Property Summary is not available.
- Users cannot ask free-form questions about a property (AI Property Q&A is not available).
- Lifestyle recommendations such as "Ideal for..." are not provided.
- AI-powered Property Highlights, Property Comparison, and personalized similar property recommendations are not available.
- Property locations are displayed using Google Maps; however, AI-powered Area Insights and Commute Insights are not available.
- EPC certificates and Floor Plans are provided, but they are not explained or summarized by AI.

## Valuation

- Instant Valuation and a Mortgage Calculator are available.
- The Mortgage Calculator performs calculations only and does not provide AI-powered financial advice or recommendations.
- AI-generated valuation explanations or personalized valuation insights are not available.

## Contact

- A contact form and property viewing request are available.
- No AI chatbot or AI-powered customer assistant is provided.
- Users cannot ask natural language questions about a property.
- AI-powered lead qualification or visitor prioritization is not available.
- AI-assisted viewing scheduling and out-of-hours automated responses are not available.

## Technical / General

- The website has a modern and user-friendly interface.
- Google Maps integration is available.
- Search, filters, and contact forms are usable on mobile devices.
- No obvious AI service or Neuron API integrations were observed during the inspection.
- Core real estate features (search, filtering, valuation, and mortgage calculator) function effectively.

**Status:** Done

### Round 2 — Görkem

**Search:**
- I agree with Ayselin's Round 1 (filter-only, no natural language) and can now add the platform context: having seen the whole Neuron group, this isn't a Property Connections choice — it's the untouched platform default. Buy/Rent toggle on the homepage; results page limited to price interval, min–max beds and radius 0–40mi; no type, no keyword, no map, list-only, sort = Suggested/price/date. Scottish agency (Livingston/Bathgate, SC company).
- **AI opportunity (platform-level):** natural-language search mapped onto the shared filter API — reusable across every tenant, not just this one.

**Listing Detail:**
- Confirmed the same template as Group A: bullet key-features + long hand-written narrative, floorplan, sometimes video, no 360, no AI summary, no ask-a-question, area info as prose, thin map tab. The "similar" block is just "our latest properties" — newest-in, not matched to the viewer.
- **AI opportunities:** listing summary + grounded Q&A, and a genuinely personalised "similar homes" using listing embeddings instead of latest-in.

**Valuation:**
- Instant tool (`valuation.propertyconnections.uk.com`) + in-person. Same as the group: it promises an "immediate estimate" but is really a gated lead form — collects details then follows up. The on-screen wording oversells what actually happens (I didn't submit it).

**Contact:**
- Form + phone (01506) + email; no chat, no out-of-hours, no lead qualification — the same generic single form for everyone.
- **AI opportunity:** a lightweight out-of-hours assistant / lead qualifier grounded in this tenant's own stock + FAQs would at least acknowledge and triage enquiries when the office is closed.

**Technical / General:**
- Neuron/Iceberg, Vercel, S3 CDN. Trust is good (named-agent reviews — Kevin/Chris/Sarah, SC company reg, redress scheme).
- Telling detail: the "A Different Kind Of Estate Agency" tagline is **identical to Jacksons (08)** — clear evidence of shared template copy across tenants, which reinforces that AI features should be built once at platform level, not per agency.

**Status:** Done

### Round 3 — Berkay

**Search:**
-

**Listing Detail:**
-

**Valuation:**
-

**Contact:**
-

**Technical / General:**
-

**Status:** Not done

### Round 4 — Yasemin

## **Search:**

- **Natural Language Search:** **No** — "3 bed near a school under £250k in Bathgate" returns "Couldn't find the address". Identical failure mode to Property Cloud. (SS-03)
- **Smart Suggestions / Query Interpretation:** **Partial** — "bathgt" still resolves to Bathgate, but the dropdown offers "Bathgate Road, London", "Bathgate, Eyemouth" and "Bathgate Academy" — Google Places geocoding, confirmed by `place_id: ChIJF3gcD1rYh0gR6_6GWy6EAhw` in the URL. It corrects the address, not the property intent — and it will happily send a West Lothian buyer to London. (SS-01, SS-02, SS-05)
- **Saved Search / Alerts:** **Yes** — "Setup Heads Up Alert" sits directly on the results header. Criteria-based, rule-driven; no AI interpretation. (SS-05, SS-09)
- **Additional note:** Same unbacked personalisation pattern as Property Cloud — **"SUGGESTED"** sort, **"100% MATCH"** badges on every card, and **"HAVE YOU LOGGED IN?"** sitting right beside them. Logged out, every one of the 27 results is a 100% match. (SS-05)
- **Additional note:** Filters are conventional dropdowns — Bathrooms, Reception, Include SSTC/Under Offer, Retirement Homes, Shared Ownership, Investment Property, Must Haves, Property Type tiles. There is an **"Other / Advanced"** expander, which Property Cloud's build does not surface. (SS-04)

## **Listing Detail:**

- **Property Summary (AI Summary):** **No** — Description is hand-written prose, no bullet summary at the top.
- **Property Q&A:** **No** — "Make an Enquiry" is a form, not a question channel.
- **Property Highlights:** **Partial** — A Features list exists, entered by hand in all-caps at listing creation ("RARELY AVAILABLE IMMACULATE AND SPACIOUS DETACHED BUNGALOW", "CLOSE TO AMENITIES"). Not AI-extracted, and vague enough that it adds little. (SS-07)
- **Lifestyle / "Ideal for..." Matching:** **Partial** — Phrases like "comfortable and convenient lifestyle" and "friendly and respected local community" sit inside the free text. No structured matching.
- **Property Comparison:** **No** — No compare or favourites function.
- **Similar Listing Suggestions:** **No** — The bottom of the page carries alerts, guides and "Thinking of selling?" CTAs instead.
- **Area Insights:** **No** — A Map tab exists, but the points are Google's own data. No neighbourhood, school or crime layer.
- **Commute Insights:** **No** — Travel time is never calculated.
- **Document Explanation (EPC / Floor Plan / Home Report):** **No** — **This is the biggest gap on this site.** A prominent "GET HOME REPORT" button downloads the raw Scottish Home Report PDF — a document bundling a single survey, energy report and property questionnaire, typically 20–40 pages. It is handed over completely unsummarised. Floor plans and EPC are images only. (SS-06)
- **Mortgage Calculator:** **Yes** — Present on the listing page, pre-filled with the asking price, deposit (10% = £28,000), 6.01% interest and 25-year term, returning "Monthly repayments: £1,625" live. Functional but purely arithmetic — no affordability commentary, no rate sourcing, no explanation. (SS-08)
- **Stamp Duty Calculator:** **Yes — but likely mislabelled.** ⚠️ The property is in Armadale, West Lothian. Scotland does not levy Stamp Duty; it levies **LBTT** (plus ADS on additional homes), with different bands and thresholds. The tool is titled "Stamp Duty Calculator" with an "I am... / Buying my first home" selector. Whether the underlying rates are LBTT or English SDLT needs confirming by running it and comparing to the LBTT bands — but either way, the label is wrong for a Scottish agency and gives buyers the wrong mental model. (SS-08)
- **Additional note:** The listing carries a **Vimeo agent-presented video** ("23 Barlaw Gardens — Sharon Forrester") and a **Matterport virtual tour**. Rich media is genuinely strong here; nothing sits on top of it.
- **Additional note:** **"Offers Over" pricing with no offer guidance.** Every listing is priced "Offers Over £X" — the Scottish norm — yet nothing on the site tells a buyer what a realistic offer looks like, what similar homes closed at, or how far over the guide typically goes. A clear, market-specific AI opportunity that has no equivalent in the English sites.

## **Valuation:**

- **Instant Valuation:** **Yes — third-party, same as Property Cloud.** Hosted at `valuation.propertyconnections.uk.com/home/4076` and marked **"Powered by The ValPal Network"**. Inputs: postcode → Find Address, Number of Bedrooms, Property Type, Submit. Visually disconnected from the main site, and it fires its own cookie consent banner. (SS-10)
- **AI Valuation Explanation:** **No** — No reasoning, no comparables, no personalisation.
- **Additional note — marketing contradiction:** The homepage sells this tool as **"quick and accurate"** and **"in seconds"**. The same ValPal tool on Property Cloud is advertised by that agency as **"Up to 60% accurate"**. Same engine, opposite claims — worth flagging as a platform-level messaging problem.
- **Additional note:** The in-person route (`/valuations`) is a plain lead form — salutation, name, email, mobile, and the property address as a **free-text box with no postcode lookup**, weaker than the postcode-search version on Property Cloud. No calendar, no slot selection. (SS-11)

## **Contact / Lead:**

- **AI Chat Assistant / Chatbot:** **No** — No widget on any page. **But the page source again defines `.whatsapp-chatbot` with `--wa-green`, `--wa-header-bg`, `--wa-bubble-bg`, `--wa-chat-bg` and `--wa-input-bg`.** Second site in a row where Neuron ships the WhatsApp chatbot component and the agency has not enabled it. This is now a platform pattern, not a one-off. (SS-15)
- **Lead Qualification:** **Partial** — The Heads Up registration collects reason for buying, moving timeline, solicitors arranged, how they heard about the agency, and — one question more than Property Cloud — **"Do you need to sell the property you currently live in?"**. Genuinely useful chain data, collected into a static form with no branching or prioritisation. (SS-09)
- **Automated Appointment / Viewing Scheduling:** **No** — "Make an Enquiry" and the valuation form both submit requests.
- **Out-of-Hours Response:** **No — and this one contradicts the agency's own copy.** ⚠️ The homepage states: *"We're not a nine-to-five operation - we're here when you need us."* The Contact page publishes **Opening Hours: Monday–Friday 9:00–17:00, Saturday 9:00–14:00, Sunday CLOSED.** Outside those hours there is no chat, no WhatsApp, no automated reply — only a form. The promise and the published reality point in opposite directions, and an always-on assistant is exactly what would close that gap. (SS-12)
- **Additional note:** The contact form is single-type — first name, last name, mobile, email, a Buy/Sell/Rent/Let checkbox row, free-text message, consent checkbox. No branching on that selection. (SS-13)

## **Technical / General:**

- **SSR vs CSR:** **Hybrid, and different from Property Cloud.** The document is Nuxt-rendered (`/_nuxt/` bundles), but the results list is fetched client-side: Network shows **`filter?search_type=sales&is_website=...` returning 36.7 kB in 245 ms**, initiated by `Bt02TWCK.js`. On Property Cloud the listing set arrived inside the HTML. Same platform, different rendering path. (SS-14)
- **API calls:** Besides the filter call — `anonymous` from `ice.js` (Iceberg tracker), three `envelope/?sentry_version=7...` (Sentry), and a cached asset. **No AI/LLM service is contacted.** 7/158 requests, 326 kB transferred, finish 3.51 s. (SS-14)
- **Theme version:** Source loads `/common/css/neuron.css` plus `/theme3/css/propertyconnections/index.css`, alongside **Bootstrap, Owl Carousel and FontAwesome**. Property Cloud runs `theme4`. This agency is on an **older Neuron theme generation** — relevant context for why some components differ. (SS-15)
- **Iceberg traces:** `window.IcebergTracker` and `__akyaCookieStarted` in source; assets from `files.propertyconnections.neuronwebsites.co.uk` and `lifesycle-cdn.s3.eu-west-2.amazonaws.com`. (SS-15)
- **Mobile behaviour:** **Fine** — At 400px the search bar, price selectors, bed range and filters stack cleanly and remain usable. (SS-14)
- **Additional note — broken map:** ⚠️ The "Visit Us" Google map on the Contact page is centred on **Folkestone, Dymchurch, New Romney and Dungeness — the Kent coast in south-east England**, roughly 600 km from the agency's actual office at 80 North Bridge Street, Bathgate. A visitor trying to find the branch is sent to the wrong end of the country. Worth re-checking on a fresh load to rule out a transient failure, but as captured it is a live, user-facing fault. (SS-13)
- **Additional note:** Footer copyright reads **© 2025** while the site is live in 2026 — a small sign that static content is maintained by hand. (SS-16)

**Status:** Done

### Findings / Synthesis (filled once all 4 rounds are done)

- Commonly missing AI features: Natural-language search, AI listing summaries, Property Q&A, AI lead scoring, out-of-hours automated response.
- Standout opportunities: (1) Scotland-specific Home Report (20-40 page PDF) downloaded completely unsummarised. (2) "Offers Over" pricing model gives buyers no guidance. (3) Same ValPal tool marketed inconsistently across tenants.
- Disagreements / to verify: ✅ **Confirmed by Ayselin (live check, August 2026):** The "Visit Us" map on the Contact page still shows Folkestone/Dymchurch/New Romney/Dungeness/Lydd (Kent, England) — roughly 600km from the agency's actual Bathgate, West Lothian address. This is a persistent, unfixed live error, not transient. ✅ **Confirmed and clarified:** The Stamp Duty Calculator returns "From 16 December 2024: £15,150" on a £424,000 property — the "16 December 2024" reference date corresponds to an English SDLT threshold change, not a Scottish LBTT band. This strongly suggests the calculator is genuinely running SDLT logic (not LBTT) for a Scottish agency, which would produce materially incorrect figures for Scottish buyers — a real, functional bug beyond just mislabelling, worth flagging directly to the platform team. Homepage also states the instant valuation is "quick and accurate" — confirmed live, word-for-word — versus "Up to 60% accurate" for the same ValPal tool on 05 · Property Cloud.

---

## Türkçe

Bu siteyi 4 tur boyunca 4 farklı kişi bağımsız inceler.

| Tur | İnceleyen | Durum |
|---|---|---|
| 1 | Ayselin | Yapıldı |
| 2 | Görkem | Yapıldı |
| 3 | Berkay | Yapılmadı |
| 4 | Yasemin | Yapıldı |

> Sadece kendi tur bloğunuzu doldurun; başkasının bloğunu değiştirmeyin.
> Kısa, somut cümleler yazın ("Var/Yok" değil, ne olduğunu yazın).
> Neye bakılacağı: ../checklist.md · Terimler: ../info/ai-feature-glossary.md

### Tur 1 — Ayselin

## Arama

- Klasik filtre tabanlı arama mevcut (price, bedrooms, property type vb.).
- Doğal dil araması (Natural Language Search) bulunmuyor. "3 bedroom house under £300k near schools" gibi sorgular desteklenmiyor.
- Akıllı öneri / sorgu yorumlama (yazım hatası düzeltme, eş anlamlı anlama veya AI destekli sonuç iyileştirme) bulunmuyor.
- Kayıtlı arama veya otomatik ilan bildirimleri (Alerts) sunulmuyor.

## İlan Detay

- Property açıklamaları detaylı ancak oldukça uzun; AI destekli özet (Property Summary) bulunmuyor.
- Kullanıcı ilan hakkında soru soramıyor (AI Property Q&A yok).
- "Ideal for..." gibi yaşam tarzına yönelik öneriler bulunmuyor.
- AI destekli Property Highlights, Property Comparison ve kişiselleştirilmiş benzer ilan önerileri bulunmuyor.
- Google Maps ile konum gösteriliyor ancak AI destekli Commute Insights veya Area Insights sunulmuyor.
- EPC, Floor Plan gibi belgeler mevcut ancak AI tarafından açıklanmıyor.

## Değerleme

- Instant Valuation ve Mortgage Calculator mevcut.
- Mortgage Calculator yalnızca hesaplama yapıyor; AI destekli finansal yorum veya öneri sunmuyor.
- AI destekli valuation açıklamaları veya kişiselleştirilmiş öneriler bulunmuyor.

## İletişim

- İletişim formu ve viewing talebi mevcut.
- AI chatbot veya AI destekli müşteri asistanı bulunmuyor.
- Kullanıcı ilan hakkında doğal dilde soru soramıyor.
- AI destekli lead qualification (ön eleme/önceliklendirme) bulunmuyor.
- AI destekli otomatik viewing planlama veya mesai dışı otomatik yanıt sistemi bulunmuyor.

## Teknik / Genel

- Site modern ve kullanıcı dostu.
- Google Maps entegrasyonu mevcut.
- Mobil cihazlarda temel arama, filtreleme ve iletişim formları kullanılabiliyor.
- İnceleme sırasında AI servislerine veya Neuron API'lerine ait belirgin API entegrasyonları gözlemlenmedi.
- Temel emlak fonksiyonları (arama, filtreleme, valuation, mortgage calculator) başarılı çalışıyor.

**Durum:** Yapıldı

### Tur 2 — Görkem

**Arama:**
- Ayselin'in Tur 1 gözlemine katılıyorum (sadece filtre, doğal dil yok) ve şimdi platform bağlamını ekleyebilirim: tüm Neuron grubunu gördükten sonra bunun Property Connections'a özel bir tercih olmadığı, dokunulmamış platform varsayılanı olduğu net. Ana sayfada Buy/Rent toggle; sonuç sayfası price interval, min–max beds ve 0–40mil yarıçapla sınırlı; type yok, keyword yok, harita yok, sadece liste, sıralama = Suggested/price/date. İskoç acente (Livingston/Bathgate, SC şirket).
- **AI fırsatı (platform seviyesi):** paylaşılan filtre API'sine bağlanan doğal dil araması — sadece bu değil, her tenant için yeniden kullanılabilir.

**İlan Detay:**
- Grup A ile aynı şablon doğrulandı: bullet key-features + uzun elle yazılmış anlatı, floorplan, bazen video, 360 yok, AI özet yok, soru sorma yok, bölge bilgisi düz yazı, zayıf map sekmesi. "Similar" bloğu sadece "our latest properties" — en yeni, izleyiciye göre eşleştirilmiş değil.
- **AI fırsatları:** ilan özeti + veriye dayalı Q&A, ve latest-in yerine listing embedding'leriyle gerçekten kişiselleştirilmiş "similar homes".

**Değerleme:**
- Anlık araç (`valuation.propertyconnections.uk.com`) + yüz yüze. Grupla aynı: "immediate estimate" vaat ediyor ama aslında kapı-tutan lead formu — bilgi toplayıp sonra dönüyor. Ekrandaki ifade gerçekte olanı abartıyor (göndermedim).

**İletişim:**
- Form + telefon (01506) + e-posta; chat yok, mesai dışı yok, lead qualification yok — herkese aynı tek tip form.
- **AI fırsatı:** bu tenant'ın kendi stoğu + FAQ'larına dayalı hafif bir mesai dışı asistanı / lead qualifier, ofis kapalıyken enquiry'leri en azından karşılayıp önceliklendirir.

**Teknik/Genel:**
- Neuron/Iceberg, Vercel, S3 CDN. Güven iyi (isimli-danışman yorumları — Kevin/Chris/Sarah, SC şirket kaydı, redress scheme).
- Anlamlı detay: "A Different Kind Of Estate Agency" tagline'ı **Jacksons (08) ile birebir aynı** — tenant'lar arası paylaşılan şablon metnine açık kanıt; bu da AI özelliklerinin acente başına değil, platform seviyesinde bir kez inşa edilmesi gerektiğini pekiştiriyor.

**Durum:** Yapıldı

### Tur 3 — Berkay

**Arama:**
-

**İlan Detay:**
-

**Değerleme:**
-

**İletişim:**
-

**Teknik/Genel:**
-

**Durum:** Yapılmadı

### Tur 4 — Yasemin

## **Arama:**

- **Doğal Dil Araması:** **Yok** — "3 bed near a school under £250k in Bathgate" yazıldığında "Couldn't find the address" dönüyor. Property Cloud ile birebir aynı hata biçimi. (SS-03)
- **Akıllı Öneri / Sorgu Yorumlama:** **Kısmen** — "bathgt" yine Bathgate'e çözülüyor, ama dropdown "Bathgate Road, London", "Bathgate, Eyemouth" ve "Bathgate Academy" öneriyor. URL'deki `place_id: ChIJF3gcD1rYh0gR6_6GWy6EAhw` bunun Google Places geocoding olduğunu doğruluyor. Adresi düzeltiyor, emlak niyetini değil — ve West Lothian'daki bir alıcıyı gönül rahatlığıyla Londra'ya yollayabiliyor. (SS-01, SS-02, SS-05)
- **Kayıtlı Arama / Alerts:** **Var** — "Setup Heads Up Alert" doğrudan sonuç başlığında duruyor. Kriter bazlı, kural odaklı; AI yorumu yok. (SS-05, SS-09)
- **Ek not:** Property Cloud'daki karşılıksız kişiselleştirme deseni burada da aynen var — **"SUGGESTED"** sıralaması, her kartta **"100% MATCH"** rozeti ve hemen yanlarında **"HAVE YOU LOGGED IN?"**. Giriş yapılmadan 27 sonucun tamamı %100 eşleşme görünüyor. (SS-05)
- **Ek not:** Filtreler klasik dropdown — Bathrooms, Reception, Include SSTC/Under Offer, Retirement Homes, Shared Ownership, Investment Property, Must Haves, Property Type kutucukları. Bir de **"Other / Advanced"** açılırı var; Property Cloud'un sürümünde bu yok. (SS-04)

## **İlan Detay:**

- **Property Summary (AI Özet):** **Yok** — Description elle yazılmış düz metin, üstte madde özeti yok.
- **Property Q&A:** **Yok** — "Make an Enquiry" bir form, soru kanalı değil.
- **Property Highlights:** **Kısmen** — Features listesi var ama ilan girişinde elle ve tamamı büyük harfle yazılmış ("RARELY AVAILABLE IMMACULATE AND SPACIOUS DETACHED BUNGALOW", "CLOSE TO AMENITIES"). AI çıkarımı değil ve o kadar genel ki pek bir şey katmıyor. (SS-07)
- **Lifestyle / "Ideal for..." Eşleştirme:** **Kısmen** — "comfortable and convenient lifestyle", "friendly and respected local community" gibi ifadeler serbest metinde geçiyor. Yapılandırılmış eşleştirme yok.
- **Property Comparison:** **Yok** — Karşılaştırma veya favori fonksiyonu yok.
- **Benzer İlan Önerisi:** **Yok** — Sayfanın altı alert, rehber ve "Thinking of selling?" CTA'ları ile dolduruluyor.
- **Belge Açıklama (EPC / Floor Plan / Home Report):** **Yok** — **Bu sitedeki en büyük gap.** Göze çarpan bir "GET HOME REPORT" butonu, ham İskoç Home Report PDF'ini indiriyor: tek bir ekspertiz raporu, enerji raporu ve property questionnaire'i bir arada taşıyan, tipik olarak 20–40 sayfalık bir belge. Hiç özetlenmeden kullanıcının kucağına bırakılıyor. Floor plan ve EPC yalnızca görsel. (SS-06)
- **Mortgage Calculator:** **Var** — İlan sayfasında, satış fiyatıyla önceden doldurulmuş: depozito (%10 = £28,000), %6,01 faiz, 25 yıl vade ve canlı olarak "Monthly repayments: £1,625". Çalışıyor ama tamamen aritmetik — ödeyebilirlik yorumu, faizin kaynağı veya açıklama yok. (SS-08)
- **Stamp Duty Calculator:** **Var — ama muhtemelen yanlış etiketli.** ⚠️ Mülk Armadale, West Lothian'da. İskoçya'da Stamp Duty alınmaz; **LBTT** alınır (ek konutta ayrıca ADS) ve bantları, eşikleri farklıdır. Araç "Stamp Duty Calculator" başlığıyla ve "I am... / Buying my first home" seçiciyle duruyor. Arkadaki oranların LBTT mi SDLT mi olduğu, çalıştırıp LBTT bantlarıyla karşılaştırılarak doğrulanmalı — ama her hâlükârda etiket bir İskoç acentesi için yanlış ve alıcıya yanlış zihinsel model veriyor. (SS-08)
- **Ek not:** İlanda **Vimeo üzerinden danışman anlatımlı video** ("23 Barlaw Gardens — Sharon Forrester") ve **Matterport sanal turu** var. Medya tarafı burada gerçekten güçlü; üzerine hiçbir şey konulmamış.
- **Ek not:** **"Offers Over" fiyatlama, teklif yönlendirmesi yok.** Her ilan "Offers Over £X" ile fiyatlanıyor — İskoçya'nın normu — ama sitede hiçbir yer alıcıya gerçekçi teklifin ne olduğunu, benzer evlerin kaça kapandığını veya tipik olarak rehber fiyatın ne kadar üstüne çıkıldığını söylemiyor. İngiltere'deki sitelerde karşılığı olmayan, piyasaya özgü çok net bir AI fırsatı.

## **Değerleme:**

- **Instant Valuation:** **Var — 3. parti, Property Cloud ile aynı.** `valuation.propertyconnections.uk.com/home/4076` adresinde ve **"Powered by The ValPal Network"** ibaresi taşıyor. Girdiler: postcode → Find Address, Number of Bedrooms, Property Type, Submit. Ana siteden görsel olarak kopuk ve kendi çerez onay banner'ını açıyor. (SS-10)
- **AI Valuation Açıklaması:** **Yok** — Gerekçe, karşılaştırılabilir satış, kişiselleştirme yok.
- **Ek not — pazarlama çelişkisi:** Ana sayfa bu aracı **"quick and accurate"** ve **"in seconds"** diye satıyor. Aynı ValPal aracı Property Cloud'da o acente tarafından **"Up to 60% accurate"** diye tanıtılıyor. Aynı motor, zıt iddialar — platform düzeyinde bir mesaj sorunu olarak işaretlenmeli.
- **Ek not:** Yüz yüze yol (`/valuations`) düz bir lead formu — hitap, ad, e-posta, telefon ve değerlenecek adres **postcode araması olmayan serbest metin kutusu** olarak. Property Cloud'daki postcode aramalı versiyondan daha zayıf. Takvim ve slot seçimi yok. (SS-11)

## **İletişim / Lead:**

- **AI Chat Assistant / Chatbot:** **Yok** — Hiçbir sayfada widget yok. **Ama sayfa kaynağı yine `.whatsapp-chatbot` sınıfını `--wa-green`, `--wa-header-bg`, `--wa-bubble-bg`, `--wa-chat-bg` ve `--wa-input-bg` ile tanımlıyor.** Neuron'un WhatsApp chatbot bileşenini gönderdiği ve acentenin açmadığı üst üste ikinci site. Artık tek seferlik bir durum değil, platform deseni. (SS-15)
- **Lead Qualification:** **Kısmen** — Heads Up kaydı alma sebebini, taşınma zamanını, avukat durumunu, acenteyi nereden duyduğunu ve Property Cloud'dan bir soru fazlasıyla **"Do you need to sell the property you currently live in?"** bilgisini topluyor. Gerçekten değerli zincir verisi, statik bir forma giriyor; dallanma veya önceliklendirme yok. (SS-09)
- **Otomatik Randevu / Viewing Planlama:** **Yok** — "Make an Enquiry" ve değerleme formu talep gönderiyor.
- **Mesai Dışı Yanıt:** **Yok — ve bu, acentenin kendi metniyle çelişiyor.** ⚠️ Ana sayfa şunu diyor: *"We're not a nine-to-five operation - we're here when you need us."* İletişim sayfası ise **Opening Hours: Pazartesi–Cuma 9:00–17:00, Cumartesi 9:00–14:00, Pazar KAPALI** yayınlıyor. Bu saatlerin dışında chat yok, WhatsApp yok, otomatik yanıt yok — sadece form var. Vaat ile yayınlanan gerçeklik zıt yönleri gösteriyor ve bu boşluğu tam olarak 7/24 çalışan bir asistan kapatır. (SS-12)
- **Ek not:** İletişim formu tek tip — ad, soyad, telefon, e-posta, Buy/Sell/Rent/Let checkbox satırı, serbest mesaj, onay kutusu. Seçime göre dallanma yok. (SS-13)

## **Teknik / Genel:**

- **SSR vs CSR:** **Hibrit ve Property Cloud'dan farklı.** Doküman Nuxt ile render ediliyor (`/_nuxt/` bundle'ları) ama sonuç listesi client-side çekiliyor: Network'te **`filter?search_type=sales&is_website=...` 245 ms'de 36,7 kB** dönüyor, initiator `Bt02TWCK.js`. Property Cloud'da ilan seti HTML'in içinde geliyordu. Aynı platform, farklı render yolu. (SS-14)
- **API çağrıları:** Filter çağrısı dışında — `ice.js` kaynaklı `anonymous` (Iceberg tracker), üç adet `envelope/?sentry_version=7...` (Sentry) ve bir cache'lenmiş varlık. **Hiçbir AI/LLM servisine gidilmiyor.** 7/158 istek, 326 kB transfer, 3,51 sn'de bitiyor. (SS-14)
- **Tema sürümü:** Kaynak `/common/css/neuron.css` ile birlikte `/theme3/css/propertyconnections/index.css` ve ayrıca **Bootstrap, Owl Carousel, FontAwesome** yüklüyor. Property Cloud `theme4` kullanıyor. Bu acente **daha eski bir Neuron tema kuşağında** — bazı bileşenlerin neden farklı olduğunu açıklayan önemli bir bağlam. (SS-15)
- **Iceberg izleri:** Kaynakta `window.IcebergTracker` ve `__akyaCookieStarted`; varlıklar `files.propertyconnections.neuronwebsites.co.uk` ve `lifesycle-cdn.s3.eu-west-2.amazonaws.com` üzerinden. (SS-15)
- **Mobil davranış:** **Sorunsuz** — 400px'te arama çubuğu, fiyat seçicileri, oda aralığı ve filtreler düzgün yığılıyor, kullanılabilir kalıyor. (SS-14)
- **Ek not — bozuk harita:** ⚠️ İletişim sayfasındaki "Visit Us" Google haritası **Folkestone, Dymchurch, New Romney ve Dungeness** merkezli — yani güneydoğu İngiltere'deki Kent sahili, acentenin 80 North Bridge Street, Bathgate'teki gerçek ofisinden yaklaşık 600 km uzakta. Şubeyi bulmaya çalışan ziyaretçi ülkenin öbür ucuna yönlendiriliyor. Geçici bir hata olma ihtimalini elemek için yeniden yüklenip kontrol edilmeli, ama çekildiği hâliyle canlıda duran, kullanıcıya dokunan bir arıza. (SS-13)
- **Ek not:** Footer'daki telif **© 2025** yazıyor, site 2026'da canlı — statik içeriğin elle bakıldığının küçük bir işareti. (SS-16)


**Durum:** Yapıldı

### Ortak Bulgular / Sentez (4 tur bitince doldurulur)

- Ortak eksik AI özellikleri: Doğal dil arama, AI ilan özeti, Property Q&A, AI lead scoring, mesai dışı otomatik yanıt.
- Öne çıkan fırsatlar: (1) İskoçya'ya özgü Home Report (20-40 sayfalık PDF) hiç özetlenmeden indiriliyor. (2) "Offers Over" fiyatlama modeli alıcıya rehberlik sunmuyor. (3) Aynı ValPal aracı tenant'lar arasında tutarsız pazarlanıyor.
- Görüş ayrılıkları / doğrulanması gerekenler: ✅ **Ayselin tarafından doğrulandı (canlı kontrol, Ağustos 2026):** Contact sayfasındaki "Visit Us" haritası hâlâ Folkestone/Dymchurch/New Romney/Dungeness/Lydd (Kent, İngiltere) gösteriyor — acentenin gerçek Bathgate, West Lothian adresinden ~600km uzakta. Bu, geçici değil, kalıcı ve düzeltilmemiş canlı bir hata. ✅ **Doğrulandı ve netleşti:** Stamp Duty Calculator, £424,000'lik bir mülk için "From 16 December 2024: £15,150" sonucunu veriyor — "16 December 2024" referans tarihi bir **İngiltere SDLT eşik değişikliğine** karşılık geliyor, İskoç LBTT bandına değil. Bu, hesaplayıcının bir İskoç acentesi için gerçekten SDLT mantığıyla çalıştığını (LBTT değil) güçlü şekilde gösteriyor — bu da İskoç alıcılar için maddi olarak yanlış rakamlar üretir; sadece yanlış etiketlemenin ötesinde gerçek, işlevsel bir hata, platform ekibine doğrudan bildirilmeye değer. Ana sayfa ayrıca anlık değerlemenin "quick and accurate" olduğunu belirtiyor — canlı olarak, kelimesi kelimesine doğrulandı — 05 · Property Cloud'daki aynı ValPal aracı için "Up to 60% accurate" ile karşılaştırıldığında.
