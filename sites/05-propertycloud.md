# 05 · thepropertycloud.uk

**URL:** https://thepropertycloud.uk/
**Group / Grup:** A

---

## English

This site is reviewed independently by 4 people across 4 rounds.

| Round | Reviewer | Status |
|---|---|---|
| 1 | Görkem | Done |
| 2 | Berkay | Done |
| 3 | Yasemin | Done |
| 4 | Ayselin | Done |

> Fill in only your own round block; don't edit anyone else's.
> Write short, concrete sentences (not "yes/no" — say what it is).
> What to check: ../checklist.md · Terms: ../info/ai-feature-glossary.md

### Round 1 — Görkem

**Search:**
- Same Buy/Rent toggle + thin filters. Their whole positioning is "Property Marketing, Done Properly" — i.e. photography and video quality — so search was clearly never the priority, and it shows: it's the untouched platform default (price/beds/radius, no type, no free text, no map).

**Listing Detail:**
- Standard Neuron template. Their genuine edge is production quality, so on a listing that (sometimes) means a proper video — but structurally it's the same page as the rest: bullet features + hand-written narrative, no AI summary, no ask-a-question, area info as prose.
- Worth flagging: if a tenant invests in great photos/video, an **image-aware highlight/summary** (auto-tagging standout features from the media) would let that investment do double duty. Realistic, but I'd rank it a nice-to-have, not a priority.

**Valuation:**
- Instant tool + book, and they're refreshingly blunt about it: instant "up to 60% accurate", in-person "up to 100%". Same gated lead-capture pattern as the others behind the honest framing.

**Contact:**
- Email only on the homepage (`sales@` / `lettings@`), no phone shown — more friction than the phone-first tenants. No chat, no out-of-hours.

**Technical / General:**
- Neuron/Iceberg, Vercel, Lifesycle CDN.
- Named, recently-dated reviews and ethical-agent badges give reasonable trust, but with no phone number up front it leans a bit impersonal for a high-emotion purchase. Modern-looking, but the polish is all in the marketing shell, not the discovery flow.

**Status:** Done

### Round 2 — Berkay

## **Search:**

- **Natural Language Search:** **Absent** — Property search uses structured Buy/Rent controls, price and bedroom filters rather than free-sentence queries.
- **Smart Suggestions / Query Understanding:** **Absent** — Every listing shows a "100% MATCH" badge, with no variation across price, beds, or listing status (anonymous visitor, no saved criteria). This is the same Neuron/Iceberg Digital platform used across this group of sites. A fixed 100% regardless of profile points to a static UI label, not real AI matching — vendor branding alone doesn't confirm otherwise.
- **Saved Search / Alerts:** **Present** — Property Alerts allow buyers and tenants to register their requirements and receive tailored updates when suitable properties become available. The site specifically promotes access to properties before they appear on the main portals.

## **Listing Detail:**

- **Property Summary (AI):** **Absent** — Listings contain property descriptions and structured information, but no AI-generated 2–3 point summary was observed.
- **Property Q&A:** **Absent** — No free-form AI Q&A for individual properties was observed.
- **Property Highlights:** **Partial** — Listings contain concise feature information and descriptive titles, but there is no evidence that these highlights are AI-generated.
- **Lifestyle / "Ideal for…" Matching:** **Partial** — Listings can contain suitability statements such as "Ideal First Time Purchase" and references to schools, transport and local amenities. No explicit AI-generated lifestyle commentary was observed.
- **Property Comparison:** **Absent** — No AI-powered comparison of two or more listings was observed.
- **Similar Listings (personalised):** **Present** — The Neuron matching system connects registered buyer requirements with suitable properties and exposes match percentages on property results. As with Smart Suggestions above, this rests on vendor description plus the observable match-% indicator, not confirmed backend inspection.
- **Area Insights:** **Partial** — Property descriptions include information about nearby schools, shops, transport and local amenities. The site also provides local guides, but no AI-generated neighbourhood analysis covering demographics, crime or similar data was observed.
- **Commute Insights:** **Partial** — Listings mention nearby stations, DLR/Elizabeth Line links and other transport connections, but there is no personalised commute-time analysis based on a user's workplace or school.
- **Document Explanation (EPC / Floor Plan):** **Absent** — EPCs and floor plans can be part of listing information, but no AI-powered explanation of these documents in plain language was observed.

## **Valuation:**

- **Instant Valuation:** **Present** — The site provides a 24/7 instant online valuation tool that gives a quick estimate of what a property may be worth. The site states that the instant tool can be up to 60% accurate.
- **AI Valuation Explanation:** **Absent** — The instant valuation provides an estimated figure but does not provide an AI-generated explanation or personalised breakdown of the factors behind the valuation.
- **Mortgage / Stamp Duty Calculator:** **Absent** — No dedicated mortgage or Stamp Duty calculator with AI financial commentary was observed.

## **Contact:**

- **AI Chat Assistant / Chatbot:** **Absent** — No site-wide or listing-level AI chat assistant was observed.
- **Lead Qualification:** **Partial** — Buyer and tenant registration through Property Alerts collects user requirements and search preferences, allowing the agency to understand what type of property the lead is looking for. No AI-powered lead scoring or prioritisation was observed.
- **Automated Booking / Viewing Scheduling:** **Partial** — Properties provide viewing/contact options and the agency promotes flexible viewing arrangements, but no AI-driven booking or conversational scheduling system was observed.
- **Out-of-hours Response:** **Partial** — The instant valuation is available 24/7 and Property Alerts operate continuously, but no AI-powered out-of-hours conversational response system was observed.

## **Technical / General:**

- **SSR vs CSR:** **Hybrid (SSR + CSR)** — Initial page load is server-side rendered, with core property and content information present directly in the delivered HTML. Client-side hydration then takes over for interactive elements and further navigation. 
- **API calls:** **Partial** — The property search and matching functionality clearly uses external/property-platform infrastructure, but the specific runtime API endpoints were not confirmed through Network-tab inspection, and unlike sites 22/23 the platform is not explicitly self-identified as Neuron/Iceberg Digital.
- **Mobile behaviour:** **Present** — The responsive site provides access to property search, listings, alerts, valuation and contact forms on mobile.


