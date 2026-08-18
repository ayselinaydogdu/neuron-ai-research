# 17 · greyandco.co.uk

**URL:** https://greyandco.co.uk/
**Group / Grup:** D

---

## English

This site is reviewed independently by 4 people across 4 rounds.

| Round | Reviewer | Status   |
| ----- | -------- | -------- |
| 1     | Berkay   | Done     |
| 2     | Yasemin  | Done     |
| 3     | Ayselin  | Done |
| 4     | Görkem   | Done |

> Fill in only your own round block; don't edit anyone else's.
> Write short, concrete sentences (not "yes/no" — say what it is).
> What to check: ../checklist.md · Terms: ../info/ai-feature-glossary.md

### Round 1 — Berkay

## **Search:**

- **Natural Language Search:** **Absent** — Property search uses structured search controls for buying or renting rather than free-sentence queries.
- **Smart Suggestions / Query Understanding:** **Partial** — Search results can display a "100% MATCH" indicator against the user's saved criteria, but no natural-language interpretation, typo handling, or intelligent query refinement was observed.
- **Saved Search / Alerts:** **Present** — Heads Up Property Alerts allow users to receive updates about new properties matching their wish list and criteria.

## **Listing Detail:**

- **Property Summary (AI):** **Absent** — Listings provide manually written descriptions and property information, but no AI-generated 2–3 point summary was observed.
- **Property Q&A:** **Absent** — No free-form AI Q&A for individual listings was observed.
- **Property Highlights:** **Absent** — Listings contain a manually written Features section, but no AI-extracted property highlights were observed.
- **Lifestyle / "Ideal for…" Matching:** **Absent** — Listings may describe suitability for families or other uses, but no AI-powered lifestyle matching was observed.
- **Property Comparison:** **Absent** — No AI-powered comparison of multiple properties was observed.
- **Similar Listings (personalised):** **Absent** — No behaviour-based or personalised "you might also like" recommendations were observed.
- **Area Insights:** **Partial** — Property descriptions can include local information such as nearby stations, schools and amenities, and the site provides local guides, but no AI-generated area commentary was observed.
- **Commute Insights:** **Absent** — Transport links are sometimes mentioned in property descriptions, but there is no dedicated commute-time analysis with commentary.
- **Document Explanation (EPC / Floor Plan):** **Absent** — Floor plans and EPC information are provided on listings, but no AI-powered plain-language explanation of these documents was observed.

## **Valuation:**

- **Instant Valuation:** **Present** — A 60-second online valuation provides an estimated property value using a computer algorithm based on previous sales data.
- **AI Valuation Explanation:** **Absent** — The valuation does not provide an AI-generated explanation or personalised commentary explaining the estimated value.
- **Mortgage / Stamp Duty Calculator:** **Partial** — Mortgage guidance and broker recommendations are available, but no dedicated mortgage/stamp-duty calculator with AI financial commentary was observed.

## **Contact:**

- **AI Chat Assistant / Chatbot:** **Absent** — No site-wide or property-level AI chat assistant was observed.
- **Lead Qualification:** **Absent** — The contact form collects standard information such as name, email, phone number, enquiry type and message, with no AI pre-screening or lead scoring observed.
- **Automated Booking / Viewing Scheduling:** **Partial** — Properties provide a "BOOK A VIEWING" option, but no AI-driven scheduling or automated qualification was observed.
- **Out-of-hours Response:** **Absent** — The site displays office opening hours and contact details, but no automated out-of-hours chatbot or response system was observed.

## **Technical / General:**

- **SSR vs CSR:** **Hybrid (SSR + CSR)** — Initial page load is server-side rendered, with core property and content information present directly in the delivered HTML. Client-side hydration then takes over for interactive elements and further navigation. 
- **API calls:** **Present** — The site is explicitly powered by Neuron / Iceberg Digital's "AI Operating System for Estate Agents". Property search results also expose the AI matching functionality through percentage-based match indicators. This verdict rests on vendor self-identification plus the observable match-% UI element; specific runtime API endpoints were not confirmed through Network-tab inspection.
- **Mobile behaviour:** **Present** — The responsive site provides access to property search, listings, alerts, valuation and contact functionality on mobile.

**Status:** Done

### Round 2 — Yasemin

**Search:**

