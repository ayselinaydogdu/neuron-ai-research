# 07 · keystoneestateagents.co.uk

**URL:** https://keystoneestateagents.co.uk/
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

- Traditional filter-based search is available (location, price, property type, bedrooms, etc.).
- Natural Language Search is not available.
- Property Alerts are available, allowing users to receive email notifications for properties matching their search criteria.

## Property Details

- Property descriptions are detailed, but an AI-generated Property Summary is not available.
- Users cannot ask free-form questions about a property (AI Property Q&A is not available).
- Lifestyle recommendations such as "Ideal for..." are not provided.
- AI-powered Property Highlights and Property Comparison features are not available.
- EPC certificates and Floor Plans are provided where available, but they are not explained or summarized by AI.

## Valuation

- An Instant Online Valuation service is available.
- Users can request a free property valuation.

## Contact

- A contact form is available.
- Users can request property viewings and property valuations.
- No AI chatbot or AI-powered customer assistant is available.

## Technical / General

- The website has a modern and user-friendly interface.
- Core real estate features (property search, property listings, valuation, and contact services) function effectively.

**Status:** Done

### Round 2 — Görkem

**Search:**
- Same platform search. Flintshire/Chester (01244). Homepage teases "Latest properties for sale in Flintshire" but has no on-page filters — you go to `/properties` for the standard price/beds/radius set. No type, no keyword, no natural language, no map, list-only.
- "Register for Property Alerts" is present (the Heads-Up equivalent) — again criteria matching, not smart matching.

**Listing Detail:**
- Same Neuron template, same gaps: bullet features + hand-written narrative, floorplan, no AI summary/Q&A, area info as prose.
- Their real differentiator is the service model — "a single dedicated consultant", Case Studies, a "How We Help You Move" explainer. It's good, reassuring content, but none of it enriches the listing page itself, where a buyer actually makes the shortlist decision.

**Valuation:**
- Online tool (`valuation.keystonepmc.co.uk`) + face-to-face + an "Instruct Keystone" shortcut. Same gated instant-valuation pattern as the group — details captured, number delivered later.

**Contact:**
- Phone (01244), email, contact form; Trustpilot referenced. No chat, no out-of-hours, no qualification.

**Technical / General:**
- Neuron/Iceberg, Vercel.
- Trust is fine (87% completion stat, TPO, company reg, "personal consultant" framing). Small consistency snag: the valuation subdomain uses the `keystonepmc` brand while the main site is `keystoneestateagents` — a minor trust wobble mid-journey, worth noting because that split-domain valuation flow is a shared platform pattern.

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

- **Natural Language Search:** **No** — "3 bed near a school under £160k in Shotton" → "Couldn't find the address". Fourth site, fourth time the same failure. (SS-03)
- **Smart Suggestions / Query Interpretation:** **Partial — not AI** — "conahs quay" resolves correctly, but that's Google Places; the URL carries a `place_id` and the suggestions are POIs (school, power station, civic hall). (SS-01, SS-02, SS-05)
- **Welsh place names:** **No problem.** "Rhosllanerchrugog" returns correctly. The expected gap didn't materialise. (SS-04)
- **Saved Search / Alerts:** **Yes** — Rule-based. (SS-06)
- **"100% MATCH" badge: absent on this site.** The unbacked badge that sits on every card on the other two sites has been removed in `theme7`. Only "SUGGESTED" and "HAVE YOU LOGGED IN?" remain. (SS-06)
- Filters are the same set as the other sites; no "Other/Advanced". (SS-05)

## **Listing Detail:**

- **Property Summary (AI Summary):** **No** — Long hand-written prose. (SS-08)
- **Property Q&A:** **No**
- **Property Highlights:** **Partial — manual** — Entered by hand, but written better than on the other sites (school names, park, station each listed individually).
- **Lifestyle Matching:** **Partial** — In the free text, unstructured.
- **Property Comparison:** **No**
- **Similar Listing Suggestions:** **No**
- **Area Insights:** **Partial — manual**
- **Commute Insights:** **Partial — manual** — No travel time calculated.
- **Document Explanation:** **No** — Five separate EPC images, all raw pictures.
- **Mortgage / LTT Calculator:** **No**