**Status:** Done

### Round 3 — Yasemin

## **Search:**

- **Natural Language Search:** **No** — Typing a free-form sentence ("3 bed near a station under £450k chain free") returns "Couldn't find the address". The box is an address field, not a property-intent field.
- **Smart Suggestions / Query Interpretation:** **Partial** — Typo tolerance works ("bexlyheath" → "Bexleyheath"), but this is Google Places autocomplete, not Neuron AI. The URL carries `place_id: ChIJM4rYYiWu2EcRUiodCtnqA5Q` and the dropdown returns POIs like "Bexleyheath Clock Tower" and "Bexleyheath Police Station".
- **Saved Search / Alerts:** **Yes** — "Heads Up Property Alerts" offers criteria-based registration. The page promises alerts on suggested properties and price reductions, but matching is rule-based; no evidence of AI interpretation or behavioural learning.
- **Additional note:** The default sort is labelled **"Suggested"** and cards carry a **"100% MATCH"** badge, but every card shows 100% while logged out — with a "HAVE YOU LOGGED IN?" button sitting next to it. The personalisation promise exists in the UI with nothing behind it for anonymous users.
- **Additional note:** Filters are entirely conventional dropdowns — Bathrooms, Reception, Include SSTC, New Homes, Retirement Homes, Shared Ownership, Investment Property, Must Haves, Property Type (Detached / Semi-Detached / Terraced / Flats / Bungalow / Land / Park Home).

## **Listing Detail:**

- **Property Summary (AI Summary):** **No** — Property Info is one long hand-written block of prose. No 2–3 bullet summary at the top.
- **Property Q&A:** **No** — No channel for asking free-form questions. The only routes are "Book a viewing" or the contact form.
- **Property Highlights:** **Partial** — A Features tab exists, entered by hand at listing creation. Not AI-extracted.
- **Lifestyle / "Ideal for..." Matching:** **Partial** — Phrases like "young family" and "first purchase" appear inside the free text, but there is no structured lifestyle matching.
- **Property Comparison:** **No** — No comparison or favourites function on cards or detail pages.
- **Similar Listing Suggestions:** **No** — No similar-listings block at the bottom; the space is used for "Why buy with us" and an alerts CTA instead.
- **Area Insights:** **Partial** — School names, walking distances, Council Tax band and high street info are present but hand-written as prose. No structured neighbourhood data (crime, demographics, school ratings) and no AI commentary.
- **Commute Insights:** **Partial** — Station walk times and the "301 bus to Abbey Wood for the Elizabeth Line" are written into the description as fixed text. Travel time is never calculated against the user's own destination.
- **Document Explanation (EPC / Floor Plan):** **No** — Floor Plans are images only; the EPC tab exists but loads empty. No plain-language explanation.
- **Additional note:** The listing detail includes **Property Video and Virtual Tour as separate tabs** alongside Features, Property Info, Floor Plans, Map and EPC — rich media is there, the AI layer over it is not.
- **Additional note:** The right-hand sidebar card renders a broken-image icon across multiple tabs (Property Info, Virtual Tour) — a live rendering fault.
- **Additional note:** The same listing's Instagram post (@jordanevans_thepropertycloud) is written from scratch a second time. Site copy, social copy and portal copy are all produced manually from the same source data.

## **Valuation:**

- **Instant Valuation:** **Yes — but third-party** — Hosted on the `valuation.thepropertycloud.uk` subdomain and marked **"Powered by The ValPal Network"**. Visually disconnected from the main site. Inputs: postcode → Find Address, Number of Bedrooms, Property Type, Type of Valuation. The homepage itself advertises it as "Up to 60% accurate".
- **AI Valuation Explanation:** **No** — No reasoning behind the figure, no comparable sales, no personalisation.
- **Mortgage / Stamp Duty Calculator:** **No** — Not present on listing details or the buyer pages.
- **Additional note:** The face-to-face route (`/valuations/book-a-face-to-face-valuation`) is a plain lead form — name, postcode lookup, phone, email, consent checkbox. No calendar or slot selection, so it submits a request rather than booking anything.

## **Contact / Lead:**

- **AI Chat Assistant / Chatbot:** **No** — No chat widget on any page; the bottom-right corner is empty on home, search, listing detail and contact. **However**, the page source defines a `.whatsapp-chatbot` class with `--wa-green`, `--wa-header-bg`, `--wa-bubble-bg`, `--wa-chat-bg` and `--wa-input-bg` variables. The Neuron platform ships a WhatsApp chatbot component that this agency has not switched on.
- **Lead Qualification:** **Partial** — The Heads Up Alerts registration has a "Circumstances" section (reason for buying, moving timeline, solicitors arranged, how you heard about us). Qualification data is collected, but the form is identical for everyone — no branching, prioritisation or AI pre-screening.
- **Automated Appointment / Viewing Scheduling:** **No** — "Book a viewing" and the valuation forms show no availability; they submit a request.
- **Out-of-Hours Response:** **No (as far as observable)** — There is no channel capable of an automatic reply: no chat, WhatsApp not enabled. Outside working hours the only option is to submit a form and wait.
- **Additional note:** The contact form is single-type — first name, last name, mobile, email, a Buy/Sell/Rent/Let checkbox row and a free-text message. The form does not change based on that selection.

## **Technical / General:**