- Classic filter-based search is available (price, bedrooms, bathrooms, receptions, property type, Must Haves, radius); no map view is offered.
- Natural Language Search is not available; entering a free-text sentence returns "Couldn't find the address".
- Spelling mistakes are corrected, but this comes from the address autocomplete; AI-supported query interpretation is not available.
- Personalised ranking is not available; the "Suggested" default and the "100% MATCH" badge only reflect filter compliance.
- The 30 results are listed only through "LOAD MORE"; no intelligent suggestion appears when results narrow down or return empty.

**Property Detail:**

- Listing copy is written manually and varies in length and tone between listings; no AI Summary or Property Highlights are generated.
- There are 26 photos, a floor plan and an EPC image; no 360° virtual tour and no layer explaining these documents in plain language.
- There is no "similar properties" section; the page goes straight from the EPC to the footer.
- The only contact route is the Book a Viewing form; no AI Chat Assistant provides an immediate answer.
- The map shows the property location; Area Insights and Commute Insights are not offered.

**Valuation:**

- Instant Valuation runs on ValPal on a separate subdomain in two steps; an address is selected, then name, email and phone are requested.
- The figure is not shown on screen; the user is told it is being calculated and it is sent later in exchange for contact details, so there is no estimate to explain either.
- The face-to-face valuation form asks detailed questions about the reason for moving, timescale and previous agency experience; none of these answers feed into any output.
- No mortgage or stamp duty calculator is offered; mortgages are covered only by a text block and a link to guides.

**Contact:**

- No active AI Chat Assistant / Chatbot is present; a msgboxx-based WhatsApp widget appears in the source but does not run in the interface.
- The contact form asks for first name, surname, email, phone, message and a Buy/Sell/Rent/Let selection; the selection does not change the flow and no AI Lead Qualification is performed.
- Viewing appointments are requested by picking a day and time from a calendar, but availability is not confirmed and no AI-supported scheduling is offered.
- Opening hours are listed on the page, but no automated response is provided outside working hours.

**Technical/General:**

- The page is rendered server-side with Nuxt, while listing content arrives client-side through the `filter?search_type=sales` call.
- Requests for `property_types`, `property_styles` and `tenure_types` go to the Neuron API; `ice.js` and Sentry are running, but the data collected does not turn into personalisation.
- Filters and forms work without issue on mobile; no screen-specific simplification or suggestion layer is provided.

**Status:** Done

### Round 3 — Ayselin

## Search

- A conventional property search is available with standard filters such as price, bedrooms, bathrooms, reception rooms, property type, Must Haves, and distance. There is no map-based search view.
- Natural Language Search is not supported. When a free-form sentence is entered, it is treated as an address query and returns `"Couldn't find the address"` instead of interpreting the user's intent.
- Spelling correction is available, but this appears to be part of the address autocomplete functionality rather than AI-powered query interpretation.
- A `Suggested` sorting option and `100% MATCH` indicator are available. However, these represent matching against the selected filters rather than personalized ranking based on user behavior.
- Around 30 results are displayed with a `LOAD MORE` option. There is no AI-powered refinement or automatic suggestion of additional search criteria when there are many results.
- Heads Up Property Alerts are available, allowing users to receive notifications about new properties matching their selected criteria.

## Property Details

- Property descriptions are manually written and vary in length and style between listings. There is no AI-generated Property Summary or automatically generated Property Highlights.
- Property pages include photo galleries, Floor Plans, and EPC information. However, there is no 360° virtual tour or AI-powered explanation of EPC/Floor Plan documents.
- Users cannot ask natural-language questions about a property; no AI Property Q&A feature is available.
- Property Comparison and personalized Similar Property recommendations are not provided. After the main property content, the page mainly directs users to other sections of the website.
- A map is provided to show the property location, but there are no AI-powered Area Insights or Commute Insights.
- A `Book a Viewing` form is available, but there is no active AI Chat Assistant providing instant responses on the property page.

## Valuation

- Instant Valuation is available and operates through ValPal on a separate subdomain.
- The valuation process first requires the user to select the property address, followed by their name, email, and phone number. The estimated value is not displayed directly on the screen and is provided after the contact details are submitted.
- The Face-to-Face Valuation form collects additional information such as the reason for moving, expected timeframe, and previous estate agent experience. These answers are not turned into an AI-generated analysis or personalized result.
- There is no AI-generated explanation of how the estimated property value is calculated.
- No Mortgage or Stamp Duty Calculator is available; mortgage-related information is provided mainly through informational content and guidance.