**Additional notes:**
- Sections load as collapsed accordions (Features, Property Information, Floor Plan, Map, EPC, Media Links). Rich content hidden by default. (SS-09)
- **A Sprift "Key Facts for Buyers" report exists** — the only one in this study. But it's buried inside the "MEDIA LINKS" accordion, effectively invisible.
- Seller disclosure sits there structured: boiler 10 years, **prepayment meter**, windows 11–20 years, bathroom refurbished. An uninterpreted raw list.
- ⚠️ **Price inconsistency:** Heading says "GUIDE PRICE £150,000", description says "OFFERS INVITED BETWEEN £150,000 and £170,000". (SS-08)
- Strongest media set: Giraffe360 tour + narrated drone video + 22 photos. No AI layer over it. (SS-07)

## **Valuation:**

Three separate routes (two on the other sites).

- **Instant Valuation:** **Yes — third-party, ValPal for the third time.** Separate subdomain, disconnected design. (SS-18)
- **AI Valuation Explanation:** **No**

**Additional notes:**
- The face-to-face form is the richest in this study: 8 property types, room counts, **Condition (Excellent/Good/Average/Needs work)**, parking, other features. It could produce an instant estimate from this data and instead only submits a request. (SS-15, SS-16)
- `/instruct-us-valuation` → skips valuation entirely and goes straight to instructing the agency. Not present on the other sites. (SS-17)

## **Contact / Lead:**

- **Chatbot:** **No** — But `.whatsapp-chatbot` is again defined in the page source. **Third site, third time.** (SS-20)
- **Lead Qualification:** **Partial — manual** — Identical form to PConn, no branching. (SS-13)
- **Automated Appointment:** **No — and here it's documented most explicitly.** ⚠️ The "BOOK A VIEWING" modal has a **working calendar and time picker**, but above it reads "This is a request only, not a confirmed viewing", and below it the user is asked to describe their availability **in writing** as well. Availability is collected in two different forms, and neither results in a booking. (SS-11)
- **Out-of-Hours Response:** **No** — And **opening hours are never published** anywhere. (SS-14)

**Additional note:** The viewing modal doubles as a lead form — it asks for the user's own address, "property to sell", "property to let", "my property valued". Chain status is collected from someone who just wants to view a house; no automation follows. (SS-12)

## **Technical / General:**

- **SSR vs CSR:** **SSR** — No `filter?search_type=` call; the list is in the HTML. Nuxt. (SS-19, SS-20)
- **API calls:** `ice.js` (Iceberg tracker), 3× Sentry, `view`. **No AI/LLM call.** 6/137 requests, 283 kB, **2.25 s — the fastest of the three sites.** (SS-19)
- **Theme / third-party:** `neuron.css` + `theme7`. Also loads a **Trustpilot widget** (absent on the others). (SS-20)
- **Mobile:** **Fine.** (SS-19)
- ⚠️ The footer renders twice, and the second block reads **"Company Number: NaN"**. *(Found in source, needs confirming with a screenshot.)*

**Status:** 

### Findings / Synthesis (filled once all 4 rounds are done)

- Commonly missing AI features: Natural-language search, AI listing summaries, Property Q&A, AI lead scoring, out-of-hours automated response; opening hours not published anywhere.
- Standout opportunities: (1) A Sprift "Key Facts for Buyers" report exists but is buried inside the "Media Links" accordion. (2) The face-to-face valuation form is the richest in the study but only submits a request.
- Disagreements / to verify: ✅ **Confirmed by Ayselin (live check, August 2026):** The footer genuinely renders twice on the page. The first block correctly shows "Company Number: 09267819"; the second block shows "Company Number: NaN" — Yasemin's Round 3 finding is fully verified, not a one-off. **Cross-referencing with 01 · Kinetic (also confirmed to have this exact defect) and 02–05 · Town&City/Harrisons/Lloyds/Property Cloud (confirmed NOT to have it):** this revises our earlier working theory. The bug is not platform-wide, but it is not single-tenant either — it affects at least 2 of 7 sites checked so far (01, 07), suggesting it's tied to a specific theme/template version shared by a subset of tenants rather than either "every site" or "one site." Worth checking whether 01 and 07 share the same theme build. The "100% MATCH" badge is also confirmed absent on this site (theme7), unlike 03/04/05/06 — consistent with the theme-version hypothesis above; these two findings together suggest 07 Keystone runs on a distinguishable theme generation from the Town&City/Harrisons/Lloyds/Property Cloud/Property Connections group.

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

