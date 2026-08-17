# 03 · harrisonshomes.co.uk

**URL:** https://harrisonshomes.co.uk/
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
- Same toggle-and-thin-filters pattern as the group. The homepage "Find your dream home" line is aspirational, but the actual search is the same price/beds/radius set — no property type, no keyword, no free text, no map.
- The gap between the emotive "dream home" framing and the mechanical dropdowns is jarring. **AI opportunity:** if any tenant's brand promises "dream home", natural-language search is the feature that would actually make that promise feel real.

**Listing Detail:**
- Standard Neuron template. The homepage leans on strong stats (81% of listings sell vs 50% locally, sellers achieve ~£13k more), which is persuasive — but none of that reaches the listing pages, which are the same bullet-features + hand-written narrative as everyone else. No AI summary/Q&A, area info as prose.

**Valuation:**
- Notable: the instant "price guide" is outsourced to a third party (`propalt.io/seller`) rather than the usual `valuation.{domain}` tool — so Harrisons' instant estimate genuinely lives outside Neuron. Plus book face-to-face.
- **Neuron read:** the fact a tenant bolted on propalt for a real instant number tells me the platform's own "instant valuation" (the gated lead form) isn't satisfying that need. That's a platform gap worth owning.

**Contact:**
- "Book a Face-to-Face Consultation" is the primary CTA; no phone visible on the homepage, which is mild friction for phone-first users. No chat, no out-of-hours.

**Technical / General:**
- Neuron/Iceberg + Vercel + Lifesycle, with the propalt valuation integration bolted on.
- Trust is strong and evidence-led (named staff in testimonials, redress scheme, CMP, full company reg). Feels a touch more corporate than Kinetic, but credible. The stats-heavy homepage is doing real persuasion work the listing pages don't back up.

**Status:** Done

### Round 2 — Berkay

## **Search:**

- **Natural Language Search:** **Absent** — Property search uses structured Buy/Rent controls, location, price, bedrooms and property type rather than free-sentence queries.
- **Smart Suggestions / Query Understanding:** **Absent** — On the property listing page, every property displays a “100% MATCH” badge (8/8 results checked for an anonymous visitor with no saved criteria — despite differences in price ranges and bedroom counts, all properties show 100%). The fact that all listings display the same fixed value regardless of the user’s profile or criteria indicates that this is not a genuine/personalized AI matching system, but rather a static UI label. No evidence of smart recommendations or query understanding functionality was observed.
- **Saved Search / Alerts:** **Present** — Heads-Up Property Alerts allow users to save detailed requirements including locations, radius, price, bedrooms, bathrooms, property type and other preferences. The system provides personalised property suggestions and price-reduction alerts, including pre-market properties.

## **Listing Detail:**

- **Property Summary (AI):** **Absent** — Property pages contain manually written descriptions and feature information, but no AI-generated 2–3 point summary was observed.
- **Property Q&A:** **Absent** — No free-form AI Q&A for individual listings was observed.
- **Property Highlights:** **Partial** — Listings contain a dedicated FEATURES section with concise property information, but no evidence that these highlights are AI-generated was observed.
- **Lifestyle / "Ideal for…" Matching:** **Partial** — Property titles and descriptions can explicitly identify suitability, such as "Ideal for First-Time Buyers" or "Ideal Buy-to-Let", but no AI-generated lifestyle matching commentary was observed.
- **Property Comparison:** **Absent** — No AI-powered comparison of two or more properties was observed.
- **Similar Listings (personalised):** **Present** — The Neuron matching system connects registered buyer requirements with suitable properties and displays match percentages on property results.
- **Area Insights:** **Partial** — Property pages provide location information and descriptions of nearby amenities, transport and local facilities, but no dedicated AI-generated neighbourhood analysis was observed.
- **Commute Insights:** **Partial** — Property information can mention proximity to railway stations and other transport links, but there is no personalised commute-time analysis based on the user's workplace or school.
- **Document Explanation (EPC / Floor Plan):** **Absent** — EPC information and floor plans are provided where available, but no AI-powered plain-language explanation of these documents was observed.

## **Valuation:**

- **Instant Valuation:** **Present** — Harrisons offers a free instant online valuation described as "70%-80% Accurate," calculated by a computer algorithm using previous sales data (via a separate salesval.harrisonshomes.co.uk / propalt.io setup). The site positions this as a rough, preliminary estimate, alongside an "80%-90% Accurate" virtual valuation and a "100% Accurate" face-to-face valuation option.
- **AI Valuation Explanation:** **Absent** — The instant valuation provides an estimated figure, but no AI-generated explanation or personalised breakdown of the valuation factors was observed.
- **Mortgage / Stamp Duty Calculator:** **Present** — A mortgage calculator is available on the valuation/property flow. Users enter property price, deposit, loan length and interest rate to calculate an approximate monthly cost. No AI financial commentary or personalised advice was observed.

## **Contact:**

- **AI Chat Assistant / Chatbot:** **Absent** — No site-wide or property-level AI chat assistant was observed.
- **Lead Qualification:** **Partial** — Heads-Up registration collects detailed buyer circumstances including reason for buying, moving timeframe, solicitor status, whether the user needs to sell their current property and mortgage requirements. This provides structured lead information, but no AI-powered lead scoring or prioritisation was observed.
- **Automated Booking / Viewing Scheduling:** **Partial** — Property pages provide a "BOOK A VIEWING" option and the valuation system supports date/time selection. However, no AI-driven appointment scheduling or conversational booking assistant was observed.
- **Out-of-hours Response:** **Absent** — No automated out-of-hours AI chatbot or conversational response system was observed.

## **Technical / General:**