- **SSR vs CSR:** **SSR** — `/_nuxt/` bundles in the source confirm **Nuxt (Vue)**, deployed on Vercel (`/_vercel/image` for image optimisation). The property list arrives inside the HTML rather than via a separate XHR.
- **API calls:** No visible Neuron data API in Fetch/XHR. What appears: an `anonymous` call from `ice.js` (Iceberg tracker), three `envelope/?sentry_version=7...` requests (Sentry error tracking), plus `log_event?alt=json` and `id` (analytics). **No request to any AI/LLM service.**
- **Iceberg traces:** The source defines `window.IcebergTracker` and `__akyaCookieStarted`; assets are served from `files.thepropertycloud.neuronwebsites.co.uk` and `lifesycle-cdn.s3.eu-west-2.amazonaws.com` — Iceberg/Lifesycle CRM infrastructure.
- **Mobile behaviour:** **Fine** — At 400px the filters stack vertically and search and buttons remain usable. Page finishes in 4.60s, ~295 kB transferred.

**Status:** Done

### Round 4 — Ayselin

## **Search:**

- **Natural Language Search:** **Absent** — The website follows the same Buy/Rent and basic-filter structure used across the platform. Users can search using price and bedroom criteria, but there is no free-text search, keyword input, property-type filter or map-based discovery. The agency positions itself around “Property Marketing, Done Properly,” with a strong emphasis on photography and video rather than search functionality, so the discovery experience remains largely unchanged from the platform default.

- **Smart Suggestions / Query Understanding:** **Absent** — Every listing displays a “100% MATCH” badge, with no meaningful variation across price, bedroom count or listing status for an anonymous visitor without saved criteria. This strongly suggests a static or rule-based UI element rather than genuine AI-powered matching. The presence of Neuron/Iceberg Digital branding alone does not confirm that the visible match percentage is AI-driven.

- **Saved Search / Alerts:** **Present** — Property Alerts allow buyers and tenants to register their requirements and receive updates when suitable properties become available. The service also promotes access to properties before they appear on major property portals.

---

## **Listing Detail:**

- **Property Summary (AI):** **Absent** — Listings contain manually written descriptions and structured property information, but no AI-generated 2–3 point summary was observed.

- **Property Q&A:** **Absent** — No free-form AI assistant for answering questions about individual properties was observed.

- **Property Highlights:** **Partial** — Listings include concise features and descriptive titles, but these appear to be manually created rather than AI-generated.

- **Lifestyle / "Ideal for…" Matching:** **Partial** — Some listings include suitability statements such as “Ideal First Time Purchase” and mention schools, transport and local amenities. However, there is no AI-generated personalised lifestyle analysis.

- **Property Comparison:** **Absent** — No AI-powered comparison feature was observed for comparing multiple listings.

- **Similar Listings (personalised):** **Present** — The matching system connects registered buyer requirements with suitable properties and exposes match percentages in property results. However, as with Smart Suggestions, the visible match percentage was not verified through backend inspection and appears to rely on the same platform-level matching infrastructure.

- **Area Insights:** **Partial** — Property descriptions provide information about nearby schools, shops, transport and local amenities. Local guides are also available, but there is no AI-generated neighbourhood analysis covering factors such as demographics, crime, amenities or lifestyle suitability.

- **Commute Insights:** **Partial** — Listings mention nearby stations and transport connections, including DLR and Elizabeth Line links, but there is no personalised commute-time analysis based on the user's workplace or school.

- **Document Explanation (EPC / Floor Plan):** **Absent** — EPCs and floor plans may be included with listings, but there is no AI-powered feature that explains these documents in plain language.

- **AI / Media Opportunity:** **Partial** — The agency's strongest differentiator is the quality of its photography and video marketing. An image-aware AI feature could automatically identify and highlight visual characteristics such as large gardens, renovated kitchens, period features or natural light. This could turn existing media investment into additional searchable and summarised property data. However, this would be a secondary opportunity rather than a core priority.

---

## **Valuation:**

- **Instant Valuation:** **Present** — The website provides a 24/7 instant online valuation tool that gives users a quick estimate of what their property may be worth. The site states that the instant valuation can be up to 60% accurate.

- **AI Valuation Explanation:** **Absent** — The instant valuation provides an estimated figure but does not explain the result through an AI-generated narrative or personalised breakdown of the factors behind the estimate.  
  **AI opportunity:** The valuation could be made more useful by explaining comparable properties, local market conditions and property characteristics instead of presenting the estimate as a standalone number.

- **Mortgage / Stamp Duty Calculator:** **Absent** — No dedicated mortgage or Stamp Duty calculator with AI-generated financial commentary was observed.

---

## **Contact:**

- **AI Chat Assistant / Chatbot:** **Absent** — No site-wide or property-level AI chat assistant was observed.

- **Lead Qualification:** **Partial** — Property Alerts collect buyer and tenant requirements and search preferences, giving the agency structured information about what each lead is looking for. However, there is no AI-powered lead scoring, qualification or prioritisation.

- **Automated Booking / Viewing Scheduling:** **Partial** — Property pages provide viewing and contact options, and the agency promotes flexible viewing arrangements. However, no AI-driven booking system or conversational scheduling assistant was observed.

- **Out-of-hours Response:** **Partial** — The instant valuation is available 24/7 and Property Alerts operate continuously, but there is no AI-powered conversational system handling customer questions outside business hours.

---

## **Technical / General:**

- **SSR vs CSR:** **Hybrid (SSR + CSR)** — The initial page load is server-side rendered, with core property and content information available directly in the delivered HTML. Client-side JavaScript then handles interactive elements and further navigation.

- **API calls:** **Partial** — Property search and matching functionality clearly relies on external or property-platform infrastructure. However, the specific runtime API endpoints were not confirmed through Network-tab inspection, and the website does not explicitly identify the platform as Neuron/Iceberg Digital in the same way as some other sites in the group.

- **Mobile behaviour:** **Present** — The responsive website provides access to property search, listings, alerts, valuation and contact functionality on mobile devices.

- **Overall UX:** **Good** — The website's main strength is its visual presentation and property marketing quality. Photography, video and professionally presented listings create a strong first impression. However, the underlying property discovery experience remains relatively basic and does not fully benefit from the quality of the media content.