- Klasik filtre tabanlı arama mevcut (konum, fiyat, emlak türü, oda sayısı vb.).
- Doğal dil araması (Natural Language Search) bulunmuyor.
- Kayıtlı arama / Property Alerts özelliği mevcut. Kullanıcılar kriterlerine uygun yeni ilanlar için e-posta bildirimi alabiliyor.

## İlan Detay

- Property açıklamaları detaylı ancak AI destekli Property Summary (özet) bulunmuyor.
- Kullanıcı ilan hakkında serbest şekilde soru soramıyor (AI Property Q&A bulunmuyor).
- "Ideal for..." gibi yaşam tarzına yönelik öneriler sunulmüyor.
- AI destekli Property Highlights veya Property Comparison özellikleri bulunmuyor.
- EPC ve Floor Plan belgeleri mevcut olduğunda sunuluyor ancak AI tarafından açıklanmıyor.

## Değerleme

- Instant Online Valuation hizmeti mevcut.
- Satıcılar için ücretsiz değerleme talebi oluşturulabiliyor.

## İletişim

- İletişim formu mevcut.
- Property viewing ve valuation talepleri oluşturulabiliyor.
- AI chatbot veya AI destekli müşteri asistanı bulunmuyor.

## Teknik / Genel

- Site modern ve kullanıcı dostu bir arayüze sahip.
- Temel emlak fonksiyonları (arama, ilan görüntüleme, değerleme ve iletişim) sorunsuz çalışıyor.

**Durum:** Yapıldı

### Tur 2 — Görkem

**Arama:**
- Aynı platform araması. Flintshire/Chester (01244). Ana sayfa "Latest properties for sale in Flintshire" gösteriyor ama sayfa içi filtre yok — standart price/beds/radius için `/properties`'e gidiyorsun. Type yok, keyword yok, doğal dil yok, harita yok, sadece liste.
- "Register for Property Alerts" mevcut (Heads-Up karşılığı) — yine kriter eşleşmesi, akıllı eşleşme değil.

**İlan Detay:**
- Aynı Neuron şablonu, aynı açıklar: bullet features + elle yazılmış anlatı, floorplan, AI özet/Q&A yok, bölge bilgisi düz yazı.
- Gerçek farklılaştırıcıları hizmet modeli — "tek özel danışman", Case Studies, "How We Help You Move" anlatımı. Güzel, güven veren içerik, ama hiçbiri alıcının aslında kısa listeyi oluşturduğu ilan sayfasını zenginleştirmiyor.

**Değerleme:**
- Online araç (`valuation.keystonepmc.co.uk`) + yüz yüze + "Instruct Keystone" kısayolu. Grupla aynı kapı-tutan instant-valuation kalıbı — bilgi toplanıyor, rakam sonra veriliyor.

**İletişim:**
- Telefon (01244), e-posta, iletişim formu; Trustpilot referansı. Chat yok, mesai dışı yok, kalifikasyon yok.

**Teknik/Genel:**
- Neuron/Iceberg, Vercel.
- Güven iyi (%87 completion istatistiği, TPO, şirket kaydı, "kişisel danışman" çerçevesi). Küçük tutarlılık pürüzü: valuation subdomain'i `keystonepmc` markasını kullanırken ana site `keystoneestateagents` — yolun ortasında minör bir güven sarsıntısı; bu bölünmüş-domain valuation akışı paylaşılan bir platform kalıbı olduğu için not edilmeye değer.

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