- **SSR vs CSR:** **Hybrid (SSR + CSR)** — Initial page load is server-side rendered, with core property and content information present directly in the delivered HTML. Client-side hydration then takes over for interactive elements and further navigation. 
- **API calls:** **Present** — The website identifies itself as powered by Neuron / Iceberg Digital's "AI Operating System for Estate Agents".
- **Mobile behaviour:** **Present** — The responsive website provides access to property search, listings, alerts, valuation and contact forms on mobile.

**Status:** Done

### Round 3 — Yasemin

## **Search:**

- **Natural Language Search:** **No** — Typing a free-form sentence returns a "Couldn't find the address" error. The box only matches addresses.
- **Smart Suggestions / Query Interpretation:** **Partial** — Typo tolerance works ("Sittingborne" → Sittingbourne). It comes from Google Places; typing "Sitt" also suggests POIs such as Sittingbourne Golf Centre. The default sort is "SUGGESTED" with no stated basis.
- **Saved Search / Alerts:** **Yes** — A criteria-based registration flow exists (Contact / Property Type / Circumstances), collecting multiple locations, radius and property type. Price-reduction notifications are also promised. There is no layer that learns from behaviour.

## **Listing Detail:**

- **Property Summary (AI Summary):** **No** — The description is fluent and well written but there is no summary block. The text is long and never condensed.
- **Property Q&A:** **No** — No channel for asking free-form questions.
- **Property Highlights:** **Partial** — A Features tab exists, entered by hand.
- **Lifestyle / "Ideal for..." Matching:** **Partial** — Target-audience phrases like "first-time buyers" and "busy professionals" appear manually in the description. There is no profile-based matching.
- **Property Comparison:** **No** — No comparison or favourites function.
- **Similar Listing Suggestions:** **No** — "Our Latest Homes" appears in the sidebar but shows the newest listings, unrelated to the current property or the user.
- **Area Insights:** **No** — A Map tab exists, but the points are Google's own data. No school, crime or demographic commentary.
- **Commute Insights:** **No** — Travel time is never calculated. Phrases like "reducing travel time" are written by hand in the description.
- **Document Explanation (EPC / Floor Plan):** **Partial** — The Floor Plans tab holds images only. However, the description does interpret the EPC: "EPC rating of B highlights the property's efficiency, which can lead to lower utility costs". This is the manual version of the glossary item.
- **Additional note:** A structured Property Info block exists (tenure, age, council tax, sewerage, water, **condition**). The condition field wasn't present on the other sites.

## **Valuation:**

- **Instant Valuation:** **Yes** — Provided by **Propalt** at `harrisonshomes.propalt.io/seller`. Positioned on the homepage as an "instant report" — described as fast, simple and pressure-free. A third-party integration.
- **AI Valuation Explanation:** **No** — The basis of the figure isn't explained on the site; the instant report is framed as a starting point, with the real number coming from the face-to-face meeting.
- **Mortgage / Stamp Duty Calculator:** **No** — No calculator anywhere on the site.

## **Contact / Lead:**

- **AI Chat Assistant / Chatbot:** **Partial** — A fixed **WhatsApp button** appears on every page (bottom right). It isn't a bot, however — just a direct link to WhatsApp with no automated replies.
- **Lead Qualification:** **Yes** — It works at two points: the Circumstances section of the alert form (5 questions) and the viewing modal ("do I have a property to sell", "a property to let", "would I like it valued"). The questions are fixed with no branching.
- **Automated Booking / Viewing Scheduling:** **Yes** — Valuation appointments run through **Cal.com** as a genuine booking: consultant-specific (Sales Market Appraisal – Ben), one-hour slots, real availability. The viewing modal opens a calendar but states that it does not confirm the viewing, so it only collects preferences.
- **Out-of-Hours Response:** **Partial** — Closed Sunday, closing at 17:30 on weekdays. The WhatsApp button remains reachable outside hours but returns no automated reply; the message simply waits for a human.

## **Technical / General:**

- **SSR vs CSR:** **SSR** — Content present in the HTML. Theme layer `/theme6/`, shared layer `/common/css/neuron.css`.
- **Different build:** This theme loads jQuery-based vendor scripts (jquery, slick, jarallax, odometer, magnific-popup, wow) — an older and heavier approach than the other themes.
- **API calls:** 6 requests under Fetch/XHR: IcebergTracker (`ice.js`), three Sentry envelopes, a `view` call. Listing data does not arrive via XHR. 109 requests, 9.5 MB, 1.99 s.
- **Analytics:** IcebergTracker + Sentry + a **Metricool** tracker.
- **Mobile behaviour:** Responsive; filters collapse into a vertical panel.
- **Key finding 1:** The source defines a `.whatsapp-chatbot` class. The site does show a WhatsApp button, but it is a plain redirect link rather than that chatbot component — so the component remains switched off.
- **Key finding 2:** The statistics band on the homepage (£0, 0 days, 0%) reads zero because the counter animation never fires. The same figures render correctly on `/sellers` (£17,805, 68 days, 118 days, 100.04%). It is broken on the homepage only.

## **Distinguishing feature: Pre-market listings**

The homepage and listings carry blurred "Coming Soon" entries. These are released only to registered users before reaching the portals. Access requires **email login via magic link** (passwordless, reCAPTCHA-protected).

This is the site's strongest asset: a genuinely working user account system with a content-gating mechanism. Yet nothing changes for a logged-in user — sorting, recommendations and personalisation stay the same. The account system functions purely as a gate.

**Status:** Done

### Round 4 — Ayselin

## **Search:**