## Contact

- There is no active AI Chat Assistant or chatbot across the website or property pages.
- The contact form contains standard fields such as first name, last name, email, phone number, message, and Buy/Sell/Rent/Let selection. The selected option does not appear to change the form flow, and no AI-powered Lead Qualification is provided.
- Viewing requests can be submitted by selecting a date and time through a calendar, but real-time availability is not confirmed and there is no AI-powered automatic scheduling.
- Business hours are provided, but there is no automated AI response system outside working hours.
- A WhatsApp/msgboxx-based widget is referenced in the source, but it was not observed as an active chatbot in the user interface.

## Technical / General

- The website uses Nuxt-based SSR. Core property content is rendered on the server during the initial page load, while search results are loaded client-side.
- Network requests to the Neuron API use standard filter parameters such as `property_types`, `property_styles`, and `tenure_types`. `ice.js` and Sentry services are also observed.
- No separate API request to an AI/LLM service was identified for processing user queries with generative AI.
- The website is responsive on mobile; filters, property listings, and contact forms remain usable on smaller screens. No mobile-specific AI functionality is provided.

**Status:** Done

### Round 4 — Görkem

**Search:**
- Full platform filter set (price/beds/baths/receptions/type/Must-Haves/radius, no map). Free sentence → "Couldn't find the address". ~30 results behind "LOAD MORE".
- The "100% MATCH"/"Suggested" indicators are the platform's built-in match badge — filter-compliance, not behavioural ranking, same as every Group-D tenant. The site does have decent **local area guides**, which are static today but would make ideal grounding for an area-Q&A or a natural-language layer later.

**Listing Detail:**
- Manually written copy varying in length/tone; a listing I looked at had ~26 photos, floor plan and EPC image but **no similar-properties block at all** — the page drops from EPC straight to the footer. No summary, no Q&A, no 360.
- Standard ceiling; nothing here escapes the group pattern.

**Valuation — flagging a disagreement to verify:**
- Instant Valuation runs on **ValPal on a separate subdomain.** In my walk-through it behaved like the platform norm: select address, then name/email/phone, with **no figure shown on screen** (matches Yasemin's and Ayselin's Round 2/3 notes).
- ⚠️ But Round 1 (Berkay) recorded this as a **"60-second online valuation that returns an estimated value via algorithm on previous sales."** That's a real contradiction — either the tool shows a number or it gates it. It may vary by entry path or have changed. **This one should be re-checked live before we cite it either way.** I'm noting it rather than papering over it.
- The face-to-face form asks reason-for-moving / timescale / previous-agency, and none of those answers feed any output — captured, unused. No mortgage/stamp-duty calculator, just broker guidance text.

**Contact:**
- No working chatbot; a **msgboxx WhatsApp widget is referenced in the source but I didn't see it running** in the UI (another dormant platform hook). Contact form + Buy/Sell/Rent/Let that changes nothing; viewing via calendar with no confirmed availability. No out-of-hours answer.

**Technical / General:**
- **Hybrid SSR + CSR**: core content server-rendered, listings loaded client-side via the `filter?search_type=sales` call to the Neuron API (`property_types` etc.), with `ice.js` + Sentry. The behavioural data `ice.js` collects **is not turned into any personalisation** — it's gathered and wasted, which is a recurring theme.
- Responsive; forms not submitted; no real-device test.

**Status:** Done

### Findings / Synthesis (filled once all 4 rounds are done)

### Findings / Synthesis

- Commonly missing AI features: Natural-language search and smart query refinement, AI listing summaries, Property Q&A, personalised similar-listing recommendations, AI-powered area/commute insights, EPC/floor plan explanation, AI lead qualification, automated viewing scheduling, out-of-hours response, and mortgage/stamp-duty calculators with AI commentary.

- Standout opportunities: The site already has detailed **local area guides**, providing useful existing content that could ground an AI Area Q&A or natural-language property search without requiring a new knowledge base from scratch. **ice.js** also collects behavioural data, but no resulting personalisation or behavioural ranking was observed; this creates a clear opportunity to turn existing signals into personalised property recommendations. Listing pages currently contain **no similar-properties section at all**, making criteria- or behaviour-based recommendations another straightforward improvement. The Face-to-Face Valuation form also collects useful qualification data such as moving reason, timescale and previous agency experience, but these inputs are not used to personalise the resulting journey.