- **AI Opportunity:** **Medium–High** — The strongest opportunities are not necessarily generic AI features but improvements that build on the agency's existing strengths. Image-aware property highlights, AI-generated summaries, natural-language search and smarter matching could turn high-quality property media into richer and more useful discovery data. AI valuation explanations would also improve transparency without replacing the human valuation service.

---

**Status:** Done

### Findings / Synthesis (filled once all 4 rounds are done)

- Commonly missing AI features: Natural-language search, AI listing summaries, Property Q&A, AI lead scoring, out-of-hours automated response, EPC/floor plan explanation.
- Standout opportunities: (1) Strong investment in photography/video (Giraffe360 tours, drone video) — an image-aware AI layer could auto-extract standout features (garden, renovated kitchen, etc.). (2) The same content (site copy, social media, portal listing) is written from scratch three times — a clear automation opportunity to generate multiple formats from one source.
- Disagreements / to verify: A live rendering fault was found (broken-image icon across multiple tabs) — worth re-checking. The "100% MATCH" badge shows the same fake-100% pattern here too — confirmed as a platform-wide issue.

---

## Türkçe

Bu siteyi 4 tur boyunca 4 farklı kişi bağımsız inceler.

| Tur | İnceleyen | Durum |
|---|---|---|
| 1 | Görkem | Yapıldı |
| 2 | Berkay | Yapıldı |
| 3 | Yasemin | Yapıldı |
| 4 | Ayselin | Yapıldı |

> Sadece kendi tur bloğunuzu doldurun; başkasının bloğunu değiştirmeyin.
> Kısa, somut cümleler yazın ("Var/Yok" değil, ne olduğunu yazın).
> Neye bakılacağı: ../checklist.md · Terimler: ../info/ai-feature-glossary.md

### Tur 1 — Görkem

**Arama:**
- Aynı Buy/Rent toggle + zayıf filtreler. Tüm konumlanması "Property Marketing, Done Properly" — yani fotoğraf ve video kalitesi — dolayısıyla arama hiç öncelik olmamış ve belli oluyor: dokunulmamış platform varsayılanı (price/beds/radius, type yok, serbest metin yok, harita yok).

**İlan Detay:**
- Standart Neuron şablonu. Gerçek üstünlükleri prodüksiyon kalitesi, o yüzden bir ilanda bu (bazen) düzgün bir video demek — ama yapısal olarak sayfa geri kalanla aynı: bullet features + elle yazılmış anlatı, AI özet yok, soru sorma yok, bölge bilgisi düz yazı.
- Not: bir tenant iyi foto/videoya yatırım yapıyorsa, **görsele duyarlı highlight/özet** (medyadan öne çıkan özellikleri otomatik etiketleme) bu yatırımı iki kat işe yaratırdı. Gerçekçi, ama önceliğe değil nice-to-have'e koyarım.

**Değerleme:**
- Anlık araç + randevu, ve bu konuda ferahlatıcı derecede açık sözlüler: anlık "up to 60% accurate", yüz yüze "up to 100%". Dürüst çerçevenin ardında diğerleriyle aynı kapı-tutan lead-capture kalıbı.

**İletişim:**
- Ana sayfada sadece e-posta (`sales@` / `lettings@`), telefon gösterilmiyor — telefon-öncelikli tenant'lardan daha fazla sürtünme. Chat yok, mesai dışı yok.

**Teknik/Genel:**
- Neuron/Iceberg, Vercel, Lifesycle CDN.
- İsimli, yeni tarihli yorumlar ve ethical-agent rozetleri makul güven veriyor, ama önde telefon numarası olmayınca yüksek-duygulu bir alım için biraz mesafeli kalıyor. Modern görünüyor, ama cila tamamen pazarlama kabuğunda, keşif akışında değil.

**Durum:** Yapıldı

### Tur 2 — Berkay

## **Arama:**

- **Doğal Dil Araması:** **Yok** — Mülk araması yapılandırılmış Satın Alma/Kiralama kontrolleri, fiyat ve oda filtrelerini kullanıyor; serbest cümleyle arama bulunmuyor.
- **Akıllı Öneriler / Sorgu Anlama:** **Yok** — Her ilanda "100% MATCH" rozeti görünüyor; fiyat, oda sayısı veya ilan durumu fark etmeksizin hiç değişmiyor (anonim ziyaretçi, kayıtlı kriter yok). Bu, gruptaki diğer sitelerle aynı Neuron/Iceberg Digital altyapısı. Profilden bağımsız sabit %100, gerçek bir AI eşleştirmesinden çok statik bir UI etiketine işaret ediyor — sadece marka ismi bunun aksini kanıtlamıyor.
- **Kayıtlı Arama / Uyarılar:** **Var** — Mülk Uyarıları ile alıcılar ve kiracılar ihtiyaçlarını kaydedebiliyor ve uygun yeni mülkler hakkında kişiselleştirilmiş bildirimler alabiliyor. Site, bazı mülklerin büyük portallarda yayınlanmadan önce alıcılara ulaştırılabildiğini belirtiyor.

## **İlan Detay:**