- **Natural Language Search:** **Absent** — The homepage follows the same Buy/Rent and basic-filter structure seen across the group. Users can search using criteria such as price, bedrooms and location radius, but there is no free-text search, keyword input, property-type filtering or map-based search. This creates a noticeable gap between the homepage's “Find your dream home” messaging and the relatively mechanical search experience.  
  **AI opportunity:** Natural-language search could make this promise more meaningful by allowing users to describe their ideal property in their own words and automatically converting the request into relevant search criteria.

- **Smart Suggestions / Query Understanding:** **Absent** — Property results display a “100% MATCH” badge, but this does not appear to represent genuine personalised matching. During testing, all 8/8 properties checked for an anonymous visitor without saved criteria displayed the same 100% value, despite differences in price and bedroom count. This suggests the badge is a static or rule-based interface element rather than an AI-driven recommendation system.

- **Saved Search / Alerts:** **Present** — Heads-Up Property Alerts allow users to save detailed requirements including location, radius, price, bedrooms, bathrooms, property type and other preferences. The system can provide property suggestions, price-reduction alerts and access to properties before they are widely marketed.

---

## **Listing Detail:**

- **Property Summary (AI):** **Absent** — Property pages use manually written descriptions and feature information. No AI-generated summary was observed to highlight the most important points of a listing.

- **Property Q&A:** **Absent** — There is no AI-powered assistant that allows users to ask free-form questions about an individual property.

- **Property Highlights:** **Partial** — Listings contain a dedicated FEATURES section with concise property information, but the content appears to be manually entered rather than dynamically generated by AI.

- **Lifestyle / "Ideal for…" Matching:** **Partial** — Some listings explicitly describe suitability, such as “Ideal for First-Time Buyers” or “Ideal Buy-to-Let.” However, these statements are part of the manually written listing content rather than AI-generated personalised recommendations.

- **Property Comparison:** **Absent** — No AI-powered comparison tool was observed for evaluating two or more properties based on price, features, location or suitability.

- **Similar Listings (personalised):** **Present** — The Neuron matching infrastructure connects registered buyer requirements with suitable properties and displays match percentages within property results. However, the visible “100% MATCH” values did not appear to change meaningfully for anonymous users, so the extent of genuine personalisation is unclear.

- **Area Insights:** **Partial** — Property pages include information about the local area, nearby amenities and transport links. However, there is no dedicated AI-generated neighbourhood analysis that combines these factors into a structured overview.

- **Commute Insights:** **Partial** — Listings can mention railway stations and other transport connections, but there is no personalised commute-time analysis based on the user's workplace, school or chosen destination.

- **Document Explanation (EPC / Floor Plan):** **Absent** — EPC information and floor plans are available where provided, but there is no AI-powered feature that explains these documents in plain language or highlights their key implications for buyers.

---

## **Valuation:**

- **Instant Valuation:** **Present** — Harrisons provides a free online valuation tool that gives an estimated property value based on previous sales data and a computer-generated calculation. The service presents the result as an initial estimate and also offers virtual and face-to-face valuation options with different levels of accuracy.

- **AI Valuation Explanation:** **Absent** — Although the online tool provides an estimated figure, it does not provide an AI-generated explanation of the factors behind the valuation or a personalised breakdown of why the property may be worth that amount.  
  **AI opportunity:** The valuation could be enhanced by showing the estimated range together with factors such as comparable sales, property characteristics, location and market conditions in an easy-to-understand format.

- **Mortgage / Stamp Duty Calculator:** **Present** — A mortgage calculator is available as part of the valuation/property journey. Users can enter property price, deposit, loan term and interest rate to estimate monthly repayments. However, there is no AI-generated financial commentary or personalised guidance.

---

## **Contact:**

- **AI Chat Assistant / Chatbot:** **Absent** — No site-wide or property-specific AI chatbot was observed.

- **Lead Qualification:** **Partial** — Heads-Up registration collects detailed buyer information, including reasons for moving, expected timeframe, solicitor status, whether the user needs to sell another property and mortgage requirements. This provides useful structured lead data, but there is no evidence of AI-powered lead scoring or prioritisation.

- **Automated Booking / Viewing Scheduling:** **Partial** — Property pages provide a “BOOK A VIEWING” option, while the valuation flow also supports selecting a date and time. However, there is no conversational AI assistant managing the complete booking process.

- **Out-of-hours Response:** **Absent** — No automated AI assistant was observed for handling enquiries or answering customer questions outside normal business hours.

---

## **Technical / General:**

- **SSR vs CSR:** **Hybrid (SSR + CSR)** — The initial page is server-rendered, with core property and content information available in the delivered HTML. Client-side JavaScript is then used for interactive elements and navigation.

- **API calls:** **Present** — The website is built on the Neuron / Iceberg Digital platform and references its “AI Operating System for Estate Agents” infrastructure. The property matching and alert functionality are integrated into the platform.

- **Mobile behaviour:** **Present** — The responsive website provides access to property search, listings, Heads-Up alerts, valuation tools and contact forms on mobile devices.

- **Overall UX:** **Good** — The website has a strong trust-oriented presentation and uses statistics and performance claims effectively on the homepage. The main weakness is that this persuasive messaging is not fully reflected in the property discovery and listing experience, which remains relatively similar to other Neuron-powered sites.

- **AI Opportunity:** **High** — The strongest opportunity is to connect the site's “dream home” positioning with genuinely intelligent property discovery. Natural-language search, meaningful personalised matching, AI property summaries, Q&A and transparent valuation explanations would make the customer experience significantly more intelligent.

---

**Status:** Done

### Findings / Synthesis (filled once all 4 rounds are done)