- Disagreements / to verify: The main disagreement concerns **ValPal Instant Valuation**. Round 1 describes it as a 60-second algorithmic valuation based on previous sales data, while Rounds 2–4 independently found that the user selects an address and then provides name, email and phone details without an estimated value being displayed on screen. The latter behaviour is therefore supported by three independent reviews, but the difference should remain flagged for live verification. Technically, the site uses **Nuxt with Neuron / Iceberg Digital infrastructure**; search data is retrieved through the Neuron API, while **ice.js and Sentry** are also present. No separate generative AI/LLM API call was identified. A **msgboxx-based WhatsApp widget** is referenced in the source but was not observed operating in the interface, suggesting an existing but inactive third-party communication component. **Analysed and verified by Berkay.**

---

## Türkçe

Bu siteyi 4 tur boyunca 4 farklı kişi bağımsız inceler.

| Tur   | İnceleyen| Durum    |
| ----- | -------- | -------- |
| 1     | Berkay   | Yapıldı  |
| 2     | Yasemin  | Yapıldı  |
| 3     | Ayselin  | Yapıldı|
| 4     | Görkem   | Yapıldı|
> Sadece kendi tur bloğunuzu doldurun; başkasının bloğunu değiştirmeyin.
> Kısa, somut cümleler yazın ("Var/Yok" değil, ne olduğunu yazın).
> Neye bakılacağı: ../checklist.md · Terimler: ../info/ai-feature-glossary.md

### Tur 1 — Berkay

## **Arama:**

- **Doğal Dil Araması:** **Yok** — Mülk araması, satın alma/kiralama için yapılandırılmış arama kontrollerini kullanıyor; serbest cümleyle arama gözlemlenmedi.
- **Akıllı Öneriler / Sorgu Anlama:** **Kısmi** — Arama sonuçlarında kullanıcının kayıtlı kriterleriyle eşleşmeyi gösteren "100% MATCH" ifadesi bulunabiliyor; ancak doğal dil yorumlama, yazım hatası yönetimi veya akıllı sorgu daraltma gözlemlenmedi.
- **Kayıtlı Arama / Uyarılar:** **Var** — Heads Up Mülk Uyarıları, kullanıcıların istek listelerine ve kriterlerine uyan yeni ilanlar hakkında bildirim almasını sağlıyor.

## **İlan Detay:**

- **Mülk Özeti (YZ):** **Yok** — İlanlarda manuel olarak hazırlanmış açıklamalar ve mülk bilgileri bulunuyor; yapay zeka tarafından oluşturulan 2–3 maddelik özet gözlemlenmedi.
- **Mülk Soru-Cevap:** **Yok** — İlan hakkında serbest biçimde soru sorulabilen yapay zeka destekli bir Q&A özelliği gözlemlenmedi.
- **Mülkün Öne Çıkan Özellikleri:** **Yok** — İlanlarda manuel olarak hazırlanmış Özellikler bölümü bulunuyor; yapay zeka tarafından çıkarılmış öne çıkan özellikler bulunmuyor.
- **Yaşam Tarzı / "... için ideal" Eşleştirmesi:** **Yok** — İlan açıklamalarında aileler veya farklı kullanım amaçları için uygunluk ifadeleri bulunabiliyor; ancak yapay zeka destekli yaşam tarzı eşleştirmesi gözlemlenmedi.
- **Mülk Karşılaştırma:** **Yok** — Birden fazla mülkü yapay zeka ile karşılaştırma özelliği gözlemlenmedi.
- **Benzer İlanlar (kişiselleştirilmiş):** **Yok** — Kullanıcı davranışına göre kişiselleştirilmiş benzer ilan önerileri gözlemlenmedi.
- **Bölge İçgörüleri:** **Kısmi** — İlan açıklamalarında istasyon, okul ve çevredeki olanaklar gibi yerel bilgiler bulunabiliyor ve sitede bölgesel rehberler yer alıyor; ancak yapay zeka tarafından oluşturulan bölge yorumu bulunmuyor.
- **Ulaşım İçgörüleri:** **Yok** — Ulaşım bağlantıları bazı ilanlarda belirtiliyor, ancak ulaşım süresini analiz eden özel bir özellik bulunmuyor.
- **Belge Açıklaması (EPC / Kat Planı):** **Yok** — Kat planları ve EPC bilgileri sunuluyor, ancak bu belgeleri sade bir dille açıklayan yapay zeka özelliği bulunmuyor.