- **Mülk Özeti (YZ):** **Yok** — İlanlarda mülk açıklamaları ve yapılandırılmış bilgiler bulunuyor; ancak yapay zeka tarafından oluşturulan 2–3 maddelik özet gözlemlenmedi.
- **Mülk Soru-Cevap:** **Yok** — İlan hakkında serbest biçimde soru sorulabilen yapay zeka destekli Q&A özelliği gözlemlenmedi.
- **Mülkün Öne Çıkan Özellikleri:** **Kısmi** — İlanlarda kısa özellik bilgileri ve açıklayıcı başlıklar bulunuyor; ancak bunların yapay zeka tarafından oluşturulduğuna dair kanıt bulunmuyor.
- **Yaşam Tarzı / "... için ideal" Eşleştirmesi:** **Kısmi** — İlanlarda "Ideal First Time Purchase" gibi uygunluk ifadeleri ve okul, ulaşım ve yerel olanaklara ilişkin bilgiler bulunabiliyor. Ancak açık bir AI yaşam tarzı yorumu bulunmuyor.
- **Mülk Karşılaştırma:** **Yok** — İki veya daha fazla mülkü yapay zeka ile karşılaştırma özelliği gözlemlenmedi.
- **Benzer İlanlar (kişiselleştirilmiş):** **Var** — Neuron matching sistemi, kayıtlı alıcı gereksinimlerini uygun mülklerle eşleştiriyor ve ilan sonuçlarında eşleşme yüzdeleri gösteriyor. Yukarıdaki Smart Suggestions maddesinde olduğu gibi, bu değerlendirme satıcı tanımı ile gözlemlenebilir eşleşme yüzdesine dayanıyor; arka planda doğrudan doğrulama yapılmadı.
- **Bölge İçgörüleri:** **Kısmi** — İlan açıklamalarında okul, mağaza, ulaşım ve yerel olanaklar hakkında bilgiler bulunuyor. Site ayrıca yerel rehberler sunuyor; ancak demografi, suç oranı ve benzeri verileri yapay zeka ile analiz eden özel bir bölge içgörü sistemi bulunmuyor.
- **Ulaşım İçgörüleri:** **Kısmi** — İlanlarda istasyonlar, DLR/Elizabeth Line ve diğer ulaşım bağlantılarından bahsediliyor; ancak kullanıcının iş veya okul konumuna göre kişiselleştirilmiş ulaşım süresi analizi bulunmuyor.
- **Belge Açıklaması (EPC / Kat Planı):** **Yok** — EPC ve kat planları ilanlarda bulunabiliyor; ancak bunları sade bir dille açıklayan yapay zeka özelliği gözlemlenmedi.

## **Değerleme:**

- **Anlık Değerleme:** **Var** — Site 7/24 kullanılabilen anlık online değerleme aracı sunuyor. Araç mülkün tahmini değerini hızlı şekilde gösteriyor ve site instant valuation için %60'a kadar doğruluk belirtiyor.
- **Yapay Zeka Değerleme Açıklaması:** **Yok** — Anlık değerleme bir tahmin sunuyor ancak değerin arkasındaki faktörleri açıklayan yapay zeka destekli veya kişiselleştirilmiş bir analiz bulunmuyor.
- **Mortgage / Damga Vergisi Hesaplayıcısı:** **Yok** — yapay zeka destekli finansal yorum içeren özel bir mortgage veya Stamp Duty hesaplayıcısı gözlemlenmedi.

## **İletişim:**

- **Yapay Zeka Sohbet Asistanı / Chatbot:** **Yok** — Site genelinde veya ilan seviyesinde yapay zeka destekli sohbet asistanı gözlemlenmedi.
- **Müşteri Adayı Nitelendirme:** **Kısmi** — Buyer ve tenant Mülk Uyarısı kayıtlarında kullanıcının ihtiyaçları ve arama tercihleri toplanıyor. Bu, müşteri adayının hangi tip mülkü aradığını anlamaya yardımcı oluyor; ancak yapay zeka destekli müşteri adayı puanlama veya önceliklendirme bulunmuyor.
- **Otomatik Rezervasyon / Görüntüleme Planlama:** **Kısmi** — İlanlarda viewing/iletişim seçenekleri bulunuyor ve ajans esnek viewing düzenlemelerini öne çıkarıyor; ancak yapay zeka destekli rezervasyon veya konuşma tabanlı randevu sistemi gözlemlenmedi.
- **Mesai Dışı Yanıt:** **Kısmi** — Anlık değerleme 7/24 kullanılabiliyor ve Mülk Uyarıları sürekli çalışıyor; ancak yapay zeka destekli mesai dışı konuşma/yanıt sistemi bulunmuyor.

## **Teknik/Genel:**

- **SSR ve CSR:** **Hibrit (SSR + CSR)** — İlk sayfa yüklemesi sunucu tarafında render ediliyor; temel ilan ve içerik bilgileri doğrudan teslim edilen HTML içinde yer alıyor. Ardından etkileşimli öğeler ve sonraki gezinmeler için istemci tarafı hydration devreye giriyor. 
- **API Çağrıları:** **Var** — Site açıkça Neuron / Iceberg Digital'in "Estate Agentlar için Yapay Zeka İşletim Sistemi" altyapısını kullanıyor. Property search sonuçlarında yapay zeka eşleştirme sistemi yüzde bazlı eşleşme göstergeleriyle görünür durumda. 
- **Mobil Davranış:** **Var** — Responsive site üzerinden mülk arama, ilanlar, alertler, değerleme ve iletişim özelliklerine mobil erişim sağlanıyor.

**Durum:** Yapıldı

### Tur 3 — Yasemin

## **Arama:**

- **Doğal Dil Araması:** **Yok** — Serbest cümle ("3 bed near a station under £450k chain free") yazıldığında "Couldn't find the address" hatası dönüyor. Kutu bir adres alanı, emlak niyeti alanı değil.
- **Akıllı Öneri / Sorgu Yorumlama:** **Kısmen** — Yazım hatası toleransı çalışıyor ("bexlyheath" → "Bexleyheath"), ama bu Neuron'un AI'ı değil Google Places autocomplete. URL'de `place_id: ChIJM4rYYiWu2EcRUiodCtnqA5Q` taşınıyor ve önerilerde "Bexleyheath Clock Tower", "Bexleyheath Police Station" gibi POI'ler çıkıyor.
- **Kayıtlı Arama / Alerts:** **Var** — "Heads Up Property Alerts" kriter bazlı kayıt sunuyor. Sayfa, önerilen ilanlar ve fiyat düşüşleri için bildirim vaat ediyor; ancak eşleşme kural tabanlı, AI yorumu veya davranışa göre öğrenme kanıtı yok.
- **Ek not:** Varsayılan sıralama **"Suggested"** ve kartlarda **"100% MATCH"** rozeti var, ama giriş yapılmadan tüm kartlar %100 gösteriyor — yanında da "HAVE YOU LOGGED IN?" butonu duruyor. Kişiselleştirme vaadi arayüzde var, anonim kullanıcıda arkasında bir şey yok.
- **Ek not:** Filtreler tamamen klasik dropdown — Bathrooms, Reception, Include SSTC, New Homes, Retirement Homes, Shared Ownership, Investment Property, Must Haves, Property Type (Detached / Semi-Detached / Terraced / Flats / Bungalow / Land / Park Home).

