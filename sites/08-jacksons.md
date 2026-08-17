# 08 · jacksonsproperty.co.uk

**URL:** https://jacksonsproperty.co.uk/
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

- The website provides standard property search filters, including price, bedroom count, location, and search radius.
- Search functionality is primarily designed for finding properties by location or address.
- Natural Language Search is not supported. The search does not interpret descriptive requests or understand user intent beyond standard location-based queries.
- AI-powered search, semantic query understanding, and intelligent property matching are not available.
- Property Alerts and Heads Up Alerts are available for users who want to receive notifications about relevant listings.

## Property Details

- Property listing pages provide detailed information such as photographs, descriptions, key property features, floor plans, EPC ratings, and other essential property data.
- AI-generated summaries are not provided, so users need to review the listing information themselves.
- There is no AI-powered question-and-answer functionality available directly on the property listing.
- Properties cannot be automatically compared using an AI-powered comparison feature.
- Floor plans and EPC information are displayed as standard property documents without AI-generated explanations.
- Google Maps/location information is available, but there are no AI-generated insights about the surrounding area or commuting options.
- Related properties are displayed based on standard listing logic rather than personalized recommendations.

## Valuation

- An online property valuation/estimate service is available, with the option for users to request further assistance.
- Mortgage and Stamp Duty calculators are available on the website.
- These tools provide numerical calculations but do not provide personalized AI explanations, affordability analysis, or recommendations based on the results.

## Contact

- Users can contact the agency through enquiry forms available on property pages.
- Property viewing requests can also be submitted through the website.
- The website primarily relies on direct contact methods such as phone and enquiry forms rather than an interactive AI chat experience.
- There is no clear AI-based lead qualification or out-of-hours conversational support.

## Technical / General

- The website uses a modern Neuron-based structure with a clear and professional interface.
- The platform includes supporting content such as property guides, FAQs, and area information, which could provide useful knowledge sources for a future AI assistant.
- The website does not currently make significant use of this content through interactive AI features.
### Round 2 — Görkem

**Search:**
- Same toggle + thin filters; Medway (Rainham/Gillingham, 01634). Confirmed on the results page: price min/max, radius 0–40mi, min–max beds, sort Suggested/price/date; no type, no keyword, no natural language, no map. "Setup Heads Up Alert" + "Register for Property Alerts".
- Jacksons has the richest supporting content of my ten — an "Advice Hub" with guides, FAQs and area guides. **That corpus is exactly the grounding a per-tenant AI assistant would need, and it's sitting there feeding no interactive feature.** Strong signal for where a Neuron assistant should draw from.

**Listing Detail:**
- I opened a live listing (Conqueror Drive, Gillingham): 20 photos, floorplan, a video, bullet FEATURES + long narrative, solid key facts (Guide £300–325k, 3 bed / 3 bath, Freehold, Council Tax C, EPC C/75, 807 sqft). Genuinely a good listing page.
- But still no AI summary, no ask-a-question, and the "OUR LATEST PROPERTIES" block is newest-in, not matched to me. So even the *best-populated* listing in the group hits the same ceiling.
- Detail page **does** include Mortgage + Stamp Duty calculators — but they're pure number-crunchers with no commentary. **AI opportunity (light):** a plain-language affordability/next-steps note on top of the calculator output (what the monthly figure means, what deposit changes do).

**Valuation:**
- Instant "quick online estimate with follow-up call" + face-to-face. Same gated pattern — the "estimate" is really the hook for the callback.

**Contact:**
- Phone-first (separate Sales/Lettings lines), "Make an Enquiry" generic form on listings, no chat, no out-of-hours, no qualification.

**Technical / General:**
- Neuron/Iceberg, Vercel, Lifesycle S3.
- Trust is strong (15+ reviews, named team, Propertymark/TPO). The "A Different Kind of Estate Agency" homepage line is the **same template copy as Property Connections (06)** — more confirmation of how much shared scaffolding sits under these tenants, and why AI belongs at platform level.
- Note to verify: Ayselin's Round 1 block reports an on-site AI Chat Assistant answering basic property questions; I didn't hit one in my pass. Worth re-checking live — it may be conditional/page-specific.

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

