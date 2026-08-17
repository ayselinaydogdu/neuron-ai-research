# 04 · lloydsestates.com

**URL:** https://lloydsestates.com/
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
- Same platform search; two London offices (Woodford Green, Bethnal Green). No natural language, no map, same price/beds/radius filters.
- The discovery friction bites harder here because it's dense London: people search by "walkable to the Central line", not a radius circle. A mile-radius filter is the wrong mental model for a Tube city.
- **AI/area opportunity (strongest for London tenants):** commute-time and area insight would map much better onto how London buyers actually think than the current distance ring.

**Listing Detail:**
- Standard Neuron template. The 12-step selling process is documented well (good transparency), but that's seller-side content — it doesn't enrich the listing pages, which are the usual bullet-features + narrative with no AI summary/Q&A.

**Valuation:**
- Instant tool (`valuation.lloydsestates.com`) + book. Interesting tension: their own copy says "real accuracy comes from experience, not algorithms" and calls the instant tool "only ever a guide."
- Honest — but it quietly undercuts the very tool they're offering. **Opportunity for Neuron:** if agencies themselves distrust the instant number, an AI valuation *explanation* (what the estimate is based on, comparable evidence) turns the figure into something defensible rather than something to apologise for.

**Contact:**
- Phone for both offices, email, contact form. No chat, no out-of-hours. Standard generic enquiry — no qualification.

**Technical / General:**
- Neuron/Iceberg, Vercel, Lifesycle. Propertymark + TPO.
- Solid, dependable feel; testimonials include 15-year clients, which reads as genuine loyalty. Trust is fine — the anti-algorithm stance is actually a subtle signal about where AI features would need to earn agent buy-in, not just user approval.

**Status:** Done

### Round 2 — Berkay

## **Search:**

- **Natural Language Search:** **Absent** — Property search uses structured Buy/Rent controls and standard criteria rather than free-sentence queries.
- **Smart Suggestions / Query Understanding:** **Absent** — Property listing pages display a "100% MATCH" badge on every property (9/9 checked, anonymous visitor, no saved criteria — including SSTC and Under Offer listings). The footer explicitly credits "Neuron | Iceberg Digital AI Operating System for Estate Agents," confirming this is the same white-labelled platform infrastructure observed on other sites in this group. As with those sites, all listings displaying an identical 100% value regardless of user profile indicates a static/rule-based UI label rather than genuine personalised AI matching. No evidence of intelligent query understanding or suggestion logic was observed.
- **Saved Search / Alerts:** **Present** — Heads-Up Property Alerts allow users to save locations, property types, price, bedrooms, bathrooms and other requirements. The system sends tailored suggestions, new-listing notifications and price-reduction alerts.

## **Listing Detail:**

- **Property Summary (AI):** **Absent** — Property pages contain manually written descriptions and feature information, but no AI-generated 2–3 point summary was observed.
- **Property Q&A:** **Absent** — No free-form AI Q&A for individual listings was observed.
- **Property Highlights:** **Partial** — Listings provide structured property features alongside the main description, but no evidence that these highlights are AI-generated was observed.
- **Lifestyle / "Ideal for…" Matching:** **Partial** — Property descriptions can explain suitability and local benefits, while the matching system connects properties with buyer requirements. No explicit AI-generated lifestyle commentary was observed.
- **Property Comparison:** **Absent** — No AI-powered comparison of two or more properties was observed.
- **Similar Listings (personalised):** **Present** — The matching system uses registered buyer requirements to identify properties that specifically match the user's profile, evidenced by the same observable match-% UI element noted above; underlying platform identity (Neuron/Iceberg or otherwise) is unconfirmed.
- **Area Insights:** **Partial** — Property and blog content provides information about local areas, amenities and transport, but no dedicated AI-generated neighbourhood analysis was observed.
- **Commute Insights:** **Partial** — Property information can mention nearby stations and transport connections, but no personalised commute-time analysis based on the user's destination was observed.
- **Document Explanation (EPC / Floor Plan):** **Absent** — EPC information and floor plans may be available with listings, but no AI-powered plain-language explanation was observed.

## **Valuation:**

- **Instant Valuation:** **Present** — Lloyds provides an instant online valuation based on property details and local market/sold-price data. The site describes it as a quick guide rather than a replacement for an in-person valuation.
- **AI Valuation Explanation:** **Absent** — The online valuation uses an algorithm and market data but does not provide an AI-generated explanation of the valuation factors or a personalised narrative.
- **Mortgage / Stamp Duty Calculator:** **Partial** — Lloyds provides access to independent mortgage advisers and explains mortgage options, but no dedicated mortgage or Stamp Duty calculator with AI financial commentary was observed.

## **Contact:**

- **AI Chat Assistant / Chatbot:** **Absent** — No site-wide or property-level AI chat assistant was observed.
- **Lead Qualification:** **Partial** — Heads-Up registration collects detailed buyer circumstances including reason for moving, moving timeframe, solicitor status, whether the user needs to sell their current property and mortgage requirements. This provides structured lead information, but no AI-powered lead scoring or prioritisation was observed.
- **Automated Booking / Viewing Scheduling:** **Partial** — Property listings provide viewing/contact options and Lloyds promotes flexible accompanied viewings, but no AI-driven appointment scheduling or conversational booking assistant was observed.
- **Out-of-hours Response:** **Partial** — Lloyds promotes flexible opening times and reports fast responses to enquiries, but no AI-powered out-of-hours chatbot or automated conversational response was observed.

## **Technical / General:**

- **SSR vs CSR:** **Hybrid (SSR + CSR)** — Initial page load is server-side rendered, with core property and content information present directly in the delivered HTML. Client-side hydration then takes over for interactive elements and further navigation. 
- **API calls:** **Partial** — The property search and matching functionality clearly uses external/property-platform infrastructure, but the specific runtime API endpoints were not confirmed through Network-tab inspection, and unlike sites 22/23 the platform is not explicitly self-identified as Neuron/Iceberg Digital.
- **Mobile behaviour:** **Present** — The responsive site provides access to property search, listings, alerts, valuation and contact forms on mobile.