## **İlan Detay:**

- **Property Summary (AI Özet):** **Yok** — Property Info tek parça, elle yazılmış uzun düz metin. Üstte 2–3 maddelik özet yok.
- **Property Q&A:** **Yok** — Serbest soru sorulabilecek hiçbir kanal yok. Tek yol "Book a viewing" veya iletişim formu.
- **Property Highlights:** **Kısmen** — Features sekmesi var ama ilan girişinde elle dolduruluyor. AI çıkarımı değil.
- **Lifestyle / "Ideal for..." Eşleştirme:** **Kısmen** — Serbest metnin içinde "young family", "first purchase" gibi ifadeler geçiyor ama yapılandırılmış yaşam tarzı eşleştirmesi yok.
- **Property Comparison:** **Yok** — Kartlarda ve detayda karşılaştırma veya favori fonksiyonu yok.
- **Benzer İlan Önerisi:** **Yok** — Sayfanın altında benzer ilan bloğu yok; o alan "Why buy with us" ve alert CTA'sı ile dolduruluyor.
- **Area Insights:** **Kısmen** — Okul isimleri, yürüme mesafeleri, Council Tax bandı ve high street bilgisi var ama elle yazılmış paragraf hâlinde. Yapılandırılmış mahalle verisi (suç, demografi, okul reytingi) ve AI yorumu yok.
- **Commute Insights:** **Kısmen** — İstasyona yürüme süresi ve "301 bus to Abbey Wood for the Elizabeth Line" bilgisi açıklamaya sabit metin olarak gömülü. Kullanıcının kendi hedefine göre süre hiçbir zaman hesaplanmıyor.
- **Belge Açıklama (EPC / Floor Plan):** **Yok** — Floor Plans sadece görsel; EPC sekmesi var ama boş yükleniyor. Sade dille açıklama yok.
- **Ek not:** İlan detayında Features, Property Info, Floor Plans, Map ve EPC'nin yanında **Property Video ve Virtual Tour ayrı sekmeler olarak** duruyor — zengin medya mevcut, üzerindeki AI katmanı yok.
- **Ek not:** Sağ sütundaki kart birden fazla sekmede (Property Info, Virtual Tour) bozuk görsel ikonu gösteriyor — canlıda duran bir render hatası.
- **Ek not:** Aynı ilanın Instagram gönderisi (@jordanevans_thepropertycloud) sıfırdan ikinci kez yazılmış. Site metni, sosyal metin ve portal metni aynı veriden tamamen elle üretiliyor.

## **Değerleme:**

- **Instant Valuation:** **Var — ama 3. parti** — `valuation.thepropertycloud.uk` subdomain'inde barınıyor ve **"Powered by The ValPal Network"** ibaresi taşıyor. Ana sitenin tasarımından tamamen kopuk. Girdiler: postcode → Find Address, Number of Bedrooms, Property Type, Type of Valuation. Ana sayfa bunu kendi ağzıyla "Up to 60% accurate" diye tanıtıyor.
- **AI Valuation Açıklaması:** **Yok** — Rakamın gerekçesi, karşılaştırılabilir satışlar veya kişiselleştirme yok.
- **Mortgage / Stamp Duty Calculator:** **Yok** — Ne ilan detayında ne de alıcı sayfalarında var.
- **Ek not:** Yüz yüze değerleme yolu (`/valuations/book-a-face-to-face-valuation`) düz bir lead formu — isim, postcode araması, telefon, e-posta, onay kutusu. Takvim veya slot seçimi yok; randevu almıyor, talep gönderiyor.

## **İletişim / Lead:**

- **AI Chat Assistant / Chatbot:** **Yok** — Hiçbir sayfada chat widget'ı yok; ana sayfa, arama, ilan detay ve iletişimde sağ alt köşe boş. **Ancak** sayfa kaynağında `.whatsapp-chatbot` sınıfı ve `--wa-green`, `--wa-header-bg`, `--wa-bubble-bg`, `--wa-chat-bg`, `--wa-input-bg` değişkenleri tanımlı. Neuron platformu bir WhatsApp chatbot bileşeni ile geliyor, bu acente açmamış.
- **Lead Qualification:** **Kısmen** — Heads Up Alerts kaydında "Circumstances" bölümü var (alma sebebi, taşınma zamanı, avukat ayarlandı mı, bizi nereden duydunuz). Nitelendirme verisi toplanıyor ama form herkese aynı — dallanma, önceliklendirme veya AI ön elemesi yok.
- **Otomatik Randevu / Viewing Planlama:** **Yok** — "Book a viewing" ve değerleme formları müsaitlik göstermiyor, talep gönderiyor.
- **Mesai Dışı Yanıt:** **Yok (gözlemlenebildiği kadarıyla)** — Otomatik yanıt verebilecek hiçbir kanal yok: chat yok, WhatsApp aktif değil. Mesai dışında tek seçenek form doldurup beklemek.
- **Ek not:** İletişim formu tek tip — ad, soyad, telefon, e-posta, Buy/Sell/Rent/Let checkbox satırı ve serbest mesaj. Form bu seçime göre değişmiyor.

## **Teknik / Genel:**