## **Değerleme:**

- **Anlık Değerleme:** **Var** — 60 saniyelik online değerleme, önceki satış verilerini kullanan bilgisayar algoritmasıyla tahmini mülk değeri sağlıyor.
- **Yapay Zeka Değerleme Açıklaması:** **Yok** — Tahmini değerin arkasındaki faktörleri açıklayan yapay zeka destekli veya kişiselleştirilmiş bir yorum bulunmuyor.
- **Mortgage / Damga Vergisi Hesaplayıcısı:** **Kısmi** — Mortgage konusunda yönlendirme ve broker önerileri bulunuyor; ancak yapay zeka destekli finansal yorum içeren özel bir mortgage/stamp duty hesaplayıcısı gözlemlenmedi.

## **İletişim:**

- **Yapay Zeka Sohbet Asistanı / Chatbot:** **Yok** — Site genelinde veya ilan seviyesinde yapay zeka destekli sohbet asistanı gözlemlenmedi.
- **Müşteri Adayı Nitelendirme:** **Yok** — İletişim formu isim, e-posta, telefon, talep türü ve mesaj gibi standart bilgileri topluyor; yapay zeka destekli ön eleme veya müşteri adayı puanlama bulunmuyor.
- **Otomatik Rezervasyon / Görüntüleme Planlama:** **Kısmi** — İlanlarda "BOOK A VIEWING" seçeneği bulunuyor; ancak yapay zeka destekli planlama veya otomatik lead değerlendirmesi gözlemlenmedi.
- **Mesai Dışı Yanıt:** **Yok** — Ofis çalışma saatleri ve iletişim bilgileri sunuluyor, ancak mesai dışı otomatik sohbet botu veya yanıt sistemi gözlemlenmedi.

## **Teknik/Genel:**

- **SSR vs CSR:** **Hybrid (SSR + CSR)** — Initial page load is server-side rendered, with core property and content information present directly in the delivered HTML. Client-side hydration then takes over for interactive elements and further navigation. 
- **API Çağrıları:** **Var** — Site açıkça Neuron / Iceberg Digital'in "Estate Agentlar için Yapay Zeka İşletim Sistemi" altyapısını kullanıyor. Property search sonuçlarında yapay zeka eşleştirme sistemi yüzde bazlı eşleşme göstergeleriyle görünür durumda. 
- **Mobil Davranış:** **Var** — Responsive site üzerinden mülk arama, ilanlar, alertler, değerleme ve iletişim özelliklerine mobil erişim sağlanıyor.


**Durum:** Yapıldı

### Tur 2 — Yasemin

**Arama:**

- Klasik filtre tabanlı arama mevcut (fiyat, oda, banyo, salon, mülk tipi, Must Haves, mesafe); harita görünümü bulunmuyor.
- Doğal dil araması bulunmuyor; serbest cümle girildiğinde "Couldn't find the address" yanıtı dönüyor.
- Yazım hatası düzeltiliyor ancak bu adres tamamlamanın özelliği; AI destekli sorgu yorumlama bulunmuyor.
- Kişiselleştirilmiş sıralama bulunmuyor; "Suggested" varsayılanı ve "100% MATCH" rozeti yalnızca filtre uyumunu gösteriyor.
- 30 sonuç yalnızca "LOAD MORE" ile listeleniyor; sonuç azaldığında veya boşaldığında akıllı öneri sunulmuyor.

**İlan Detay:**

- İlan metni elle yazılmış, uzunluk ve ton ilandan ilana değişiyor; AI Özet veya Property Highlights bulunmuyor.
- 26 fotoğraf, kat planı ve EPC görseli var; 360° sanal tur ve belgeleri sade dille açıklayan katman bulunmuyor.
- "Benzer ilanlar" bölümü bulunmuyor; sayfa EPC'den sonra footer'a iniyor.
- Tek iletişim yolu Book a Viewing formu; anlık yanıt veren AI Chat Assistant bulunmuyor.
- Harita ilan konumunu gösteriyor; Area Insights ve Commute Insights bulunmuyor.

**Değerleme:**