- **Natural Language Search:** **No** — "3 bed with a garage under £400k in Rainham" → "Couldn't find the address". **Fifth site, fifth time.**
- **Smart Suggestions / Query Interpretation:** **Partial — not AI** — "rainam" resolves correctly; suggestions are Rainham Station, Rainham Mark Grammar School, Rainham (Kent) Station Car Park. Google Places, with a `place_id` in the URL.
- **Saved Search / Alerts:** **Yes** — "Setup Heads Up Alert" in the results header. Rule-based.
- **"100% MATCH" badge:** Not seen on the result cards — like Keystone, unlike Property Connections. "SUGGESTED" and "HAVE YOU LOGGED IN?" remain.
- Filters are the same set as the other sites.

## **Listing Detail:**

Reviewed: `/properties/3-bedroom-house-.../535188` (Whitehorse Hill, Chatham)

- **Property Summary (AI Summary):** **No** — Hand-written prose.
- **Property Q&A:** **No**
- **Property Highlights:** **Partial — manual** — The Features list is entered by hand, but **EPC Rating E (50)** and **Medway Council Tax B** appear as bullets; directly useful to a buyer.
- **Lifestyle Matching:** **Partial** — "ideally suited for a growing family or as an investment" sits in the free text.
- **Property Comparison:** **No**
- **Similar Listing Suggestions:** **No** — The sidebar has a **"latest properties" carousel** navigated by arrows — chronology, not similarity. ⚠️ In at least one listing (Grain Road), the carousel lists **the property you're currently viewing as its first card**.
- **Area Insights:** **Partial** — The site has a separate **Area Guides** section, but **no link to it from the listing detail**. *(Guide content not tested.)*
- **Commute Insights:** **Partial — manual** — "Close to Chatham mainline station" appears as a bullet; no travel time calculated.
- **Document Explanation:** **No** — Floor Plan and EPC are images only.
- **Stamp Duty Calculator:** **Yes** — Correct tax for England, with a "Buying my first home" selector.
- **Mortgage Calculator:** **Yes** — Pre-filled with the price, 10% deposit, 6.01% interest, 25 years. Pure arithmetic, no commentary.
- **Additional note:** Sections are **tabs**, not accordions (Description / Video / Floor Plan / Map / EPC) — better than Keystone's hidden accordions.
- **Additional note:** Video hosted on Vimeo, agent-narrated ("Mark Jackson"). The homepage promotes "Jacqui B Videos" as a signature format.

## **Valuation:**

- **Instant Valuation:** **Yes — third-party, ValPal for the fourth time.** At `valuation.jacksonsproperty.co.uk/home/2488`, marked "Powered by The ValPal Network". Separate subdomain, separate cookie banner. A **Type of Valuation** dropdown also offers a lettings valuation.
- **AI Valuation Explanation:** **No**
- ⚠️ **Additional note — the agency admits the tool is inadequate:** The homepage says of the instant valuation: *"it's just a starting point. We'll follow up with a friendly call to understand your plans and offer real, tailored advice."* The tool is deliberately left incomplete and routed into a phone call. The clearest evidence yet for the AI-explained valuation gap.
- **Additional note:** The face-to-face form **distinguishes sales from lettings**: "I am looking to sell / to let / considering both" plus bedroom count. The only valuation form in the study with lettings awareness. Still no calendar or slot.

## **Contact / Lead:**

- **Chatbot:** **No (visibly)** — No widget on any screen. But the source carries **two separate traces**:
  - The `.whatsapp-chatbot` class — **fourth site, fourth time**, still switched off.
  - ⚠️ **`https://cdn.msgboxx.io/static/css/bundle.min.css`** — a third-party messaging platform's CSS. **First appearance in this study.** No widget surfaced on screen; whether it's loaded-but-dormant or triggered under certain conditions needs confirming.