- Commonly missing AI features: Natural-language search, AI listing summaries, Property Q&A, AI lead scoring, out-of-hours automated response.
- Standout opportunities: (1) A genuinely working account system exists (magic-link login — confirmed live: enter email, "send me a link" button, no password) gating pre-market "Coming Soon" listings — but nothing changes for a logged-in user beyond access. (2) Cal.com powers real appointment booking for valuations — confirmed live with an actual booked slot ("Sales market appraisal - Chris," 25 Aug 2026, 15:00–16:00, 1 hour, in-person, Europe/Istanbul timezone) — the clearest working booking flow found across the whole study. (3) The homepage's strong statistics (sale rate, extra proceeds) never reach the listing pages.
- Disagreements / to verify: ✅ **Confirmed by Ayselin (live check, August 2026):** The "instant report" button links to `harrisonshomes.propalt.io/seller` — a genuine third-party (Propalt) integration, entirely separate from `harrisonshomes.co.uk` and from Neuron's own infrastructure — supporting the hypothesis that Neuron's own instant-valuation tool wasn't meeting this tenant's needs. ⚠️ **Correction:** the homepage stats-counter animation bug noted in Round 1 (stuck at £0/0/0%) is **no longer present** — live testing confirms the counters now animate correctly, counting up from zero. This appears to have been fixed since the original review.

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
- Grupla aynı toggle-ve-zayıf-filtre kalıbı. Ana sayfadaki "Find your dream home" ifadesi iddialı, ama gerçek arama yine aynı price/beds/radius seti — property type yok, keyword yok, serbest metin yok, harita yok.
- Duygusal "dream home" çerçevesi ile mekanik dropdown'lar arasındaki uçurum rahatsız edici. **AI fırsatı:** bir tenant markası "dream home" vaat ediyorsa, bu vaadi gerçek hissettirecek özellik doğal dil aramasıdır.