- Instant Valuation ValPal üzerinde ayrı bir subdomain'de iki adımda ilerliyor; adres seçiliyor, ardından isim, e-posta ve telefon isteniyor.
- Rakam ekranda gösterilmiyor; hesaplandığı söylenip iletişim bilgisi karşılığında sonradan gönderiliyor, dolayısıyla açıklanacak bir tahmin de sunulmuyor.
- Yüz yüze değerleme formu taşınma nedeni, zaman planı ve önceki ajans deneyimi gibi ayrıntılı sorular soruyor; bu yanıtlar hiçbir çıktıya yansımıyor.
- Mortgage ve Stamp Duty hesaplayıcısı bulunmuyor; mortgage konusu yalnızca metin bloğu ve rehber bağlantısıyla geçiştiriliyor.

**İletişim:**

- Aktif bir AI Chat Assistant / Chatbot bulunmuyor; kaynakta msgboxx tabanlı WhatsApp widget'ı geçiyor ancak arayüzde çalışmıyor.
- İletişim formu ad, soyad, e-posta, telefon, mesaj ve Buy/Sell/Rent/Let seçimi istiyor; seçim akışı değiştirmiyor, AI Lead Qualification yapılmıyor.
- Viewing randevusu takvimden gün/saat seçilerek talep ediliyor ancak müsaitlik teyit edilmiyor, AI destekli planlama bulunmuyor.
- Çalışma saatleri sayfada listeleniyor ancak mesai dışında otomatik yanıt sunulmuyor.

**Teknik/Genel:**

- Sayfa Nuxt ile sunucuda render ediliyor, ilan içeriği `filter?search_type=sales` çağrısıyla client-side geliyor.
- Neuron API'ye `property_types`, `property_styles`, `tenure_types` istekleri gidiyor; `ice.js` ve Sentry çalışıyor, toplanan veri kişiselleştirmeye dönüşmüyor.
- Mobilde filtreler ve formlar sorunsuz kullanılıyor; ekrana özel sadeleştirme veya öneri katmanı bulunmuyor.

**Durum:** Yapıldı

### Tur 3 — Ayselin

## Arama

- Klasik property search mevcut; fiyat, bedrooms, bathrooms, reception rooms, property type, Must Haves ve distance gibi standart filtreler kullanılabiliyor. Harita tabanlı arama görünümü bulunmuyor.
- Natural Language Search desteklenmiyor. Serbest bir cümle girildiğinde sorgu kullanıcı niyeti olarak yorumlanmak yerine `"Couldn't find the address"` şeklinde sonuçlanıyor.
- Yazım hatası düzeltme mevcut ancak bunun AI tabanlı sorgu yorumlama değil, adres autocomplete özelliği olduğu görülüyor.
- `Suggested` sıralama seçeneği ve `100% MATCH` göstergesi bulunuyor. Ancak bunlar kullanıcı davranışına göre kişiselleştirilmiş sıralamadan ziyade girilen filtrelerle eşleşme oranını gösteriyor.
- Yaklaşık 30 sonuç `LOAD MORE` ile yükleniyor; sonuç sayısı fazla olduğunda AI destekli otomatik daraltma veya akıllı kriter önerisi sunulmuyor.
- Heads Up Property Alerts mevcut; kullanıcı belirlediği kriterlere göre yeni ilanlar için bildirim alabiliyor.

## İlan Detay

- İlan açıklamaları manuel olarak hazırlanmış ve ilanlar arasında uzunluk ve anlatım şekli değişiyor. AI-generated Property Summary veya otomatik Property Highlights bulunmuyor.
- İlan sayfalarında fotoğraf galerisi, Floor Plan ve EPC bilgileri mevcut. Ancak 360° virtual tour veya EPC/Floor Plan belgelerini AI ile sadeleştiren bir özellik bulunmuyor.
- Kullanıcının ilan hakkında doğal dilde soru sorabileceği AI Property Q&A özelliği bulunmuyor.
- Property Comparison veya kullanıcı davranışına göre kişiselleştirilmiş Similar Properties önerileri sunulmuyor; ilan içeriğinden sonra doğrudan diğer site bölümlerine geçiliyor.
- Harita ilan konumunu gösteriyor ancak AI destekli Area Insights veya Commute Insights bulunmuyor.
- İletişim için `Book a Viewing` formu bulunuyor; ancak ilan sayfasında anlık cevap veren bir AI Chat Assistant mevcut değil.

## Değerleme