- **SSR vs CSR:** **SSR** — Kaynaktaki `/_nuxt/` bundle'ları **Nuxt (Vue)** olduğunu doğruluyor, Vercel üzerinde deploy edilmiş (`/_vercel/image` ile görsel optimizasyonu). İlan listesi ayrı bir XHR ile değil, HTML'in içinde geliyor.
- **API çağrıları:** Fetch/XHR'da görünür bir Neuron veri API'si yok. Görülenler: `ice.js` kaynaklı `anonymous` çağrısı (Iceberg tracker), üç adet `envelope/?sentry_version=7...` (Sentry hata takibi), ayrıca `log_event?alt=json` ve `id` (analytics). **Hiçbir AI/LLM servisine istek yok.**
- **Iceberg izleri:** Kaynakta `window.IcebergTracker` ve `__akyaCookieStarted` tanımlı; varlıklar `files.thepropertycloud.neuronwebsites.co.uk` ve `lifesycle-cdn.s3.eu-west-2.amazonaws.com` üzerinden geliyor — Iceberg/Lifesycle CRM altyapısı.
- **Mobil davranış:** **Sorunsuz** — 400px'te filtreler dikey yığılıyor, arama ve butonlar kullanılabilir kalıyor. Sayfa 4.60 sn'de tamamlanıyor, ~295 kB transfer.

**Durum:** Yapıldı

### Tur 4 — Ayselin

## **Arama:**

- **Doğal Dil Araması:** **Yok** — Web sitesi platformdaki diğer sitelerle aynı Buy/Rent ve temel filtreleme yapısını kullanıyor. Kullanıcılar fiyat ve yatak odası gibi kriterlerle arama yapabiliyor ancak serbest metin, anahtar kelime, mülk tipi filtresi veya harita tabanlı arama bulunmuyor. Ajans kendisini “Property Marketing, Done Properly” söylemiyle konumlandırıyor ve fotoğraf/video kalitesine güçlü şekilde odaklanıyor. Bu nedenle arama deneyimi platformun varsayılan yapısından büyük ölçüde farklılaşmıyor.

- **Akıllı Öneriler / Sorgu Anlama:** **Yok** — Anonim ve kayıtlı kriterleri olmayan kullanıcıyla yapılan kontrolde tüm ilanlarda “100% MATCH” rozeti görülüyor ve fiyat, yatak odası sayısı veya ilan durumuna göre anlamlı bir değişiklik göstermiyor. Bu durum göstergenin gerçek AI tabanlı eşleştirme yerine statik veya kural tabanlı bir UI öğesi olduğunu düşündürüyor. Neuron/Iceberg Digital altyapısının kullanılması tek başına bu eşleşme yüzdesinin AI tarafından üretildiğini doğrulamıyor.

- **Kayıtlı Arama / Uyarılar:** **Mevcut** — Property Alerts, alıcı ve kiracıların arama kriterlerini kaydetmesine ve uygun mülkler geldiğinde bildirim almasına olanak sağlıyor. Sistem ayrıca bazı mülkleri büyük emlak portallarında yayınlanmadan önce kullanıcılara sunmayı öne çıkarıyor.

---

## **İlan Detayı:**

- **Mülk Özeti (AI):** **Yok** — İlanlarda manuel hazırlanmış açıklamalar ve yapılandırılmış mülk bilgileri bulunuyor ancak AI tarafından oluşturulmuş 2–3 maddelik kısa bir özet bulunmuyor.

- **Mülk Soru-Cevap:** **Yok** — Kullanıcıların belirli bir mülk hakkında soru sorabileceği serbest metin tabanlı AI asistanı bulunmuyor.

- **Mülk Öne Çıkan Özellikleri:** **Kısmi** — İlanlarda kısa özellikler ve açıklayıcı başlıklar bulunuyor ancak bunların AI tarafından oluşturulduğuna dair bir kanıt yok; içerikler manuel hazırlanıyor.

- **Yaşam Tarzı / "Kimler İçin Uygun?" Eşleştirmesi:** **Kısmi** — Bazı ilanlarda “Ideal First Time Purchase” gibi uygunluk ifadeleri ve okul, ulaşım, yerel olanaklar hakkında bilgiler bulunuyor. Ancak kullanıcı profiline göre AI tarafından oluşturulmuş kişiselleştirilmiş bir yaşam tarzı analizi bulunmuyor.

- **Mülk Karşılaştırma:** **Yok** — Birden fazla ilanı karşılaştıran AI destekli bir özellik gözlemlenmedi.

- **Benzer İlanlar (kişiselleştirilmiş):** **Mevcut** — Eşleştirme sistemi kayıtlı alıcı kriterlerini uygun mülklerle ilişkilendiriyor ve sonuçlarda eşleşme yüzdeleri gösteriyor. Ancak Smart Suggestions bölümünde olduğu gibi bu eşleşmenin backend tarafındaki gerçek çalışma mantığı doğrulanmadı ve görünen sistemin platform seviyesindeki eşleştirme altyapısına dayandığı düşünülüyor.

- **Bölge İçgörüleri:** **Kısmi** — İlan açıklamalarında yakın okullar, mağazalar, ulaşım bağlantıları ve yerel olanaklar hakkında bilgiler bulunuyor. Ayrıca yerel rehberler mevcut ancak demografi, suç oranı, olanaklar veya yaşam tarzına uygunluk gibi faktörleri bir araya getiren AI destekli bir bölge analizi bulunmuyor.

- **Ulaşım / İşe Gidiş İçgörüleri:** **Kısmi** — İlanlarda yakın istasyonlardan ve DLR ile Elizabeth Line gibi ulaşım bağlantılarından bahsediliyor. Ancak kullanıcının iş yeri veya okuluna göre kişiselleştirilmiş ulaşım süresi analizi bulunmuyor.

- **Belge Açıklama (EPC / Kat Planı):** **Yok** — EPC ve kat planları ilanlarda mevcut olabiliyor ancak bu belgeleri sade bir dille açıklayan AI destekli bir özellik bulunmuyor.