**İlan Detay:**
- Standart Neuron şablonu. Ana sayfa güçlü istatistiklere yaslanıyor (ilanların %81'i satılıyor, yerelde %50; satıcılar ~£13k fazla alıyor), ikna edici — ama bunların hiçbiri ilan sayfalarına ulaşmıyor; oralar herkesle aynı bullet-features + elle yazılmış anlatı. AI özet/Q&A yok, bölge bilgisi düz yazı.

**Değerleme:**
- Dikkat çekici: anlık "price guide" olağan `valuation.{domain}` aracı yerine bir üçüncü tarafa (`propalt.io/seller`) dış kaynak veriliyor — yani Harrisons'ın anlık tahmini gerçekten Neuron dışında yaşıyor. Ayrıca yüz yüze randevu.
- **Neuron çıkarımı:** bir tenant'ın gerçek anlık rakam için propalt eklemesi, platformun kendi "instant valuation"ının (kapı tutan lead formu) bu ihtiyacı karşılamadığını gösteriyor. Sahiplenilmeye değer bir platform açığı.

**İletişim:**
- Ana CTA "Book a Face-to-Face Consultation"; ana sayfada telefon görünmüyor, bu telefon-öncelikli kullanıcılar için hafif sürtünme. Chat yok, mesai dışı yok.

**Teknik/Genel:**
- Neuron/Iceberg + Vercel + Lifesycle, üstüne propalt valuation entegrasyonu eklenmiş.
- Güven güçlü ve kanıta dayalı (testimonial'larda isimli personel, redress scheme, CMP, tam şirket kaydı). Kinetic'ten biraz daha kurumsal, ama güvenilir. İstatistik ağırlıklı ana sayfanın yaptığı ikna işini ilan sayfaları desteklemiyor.

**Durum:** Yapıldı

### Tur 2 — Berkay

## **Arama:**

- **Doğal Dil Araması:** **Yok** — Mülk araması Satın Alma/Kiralama seçenekleri, konum, fiyat, oda sayısı ve mülk tipi gibi yapılandırılmış kriterleri kullanıyor; serbest cümleyle arama bulunmuyor.
- **Akıllı Öneriler / Sorgu Anlama:** **Yok** — İlan listeleme sayfasında her mülkün yanında "100% MATCH" rozeti görünüyor (anonim ziyaretçi, kayıtlı kriter yokken kontrol edilen 8/8 sonuç — farklı fiyat aralıkları ve oda sayılarına rağmen hepsi %100). Profil veya kriter fark etmeksizin tüm ilanların aynı sabit değeri göstermesi, bunun gerçek/kişiselleştirilmiş bir yapay zeka eşleştirmesi değil, statik bir UI etiketi olduğunu gösteriyor. Akıllı öneri veya sorgu anlama özelliğine dair kanıt gözlemlenmedi.
- **Kayıtlı Arama / Uyarılar:** **Var** — Heads-Up Mülk Uyarıları ile konum, yarıçap, fiyat, oda/banyo sayısı, mülk tipi ve diğer tercihler kaydedilebiliyor. Sistem kişiselleştirilmiş mülk önerileri ve fiyat değişikliği bildirimleri sağlıyor; pre-market ilanlar da bu sisteme dahil edilebiliyor.

## **İlan Detay:**

- **Mülk Özeti (YZ):** **Yok** — İlan sayfalarında manuel olarak hazırlanmış açıklamalar ve özellik bilgileri bulunuyor; yapay zeka tarafından oluşturulan 2–3 maddelik özet gözlemlenmedi.
- **Mülk Soru-Cevap:** **Yok** — İlan hakkında serbest biçimde soru sorulabilen yapay zeka destekli Q&A özelliği gözlemlenmedi.
- **Mülkün Öne Çıkan Özellikleri:** **Kısmi** — İlanlarda kısa mülk bilgilerinin bulunduğu ayrı bir ÖZELLİKLER bölümü bulunuyor; ancak bu öne çıkan bilgilerin yapay zeka tarafından oluşturulduğuna dair kanıt bulunmuyor.
- **Yaşam Tarzı / "... için ideal" Eşleştirmesi:** **Kısmi** — İlan başlıkları ve açıklamalarında "Ideal for First-Time Buyers" veya "Ideal Buy-to-Let" gibi uygunluk ifadeleri bulunabiliyor; ancak yapay zeka tarafından oluşturulan yaşam tarzı eşleştirme yorumu bulunmuyor.
- **Mülk Karşılaştırma:** **Yok** — İki veya daha fazla mülkü yapay zeka ile karşılaştırma özelliği gözlemlenmedi.
- **Benzer İlanlar (kişiselleştirilmiş):** **Var** — Neuron matching sistemi, kayıtlı alıcı gereksinimlerini uygun mülklerle eşleştiriyor ve ilan sonuçlarında eşleşme yüzdeleri gösteriyor.
- **Bölge İçgörüleri:** **Kısmi** — İlan sayfalarında konum ve çevredeki olanaklar, ulaşım bağlantıları ve yerel tesisler hakkında bilgiler bulunuyor; ancak özel bir yapay zeka destekli bölge analizi bulunmuyor.
- **Ulaşım İçgörüleri:** **Kısmi** — İlanlarda tren istasyonlarına ve diğer ulaşım bağlantılarına yakınlık belirtilebiliyor; ancak kullanıcının iş veya okul konumuna göre kişiselleştirilmiş ulaşım süresi analizi bulunmuyor.
- **Belge Açıklaması (EPC / Kat Planı):** **Yok** — EPC bilgileri ve kat planları sunuluyor; ancak bunları sade bir dille açıklayan yapay zeka özelliği gözlemlenmedi.

## **Değerleme:**

 **Anlık Değerleme:** **Var** — Harrisons, "%70-80 doğrulukta" olarak tanımlanan, önceki satış verilerini kullanan bir bilgisayar algoritmasıyla çalışan ücretsiz anlık online değerleme sunuyor (ayrı bir salesval.harrisonshomes.co.uk / propalt.io altyapısı üzerinden). Site bunu kaba, ön bir tahmin olarak konumlandırıyor; %80-90 doğruluklu sanal değerleme ve %100 doğruluklu yüz yüze değerleme seçenekleriyle birlikte sunuyor.
- **Yapay Zeka Değerleme Açıklaması:** **Yok** — Anlık değerleme tahmini sunuluyor ancak değerin arkasındaki faktörleri açıklayan yapay zeka destekli veya kişiselleştirilmiş bir analiz bulunmuyor.
- **Mortgage / Damga Vergisi Hesaplayıcısı:** **Var** — Değerleme/mülk akışında mortgage hesaplayıcısı bulunuyor. Kullanıcı mülk fiyatı, depozito, kredi süresi ve faiz oranını girerek yaklaşık aylık maliyeti hesaplayabiliyor. yapay zeka destekli finansal yorum veya kişiselleştirilmiş tavsiye bulunmuyor.

## **İletişim:**

- **Yapay Zeka Sohbet Asistanı / Chatbot:** **Yok** — Site genelinde veya ilan seviyesinde yapay zeka destekli sohbet asistanı gözlemlenmedi.
- **Müşteri Adayı Nitelendirme:** **Kısmi** — Heads-Up kayıt süreci; satın alma nedeni, taşınma zamanı, solicitor durumu, mevcut mülkün satılması gerekip gerekmediği ve mortgage ihtiyacı gibi ayrıntılı bilgiler topluyor. Bu yapılandırılmış lead bilgisi sağlıyor ancak yapay zeka destekli müşteri adayı puanlama veya önceliklendirme bulunmuyor.
- **Otomatik Rezervasyon / Görüntüleme Planlama:** **Kısmi** — İlanlarda "BOOK A VIEWING" seçeneği bulunuyor ve değerleme sisteminde tarih/saat seçimi yapılabiliyor; ancak yapay zeka destekli randevu planlama veya konuşma tabanlı rezervasyon asistanı gözlemlenmedi.
- **Mesai Dışı Yanıt:** **Yok** — Mesai dışı otomatik AI sohbet botu veya konuşma tabanlı yanıt sistemi gözlemlenmedi.

## **Teknik/Genel:**

- **SSR ve CSR:** **Hibrit (SSR + CSR)** — İlk sayfa yüklemesi sunucu tarafında render ediliyor; temel ilan ve içerik bilgileri doğrudan teslim edilen HTML içinde yer alıyor. Ardından etkileşimli öğeler ve sonraki gezinmeler için istemci tarafı hydration devreye giriyor. 
- **API Çağrıları:** **Var** — Site kendisini Neuron / Iceberg Digital'in "Estate Agentlar için Yapay Zeka İşletim Sistemi" altyapısıyla güçlendirilmiş olarak tanımlıyor.
- **Mobil Davranış:** **Var** — Responsive site üzerinden mülk arama, ilanlar, alertler, değerleme ve iletişim formlarına mobil erişim sağlanıyor.

**Durum:** Yapıldı

### Tur 3 — Yasemin

## **Arama:**

- **Doğal Dil Araması:** **Yok** — Serbest cümle yazıldığında "Couldn't find the address" hatası dönüyor. Kutu sadece adres eşleştiriyor.
- **Akıllı Öneri / Sorgu Yorumlama:** **Kısmen** — Yazım hatası toleransı çalışıyor ("Sittingborne" → Sittingbourne). Google Places kaynaklı; "Sitt" yazınca Sittingbourne Golf Centre gibi POI'ler de öneriliyor. Sıralama varsayılanı "SUGGESTED", dayanağı belirsiz.
- **Kayıtlı Arama / Alerts:** **Var** — Kriterli kayıt akışı mevcut (Contact / Property Type / Circumstances). Çoklu konum, yarıçap ve mülk tipi alınıyor. Fiyat düşüşü bildirimi de vaat ediliyor. Davranışa göre öğrenen katman yok.

## **İlan Detay:**

- **Property Summary (AI Özet):** **Yok** — Açıklama akıcı ve iyi yazılmış ama özet bloğu yok. Metin uzun, kısaltma yapılmıyor.
- **Property Q&A:** **Yok** — Serbest soru sorma kanalı yok.
- **Property Highlights:** **Kısmen** — Features sekmesi var, elle girilmiş.
- **Lifestyle / "Ideal for..." Eşleştirme:** **Kısmen** — Açıklamada "first-time buyers", "busy professionals" gibi hedef kitle ifadeleri elle geçiyor. Profil bazlı eşleştirme yok.
- **Property Comparison:** **Yok** — Karşılaştırma ve favori özelliği yok.
- **Benzer İlan Önerisi:** **Yok** — Sağ sütunda "Our Latest Homes" var ama en yeni ilanlar; ilanla veya kullanıcıyla ilgisi yok.
- **Area Insights:** **Yok** — Harita sekmesi var, POI'ler Google'ın verisi. Okul, suç, demografi yorumu yok.
- **Commute Insights:** **Yok** — Ulaşım süresi hesaplanmıyor. Açıklamada "reducing travel time" gibi ifadeler elle yazılmış.
- **Belge Açıklama (EPC / Floor Plan):** **Kısmen** — Floor Plans sekmesi görsel olarak duruyor. Ancak açıklama metninde EPC yorumlanmış: "EPC rating of B highlights the property's efficiency, which can lead to lower utility costs". Bu, glossary'deki maddenin elle yapılmış hali.
- **Ek not:** Yapılandırılmış Property Info bloğu var (tenure, age, council tax, sewerage, water, **condition**). Condition alanı diğer sitelerde yoktu.

## **Değerleme:**

- **Instant Valuation:** **Var** — `harrisonshomes.propalt.io/seller` üzerinden **Propalt** sağlıyor. Ana sayfada "instant report" olarak konumlanmış, "hızlı, basit, baskı yok" deniyor. Üçüncü parti entegrasyon.
- **AI Valuation Açıklaması:** **Yok** — Sitede rakamın dayanağı açıklanmıyor; anlık raporun "başlangıç noktası" olduğu, gerçek değerin yüz yüze görüşmede verileceği belirtiliyor.
- **Mortgage / Stamp Duty Calculator:** **Yok** — Hesaplayıcı bulunmuyor.

## **İletişim / Lead:**

- **AI Chat Assistant / Chatbot:** **Kısmen** — Tüm sayfalarda sabit bir **WhatsApp butonu** var (sağ alt köşe). Ancak bu bir bot değil, doğrudan WhatsApp'a yönlendiren bir bağlantı; otomatik yanıt üretmiyor.
- **Lead Qualification:** **Var** — İki noktada çalışıyor: alert formundaki Circumstances (5 soru) ve viewing modalı ("satılacak mülküm var mı", "kiralanacak mülküm var mı", "değerlensin mi"). Sorular sabit, dallanma yok.
- **Otomatik Randevu / Viewing Planlama:** **Var** — Değerleme randevusu **Cal.com** ile gerçek rezervasyon yapıyor: danışman bazlı (Sales Market Appraisal – Ben), 1 saatlik slot, gerçek müsaitlik gösteriyor. Viewing modalı ise takvim açıyor ama "bu görüntülemeyi onaylamaz" diyor, yani sadece tercih topluyor.
- **Mesai Dışı Yanıt:** **Kısmen** — Pazar kapalı, hafta içi 17.30'da kapanıyor. WhatsApp butonu mesai dışında da erişilebilir ancak otomatik yanıt vermiyor, mesaj insana düşüyor.

## **Teknik/Genel:**

- **SSR vs CSR:** **SSR** — İçerik HTML'de mevcut. Tema katmanı `/theme6/`, ortak katman `/common/css/neuron.css`.
- **Farklı yapı:** Bu temada jQuery tabanlı vendor script'ler var (jquery, slick, jarallax, odometer, magnific-popup, wow). Diğer temalara göre daha eski/ağır bir yaklaşım.
- **API çağrıları:** Fetch/XHR'da 6 istek: IcebergTracker (`ice.js`), üç Sentry envelope, `view` çağrısı. İlan verisi XHR ile gelmiyor. 109 istek, 9.5 MB, 1.99 s.
- **Mobil davranış:** Responsive, filtreler dikey panele dönüşüyor.

## **Ayırt edici özellik: Pre-market ilanlar**

Ana sayfa ve listelerde "Coming Soon" etiketli, bulanıklaştırılmış ilanlar var. Bunlar portallara çıkmadan önce sadece kayıtlı kullanıcılara açılıyor. Erişim için **magic link ile e-posta girişi** gerekiyor (şifresiz, reCAPTCHA korumalı).

Bu, sitenin en güçlü tarafı: gerçek çalışan bir kullanıcı hesabı sistemi ve içerik kilitleme mekanizması mevcut. Ancak giriş yapan kullanıcı için sıralama, öneri veya kişiselleştirme değişmiyor — hesap sistemi sadece kapı görevi görüyor.

**Durum:** Yapıldı


### Tur 4 — Ayselin

## **Arama:**

- **Doğal Dil Araması:** **Yok** — Ana sayfa, grup içerisindeki diğer sitelere benzer şekilde Buy/Rent seçimi ve temel filtreleme yapısını kullanıyor. Kullanıcılar fiyat, yatak odası ve konum yarıçapı gibi kriterlerle arama yapabiliyor ancak serbest metin, anahtar kelime, mülk tipi veya harita tabanlı arama bulunmuyor. Bu durum ana sayfadaki “Find your dream home” söylemi ile mekanik arama deneyimi arasında belirgin bir fark oluşturuyor.  
  **AI fırsatı:** Doğal dil araması, kullanıcıların hayallerindeki mülkü kendi cümleleriyle tanımlamasına ve bu ifadelerin otomatik olarak uygun arama kriterlerine dönüştürülmesine olanak sağlayarak bu söylemi gerçek bir kullanıcı deneyimine dönüştürebilir.

- **Akıllı Öneriler / Sorgu Anlama:** **Yok** — İlan sonuçlarında “100% MATCH” rozeti bulunuyor ancak bunun gerçek anlamda kişiselleştirilmiş bir eşleştirmeyi temsil ettiği görülmüyor. Kayıtlı kriterleri olmayan anonim bir kullanıcıyla yapılan kontrolde 8/8 ilanın tamamında aynı %100 değeri gösterildi; ilanların fiyat ve yatak odası sayıları farklı olmasına rağmen sonuç değişmedi. Bu nedenle göstergenin AI tabanlı bir öneri sisteminden ziyade statik veya kural tabanlı bir arayüz öğesi olduğu düşünülüyor.

- **Kayıtlı Arama / Uyarılar:** **Mevcut** — Heads-Up Property Alerts; konum, yarıçap, fiyat, yatak odası, banyo, mülk tipi ve diğer tercihlerin kaydedilmesine olanak sağlıyor. Sistem uygun mülk önerileri, fiyat düşüşü bildirimleri ve henüz geniş çapta pazarlanmamış mülklere erken erişim sağlayabiliyor.

---

## **İlan Detayı:**

- **Mülk Özeti (AI):** **Yok** — İlan sayfalarında manuel olarak hazırlanmış açıklamalar ve özellik bilgileri bulunuyor. Ancak ilanın en önemli noktalarını kısa şekilde öne çıkaran AI tarafından oluşturulmuş bir özet bulunmuyor.

- **Mülk Soru-Cevap:** **Yok** — Kullanıcıların belirli bir mülk hakkında serbest biçimde soru sorabileceği AI destekli bir asistan bulunmuyor.

- **Mülk Öne Çıkan Özellikleri:** **Kısmi** — İlanlarda kısa mülk bilgilerinin yer aldığı özel bir FEATURES bölümü bulunuyor ancak içerikler AI tarafından dinamik olarak oluşturulmuyor; manuel olarak hazırlanıyor.

- **Yaşam Tarzı / "Kimler İçin Uygun?" Eşleştirmesi:** **Kısmi** — Bazı ilanlarda “Ideal for First-Time Buyers” veya “Ideal Buy-to-Let” gibi mülkün kimler için uygun olduğunu belirten ifadeler bulunuyor. Ancak bunlar AI tarafından oluşturulmuş kişiselleştirilmiş öneriler değil, manuel ilan içeriğinin bir parçası.

- **Mülk Karşılaştırma:** **Yok** — İki veya daha fazla mülkü fiyat, özellik, konum veya kullanıcıya uygunluk açısından karşılaştıran AI destekli bir araç gözlemlenmedi.

- **Benzer İlanlar (kişiselleştirilmiş):** **Mevcut** — Neuron'un eşleştirme altyapısı, kayıtlı alıcı kriterlerini uygun mülklerle eşleştiriyor ve sonuçlarda eşleşme yüzdeleri gösteriyor. Ancak anonim kullanıcılarla yapılan kontrolde görülen “100% MATCH” değerlerinin değişmemesi nedeniyle bu eşleştirmenin ne ölçüde gerçek bir kişiselleştirme sunduğu belirsiz.

- **Bölge İçgörüleri:** **Kısmi** — İlan sayfalarında bölge, yakın çevredeki olanaklar ve ulaşım bağlantıları hakkında bilgiler bulunuyor. Ancak bu bilgileri bir araya getirerek yapılandırılmış bir bölge analizi sunan AI destekli bir sistem bulunmuyor.

- **Ulaşım / İşe Gidiş İçgörüleri:** **Kısmi** — İlanlarda tren istasyonları ve diğer ulaşım bağlantılarından bahsedilebiliyor ancak kullanıcının iş yeri, okulu veya belirlediği hedef noktaya göre kişiselleştirilmiş ulaşım süresi analizi bulunmuyor.

- **Belge Açıklama (EPC / Kat Planı):** **Yok** — EPC bilgileri ve kat planları mevcut olduğunda sunuluyor ancak bu belgeleri sade bir dille açıklayan veya önemli noktaları öne çıkaran AI destekli bir özellik bulunmuyor.

---

## **Değerleme:**

- **Anlık Değerleme:** **Mevcut** — Harrisons, geçmiş satış verilerine ve bilgisayar tabanlı bir hesaplamaya dayanan ücretsiz bir online değerleme aracı sunuyor. Sistem bir başlangıç tahmini sağlıyor ve bunun yanında farklı doğruluk seviyeleriyle sanal ve yüz yüze değerleme seçenekleri de sunuluyor.

- **AI Değerleme Açıklaması:** **Yok** — Online araç tahmini bir değer sunsa da bu değerin arkasındaki faktörleri açıklayan AI destekli bir analiz veya kişiselleştirilmiş bir değerleme kırılımı bulunmuyor.  
  **AI fırsatı:** Değerleme sistemi; benzer satışlar, mülk özellikleri, konum ve piyasa koşulları gibi faktörleri kullanarak tahmini fiyat aralığını ve bu tahminin nedenlerini kullanıcıya anlaşılır şekilde gösterebilir.

- **Mortgage / Stamp Duty Calculator:** **Mevcut** — Değerleme/mülk sürecinin bir parçası olarak mortgage hesaplayıcısı bulunuyor. Kullanıcı mülk fiyatı, peşinat, kredi süresi ve faiz oranını girerek yaklaşık aylık ödeme tutarını hesaplayabiliyor. Ancak AI tarafından oluşturulan finansal yorum veya kişiselleştirilmiş finansal yönlendirme bulunmuyor.

---

## **İletişim:**

- **AI Chat Assistant / Chatbot:** **Yok** — Site genelinde veya mülk sayfalarında AI destekli chatbot bulunmuyor.

- **Lead Qualification:** **Kısmi** — Heads-Up kayıt süreci; taşınma nedeni, taşınma zamanı, solicitor durumu, mevcut mülkün satılması gerekip gerekmediği ve mortgage ihtiyaçları gibi detaylı alıcı bilgilerini topluyor. Bu bilgiler yapılandırılmış lead verisi sağlıyor ancak AI destekli lead scoring veya önceliklendirme sistemi bulunmuyor.

- **Otomatik Rezervasyon / Viewing Scheduling:** **Kısmi** — İlan sayfalarında “BOOK A VIEWING” seçeneği bulunuyor ve değerleme sürecinde tarih/saat seçimi yapılabiliyor. Ancak tüm rezervasyon sürecini yöneten konuşma tabanlı bir AI asistanı bulunmuyor.

- **Mesai Dışı Yanıt:** **Yok** — Normal çalışma saatleri dışında kullanıcı sorularını yanıtlayan veya talepleri otomatik olarak yöneten AI destekli bir sistem gözlemlenmedi.

---

## **Teknik / Genel:**

- **SSR vs CSR:** **Hibrit (SSR + CSR)** — Sayfanın ilk yüklenmesi server-side olarak gerçekleştiriliyor ve temel mülk ve içerik bilgileri doğrudan HTML içerisinde bulunuyor. Daha sonra client-side JavaScript etkileşimli bileşenleri ve navigasyonu yönetiyor.

- **API çağrıları:** **Mevcut** — Web sitesi Neuron / Iceberg Digital platformu üzerinde çalışıyor ve “AI Operating System for Estate Agents” altyapısını kullanıyor. Mülk eşleştirme ve alert özellikleri platforma entegre edilmiş durumda.

- **Mobil davranış:** **Mevcut** — Responsive web sitesi mobil cihazlarda mülk arama, ilanlar, Heads-Up uyarıları, değerleme araçları ve iletişim formlarına erişim sağlıyor.

- **Genel UX:** **İyi** — Web sitesi güçlü bir güven odaklı sunuma sahip ve ana sayfadaki istatistikleri ve performans verilerini etkili şekilde kullanıyor. Temel problem bu ikna edici mesajların mülk keşif ve ilan deneyimine aynı şekilde yansımaması. İlan deneyimi diğer Neuron tabanlı sitelere oldukça benzer ve temel seviyede kalıyor.

- **AI Fırsatı:** **Yüksek** — En büyük fırsat, sitenin “dream home” söylemini gerçekten akıllı bir mülk keşif deneyimiyle desteklemek. Doğal dil araması, gerçek anlamda kişiselleştirilmiş eşleştirme, AI mülk özetleri, Q&A ve şeffaf değerleme açıklamaları kullanıcı deneyimini önemli ölçüde geliştirebilir.

---

**Durum:** Yapıldı


### Ortak Bulgular / Sentez (4 tur bitince doldurulur)

- Ortak eksik AI özellikleri: Doğal dil arama, AI ilan özeti, Property Q&A, AI lead scoring, mesai dışı otomatik yanıt.
- Öne çıkan fırsatlar: (1) Gerçek çalışan bir hesap sistemi var (magic-link login — canlı doğrulandı: email gir, "send me a link" butonu, şifre yok) ve pre-market "Coming Soon" ilanları buna kilitli — ama giriş yapmış kullanıcı için erişim dışında hiçbir şey değişmiyor. (2) Cal.com üzerinden değerleme için gerçek randevu rezervasyonu çalışıyor — canlı olarak gerçek bir rezerve edilmiş slotla doğrulandı ("Sales market appraisal - Chris," 25 Ağustos 2026, 15:00–16:00, 1 saat, yüz yüze, Europe/Istanbul saat dilimi) — tüm çalışmada bulunan en net çalışan rezervasyon akışı. (3) Homepage'deki güçlü istatistikler ilan sayfalarına hiç yansımıyor.
- Görüş ayrılıkları / doğrulanması gerekenler: ✅ **Ayselin tarafından doğrulandı (canlı kontrol, Ağustos 2026):** "instant report" butonu `harrisonshomes.propalt.io/seller` adresine yönlendiriyor — `harrisonshomes.co.uk`'tan ve Neuron'un kendi altyapısından tamamen ayrı, gerçek bir 3. parti (Propalt) entegrasyonu — Neuron'un kendi anlık değerleme aracının bu tenant'ın ihtiyacını karşılamadığı hipotezini destekliyor. ⚠️ **Düzeltme:** Round 1'de belirtilen ana sayfa istatistik sayacı animasyon hatası (£0/0/0%'da takılı kalma) **artık mevcut değil** — canlı test, sayaçların şimdi sıfırdan doğru şekilde sayarak animasyonla yükseldiğini doğruluyor. Bu, orijinal incelemeden bu yana düzeltilmiş görünüyor.