- Instant Valuation mevcut ve ValPal üzerinden ayrı bir subdomain'de çalışıyor.
- Valuation sürecinde önce property adresi seçiliyor, ardından isim, e-posta ve telefon bilgileri isteniyor. Tahmini değer doğrudan ekranda gösterilmiyor; iletişim bilgileri sonrasında iletiliyor.
- Yüz yüze valuation formunda taşınma nedeni, zaman planı ve önceki estate agent deneyimi gibi ek bilgiler alınıyor. Bu bilgiler kullanıcıya AI destekli bir analiz veya kişiselleştirilmiş sonuç olarak geri sunulmuyor.
- Tahmini değerin nasıl hesaplandığını açıklayan AI-generated valuation explanation bulunmuyor.
- Mortgage veya Stamp Duty Calculator bulunmuyor; mortgage ile ilgili içerik yalnızca bilgilendirici metin ve yönlendirmeler şeklinde sunuluyor.

## İletişim

- Site genelinde veya ilan sayfalarında aktif bir AI Chat Assistant / Chatbot bulunmuyor.
- İletişim formu ad, soyad, e-posta, telefon, mesaj ve Buy/Sell/Rent/Let seçimi gibi standart alanlardan oluşuyor. Seçilen seçenek formun sonraki akışını değiştirmiyor ve AI Lead Qualification yapılmıyor.
- Viewing talebi için takvim üzerinden gün ve saat seçilebiliyor ancak gerçek zamanlı müsaitlik teyidi sunulmuyor; AI destekli otomatik randevu planlama bulunmuyor.
- Çalışma saatleri belirtiliyor ancak mesai dışında otomatik AI yanıt sistemi bulunmuyor.
- Kaynaklarda WhatsApp/msgboxx tabanlı bir widget referansı görülse de aktif kullanıcı arayüzünde çalışan bir chatbot olarak gözlemlenmiyor.

## Teknik / Genel

- Site Nuxt tabanlı SSR kullanıyor; ilk sayfa yüklemesinde temel property içeriği sunucu tarafından render ediliyor, arama sonuçları ise client-side olarak yükleniyor.
- Network tarafında Neuron API üzerinden `property_types`, `property_styles` ve `tenure_types` gibi klasik filtre parametreleri kullanılıyor. `ice.js` ve Sentry gibi servisler de gözlemleniyor.
- AI/LLM servisine gönderilen ve kullanıcı sorgusunu generative AI ile işleyen ayrı bir API çağrısı tespit edilmiyor.
- Mobil görünüm responsive; filtreler, ilanlar ve iletişim formları küçük ekranlarda kullanılabilir durumda. Mobil cihazlara özel AI destekli bir özellik bulunmuyor.

**Durum:** Yapıldı

### Tur 4 — Görkem

**Arama:**
- Tam platform filtre seti (fiyat/oda/banyo/salon/tip/Must-Haves/yarıçap, harita yok). Serbest cümle → "Couldn't find the address". ~30 sonuç "LOAD MORE" arkasında.
- "100% MATCH"/"Suggested" göstergeleri platformun yerleşik eşleşme rozeti — filtre-uyumu, davranışsal sıralama değil, her Grup-D tenant'ıyla aynı. Sitenin düzgün **yerel bölge rehberleri** var, bugün statik ama sonradan bir bölge-Q&A veya doğal dil katmanı için ideal grounding olur.

**İlan Detay:**
- Uzunluğu/tonu değişen elle yazılmış metin; baktığım bir ilanda ~26 fotoğraf, kat planı ve EPC görseli vardı ama **hiç benzer-ilan bloğu yok** — sayfa EPC'den doğrudan footer'a düşüyor. Özet yok, Q&A yok, 360 yok.
- Standart tavan; burada grup kalıbından kaçan bir şey yok.

**Değerleme — doğrulanması gereken bir görüş ayrılığı:**
- Instant Valuation **ayrı bir subdomain'de ValPal** üzerinde çalışıyor. Benim gezimde platform normu gibi davrandı: adres seç, sonra ad/e-posta/telefon, **ekranda rakam yok** (Yasemin ve Ayselin'in Round 2/3 notlarıyla uyumlu).
- ⚠️ Ama Round 1 (Berkay) bunu **"önceki satışlara dayalı algoritmayla tahmini değer veren 60 saniyelik online değerleme"** olarak kaydetmiş. Bu gerçek bir çelişki — ya araç rakam gösteriyor ya da kapı tutuyor. Giriş yoluna göre değişebilir ya da değişmiş olabilir. **Bunu ikimizden birini alıntılamadan önce canlı olarak yeniden kontrol etmeli.** Üstünü örtmek yerine not düşüyorum.
- Yüz yüze form taşınma-nedeni / zaman-planı / önceki-ajans soruyor ve bu yanıtların hiçbiri bir çıktıya beslenmiyor — toplanıyor, kullanılmıyor. Mortgage/stamp-duty hesaplayıcı yok, sadece broker yönlendirme metni.