- **Lead Qualification:** **Partial — manual** — The Heads Up registration uses the same Circumstances set as the other sites. No branching.
- **Automated Appointment:** **No** — The "MAKE AN ENQUIRY" modal has a calendar and time picker, but above it reads *"We'll confirm availability for you. (This does not confirm the viewing)"*. The same pattern as Keystone, except availability isn't asked for a second time in writing here.
- **Out-of-Hours Response:** **No** — No automated channel. Opening hours are published: Mon–Fri 9:00–18:00, Sat 9:00–17:00, **Sunday "BY APPOINTMENT"**.
- **Additional note:** The enquiry modal doubles as a lead form — the user's own address, "property to sell", "property to let", "my property valued".
- **Additional note:** Two separate phone numbers (Sales …37 / Lettings …38) sit at the top of every page. The user has to decide which to call; no guidance.

## **Technical / General:**

- **SSR vs CSR:** **SSR** — No `filter?search_type=` call; the list is in the HTML. Nuxt (`/_nuxt/`).
- **API calls:** `ice.js` (Iceberg tracker), 3× Sentry, `view`. **No AI/LLM call.** 6/107 requests, 246 kB, **2.07 s — the fastest site in the study.**
- **Theme / third-party:** `neuron.css` + `theme3` + Bootstrap/Owl/FontAwesome, plus **msgboxx.io**.
- **Mobile:** **Fine** — At 400px search, price, beds and filters stack cleanly.
- ✅ **The contact map is correct** — it shows the Rainham branch accurately (Property Connections pointed to the wrong end of the country).
- ✅ **The footer is clean** — one block, correct Company Number (040 158 04), no NaN. Only the copyright reads **© 2025** while the site is live in 2026.


**Status:** Done

### Findings / Synthesis (filled once all 4 rounds are done)

- Commonly missing AI features: Natural-language search, AI listing summaries, Property Q&A (see disagreement), AI lead scoring.
- Standout opportunities: (1) The "Advice Hub" (guides, FAQs, area guides) is the richest supporting content in the study — exactly the grounding an AI assistant would need, and it currently feeds no interactive feature. (2) Mortgage + Stamp Duty calculators exist but are purely numerical — adding plain-language commentary on top would be low effort, medium impact. (3) The agency itself describes its valuation tool as "just a starting point" — the clearest evidence yet for the value of an AI explanation layer.
- Disagreements / to verify: Round 1 (Ayselin) reported seeing an AI chat assistant; Round 2 (Görkem) did not — may be page-specific/conditional, needs live re-checking. The source contains both the `.whatsapp-chatbot` class and, for the first time in the study, a `cdn.msgboxx.io` (third-party messaging) trace — not visible on screen, unclear whether dormant or active under certain conditions.

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

- Web sitesinde fiyat, yatak odası sayısı, konum ve arama yarıçapı gibi standart mülk arama filtreleri bulunmaktadır.
- Arama işlevi ağırlıklı olarak konum veya adres üzerinden mülk bulmaya odaklanmaktadır.
- Doğal Dil Araması desteklenmemektedir. Arama sistemi, açıklayıcı kullanıcı taleplerini veya kullanıcı niyetini standart konum tabanlı sorguların ötesinde yorumlamamaktadır.
- Yapay zeka destekli arama, anlamsal sorgu anlama ve akıllı mülk eşleştirme özellikleri bulunmamaktadır.
- Kullanıcıların ilgili ilanlardan haberdar olabilmesi için Property Alerts ve Heads Up Alerts özellikleri bulunmaktadır.

## Mülk Detayları