**Status:** Done


### Round 3 — Yasemin

## **Search:**

- **Natural Language Search:** **No** — Typing a free-form sentence returns a "Couldn't find the address" error. The box only matches addresses.
- **Smart Suggestions / Query Interpretation:** **Partial** — Typo tolerance works ("Woodfrd" → Woodford). It comes from Google Places; typing "wood" suggests places outside the service area such as Woodbridge, Woodhall Spa and Woodstock. The default sort is "Suggested" (visible in the URL as `sort=suggested`) with no stated basis.
- **Saved Search / Alerts:** **Yes** — A criteria-based registration flow exists (Contact / Property Type / Circumstances), collecting multiple locations, radius and property type. Price-reduction notifications are promised. There is no layer that learns from behaviour.
- **Additional note:** The no-results page is well constructed — it states that no properties match the search criteria and directs the user to set up a Heads Up alert. An empty result is turned into a lead opportunity rather than a dead end. Still, nothing is recommended; the user only gets a link to a form.

## **Listing Detail:**

- **Property Summary (AI Summary):** **No** — The description is fluent and sales-oriented but there is no summary block. Campaign information such as "OPEN DAY - SATURDAY 15TH AUGUST" is added manually at the top of the text.
- **Property Q&A:** **No** — No channel for asking free-form questions.
- **Property Highlights:** **Partial** — A Features tab exists, entered by hand.
- **Lifestyle / "Ideal for..." Matching:** **Partial** — Phrases like "room to grow and adapt to your lifestyle" and "busy households" appear manually in the description. There is no profile-based matching.
- **Property Comparison:** **No** — No comparison or favourites function.
- **Similar Listing Suggestions:** **No** — No similar-listings block at the bottom of the page.
- **Area Insights:** **No** — A Map tab exists, but the points are Google's own data. No school, crime or demographic commentary.
- **Commute Insights:** **No** — Travel time is never calculated. Location advantages such as "Near Broadway Market" and "Near Clapton Station" are written by hand into listing titles.
- **Document Explanation (EPC / Floor Plan):** **No** — The EPC (current C 75, potential C 77) and floor plans sit on the page as images and are never explained.
- **Additional note:** The listing detail includes **Property Video as a separate tab**. The tab structure is: Features / Property Info / Property Video / Floor Plans / Map / EPC.

## **Valuation:**

- **Instant Valuation:** **Yes** — Hosted on the `valuation.lloydsestates.com` subdomain and provided by **ValPal Network**. It asks for postcode, number of bedrooms and property type. A third-party integration.
- **AI Valuation Explanation:** **No** — The basis of the figure isn't explained. The homepage states plainly that the tool is only ever a guide and that real accuracy comes from experience rather than algorithms.
- **Mortgage / Stamp Duty Calculator:** **No** — No calculator anywhere on the site.
- **Additional note:** Valuation is presented as three separate routes: Instant Valuation, On Site Valuation and **Instruct Us Now**. The third is a flow not seen on the other sites — it invites the user to instruct the agency directly without a valuation first. On `/valuations`, On Site and Instruct Us appear as two separate forms side by side.

## **Contact / Lead:**

- **AI Chat Assistant / Chatbot:** **No** — No chat widget or WhatsApp button on any page.
- **Lead Qualification:** **Yes** — It works at two points: the Circumstances section of the alert form (5 questions) and the viewing modal ("do I have a property to sell", "a property to let", "would I like it valued"). The questions are fixed with no branching.
- **Automated Booking / Viewing Scheduling:** **Partial** — "Arrange a Viewing" opens a calendar and time picker, but the modal states that this does not confirm the viewing. Preferences are collected; the booking is left to a human.
- **Out-of-Hours Response:** **Partial** — All three offices are closed Sunday and shut at 18:00 on weekdays. The Management Office lists a separate **"Out of Hours Emergency Repair Line"** — a genuine after-hours channel, but a phone line rather than automation.

## **Technical / General:**

- **SSR vs CSR:** **SSR** — Nuxt-based, content present in the HTML. Hosted on Vercel, files served from a `neuronwebsites.co.uk` subdomain. Theme layer `/theme4/`.
- **API calls:** 7 requests under Fetch/XHR: IcebergTracker (`ice.js`), four Sentry envelopes, a `view` call and a UUID fetch. Listing data does not arrive via XHR. 95 requests, 8.5 MB, 5.96 s — noticeably slower than the other sites.
- **Mobile behaviour:** Responsive; filters collapse into a vertical panel.
- **Key finding 1:** The source defines `.whatsapp-chatbot` and `.live-search-container` classes, but neither is active on the site. These components exist on the platform and haven't been switched on for this client.
- **Key finding 2:** The privacy policy link in the footer points to `lloydsestates.lifesycle.co.uk` — a separate Iceberg product or infrastructure layer.

## **Distinguishing feature: Multi-office structure**

The agency operates three locations: Woodford Green, Bethnal Green and a Management Office, with separate phone numbers for sales and lettings.

None of this reaches the site experience, however: search results aren't split by office, the contact form doesn't ask which office the enquiry concerns, and listing pages carry no responsible-office information. The user is left to work out which office is relevant to them.

### **Overall AI Opportunities**

Conventional estate agency functionality is in place: clean SSR, a broad filter set, a video tab, complete floor plans / map / EPC, and an instant valuation. None of it involves generative AI, however — the instant valuation is third-party, the viewing calendar only collects preferences, and the data sits unprocessed.