**İletişim:**
- Çalışan chatbot yok; **kaynakta msgboxx WhatsApp widget'ı geçiyor ama arayüzde çalıştığını görmedim** (başka bir uykudaki platform kancası). İletişim formu + hiçbir şeyi değiştirmeyen Buy/Sell/Rent/Let; viewing takvimle ama teyitli müsaitlik yok. Mesai dışı yanıt yok.

**Teknik/Genel:**
- **Hibrit SSR + CSR**: temel içerik sunucuda render, ilanlar client-side olarak Neuron API'ye `filter?search_type=sales` çağrısıyla yükleniyor (`property_types` vb.), `ice.js` + Sentry ile. `ice.js`'in topladığı davranış verisi **hiçbir kişiselleştirmeye dönüşmüyor** — toplanıp ziyan ediliyor, tekrar eden bir tema.
- Responsive; form gönderilmedi; gerçek cihaz testi yok.

**Durum:** Yapıldı

### Ortak Bulgular / Sentez (4 tur bitince doldurulur)

### Ortak Bulgular / Sentez

- Ortak eksik AI özellikleri: Doğal dil arama ve akıllı sorgu daraltma, AI ilan özeti, Property Q&A, kişiselleştirilmiş benzer ilan önerileri, AI destekli alan/commute içgörüleri, EPC/floor plan açıklaması, AI lead qualification, otomatik viewing planlama, mesai dışı yanıt ve AI yorumlu mortgage/stamp-duty hesaplayıcıları.

- Öne çıkan fırsatlar: Sitede halihazırda detaylı **yerel bölge rehberleri** bulunuyor; bu mevcut içerik, sıfırdan yeni bir bilgi tabanı oluşturmadan AI Area Q&A veya doğal dil property search için kullanılabilecek güçlü bir kaynak oluşturuyor. **ice.js** davranışsal veri topluyor ancak bu verinin kişiselleştirme veya davranışsal sıralamaya dönüştüğü gözlemlenmedi; mevcut sinyallerin kişiselleştirilmiş ilan önerilerinde kullanılması açık bir fırsat. İlan sayfalarında ayrıca **hiçbir benzer ilan bölümü bulunmuyor**, dolayısıyla kriter veya kullanıcı davranışına dayalı öneriler doğrudan bir boşluğu kapatabilir. Face-to-Face Valuation formu da taşınma nedeni, zaman planı ve önceki ajans deneyimi gibi değerli qualification verileri topluyor ancak bunlar kullanıcı yolculuğunu kişiselleştirmek için kullanılmıyor.

- Görüş ayrılıkları / doğrulanması gerekenler: Temel görüş ayrılığı **ValPal Instant Valuation** akışında. Round 1 bunu önceki satış verilerine dayalı 60 saniyelik algoritmik bir değerleme olarak tanımlarken, Round 2–4 bağımsız olarak kullanıcının adres seçtikten sonra ad, e-posta ve telefon bilgilerini verdiğini ve tahmini değerin ekranda gösterilmediğini gözlemledi. İkinci davranış üç bağımsız incelemeyle destekleniyor ancak farklılık yine de canlı doğrulama için işaretlenmeli. Teknik olarak site **Nuxt ve Neuron / Iceberg Digital altyapısını** kullanıyor; arama verileri Neuron API üzerinden alınırken **ice.js ve Sentry** de çalışıyor. Ayrı bir generative AI/LLM API çağrısı tespit edilmedi. Kaynak kodda **msgboxx tabanlı WhatsApp widget'ı** bulunmasına rağmen arayüzde aktif olarak gözlemlenmedi; bu da mevcut ancak kullanılmayan bir third-party iletişim bileşenine işaret ediyor.**Berkay tarafından analiz edilip doğrulanmıştır.**