- Mülk ilanlarında fotoğraflar, açıklamalar, temel mülk özellikleri, kat planları, EPC derecelendirmeleri ve diğer önemli mülk bilgileri sunulmaktadır.
- Yapay zeka tarafından oluşturulan mülk özetleri bulunmamaktadır; kullanıcıların ilan bilgilerini kendilerinin incelemesi gerekmektedir.
- Mülk ilanı üzerinde doğrudan kullanılabilen yapay zeka destekli soru-cevap özelliği bulunmamaktadır.
- Mülkler yapay zeka destekli bir karşılaştırma özelliğiyle otomatik olarak karşılaştırılamamaktadır.
- Kat planları ve EPC bilgileri standart belgeler olarak sunulmakta, yapay zeka tarafından açıklanmamaktadır.
- Google Maps/konum bilgisi sunulmaktadır ancak çevre veya ulaşım hakkında yapay zeka tarafından oluşturulan içgörüler bulunmamaktadır.
- İlgili mülkler kişiselleştirilmiş öneriler yerine standart listeleme mantığına göre gösterilmektedir.

## Değerleme

- Kullanıcıların ek destek talep edebileceği çevrim içi bir mülk değerleme/tahmin hizmeti bulunmaktadır.
- Web sitesinde Mortgage Calculator ve Stamp Duty Calculator araçları bulunmaktadır.
- Bu araçlar yalnızca sayısal hesaplama sonuçları sunmakta; kişiselleştirilmiş yapay zeka açıklamaları, ödeme gücü analizi veya öneriler sağlamamaktadır.

## İletişim

- Kullanıcılar mülk sayfalarında bulunan iletişim formları üzerinden acenteyle iletişime geçebilmektedir.
- Mülk görüntüleme talepleri de web sitesi üzerinden gönderilebilmektedir.
- Web sitesi, etkileşimli bir yapay zeka sohbet deneyiminden ziyade telefon ve iletişim formlarına dayalı bir iletişim yapısı kullanmaktadır.
- Belirgin bir yapay zeka destekli müşteri adayı nitelendirme veya mesai dışı iletişim desteği bulunmamaktadır.

## Teknik / Genel

- Web sitesi, modern bir Neuron yapısı üzerinde geliştirilmiş, profesyonel ve kullanıcı dostu bir arayüze sahiptir.
- Platformda mülk rehberleri, SSS içerikleri ve bölge rehberleri gibi destekleyici içerikler bulunmaktadır. Bu içerikler gelecekte geliştirilecek bir yapay zeka asistanı için bilgi kaynağı olarak kullanılabilir.
- Web sitesi mevcut destekleyici içeriklerini etkileşimli yapay zeka özellikleriyle aktif şekilde kullanmamaktadır.

**Durum:** Yapıldı

### Tur 2 — Görkem

**Arama:**
- Aynı toggle + zayıf filtreler; Medway (Rainham/Gillingham, 01634). Sonuç sayfasında doğrulandı: price min/max, 0–40mil yarıçap, min–max beds, sıralama Suggested/price/date; type yok, keyword yok, doğal dil yok, harita yok. "Setup Heads Up Alert" + "Register for Property Alerts".
- Jacksons on sitem içinde en zengin destek içeriğine sahip — guide'lar, FAQ'lar ve area guide'larla bir "Advice Hub". **Bu içerik yığını tam da tenant'a özel bir AI asistanının ihtiyaç duyacağı zemindir ve hiçbir interaktif özelliği beslemeden orada duruyor.** Bir Neuron asistanının neyi kaynak alması gerektiğine güçlü bir işaret.

**İlan Detay:**
- Canlı bir ilan açtım (Conqueror Drive, Gillingham): 20 fotoğraf, floorplan, video, bullet FEATURES + uzun anlatı, sağlam key facts (Guide £300–325k, 3 yatak / 3 banyo, Freehold, Council Tax C, EPC C/75, 807 sqft). Gerçekten iyi bir ilan sayfası.
- Ama yine AI özet yok, soru sorma yok ve "OUR LATEST PROPERTIES" bloğu en yeni, bana göre eşleştirilmiş değil. Yani gruptaki *en dolu* ilan bile aynı tavana çarpıyor.
- Detay sayfasında Mortgage + Stamp Duty hesaplayıcıları **var** — ama sadece rakam üreten, yorumsuz araçlar. **AI fırsatı (hafif):** hesaplayıcı çıktısının üstüne düz dilde bir affordability/sonraki-adım notu (aylık rakam ne anlama geliyor, depozito değişince ne oluyor).