1. **The multi-office structure goes unused** — Three locations, two business lines (sales and lettings) and separate phone lines exist, yet the site behaves as a single undifferentiated agency. Users could be routed to the right office based on their location or search area.
2. **Collected data goes nowhere** — Location, property type and urgency are captured in the alert registration, seller status in the viewing modal, and property details in ValPal. Sorting still reads "Suggested" for everyone and no recommendations appear.
3. **The empty-result moment is well framed but incomplete** — When nothing matches, a dedicated page directs the user to alert registration. This is precisely where AI belongs: criteria could be relaxed to surface near alternatives, showing results immediately instead of asking for another form.

**Status:** Done

### Round 4 — Ayselin

## **Search:**

- **Natural Language Search:** **Absent** — The website follows the same structured search model used across the platform. Users can select Buy/Rent and filter properties using standard criteria such as price, bedrooms and location radius. There is no free-text search, natural-language input or map-based property discovery. For a London-focused agency, this is particularly limiting because users often search based on practical travel needs rather than simple distance.

- **Smart Suggestions / Query Understanding:** **Absent** — Property results display a “100% MATCH” indicator, but this does not appear to represent meaningful personalised matching. During testing, all 9/9 properties checked for an anonymous visitor without saved criteria displayed the same 100% value, including properties marked SSTC or Under Offer. This suggests a static or rule-based UI element rather than genuine AI-powered recommendations or query understanding.

- **Saved Search / Alerts:** **Present** — Heads-Up Property Alerts allow users to save requirements such as locations, property types, price, bedrooms, bathrooms and other preferences. The system provides property suggestions, new-listing notifications and price-reduction alerts.

- **AI / Area Opportunity:** **High** — London property searches often depend on questions such as “Can I walk to the Central line?” or “Can I get to work within 40 minutes?” A commute-time and area-insight layer would therefore be more useful than a simple radius filter. AI could combine transport data, travel time and neighbourhood information to provide more meaningful location-based recommendations.

---

## **Listing Detail:**

- **Property Summary (AI):** **Absent** — Property pages contain manually written descriptions and structured feature information, but no AI-generated summary was observed.

- **Property Q&A:** **Absent** — No property-specific AI assistant was available for answering free-form questions about individual listings.

- **Property Highlights:** **Partial** — Listings provide structured property features alongside the main description, but there is no evidence that these highlights are dynamically generated by AI.

- **Lifestyle / "Ideal for…" Matching:** **Partial** — Property descriptions can explain who a property may suit and highlight local benefits. However, there is no AI-generated lifestyle analysis connecting these characteristics with individual buyer preferences.

- **Property Comparison:** **Absent** — No AI-powered comparison feature was observed for comparing multiple properties based on price, location, features or suitability.

- **Similar Listings (personalised):** **Present** — The platform includes a matching mechanism that can connect registered buyer requirements with suitable properties. However, the visible match-percentage element does not appear to provide meaningful personalisation for anonymous users, so the extent of genuine AI-driven similarity matching remains unclear.

- **Area Insights:** **Partial** — Property and blog content provides information about local areas, amenities and transport. However, there is no dedicated AI-generated neighbourhood analysis combining these factors into a structured overview.

- **Commute Insights:** **Partial** — Listings may mention nearby stations and transport links, but there is no personalised commute-time analysis based on a user's workplace, school or chosen destination.  
  **AI opportunity:** This is one of the strongest opportunities for a London-focused agency. Users could enter a destination and receive estimated travel times, nearby transport options and an explanation of how the property's location fits their daily routine.

- **Document Explanation (EPC / Floor Plan):** **Absent** — EPC information and floor plans may be available, but no AI-powered plain-language explanation or document summary was observed.

---

## **Valuation:**

- **Instant Valuation:** **Present** — Lloyds provides an online valuation tool using property details and local market or sold-price information. The service is positioned as a quick guide rather than a replacement for a professional face-to-face valuation.

- **AI Valuation Explanation:** **Absent** — The online valuation provides an estimated figure based on algorithms and market information but does not explain the result through an AI-generated narrative or personalised breakdown.  
  **AI opportunity:** Instead of simply presenting an estimate, the system could explain which comparable properties, local market conditions and property characteristics influenced the result. This would make the automated valuation easier for both users and agents to trust.

- **Mortgage / Stamp Duty Calculator:** **Partial** — The agency provides access to independent mortgage advisers and information about mortgage options, but no dedicated mortgage or Stamp Duty calculator with AI-generated financial commentary was observed.

---

## **Contact:**

- **AI Chat Assistant / Chatbot:** **Absent** — No site-wide or property-level AI chatbot was observed.

- **Lead Qualification:** **Partial** — Heads-Up registration collects detailed buyer information including reason for moving, moving timeframe, solicitor status, whether the user needs to sell their existing property and mortgage requirements. However, there is no AI-powered lead scoring or prioritisation.

- **Automated Booking / Viewing Scheduling:** **Partial** — Property pages provide viewing and contact options, and the agency promotes flexible accompanied viewings. However, no AI-driven appointment scheduling or conversational booking assistant was observed.

- **Out-of-hours Response:** **Partial** — The agency promotes flexible opening times and quick responses to enquiries, but there is no evidence of an AI-powered out-of-hours chatbot or automated conversational response system.

---

## **Technical / General:**

- **SSR vs CSR:** **Hybrid (SSR + CSR)** — The initial page is server-rendered, with core property and content information available in the delivered HTML. Client-side JavaScript is then used for interactive components and navigation.

- **API calls:** **Partial** — Property search and matching functionality clearly relies on external or property-platform infrastructure. However, the exact runtime API endpoints were not confirmed through Network-tab inspection, and the website does not explicitly identify the underlying platform as Neuron/Iceberg Digital.

- **Mobile behaviour:** **Present** — The responsive website provides access to property search, listings, alerts, valuation tools and contact forms on mobile devices.

- **Overall UX:** **Good** — The website presents a solid and dependable brand image, supported by long-term customer relationships, testimonials and industry credentials. Trust does not appear to be the main issue. The bigger opportunity is improving property discovery, particularly for London users whose search behaviour is strongly influenced by transport and commute times.