- **Doğal Dil Araması:** **Yok** — "3 bed near a school under £160k in Shotton" → "Couldn't find the address". Dört sitede dördüncü kez aynı hata. (SS-03)
- **Akıllı Öneri / Sorgu Yorumlama:** **Kısmen — AI değil** — "conahs quay" doğru çözülüyor ama bu Google Places; URL'de `place_id` var, öneriler POI (okul, power station, civic hall). (SS-01, SS-02, SS-05)
- **Galce yer adları:** **Sorun yok.** "Rhosllanerchrugog" doğru dönüyor. Beklenen gap çıkmadı. (SS-04)
- **Kayıtlı Arama / Alerts:** **Var** — Kural tabanlı. (SS-06)
- **"100% MATCH" rozeti: bu sitede yok.** Diğer iki sitede her kartta duran karşılıksız rozet `theme7`'de kaldırılmış. Sadece "SUGGESTED" ve "HAVE YOU LOGGED IN?" kalmış. (SS-06)
- Filtreler diğer sitelerle aynı set; "Other/Advanced" yok. (SS-05)

## **İlan Detay:**

- **Property Summary (AI Özet):** **Yok** — Elle yazılmış uzun düz metin. (SS-08)
- **Property Q&A:** **Yok**
- **Property Highlights:** **Kısmen — manuel** — Elle girilmiş ama diğerlerinden iyi yazılmış (okul isimleri, park, istasyon tek tek).
- **Lifestyle Eşleştirme:** **Kısmen** — Serbest metinde, yapılandırılmamış.
- **Property Comparison:** **Yok**
- **Benzer İlan Önerisi:** **Yok**
- **Area Insights:** **Kısmen — manuel**
- **Commute Insights:** **Kısmen — manuel** — Süre hesabı yok.
- **Belge Açıklama:** **Yok** — 5 ayrı EPC görseli, hepsi ham resim.
- **Mortgage / LTT Calculator:** **Yok**

**Ek notlar:**
- Bölümler kapalı akordeon geliyor (Features, Property Information, Floor Plan, Map, EPC, Media Links). Zengin içerik varsayılan olarak gizli. (SS-09)
- **Sprift "Key Facts for Buyers" raporu var** — bu çalışmada tek. Ama "MEDIA LINKS" akordeonunun içine gömülü, pratikte görünmez.
- Satıcı beyanı yapılandırılmış duruyor: kombi 10 yıl, **prepayment sayaç**, pencere 11–20 yıl, banyo yenilenmiş. Yorumlanmamış ham liste.
- ⚠️ **Fiyat tutarsız:** Başlık "GUIDE PRICE £150,000", açıklama "OFFERS INVITED BETWEEN £150,000 and £170,000". (SS-08)
- Medya en güçlüsü: Giraffe360 turu + anlatımlı drone videosu + 22 fotoğraf. Üzerinde AI yok. (SS-07)

## **Değerleme:**

Üç ayrı yol var (diğerlerinde iki).

- **Instant Valuation:** **Var — 3. parti, üçüncü kez ValPal.** Ayrı subdomain, kopuk tasarım. (SS-18)
- **AI Valuation Açıklaması:** **Yok**

**Ek notlar:**
- Face-to-face formu çalışmadaki en zengini: 8 tip seçeneği, oda sayıları, **Condition (Excellent/Good/Average/Needs work)**, parking, ek özellikler. Bu veriyle anında tahmin üretilebilecekken sadece talep gönderiyor. (SS-15, SS-16)
- `/instruct-us-valuation` → değerlemeyi atlayıp doğrudan iş verme akışı. Diğer sitelerde yok. (SS-17)

## **İletişim / Lead:**