**Değerleme:**
- Anlık "takip aramalı hızlı online tahmin" + yüz yüze. Aynı kapı-tutan kalıp — "tahmin" aslında geri arama için kanca.

**İletişim:**
- Telefon-öncelikli (ayrı Sales/Lettings hatları), ilanlarda "Make an Enquiry" tek tip form, chat yok, mesai dışı yok, kalifikasyon yok.

**Teknik/Genel:**
- Neuron/Iceberg, Vercel, Lifesycle S3.
- Güven güçlü (15+ yorum, isimli ekip, Propertymark/TPO). Ana sayfadaki "A Different Kind of Estate Agency" ifadesi **Property Connections (06) ile aynı şablon metni** — bu tenant'ların altında ne kadar çok paylaşılan iskelet olduğunun ve AI'nin neden platform seviyesine ait olduğunun bir başka teyidi.
- Doğrulanacak not: Ayselin'in Tur 1 bloğu sitede temel ilan sorularını yanıtlayan bir AI Chat Assistant olduğunu söylüyor; ben kendi gezimde böyle bir asistana rastlamadım. Canlı tekrar kontrol edilmeli — koşullu/sayfaya özel olabilir.

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

- **Doğal Dil Araması:** **Yok** — "3 bed with a garage under £400k in Rainham" → "Couldn't find the address". **Beş sitede beşinci kez.** (SS-02)
- **Akıllı Öneri / Sorgu Yorumlama:** **Kısmen — AI değil** — "rainam" doğru çözülüyor; öneriler Rainham Station, Rainham Mark Grammar School, Rainham (Kent) Station Car Park. Google Places, URL'de `place_id`. (SS-01, SS-03)
- **Kayıtlı Arama / Alerts:** **Var** — "Setup Heads Up Alert" sonuç başlığında. Kural tabanlı. (SS-03)
- **"100% MATCH" rozeti:** Sonuç kartlarında görülmedi — Keystone gibi, Property Connections'ın aksine. "SUGGESTED" ve "HAVE YOU LOGGED IN?" duruyor. (SS-03)
- Filtreler diğer sitelerle aynı set. (SS-05)

## **İlan Detay:**

İncelenen: `/properties/3-bedroom-house-.../535188` (Whitehorse Hill, Chatham)

- **Property Summary (AI Özet):** **Yok** — Elle yazılmış düz metin. (SS-07)
- **Property Q&A:** **Yok**
- **Property Highlights:** **Kısmen — manuel** — Features listesi elle girilmiş ama **EPC Rating E (50)** ve **Medway Council Tax B** madde olarak veriliyor; alıcı için doğrudan kullanışlı. (SS-07)
- **Lifestyle Eşleştirme:** **Kısmen** — "ideally suited for a growing family or as an investment" serbest metinde.
- **Property Comparison:** **Yok**
- **Benzer İlan Önerisi:** **Yok** — Kenar çubuğunda oklarla gezilen bir **"son ilanlar" karuseli** var, benzerlik değil kronoloji. ⚠️ Kaynak koddan bakıldığında en az bir ilanda (Grain Road) karusel **o an açık olan ilanı ilk kart olarak** listeliyor. (SS-08)
- **Area Insights:** **Kısmen** — Sitede ayrı bir **Area Guides** bölümü var ama **ilan detayından oraya link yok**. *(Rehberlerin içeriği test edilmedi.)*
- **Commute Insights:** **Kısmen — manuel** — "Close to Chatham mainline station" madde olarak var, süre hesabı yok.
- **Belge Açıklama:** **Yok** — Floor Plan ve EPC sadece görsel.
- **Stamp Duty Calculator:** **Var** — İngiltere'de doğru vergi, "Buying my first home" seçicisi ile. (SS-08)
- **Mortgage Calculator:** **Var** — Fiyatla önceden doldurulmuş, %10 depozito, %6,01 faiz, 25 yıl. Salt aritmetik, yorum yok. (SS-08)
- **Ek not:** Bölümler akordeon değil **sekme** (Description / Video / Floor Plan / Map / EPC) — Keystone'un gizlenen akordeonundan iyi. (SS-07)
- **Ek not:** Video Vimeo'da, danışman anlatımlı ("Mark Jackson"). Ana sayfada "Jacqui B Videos" imza formatı olarak tanıtılıyor.