- **AI Opportunity:** **High** — The strongest AI opportunity is location intelligence rather than simply adding a generic chatbot. Commute analysis, area insights and natural-language search would better match the way London buyers think about property. AI valuation explanations could also address the agency's cautious attitude toward automated valuations by making estimates more transparent and defensible.

---

**Status:** Done

### Findings / Synthesis (filled once all 4 rounds are done)

- Commonly missing AI features: Natural-language search, AI listing summaries, Property Q&A, AI lead scoring, out-of-hours automated response, commute calculation.
- Standout opportunities: (1) The strongest opportunity for a London-based tenant: commute-time/transport-based search and area insight instead of radius-based search. (2) The empty-results page is well designed but static — AI could relax the criteria and surface near alternatives immediately. (3) The multi-office structure (3 locations, separate sales/lettings lines) goes entirely unused on the site — location-based automatic routing could be added.
- Disagreements / to verify: The site says "real accuracy comes from experience, not algorithms," yet still offers its own instant valuation tool — this tension may show the value of an AI explanation layer. Page load time is noticeably slower than the other sites (5.96s) — a performance issue worth confirming.

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
- Aynı platform araması; iki Londra ofisi (Woodford Green, Bethnal Green). Doğal dil yok, harita yok, aynı price/beds/radius filtreleri.
- Keşif sürtünmesi burada daha çok canını yakıyor çünkü yoğun Londra: insanlar yarıçap dairesiyle değil "Central line'a yürüme mesafesi" ile arıyor. Mil yarıçapı filtresi bir metro şehri için yanlış zihinsel model.
- **AI/bölge fırsatı (Londra tenant'ları için en güçlüsü):** commute süresi ve bölge içgörüsü, Londralı alıcıların düşünme biçimine mevcut mesafe halkasından çok daha iyi oturur.

**İlan Detay:**
- Standart Neuron şablonu. 12 adımlı satış süreci iyi belgelenmiş (güzel şeffaflık), ama bu satıcı tarafı içeriği — ilan sayfalarını zenginleştirmiyor; onlar yine bullet-features + anlatı, AI özet/Q&A yok.

**Değerleme:**
- Anlık araç (`valuation.lloydsestates.com`) + randevu. İlginç bir gerilim: kendi metinleri "real accuracy comes from experience, not algorithms" diyor ve anlık aracı "only ever a guide" olarak niteliyor.
- Dürüst — ama sundukları aracın değerini sessizce baltalıyor. **Neuron için fırsat:** acenteler anlık rakama güvenmiyorsa, bir AI valuation *açıklaması* (tahminin neye dayandığı, comparable kanıtı) rakamı özür dilenen bir şey yerine savunulabilir bir şeye çevirir.

**İletişim:**
- Her iki ofis için telefon, e-posta, iletişim formu. Chat yok, mesai dışı yok. Standart tek tip enquiry — kalifikasyon yok.

**Teknik/Genel:**
- Neuron/Iceberg, Vercel, Lifesycle. Propertymark + TPO.
- Sağlam, güvenilir his; testimonial'larda 15 yıllık müşteriler var, bu gerçek sadakat gibi okunuyor. Güven iyi — anti-algoritma duruşu, AI özelliklerinin sadece kullanıcı onayı değil, danışman kabulü de kazanması gerektiğine dair ince bir işaret.

**Durum:** Yapıldı

### Tur 2 — Berkay

## **Arama:**

- **Doğal Dil Araması:** **Yok** — Mülk araması yapılandırılmış Satın Alma/Kiralama kontrolleri ve standart kriterleri kullanıyor; serbest cümleyle arama bulunmuyor.
- **Akıllı Öneriler / Sorgu Anlama:** **Yok** — İlan listeleme sayfalarında her mülkün yanında "100% MATCH" rozeti görünüyor .Diğer sitelerde olduğu gibi, tüm ilanların profil fark etmeksizin aynı %100 değerini göstermesi, gerçek kişiselleştirilmiş yapay zeka eşleştirmesi yerine statik/kural tabanlı bir UI etiketine işaret ediyor. Akıllı sorgu anlama veya öneri mantığına dair kanıt gözlemlenmedi.
- **Kayıtlı Arama / Uyarılar:** **Var** — Heads-Up Mülk Uyarıları ile konum, mülk tipi, fiyat, oda/banyo sayısı ve diğer kriterler kaydedilebiliyor. Sistem kişiselleştirilmiş öneriler, yeni ilan bildirimleri ve fiyat değişikliği bildirimleri sağlıyor.

## **İlan Detay:**

- **Mülk Özeti (YZ):** **Yok** — İlan sayfalarında manuel olarak hazırlanmış açıklamalar ve özellik bilgileri bulunuyor; yapay zeka tarafından oluşturulan 2–3 maddelik özet gözlemlenmedi.
- **Mülk Soru-Cevap:** **Yok** — İlan hakkında serbest biçimde soru sorulabilen yapay zeka destekli Q&A özelliği gözlemlenmedi.
- **Mülkün Öne Çıkan Özellikleri:** **Kısmi** — İlanlarda ana açıklamanın yanında yapılandırılmış mülk özellikleri bulunuyor; ancak bu özelliklerin yapay zeka tarafından oluşturulduğuna dair kanıt bulunmuyor.
- **Yaşam Tarzı / "... için ideal" Eşleştirmesi:** **Kısmi** — İlan açıklamalarında mülkün uygunluğu ve yerel avantajları anlatılabiliyor; matching sistemi de mülkleri alıcı gereksinimleriyle eşleştiriyor. Ancak açık bir AI yaşam tarzı yorumu gözlemlenmedi.
- **Mülk Karşılaştırma:** **Yok** — İki veya daha fazla mülkü yapay zeka ile karşılaştırma özelliği gözlemlenmedi.
- **Benzer İlanlar (kişiselleştirilmiş):** **Var** — Matching sistemi, kayıtlı alıcı gereksinimlerini kullanarak kullanıcının profiline özel uygun mülkleri belirliyor; bu, yukarıda belirtilen aynı gözlemlenebilir eşleşme yüzdesi arayüz öğesine dayanıyor.
- **Bölge İçgörüleri:** **Kısmi** — İlan ve blog içeriklerinde yerel bölgeler, olanaklar ve ulaşım hakkında bilgiler bulunuyor; ancak özel bir yapay zeka destekli bölge analizi bulunmuyor.
- **Ulaşım İçgörüleri:** **Kısmi** — İlanlarda istasyonlara ve ulaşım bağlantılarına yakınlık belirtilebiliyor; ancak kullanıcının hedef konumuna göre kişiselleştirilmiş ulaşım süresi analizi bulunmuyor.
- **Belge Açıklaması (EPC / Kat Planı):** **Yok** — EPC bilgileri ve kat planları ilanlarda bulunabiliyor; ancak bu belgeleri sade bir dille açıklayan yapay zeka özelliği gözlemlenmedi.

## **Değerleme:**

- **Anlık Değerleme:** **Var** — Lloyds, mülk bilgileri ve yerel piyasa/satış verilerine dayanan anlık online değerleme sunuyor. Site bunu yüz yüze değerlemenin yerine geçmeyen hızlı bir başlangıç tahmini olarak tanımlıyor.
- **Yapay Zeka Değerleme Açıklaması:** **Yok** — Online değerleme algoritma ve piyasa verilerini kullanıyor ancak değerlemenin faktörlerini açıklayan yapay zeka destekli bir anlatım veya kişiselleştirilmiş analiz bulunmuyor.
- **Mortgage / Damga Vergisi Hesaplayıcısı:** **Kısmi** — Lloyds bağımsız mortgage danışmanlarına erişim sağlıyor ve mortgage seçeneklerini açıklıyor; ancak yapay zeka destekli finansal yorum içeren özel bir mortgage veya Stamp Duty hesaplayıcısı gözlemlenmedi.

## **İletişim:**

- **Yapay Zeka Sohbet Asistanı / Chatbot:** **Yok** — Site genelinde veya ilan seviyesinde yapay zeka destekli sohbet asistanı gözlemlenmedi.
- **Müşteri Adayı Nitelendirme:** **Kısmi** — Heads-Up kayıt süreci; taşınma nedeni, taşınma zamanı, solicitor durumu, mevcut mülkün satılması gerekip gerekmediği ve mortgage ihtiyacı gibi ayrıntılı bilgiler topluyor. Bu yapılandırılmış lead bilgisi sağlıyor ancak yapay zeka destekli müşteri adayı puanlama veya önceliklendirme bulunmuyor.
- **Otomatik Rezervasyon / Görüntüleme Planlama:** **Kısmi** — İlanlarda görüntüleme/iletişim seçenekleri bulunuyor ve Lloyds esnek, danışman eşliğinde viewing hizmetini öne çıkarıyor; ancak yapay zeka destekli randevu planlama veya konuşma tabanlı rezervasyon asistanı gözlemlenmedi.
- **Mesai Dışı Yanıt:** **Kısmi** — Lloyds esnek çalışma saatlerini ve hızlı iletişimi öne çıkarıyor; ancak yapay zeka destekli mesai dışı sohbet botu veya otomatik konuşma tabanlı yanıt sistemi gözlemlenmedi.

## **Teknik/Genel:**

- **SSR ve CSR:** **Hibrit (SSR + CSR)** — İlk sayfa yüklemesi sunucu tarafında render ediliyor; temel ilan ve içerik bilgileri doğrudan teslim edilen HTML içinde yer alıyor. Ardından etkileşimli öğeler ve sonraki gezinmeler için istemci tarafı hydration devreye giriyor. 
- **API Çağrıları:** **Var** — Site kendisini Neuron / Iceberg Digital'in "Estate Agentlar için Yapay Zeka İşletim Sistemi" altyapısıyla güçlendirilmiş olarak tanımlıyor.
- **Mobil Davranış:** **Var** — Responsive site üzerinden mülk arama, ilanlar, alertler, değerleme ve iletişim formlarına mobil erişim sağlanıyor.

**Durum:** Yapıldı

### Tur 3 — Yasemin

## **Arama:**

- **Doğal Dil Araması:** **Yok** — Serbest cümle yazıldığında "Couldn't find the address" hatası dönüyor. Kutu sadece adres eşleştiriyor.
- **Akıllı Öneri / Sorgu Yorumlama:** **Kısmen** — Yazım hatası toleransı çalışıyor ("Woodfrd" → Woodford). Google Places kaynaklı; "wood" yazınca Woodbridge, Woodhall Spa, Woodstock gibi hizmet alanı dışı yerler öneriliyor. Sıralama varsayılanı "Suggested" (URL'de `sort=suggested`), dayanağı açıklanmıyor.
- **Kayıtlı Arama / Alerts:** **Var** — Kriterli kayıt akışı mevcut (Contact / Property Type / Circumstances). Çoklu konum, yarıçap ve mülk tipi alınıyor. Fiyat düşüşü bildirimi vaat ediliyor. Davranışa göre öğrenen katman yok.
- **Ek not:** Sonuç bulunamayan sayfa iyi kurgulanmış — "no properties matching your search criteria" mesajıyla birlikte Heads Up alert kurmaya yönlendiriyor. Yani boş sonuç bir kayıp değil, lead fırsatına çevriliyor. Ancak öneri üretilmiyor, sadece form linki veriliyor.

## **İlan Detay:**

- **Property Summary (AI Özet):** **Yok** — Açıklama akıcı ve satış odaklı yazılmış ama özet bloğu yok. Metnin başında "OPEN DAY - SATURDAY 15TH AUGUST" gibi kampanya bilgisi elle eklenmiş.
- **Property Q&A:** **Yok** — Serbest soru sorma kanalı yok.
- **Property Highlights:** **Kısmen** — Features sekmesi var, elle girilmiş.
- **Lifestyle / "Ideal for..." Eşleştirme:** **Kısmen** — Açıklamada "room to grow and adapt to your lifestyle", "busy households" gibi ifadeler elle geçiyor. Profil bazlı eşleştirme yok.
- **Property Comparison:** **Yok** — Karşılaştırma ve favori özelliği yok.
- **Benzer İlan Önerisi:** **Yok** — Sayfa altında benzer ilan bloğu yok.
- **Area Insights:** **Yok** — Map sekmesi var, POI'ler Google'ın verisi. Okul, suç, demografi yorumu yok.
- **Commute Insights:** **Yok** — Ulaşım süresi hesaplanmıyor. İlan başlıklarında "Near Broadway Market", "Near Clapton Station" gibi konum avantajları elle yazılmış.
- **Belge Açıklama (EPC / Floor Plan):** **Yok** — EPC (mevcut C 75, potansiyel C 77) ve kat planları görsel olarak duruyor, açıklanmıyor.
- **Ek not:** İlan detayında **Property Video ayrı bir sekme** olarak yer alıyor. Sekme yapısı: Features / Property Info / Property Video / Floor Plans / Map / EPC.

## **Değerleme:**

- **Instant Valuation:** **Var** — `valuation.lloydsestates.com` alt alan adında, **ValPal Network** sağlıyor. Posta kodu, oda sayısı ve mülk tipi soruyor. Üçüncü parti entegrasyon.
- **AI Valuation Açıklaması:** **Yok** — Rakamın dayanağı açıklanmıyor. Ana sayfada aracın "yalnızca bir rehber" olduğu, gerçek doğruluğun "algoritmalardan değil deneyimden" geldiği açıkça yazıyor.
- **Mortgage / Stamp Duty Calculator:** **Yok** — Hesaplayıcı bulunmuyor.
- **Ek not:** Değerleme üç ayrı yol olarak sunuluyor: Instant Valuation, On Site Valuation ve **Instruct Us Now**. Üçüncüsü diğer sitelerde görülmeyen bir akış — değerleme almadan doğrudan satış yetkisi vermeye yönlendiriyor. `/valuations` sayfasında On Site ve Instruct Us iki ayrı form olarak yan yana duruyor.

## **İletişim / Lead:**

- **AI Chat Assistant / Chatbot:** **Yok** — Hiçbir sayfada chat widget'ı veya WhatsApp butonu yok.
- **Lead Qualification:** **Var** — İki noktada çalışıyor: alert formundaki Circumstances (5 soru) ve viewing modalı ("satılacak mülküm var mı", "kiralanacak mülküm var mı", "değerlensin mi"). Sorular sabit, dallanma yok.
- **Otomatik Randevu / Viewing Planlama:** **Kısmen** — "Arrange a Viewing" takvim ve saat seçimi açıyor, ancak modalda "bu görüntülemeyi onaylamaz" yazıyor. Tercih toplanıyor, rezervasyon insana bırakılıyor.
- **Mesai Dışı Yanıt:** **Kısmen** — Üç ofis de Pazar kapalı, hafta içi 18.00'de kapanıyor. Management Office'te **"Out of Hours Emergency Repair Line"** adında ayrı bir telefon hattı var — gerçek bir mesai dışı kanal, ancak otomasyon değil, telefon.

## **Teknik/Genel:**

- **SSR vs CSR:** **SSR** — Nuxt tabanlı, içerik HTML'de mevcut. Vercel'de barındırılıyor, dosyalar `neuronwebsites.co.uk` alt alan adında. Tema katmanı `/theme4/`.
- **API çağrıları:** Fetch/XHR'da 7 istek: IcebergTracker (`ice.js`), dört Sentry envelope, `view` çağrısı ve bir UUID fetch. İlan verisi XHR ile gelmiyor. 95 istek, 8.5 MB, 5.96 s (diğer sitelerden belirgin yavaş).
- **Mobil davranış:** Responsive, filtreler dikey panele dönüşüyor.
- **Önemli bulgu 1:** Kaynak kodda `.whatsapp-chatbot` ve `.live-search-container` sınıfları tanımlı ama sitede aktif değil. Bu bileşenler platformda mevcut, bu müşteride açılmamış.
- **Önemli bulgu 2:** Footer'daki privacy policy bağlantısı `lloydsestates.lifesycle.co.uk` adresine gidiyor — Iceberg'in ayrı bir ürün/altyapı katmanı.

## **Ayırt edici özellik: Çok ofisli yapı**

Ajansın üç lokasyonu var: Woodford Green, Bethnal Green ve Management Office. Satış ve kiralama için ayrı telefon numaraları kullanılıyor.

Ancak bu yapı site deneyimine hiç yansımıyor: arama sonuçları ofise göre ayrılmıyor, iletişim formu hangi ofisle ilgilenildiğini sormuyor, ilan sayfasında sorumlu ofis bilgisi yok. Kullanıcı hangi ofisin kendisine yakın olduğunu kendisi çözmek zorunda.

### **Overall AI Opportunities**

Klasik emlak işlevleri yerinde: temiz SSR, geniş filtre seti, video sekmesi, kat planı / harita / EPC tam, anlık değerleme mevcut. Buna karşılık hiçbir noktada üretken AI yok — anlık değerleme üçüncü parti, viewing takvimi sadece tercih topluyor, veriler ham halde duruyor.

1. **Çok ofisli yapı kullanılmıyor** — Üç lokasyon, iki ayrı iş kolu (sales/lettings) ve ayrı telefon hatları var, ama site tek bir ajans gibi davranıyor. Kullanıcının konumuna veya aradığı bölgeye göre doğru ofise yönlendirme yapılabilir.
2. **Toplanan veri hiçbir yere akmıyor** — Alert kaydında bölge/tip/aciliyet, viewing modalında satıcı durumu, ValPal'de mülk detayı toplanıyor. Sıralama hâlâ herkes için "Suggested", öneri yok.
3. **Boş sonuç anı iyi kurgulanmış ama eksik** — Sonuç bulunamadığında kullanıcıyı alert kaydına yönlendiren bir sayfa var. Bu tam da AI'ın devreye gireceği an: kriterleri gevşeterek yakın alternatifler önerilebilir, form doldurtmak yerine anında sonuç gösterilebilir.

**Durum:** Yapıldı

### Tur 4 — Ayselin

## **Arama:**

- **Doğal Dil Araması:** **Yok** — Web sitesi platformdaki diğer sitelere benzer şekilde yapılandırılmış bir arama modeli kullanıyor. Kullanıcılar Buy/Rent seçimi yapıp fiyat, yatak odası ve konum yarıçapı gibi standart kriterlerle filtreleme yapabiliyor. Ancak serbest metin, doğal dil veya harita tabanlı mülk araması bulunmuyor. Londra odaklı bir emlak sitesi için bu durum daha da önemli çünkü kullanıcılar genellikle yalnızca mesafeye değil, günlük ulaşım ihtiyaçlarına göre arama yapıyor.

- **Akıllı Öneriler / Sorgu Anlama:** **Yok** — İlan sonuçlarında “100% MATCH” göstergesi bulunuyor ancak bunun gerçek anlamda kişiselleştirilmiş bir eşleştirmeyi temsil ettiği görülmüyor. Kayıtlı kriterleri olmayan anonim bir kullanıcıyla yapılan kontrolde 9/9 ilanın tamamında %100 değeri gösterildi; buna SSTC ve Under Offer durumundaki ilanlar da dahil. Bu nedenle göstergenin gerçek bir AI öneri veya sorgu anlama sisteminden ziyade statik/kural tabanlı bir arayüz öğesi olduğu düşünülüyor.

- **Kayıtlı Arama / Uyarılar:** **Mevcut** — Heads-Up Property Alerts; konum, mülk tipi, fiyat, yatak odası, banyo ve diğer kullanıcı tercihlerini kaydetmeye olanak sağlıyor. Sistem uygun mülk önerileri, yeni ilan bildirimleri ve fiyat düşüşü uyarıları sunuyor.

- **AI / Bölge Fırsatı:** **Yüksek** — Londra'da kullanıcılar “Central line'a yürüyerek ulaşabilir miyim?” veya “İşe 40 dakikada gidebilir miyim?” gibi sorularla mülk arayabiliyor. Bu nedenle basit bir yarıçap filtresinden ziyade ulaşım süresi ve bölge içgörüleri sunan bir sistem daha anlamlı olur. AI; ulaşım verilerini, seyahat süresini ve bölge bilgilerini birleştirerek daha kullanışlı konum önerileri sunabilir.

---

## **İlan Detayı:**

- **Mülk Özeti (AI):** **Yok** — İlan sayfalarında manuel olarak hazırlanmış açıklamalar ve yapılandırılmış özellik bilgileri bulunuyor ancak AI tarafından oluşturulmuş kısa bir mülk özeti bulunmuyor.

- **Mülk Soru-Cevap:** **Yok** — Kullanıcıların belirli bir ilan hakkında serbest biçimde soru sorabileceği mülke özel bir AI asistanı bulunmuyor.

- **Mülk Öne Çıkan Özellikleri:** **Kısmi** — İlanlarda ana açıklamanın yanında yapılandırılmış mülk özellikleri bulunuyor ancak bu özelliklerin AI tarafından dinamik olarak oluşturulduğuna dair bir kanıt yok.

- **Yaşam Tarzı / "Kimler İçin Uygun?" Eşleştirmesi:** **Kısmi** — İlan açıklamalarında mülkün kimlere uygun olabileceği ve bölgenin avantajları anlatılabiliyor. Ancak bu özellikleri bireysel alıcı tercihleriyle eşleştiren AI destekli bir yaşam tarzı analizi bulunmuyor.

- **Mülk Karşılaştırma:** **Yok** — Birden fazla mülkü fiyat, konum, özellikler veya kullanıcıya uygunluk açısından karşılaştıran AI destekli bir özellik gözlemlenmedi.

- **Benzer İlanlar (kişiselleştirilmiş):** **Mevcut** — Platform, kayıtlı alıcı kriterlerini uygun mülklerle eşleştiren bir sistem kullanıyor. Ancak anonim kullanıcılar için görülen eşleşme yüzdesinin anlamlı bir şekilde değişmemesi nedeniyle gerçek anlamda AI tabanlı kişiselleştirmenin ne ölçüde kullanıldığı belirsiz.

- **Bölge İçgörüleri:** **Kısmi** — İlan ve blog içeriklerinde bölge, çevredeki olanaklar ve ulaşım hakkında bilgiler bulunuyor. Ancak bu bilgileri bir araya getirerek yapılandırılmış bir bölge analizi sunan AI destekli bir sistem bulunmuyor.

- **Ulaşım / İşe Gidiş İçgörüleri:** **Kısmi** — İlanlarda yakın istasyonlar ve ulaşım bağlantılarından bahsedilebiliyor ancak kullanıcının iş yeri, okulu veya belirlediği hedef noktaya göre kişiselleştirilmiş ulaşım süresi analizi bulunmuyor.  
  **AI fırsatı:** Londra odaklı bir site için bu en güçlü AI fırsatlarından biri olabilir. Kullanıcı bir hedef noktası girdiğinde sistem tahmini ulaşım sürelerini, yakın ulaşım seçeneklerini ve mülkün günlük yaşam açısından ne kadar uygun olduğunu açıklayabilir.

- **Belge Açıklama (EPC / Kat Planı):** **Yok** — EPC bilgileri ve kat planları mevcut olduğunda sunuluyor ancak bunları sade bir dille açıklayan veya özetleyen AI destekli bir özellik bulunmuyor.

---

## **Değerleme:**

- **Anlık Değerleme:** **Mevcut** — Lloyds, mülk bilgileri ile yerel piyasa ve geçmiş satış verilerini kullanarak online bir değerleme aracı sunuyor. Sistem hızlı bir başlangıç tahmini olarak konumlandırılıyor ve profesyonel yüz yüze değerlemenin yerine geçmediği belirtiliyor.

- **AI Değerleme Açıklaması:** **Yok** — Online değerleme algoritmalar ve piyasa verileri kullanılarak tahmini bir değer sunuyor ancak bu sonucu açıklayan AI tarafından oluşturulmuş bir anlatım veya kişiselleştirilmiş değerleme analizi bulunmuyor.  
  **AI fırsatı:** Sistem yalnızca tahmini bir rakam göstermek yerine benzer satışların, bölgesel piyasa koşullarının ve mülk özelliklerinin sonucu nasıl etkilediğini açıklayabilir. Bu, otomatik değerlemenin hem kullanıcı hem de emlak danışmanı açısından daha güvenilir ve savunulabilir hale gelmesini sağlayabilir.

- **Mortgage / Stamp Duty Calculator:** **Kısmi** — Web sitesi bağımsız mortgage danışmanlarına erişim ve mortgage seçenekleri hakkında bilgi sunuyor ancak AI destekli finansal yorum içeren özel bir mortgage veya Stamp Duty hesaplayıcısı gözlemlenmedi.

---

## **İletişim:**

- **AI Chat Assistant / Chatbot:** **Yok** — Site genelinde veya mülk sayfalarında AI destekli chatbot bulunmuyor.

- **Lead Qualification:** **Kısmi** — Heads-Up kayıt süreci; taşınma nedeni, taşınma zamanı, solicitor durumu, mevcut mülkün satılması gerekip gerekmediği ve mortgage ihtiyaçları gibi detaylı alıcı bilgilerini topluyor. Ancak AI destekli lead scoring veya önceliklendirme sistemi bulunmuyor.

- **Otomatik Rezervasyon / Viewing Scheduling:** **Kısmi** — İlan sayfalarında viewing ve iletişim seçenekleri bulunuyor ve esnek eşlikli viewing hizmetleri sunuluyor. Ancak AI destekli otomatik randevu planlama veya konuşma tabanlı rezervasyon asistanı bulunmuyor.

- **Mesai Dışı Yanıt:** **Kısmi** — Web sitesi esnek çalışma saatlerini ve hızlı geri dönüşleri öne çıkarıyor ancak mesai dışında çalışan AI destekli chatbot veya otomatik konuşma tabanlı yanıt sistemi bulunmuyor.

---

## **Teknik / Genel:**

- **SSR vs CSR:** **Hibrit (SSR + CSR)** — İlk sayfa yüklemesi server-side olarak gerçekleştiriliyor ve temel mülk bilgileri doğrudan HTML içerisinde bulunuyor. Daha sonra client-side JavaScript etkileşimli bileşenleri ve navigasyonu yönetiyor.

- **API çağrıları:** **Kısmi** — Mülk arama ve eşleştirme özelliklerinin harici veya emlak platformu altyapısına dayandığı açıkça görülüyor. Ancak spesifik runtime API endpoint'leri Network-tab incelemesiyle doğrulanmadı ve web sitesi kullanılan altyapıyı açık şekilde Neuron/Iceberg Digital olarak belirtmiyor.

- **Mobil davranış:** **Mevcut** — Responsive web sitesi mobil cihazlarda mülk arama, ilanlar, uyarılar, değerleme araçları ve iletişim formlarına erişim sağlıyor.

- **Genel UX:** **İyi** — Web sitesi uzun süreli müşteri ilişkileri, referanslar ve sektör belgeleriyle sağlam ve güvenilir bir marka algısı oluşturuyor. Temel problem güven değil. Daha büyük fırsat, özellikle Londra'daki kullanıcıların ulaşım ve işe gidiş sürelerine dayalı arama davranışını destekleyecek daha gelişmiş bir mülk keşif deneyimi sunmak.

- **AI Fırsatı:** **Yüksek** — En güçlü AI fırsatı genel amaçlı bir chatbot eklemekten ziyade konum zekâsını geliştirmek. Ulaşım analizi, bölge içgörüleri ve doğal dil araması Londra'daki kullanıcıların mülk arama biçimine çok daha uygun olacaktır. AI destekli değerleme açıklamaları da ajansın algoritmik değerlemelere karşı temkinli yaklaşımını destekleyebilir ve tahminleri daha şeffaf ve güvenilir hale getirebilir.

---

**Durum:** Yapıldı

### Ortak Bulgular / Sentez (4 tur bitince doldurulur)

- Ortak eksik AI özellikleri: Doğal dil arama, AI ilan özeti, Property Q&A, AI lead scoring, mesai dışı otomatik yanıt, commute hesabı.
- Öne çıkan fırsatlar: (1) Londra'ya özgü en güçlü fırsat: radius-tabanlı arama yerine commute-time/ulaşım tabanlı arama ve alan analizi. (2) Boş sonuç sayfası iyi tasarlanmış ama statik — AI ile kriterleri gevşetip yakın alternatifleri anlık gösterebilir. (3) Çok şubeli yapı (3 ofis, satış/kiralama ayrı hatlar) sitede hiç kullanılmıyor — konum bazlı otomatik yönlendirme yapılabilir.
- Görüş ayrılıkları / doğrulanması gerekenler: Site "algoritmaya değil deneyime güvenin" diyor ama kendi instant valuation aracını sunuyor — bu çelişki AI açıklama katmanının değerini gösterebilir. Sayfa yükleme süresi diğer sitelere göre belirgin şekilde yavaş (5.96s) — performans sorunu doğrulanmalı.