- **Chatbot:** **Yok** — Ama kaynak kodda yine `.whatsapp-chatbot` tanımlı. **Üç sitede üçüncü kez.** (SS-20)
- **Lead Qualification:** **Kısmen — manuel** — PConn ile birebir aynı form, dallanma yok. (SS-13)
- **Otomatik Randevu:** **Yok — en açık belgelenmiş hâliyle.** ⚠️ "BOOK A VIEWING" modalında **çalışan takvim ve saat seçici** var, ama üstünde "This is a request only, not a confirmed viewing" yazıyor ve altında ayrıca müsaitliği **yazıyla** anlatması isteniyor. Kullanıcıdan müsaitlik iki farklı biçimde alınıyor, hiçbiri randevuya dönüşmüyor. (SS-11)
- **Mesai Dışı Yanıt:** **Yok** — Ayrıca **açılış saatleri hiç yayınlanmamış**. (SS-14)

**Ek not:** Viewing modalı aynı zamanda lead formu — kendi adresi, "property to sell", "property to let", "my property valued" soruluyor. Ev görmek isteyenden zincir durumu toplanıyor, otomasyon yok. (SS-12)

## **Teknik / Genel:**

- **SSR vs CSR:** **SSR** — `filter?search_type=` çağrısı yok, liste HTML'de. Nuxt. (SS-19, SS-20)
- **API çağrıları:** `ice.js` (Iceberg tracker), 3× Sentry, `view`. **AI/LLM çağrısı yok.** 6/137 istek, 283 kB, **2,25 sn — üç site içinde en hızlısı.** (SS-19)
- **Tema / 3. parti:** `neuron.css` + `theme7`. Ayrıca **Trustpilot widget** yükleniyor (diğerlerinde yok). (SS-20)
- **Mobil:** **Sorunsuz.** (SS-19)
- ⚠️ Footer iki kez basılıyor, ikinci blokta **"Company Number: NaN"**. *(Kaynak koddan tespit, SS ile doğrulanmalı.)*

**Durum:** Yapıldı

### Ortak Bulgular / Sentez (4 tur bitince doldurulur)

- Ortak eksik AI özellikleri: Doğal dil arama, AI ilan özeti, Property Q&A, AI lead scoring, mesai dışı otomatik yanıt; opening hours hiçbir yerde yayınlanmamış.
- Öne çıkan fırsatlar: (1) Sprift "Key Facts for Buyers" raporu var ama "Media Links" akordeonunda gömülü. (2) Yüz yüze değerleme formu bu çalışmadaki en zengin form ama sadece talep gönderiyor.
- Görüş ayrılıkları / doğrulanması gerekenler: ✅ **Ayselin tarafından doğrulandı (canlı kontrol, Ağustos 2026):** Footer sayfada gerçekten iki kez render ediliyor. İlk blok doğru şekilde "Company Number: 09267819" gösteriyor; ikinci blok "Company Number: NaN" gösteriyor — Yasemin'in Round 3 bulgusu tam olarak doğrulandı, tek seferlik değil. **01 · Kinetic (bu hatayı taşıdığı doğrulanmıştı) ve 02-05 · Town&City/Harrisons/Lloyds/Property Cloud (bu hatayı taşımadığı doğrulanmıştı) ile çapraz karşılaştırıldığında:** bu, önceki çalışan teorimizi güncelliyor. Hata platform genelinde değil, ama tek bir tenant'a özgü de değil — şimdiye kadar kontrol edilen 7 sitenin en az 2'sinde (01, 07) görülüyor, bu da hatanın "her sitede" ya da "sadece bir sitede" değil, belirli bir tema/template sürümüne bağlı olduğunu, bu sürümü paylaşan bir alt gruba özgü olduğunu gösteriyor. 01 ve 07'nin aynı tema build'ini paylaşıp paylaşmadığı kontrol edilmeye değer. "100% MATCH" rozetinin de bu sitede (theme7) yokluğu doğrulandı, 03/04/05/06'nın aksine — yukarıdaki tema-sürümü hipotezini destekliyor; bu iki bulgu birlikte, 07 Keystone'un Town&City/Harrisons/Lloyds/Property Cloud/Property Connections grubundan ayırt edilebilir bir tema jenerasyonunda çalıştığını gösteriyor.