## **Değerleme:**

- **Instant Valuation:** **Var — 3. parti, dördüncü kez ValPal.** `valuation.jacksonsproperty.co.uk/home/2488`, altında "Powered by The ValPal Network". Ayrı subdomain, ayrı çerez banner'ı. **Type of Valuation** dropdown'ı ile kiralama değerlemesi de sunuyor. (SS-11)
- **AI Valuation Açıklaması:** **Yok**
- ⚠️ **Ek not — acente aracın yetersizliğini kendi kabul ediyor:** Ana sayfa instant valuation için *"it's just a starting point. We'll follow up with a friendly call to understand your plans and offer real, tailored advice"* diyor. Yani araç bilinçli olarak eksik bırakılmış ve telefon aramasına bağlanmış. AI destekli, gerekçeli değerleme gap'i için en net kanıt.
- **Ek not:** Face-to-face formu **satış/kiralama ayrımı yapıyor**: "I am looking to sell / to let / considering both" + oda sayısı. Kiralama farkındalığı olan tek değerleme formu. Yine de takvim/slot yok. (SS-10)

## **İletişim / Lead:**

- **Chatbot:** **Yok (görünürde)** — Hiçbir ekranda widget yok. Ancak kaynak kodda **iki ayrı iz** var:
  - `.whatsapp-chatbot` sınıfı — **dört sitede dördüncü kez**, yine kapalı.
  - ⚠️ **`https://cdn.msgboxx.io/static/css/bundle.min.css`** — üçüncü parti bir mesajlaşma platformunun CSS'i. **Bu çalışmada ilk kez görülüyor.** Widget ekranlarda çıkmadı; yüklü ama pasif mi, yoksa belirli koşullarda mı açılıyor, doğrulanmalı. (SS-17)
- **Lead Qualification:** **Kısmen — manuel** — Heads Up kaydı diğer sitelerle aynı Circumstances seti. Dallanma yok. (SS-04)
- **Otomatik Randevu:** **Yok** — "MAKE AN ENQUIRY" modalında takvim ve saat seçici var, ama üstünde *"We'll confirm availability for you. (This does not confirm the viewing)"* yazıyor. Keystone'daki desenin aynısı; tek farkı burada müsaitlik ikinci kez yazıyla sorulmuyor. (SS-14)
- **Mesai Dışı Yanıt:** **Yok** — Otomatik yanıt kanalı yok. Açılış saatleri yayınlanmış: Pzt–Cum 9:00–18:00, Cmt 9:00–17:00, **Pazar "BY APPOINTMENT"**. (SS-12)
- **Ek not:** Enquiry modalı aynı zamanda lead formu — kendi adresi, "property to sell", "property to let", "my property valued". (SS-15)
- **Ek not:** İki ayrı telefon (Sales …37 / Lettings …38) her sayfanın üstünde. Hangisini arayacağına kullanıcı karar veriyor, yönlendirme yok.

## **Teknik / Genel:**