- **AI / Görsel Medya Fırsatı:** **Kısmi** — Ajansın en güçlü farklılaştırıcı özelliği fotoğraf ve video kalitesi. Görsel analiz kullanan bir AI sistemi; geniş bahçe, yenilenmiş mutfak, dönemsel mimari özellikler veya doğal ışık gibi görsel özellikleri otomatik olarak tespit edip öne çıkarabilir. Böylece mevcut fotoğraf/video yatırımı ek bir veri kaynağına dönüştürülebilir. Ancak bu, temel öncelikten ziyade ikincil bir fırsat olarak değerlendirilmeli.

---

## **Değerleme:**

- **Anlık Değerleme:** **Mevcut** — Web sitesi 7/24 çalışan bir online değerleme aracı sunuyor. Kullanıcılara mülklerinin yaklaşık değerini hızlı bir şekilde gösteren bir tahmin sağlanıyor. Site, anlık değerlemenin %60'a kadar doğru olabileceğini belirtiyor.

- **AI Değerleme Açıklaması:** **Yok** — Anlık değerleme tahmini bir rakam sunuyor ancak bu tahminin nedenlerini açıklayan AI destekli bir anlatım veya kişiselleştirilmiş faktör analizi bulunmuyor.  
  **AI fırsatı:** Sistem yalnızca tahmini bir rakam göstermek yerine benzer mülkler, bölgesel piyasa koşulları ve mülk özelliklerinin tahmini nasıl etkilediğini açıklayabilir.

- **Mortgage / Stamp Duty Calculator:** **Yok** — AI destekli finansal yorum içeren özel bir mortgage veya Stamp Duty hesaplayıcısı gözlemlenmedi.

---

## **İletişim:**

- **AI Chat Assistant / Chatbot:** **Yok** — Site genelinde veya mülk sayfalarında AI destekli chatbot bulunmuyor.

- **Lead Qualification:** **Kısmi** — Property Alerts sistemi alıcı ve kiracıların ihtiyaçlarını ve arama tercihlerini topluyor. Böylece ajans, lead'in ne tür bir mülk aradığını yapılandırılmış şekilde görebiliyor. Ancak AI destekli lead scoring, otomatik nitelendirme veya önceliklendirme bulunmuyor.

- **Otomatik Rezervasyon / Viewing Scheduling:** **Kısmi** — İlan sayfalarında viewing ve iletişim seçenekleri bulunuyor ve esnek viewing hizmetleri sunuluyor. Ancak AI destekli otomatik rezervasyon veya konuşma tabanlı randevu planlama sistemi bulunmuyor.

- **Mesai Dışı Yanıt:** **Kısmi** — Anlık değerleme 7/24 kullanılabiliyor ve Property Alerts sürekli çalışıyor. Ancak mesai dışında müşteri sorularını yanıtlayan AI destekli konuşma tabanlı bir sistem bulunmuyor.

---

## **Teknik / Genel:**

- **SSR vs CSR:** **Hibrit (SSR + CSR)** — İlk sayfa yüklemesi server-side olarak gerçekleştiriliyor ve temel mülk/içerik bilgileri doğrudan HTML içerisinde bulunuyor. Daha sonra client-side JavaScript etkileşimli bölümleri ve navigasyonu yönetiyor.

- **API çağrıları:** **Kısmi** — Mülk arama ve eşleştirme özelliklerinin harici veya emlak platformu altyapısına dayandığı görülüyor. Ancak spesifik runtime API endpoint'leri Network-tab incelemesiyle doğrulanmadı ve web sitesi bazı diğer grup sitelerindeki gibi platformu açık şekilde Neuron/Iceberg Digital olarak tanımlamıyor.

- **Mobil davranış:** **Mevcut** — Responsive web sitesi mobil cihazlarda mülk arama, ilanlar, uyarılar, değerleme ve iletişim özelliklerine erişim sağlıyor.

- **Genel UX:** **İyi** — Web sitesinin en güçlü tarafı görsel sunum ve mülk pazarlama kalitesi. Fotoğraf, video ve profesyonel ilan sunumu güçlü bir ilk izlenim oluşturuyor. Ancak temel mülk keşif deneyimi oldukça standart kalıyor ve yüksek kaliteli medya içeriklerinden yeterince faydalanmıyor.

- **AI Fırsatı:** **Orta–Yüksek** — En güçlü fırsatlar genel amaçlı AI özelliklerinden ziyade ajansın mevcut güçlü yönlerini destekleyen özellikler. Görsel analiz tabanlı mülk öne çıkarma, AI mülk özetleri, doğal dil araması ve daha akıllı eşleştirme, kaliteli fotoğraf ve videoları daha zengin arama verilerine dönüştürebilir. AI destekli değerleme açıklamaları da insan danışmanlığının yerine geçmeden şeffaflığı artırabilir.

---

**Durum:** Yapıldı

### Ortak Bulgular / Sentez (4 tur bitince doldurulur)

- Ortak eksik AI özellikleri: Doğal dil arama, AI ilan özeti, Property Q&A, AI lead scoring, mesai dışı otomatik yanıt, EPC/floor plan açıklaması.
- Öne çıkan fırsatlar: (1) Görsel/video kalitesine güçlü yatırım (Giraffe360 tur, drone video) — görüntü-farkında AI ile otomatik özellik çıkarımı (bahçe, yenilenmiş mutfak vb.). (2) Aynı içerik (site metni, sosyal medya, portal) elden 3 kez yazılıyor — tek kaynaktan çoklu format üretimi net bir otomasyon fırsatı.
- Görüş ayrılıkları / doğrulanması gerekenler: Sitede canlı görsel render hatası var (kırık resim ikonu, birden fazla sekmede) — tekrar kontrol edilmeli. "100% MATCH" rozeti burada da herkese aynı gösteriliyor — platform geneli sorun olarak doğrulandı.