- **SSR vs CSR:** **SSR** — `filter?search_type=` çağrısı yok, liste HTML'de. Nuxt (`/_nuxt/`). 
- **API çağrıları:** `ice.js` (Iceberg tracker), 3× Sentry, `view`. **AI/LLM çağrısı yok.** 6/107 istek, 246 kB, **2,07 sn — çalışmadaki en hızlı site.** 
- **Tema / 3. parti:** `neuron.css` + `theme3` + Bootstrap/Owl/FontAwesome, ayrıca **msgboxx.io**. 
- **Mobil:** **Sorunsuz** — 400px'te arama, fiyat, oda ve filtreler düzgün yığılıyor. 
- ✅ **İletişim haritası doğru** — Rainham'daki şubeyi doğru gösteriyor (Property Connections'ta yanlış ülkeydi). 
- ✅ **Footer temiz** — tek blok, Company Number doğru (040 158 04), NaN yok. Yalnızca telif **© 2025** (site 2026'da canlı). 


**Durum:** Yapılmadı

### Ortak Bulgular / Sentez (4 tur bitince doldurulur)

- Ortak eksik AI özellikleri: Doğal dil arama, AI ilan özeti, Property Q&A (bkz. görüş ayrılığı), AI lead scoring.
- Öne çıkan fırsatlar: (1) "Advice Hub" (rehberler, SSS, alan rehberleri) bu çalışmadaki en zengin destekleyici içerik — bir AI asistanının besleneceği hazır kaynak, hiçbir interaktif özellikte kullanılmıyor. (2) Mortgage + Stamp Duty hesaplayıcıları var ama sadece sayısal — üstüne sade dilde yorum eklenebilir (düşük efor, orta etki). (3) Değerleme aracını acentenin kendisi "sadece başlangıç noktası" diye tanımlaması — AI açıklama katmanı için en net kanıt.
- Görüş ayrılıkları / doğrulananlar: ✅ **Yasemin tarafından doğrulandı (canlı kontrol, Ağustos 2026):** Round 1 (Ayselin) bir AI chat asistanı gördüğünü, Round 2 (Görkem) görmediğini yazmıştı. **Görkem'in gözlemi doğrulandı.** Konsolda `document.querySelector('.whatsapp-chatbot')` → `null` dönüyor; yani bileşen DOM'a hiç basılmıyor. `/valuations`, `/contact-us`, ilan arama sayfası ve mobilde (iPhone 15, 393px) hiçbir chat balonu yok, Network'te msgboxx'a giden tek bir istek bile yok (6/130 request: ice.js, 3× Sentry envelope, 1× view). `cdn.msgboxx.io` izi kaynakta duruyor ama çalışan entegrasyon yok — ölü kod.
**09 · Harris + Wood (theme7) ve 10 · Roderick Thomas (theme8) ile çapraz karşılaştırıldığında:** Jacksons `theme3` kullanıyor (konsol hatası: `/theme3/css/neuron/applicants.css`). Üç farklı tema jenerasyonunun üçünde de `.whatsapp-chatbot` CSS'i mevcut, üçünde de ekranda balon yok. `cdn.msgboxx.io` bundle'ı Jacksons ve Harris + Wood'da yüklü, Roderick Thomas'ta değil — ama yüklü olduğu iki sitede de bileşen render edilmiyor. Bu, WhatsApp chatbot'un tema seviyesinde taşınan, hiçbir tenant'ta aktifleştirilmemiş bir özellik olduğunu gösteriyor. Ayselin'in gözlemi muhtemelen başka bir öğeyle (CTA/iletişim widget'ı) karışmış.
**Ek doğrulama:** Instant valuation ayrı subdomain'de (`valuation.jacksonsproperty.co.uk/home/2488`) ve `/valuations` sayfası aracı açıkça *"it's just a starting point"* diye tanımlayıp *"we'll follow up with a friendly call"* diyor — AI açıklama katmanı yerine insan geri dönüşüne bağlanıyor. 10 · Roderick Thomas'ta da aynı desen (ayrı subdomain + acentenin kendi aracına güvenmediğini yazması) görüldüğü için bu tek siteye özgü bir tercih değil, platform davranışı.