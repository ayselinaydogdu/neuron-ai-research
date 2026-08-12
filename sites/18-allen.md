# 18 · allen-residential.co.uk

**URL:** https://allen-residential.co.uk/
**Group / Grup:** D

---

## English

This site is reviewed independently by 4 people across 4 rounds.

| Round | Reviewer | Status   |
| ----- | -------- | -------- |
| 1     | Berkay   | Done     |
| 2     | Yasemin  | Done     |
| 3     | Ayselin  | Not done |
| 4     | Görkem   | Not done |

> Fill in only your own round block; don't edit anyone else's.
> Write short, concrete sentences (not "yes/no" — say what it is).
> What to check: ../checklist.md · Terms: ../info/ai-feature-glossary.md

### Round 1 — Berkay

## **Search:**

- **Natural Language Search:** **Absent** — Property search uses structured filters and location criteria rather than free-sentence queries.
- **Smart Suggestions / Query Understanding:** **Partial** — Heads Up Alerts use detailed buyer preferences and can suggest properties and price reductions that may specifically interest the user. Search results can also display a "100% MATCH" indicator, but no natural-language interpretation, typo handling, or conversational query understanding was observed.
- **Saved Search / Alerts:** **Present** — Heads Up Property Alerts allow users to save locations, property type, price, bedrooms, bathrooms and other criteria and receive relevant property suggestions and price-reduction alerts.

## **Listing Detail:**

- **Property Summary (AI):** **Absent** — Listings provide manually written property descriptions and feature lists, but no AI-generated 2–3 point summary was observed.
- **Property Q&A:** **Absent** — No free-form AI Q&A for individual listings was observed.
- **Property Highlights:** **Absent** — Listings contain a manually written Features section, but no AI-extracted property highlights were observed.
- **Lifestyle / "Ideal for…" Matching:** **Absent** — Listings may describe suitability for first-time buyers, investors or families, but no AI-powered lifestyle matching was observed.
- **Property Comparison:** **Absent** — No AI-powered comparison of two or more properties was observed.
- **Similar Listings (personalised):** **Absent** — No personalised behaviour-based "you might also like" recommendations were observed.
- **Area Insights:** **Partial** — Property descriptions can include local amenities, schools, transport links and nearby facilities, but no dedicated AI-powered area insight or commentary was observed.
- **Commute Insights:** **Absent** — Transport information can appear in property descriptions, but there is no dedicated commute-time analysis to work or school.
- **Document Explanation (EPC / Floor Plan):** **Absent** — Floor plans and EPC information are provided, but no AI-powered plain-language explanation of these documents was observed.

## **Valuation:**

- **Instant Valuation:** **Present** — The online valuation provides an automated property value estimate after entering a postcode, bedroom count, property type and valuation type.
- **AI Valuation Explanation:** **Absent** — The valuation provides an estimated figure but no AI-generated explanation or personalised breakdown of the factors behind the valuation.
- **Mortgage / Stamp Duty Calculator:** **Absent** — No dedicated mortgage or Stamp Duty calculator with AI financial commentary was observed.

## **Contact:**

- **AI Chat Assistant / Chatbot:** **Absent** — No site-wide or property-level AI chat assistant was observed.
- **Lead Qualification:** **Partial** — The Heads Up registration process collects detailed buyer circumstances such as reason for moving, moving timeframe, mortgage requirement and whether the user needs to sell their current property. This supports applicant segmentation, but no AI-powered lead scoring or pre-screening was observed.
- **Automated Booking / Viewing Scheduling:** **Partial** — Property pages provide an "ARRANGE A VIEWING" option, but no AI-driven scheduling or automated qualification was observed.
- **Out-of-hours Response:** **Absent** — Contact details and office information are provided, but no out-of-hours AI chatbot or automated conversational response was observed.

## **Technical / General:**

- **SSR vs CSR:** **Hybrid (SSR + CSR)** — Initial page load is server-side rendered, with core property and content information present directly in the delivered HTML. Client-side hydration then takes over for interactive elements and further navigation. 
- **API calls:** **Partial** — The property search and matching functionality clearly uses external/property-platform infrastructure, but the specific runtime API endpoints were not confirmed through Network-tab inspection, and unlike sites 22/23 the platform is not explicitly self-identified as Neuron/Iceberg Digital.
- **Mobile behaviour:** **Present** — The responsive site provides access to property search, listings, alerts, valuation and contact forms on mobile.

**Status:** Done

### Round 2 — Yasemin

**Search:**

- Classic filter-based search is available (price, bedrooms, bathrooms, receptions, property type, Must Haves, radius); no map view is offered.
- Natural Language Search is not available; entering a free-text sentence returns "Couldn't find the address".
- Spelling mistakes are not corrected; "Paultn" suggests "Paul Tann Ltd" in Kings Hill instead of Paulton and launches a search in the wrong area.
- Personalised ranking is not available; the "Suggested" default and the "100% MATCH" badge only reflect filter compliance.
- When results come back empty, the only prompt is to set up a Heads Up alert; no intelligent suggestion indicates which filter to relax.

**Property Detail:**

- Listing copy is written manually and split into subheadings; no AI Summary or Property Highlights are generated.
- The page is divided into Features, Property Info, Floor Plans, Map and EPC tabs; there are 10 photos, a floor plan and an EPC, but no 360° virtual tour and no layer explaining these documents in plain language.
- There is no "similar properties" section; no comparison between listings and no behaviour-based recommendation.
- The only contact route is the Arrange a Viewing form; no AI Chat Assistant provides an immediate answer.
- The map shows the property location; travel to Bristol and Bath is written manually into the listing copy, while Area Insights and Commute Insights are not offered.

**Valuation:**

- No instant estimate is produced; the ValPal flow collects contact details first and sends the figure afterwards.
- No layer explains what the estimate is based on.
- No qualification happens in the face-to-face route; the form only takes contact details and a date, putting everyone through the same flow.
- No mortgage or stamp duty calculator is offered, and no financial commentary or recommendation is provided.

**Contact:**

- No AI Chat Assistant provides an immediate answer; every question is routed to a form or the phone.
- The Buy/Sell/Rent/Let selection and Heads Up answers are collected but never turn into Lead Qualification, so everyone goes through the same flow.
- Viewing requests get no availability confirmation and no AI-supported scheduling.
- No automated response is provided outside working hours, and no routing between the three branches takes place.

**Technical/General:**

- Listing content arrives client-side through the `filter?search_type=sales` call; no AI layer is involved in producing that content.
- The `property_types`, `property_styles` and `tenure_types` data coming from the Neuron API feeds the filters without being interpreted.
- `ice.js` and Sentry collect behavioural data, but that data does not turn into personalisation.
- A `whatsapp-chatbot` definition exists in the source, but no assistant runs in the interface.

**Status:** Done

### Round 3 — Ayselin

## Search

- A standard property search is available with filters for price, bedrooms, bathrooms, reception rooms, property type, Must Haves, and distance. There is no map-based search view.
- Natural Language Search is not available. Free-form sentences are not interpreted as property requirements and instead result in an address-related response.
- Spelling correction is not reliable. For example, entering `"Paultn"` suggests `"Paul Tann Ltd"` in Kings Hill instead of correcting it to Paulton, which can lead to a search in the wrong area.
- The `Suggested` option and `100% MATCH` badge are available, but these reflect how well properties match the selected filters rather than personalized ranking based on user behavior.
- When no properties match the selected criteria, the site mainly suggests setting up a Heads Up alert instead of recommending which filters could be relaxed.

## Property Details

- Property descriptions are manually written and divided into separate sections. There is no AI-generated Property Summary or AI-generated Property Highlights.
- Listings are organized into sections such as Features, Property Info, Floor Plans, Map, and EPC. Photos, floor plans, and EPC information are available, but there is no 360° virtual tour or AI layer explaining these documents in simple language.
- No Similar Properties section is provided, and there is no AI-powered property comparison or behavior-based recommendation system.
- The main contact option is an `Arrange a Viewing` form. There is no AI Chat Assistant providing immediate answers to property-related questions.
- The map shows the property's location. Some transport information, such as access to Bristol and Bath, is manually included in the listing description, but there are no AI-powered Area Insights or Commute Insights.

## Valuation

- An estimated property value is not displayed immediately. The ValPal valuation flow collects the user's contact information and provides the estimated value afterwards.
- There is no explanation layer showing what factors the valuation is based on or how the estimated figure was calculated.
- The Face-to-Face Valuation process does not appear to perform AI-based qualification; the form mainly collects contact details and a preferred date before moving users into the same process.
- No Mortgage or Stamp Duty Calculator is available, and there are no AI-powered financial comments or recommendations.

## Contact

- There is no AI Chat Assistant providing instant responses; users are directed to forms or phone contact for enquiries.
- The Buy/Sell/Rent/Let selection and information collected through Heads Up do not appear to result in AI-powered Lead Qualification. Users follow the same general contact flow.
- Viewing requests do not provide confirmed availability or AI-powered automatic scheduling.
- There is no automated response system outside business hours, and no automatic routing between the three branches is provided.

## Technical / General

- Property content is loaded client-side through the `filter?search_type=sales` request; there is no visible AI layer involved in generating or interpreting the property content.
- Data received from the Neuron API, including `property_types`, `property_styles`, and `tenure_types`, is used as standard search/filter parameters rather than being interpreted by an AI system.
- `ice.js` and Sentry are present for tracking and monitoring, but no evidence was found that this data is used for personalized property recommendations.
- A `whatsapp-chatbot` definition appears in the source, but no functioning chatbot or AI assistant is visible in the user interface.

**Status:** Done

### Round 4 — Görkem

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

### Findings / Synthesis (filled once all 4 rounds are done)

- Commonly missing AI features:
- Standout opportunities:
- Disagreements / to verify:

---

## Türkçe

Bu siteyi 4 tur boyunca 4 farklı kişi bağımsız inceler.

| Tur   | İnceleyen| Durum    |
| ----- | -------- | -------- |
| 1     | Berkay   | Yapıldı  |
| 2     | Yasemin  | Yapıldı  |
| 3     | Ayselin  | Yapılmadı|
| 4     | Görkem   | Yapılmadı|

> Sadece kendi tur bloğunuzu doldurun; başkasının bloğunu değiştirmeyin.
> Kısa, somut cümleler yazın ("Var/Yok" değil, ne olduğunu yazın).
> Neye bakılacağı: ../checklist.md · Terimler: ../info/ai-feature-glossary.md

### Tur 1 — Berkay

## **Arama:**

- **Doğal Dil Araması:** **Yok** — Mülk araması, serbest cümle yerine yapılandırılmış filtreler ve konum kriterleri kullanıyor.
- **Akıllı Öneriler / Sorgu Anlama:** **Kısmi** — Heads Up Uyarıları, kullanıcının ayrıntılı tercihlerine göre ilgisini çekebilecek ilanları ve fiyat değişikliklerini önerebiliyor. Arama sonuçlarında "100% MATCH" göstergesi de bulunabiliyor; ancak doğal dil yorumlama, yazım hatası yönetimi veya konuşma tabanlı sorgu anlama gözlemlenmedi.
- **Kayıtlı Arama / Uyarılar:** **Var** — Heads Up Mülk Uyarıları ile konum, mülk tipi, fiyat, oda/banyo sayısı ve diğer kriterler kaydedilerek uygun ilanlar ve fiyat değişiklikleri hakkında bildirim alınabiliyor.

## **İlan Detay:**

- **Mülk Özeti (YZ):** **Yok** — İlanlarda manuel olarak hazırlanmış açıklamalar ve özellik listeleri bulunuyor; yapay zeka tarafından oluşturulan 2–3 maddelik özet gözlemlenmedi.
- **Mülk Soru-Cevap:** **Yok** — İlan hakkında serbest biçimde soru sorulabilen yapay zeka destekli Q&A özelliği gözlemlenmedi.
- **Mülkün Öne Çıkan Özellikleri:** **Yok** — İlanlarda manuel olarak hazırlanmış Özellikler bölümü bulunuyor; yapay zeka tarafından çıkarılmış öne çıkan özellikler bulunmuyor.
- **Yaşam Tarzı / "... için ideal" Eşleştirmesi:** **Yok** — İlanlarda ilk kez ev alacaklar, yatırımcılar veya aileler için uygunluk gibi ifadeler bulunabiliyor; ancak yapay zeka destekli yaşam tarzı eşleştirmesi gözlemlenmedi.
- **Mülk Karşılaştırma:** **Yok** — İki veya daha fazla mülkü yapay zeka ile karşılaştırma özelliği gözlemlenmedi.
- **Benzer İlanlar (kişiselleştirilmiş):** **Yok** — Kullanıcı davranışına göre kişiselleştirilmiş "benzer ilanlar" önerisi gözlemlenmedi.
- **Bölge İçgörüleri:** **Kısmi** — İlan açıklamalarında yerel olanaklar, okullar, ulaşım bağlantıları ve çevredeki tesisler hakkında bilgiler bulunabiliyor; ancak özel bir yapay zeka destekli bölge analizi veya yorumu bulunmuyor.
- **Ulaşım İçgörüleri:** **Yok** — İlanlarda ulaşım bilgileri bulunabiliyor, ancak işe veya okula ulaşım süresini analiz eden özel bir özellik bulunmuyor.
- **Belge Açıklaması (EPC / Kat Planı):** **Yok** — Kat planları ve EPC bilgileri sunuluyor, ancak bunları sade bir dille açıklayan yapay zeka özelliği bulunmuyor.

## **Değerleme:**

- **Anlık Değerleme:** **Var** — Online değerleme, posta kodu, oda sayısı, mülk tipi ve değerleme türü girildikten sonra otomatik tahmini mülk değeri sağlıyor.
- **Yapay Zeka Değerleme Açıklaması:** **Yok** — Tahmini değerin arkasındaki faktörleri açıklayan yapay zeka destekli veya kişiselleştirilmiş bir analiz bulunmuyor.
- **Mortgage / Damga Vergisi Hesaplayıcısı:** **Yok** — yapay zeka destekli finansal yorum içeren özel bir mortgage veya Stamp Duty hesaplayıcısı gözlemlenmedi.

## **İletişim:**

- **Yapay Zeka Sohbet Asistanı / Chatbot:** **Yok** — Site genelinde veya ilan seviyesinde yapay zeka destekli sohbet asistanı gözlemlenmedi.
- **Müşteri Adayı Nitelendirme:** **Kısmi** — Heads Up kayıt süreci; taşınma nedeni, taşınma zamanı, mortgage ihtiyacı ve mevcut mülkün satılması gerekip gerekmediği gibi ayrıntılı bilgiler topluyor. Bu bilgiler başvuru sahiplerini segmentlere ayırmak için kullanılıyor, ancak yapay zeka destekli müşteri adayı puanlama veya ön eleme gözlemlenmedi.
- **Otomatik Rezervasyon / Görüntüleme Planlama:** **Kısmi** — İlan sayfalarında "ARRANGE A VIEWING" seçeneği bulunuyor; ancak yapay zeka destekli randevu planlama veya otomatik değerlendirme gözlemlenmedi.
- **Mesai Dışı Yanıt:** **Yok** — İletişim bilgileri ve ofis bilgileri sunuluyor, ancak mesai dışı AI sohbet botu veya otomatik konuşma tabanlı yanıt sistemi gözlemlenmedi.

## **Teknik/Genel:**

- **SSR ve CSR:** **Hibrit (SSR + CSR)** — İlk sayfa yüklemesi sunucu tarafında render ediliyor; temel ilan ve içerik bilgileri doğrudan teslim edilen HTML içinde yer alıyor. Ardından etkileşimli öğeler ve sonraki gezinmeler için istemci tarafı hydration devreye giriyor. 
- **API Çağrıları:** **Var** — Site açıkça Neuron / Iceberg Digital'in "Estate Agentlar için Yapay Zeka İşletim Sistemi" altyapısını kullanıyor. Property search sonuçlarında yapay zeka eşleştirme sistemi yüzde bazlı eşleşme göstergeleriyle görünür durumda. 
- **Mobil Davranış:** **Var** — Responsive site üzerinden mülk arama, ilanlar, alertler, değerleme ve iletişim özelliklerine mobil erişim sağlanıyor.

**Durum:** Yapıldı
### Tur 2 — Yasemin

**Arama:**

- Klasik filtre tabanlı arama mevcut (fiyat, oda, banyo, salon, mülk tipi, Must Haves, mesafe); harita görünümü bulunmuyor.
- Doğal dil araması bulunmuyor; serbest cümle girildiğinde "Couldn't find the address" yanıtı dönüyor.
- Yazım hatası düzeltilmiyor; "Paultn" için Paulton yerine Kings Hill'deki "Paul Tann Ltd" öneriliyor ve yanlış bölgede arama başlatılıyor.
- Kişiselleştirilmiş sıralama bulunmuyor; "Suggested" varsayılanı ve "100% MATCH" rozeti yalnızca filtre uyumunu gösteriyor.
- Sonuç boş kaldığında yalnızca Heads Up alert kurma önerisi çıkıyor; hangi filtrenin gevşetileceğine dair akıllı öneri sunulmuyor.

**İlan Detay:**

- İlan metni elle yazılmış ve alt başlıklara bölünmüş; AI Özet veya Property Highlights bulunmuyor.
- Sayfa Features, Property Info, Floor Plans, Map, EPC sekmelerine ayrılmış; 10 fotoğraf, kat planı ve EPC var, 360° sanal tur ve belgeleri sade dille açıklayan katman bulunmuyor.
- "Benzer ilanlar" bölümü bulunmuyor; ilanlar arası karşılaştırma veya davranışa göre öneri sunulmuyor.
- Tek iletişim yolu Arrange a Viewing formu; anlık yanıt veren AI Chat Assistant bulunmuyor.
- Harita ilan konumunu gösteriyor; ilan metninde Bristol ve Bath'a ulaşım elle yazılmış, Area Insights ve Commute Insights bulunmuyor.

**Değerleme:**

- Anlık tahmini değer üretilmiyor; ValPal akışı iletişim bilgisi topladıktan sonra rakamı sonradan gönderiyor.
- Tahminin neye dayandığını açıklayan bir katman bulunmuyor.
- Yüz yüze değerlemede nitelendirme yapılmıyor; form yalnızca iletişim ve tarih alıp herkesi aynı akışa sokuyor.
- Mortgage ve Stamp Duty hesaplayıcısı bulunmuyor; finansal yorum veya öneri sunulmuyor.

**İletişim:**

- Anlık yanıt veren AI Chat Assistant bulunmuyor; her soru forma veya telefona yönleniyor.
- Toplanan Buy/Sell/Rent/Let seçimi ve Heads Up yanıtları Lead Qualification'a dönüşmüyor, herkes aynı akıştan geçiyor.
- Viewing talebinde müsaitlik teyidi ve AI destekli planlama bulunmuyor.
- Mesai dışında otomatik yanıt sunulmuyor; üç şube arasında yönlendirme de yapılmıyor.

**Teknik/Genel:**

- İlan içeriği `filter?search_type=sales` çağrısıyla client-side geliyor; içerik üretiminde AI katmanı devrede değil.
- Neuron API'den gelen `property_types`, `property_styles`, `tenure_types` verisi yorumlanmadan filtreye besleniyor.
- `ice.js` ve Sentry davranış verisi topluyor ama bu veri kişiselleştirmeye dönüşmüyor.
- Kaynakta `whatsapp-chatbot` tanımı var, arayüzde çalışan asistan yok.

**Durum:** Yapıldı

### Tur 3 — Ayselin

## Arama

- Fiyat, oda sayısı, banyo, salon, mülk tipi, Must Haves ve mesafe gibi filtrelerin bulunduğu klasik bir emlak araması mevcut. Harita tabanlı arama görünümü bulunmuyor.
- Doğal Dil Araması bulunmuyor. Serbest cümleler mülk kriterleri olarak yorumlanmıyor ve adres odaklı sonuç veriyor.
- Yazım hatası düzeltme güvenilir değil. Örneğin `"Paultn"` aramasında Paulton yerine Kings Hill'deki `"Paul Tann Ltd"` öneriliyor ve yanlış bölgede arama yapılmasına neden olabiliyor.
- `Suggested` seçeneği ve `100% MATCH` rozeti bulunuyor ancak bunlar kullanıcı davranışına göre kişiselleştirilmiş sıralama değil, seçilen filtrelerle ilanların ne kadar eşleştiğini gösteriyor.
- Hiçbir ilan eşleşmediğinde hangi filtrelerin gevşetilebileceğine dair akıllı öneri sunulmuyor; ağırlıklı olarak Heads Up alert oluşturulması öneriliyor.

## İlan Detay

- İlan açıklamaları manuel olarak hazırlanmış ve farklı bölümlere ayrılmış. AI destekli Property Summary veya Property Highlights bulunmuyor.
- İlanlar Features, Property Info, Floor Plans, Map ve EPC gibi bölümlere ayrılmış. Fotoğraflar, kat planları ve EPC bilgileri mevcut ancak 360° sanal tur veya bu belgeleri sade bir dille açıklayan AI özelliği bulunmuyor.
- Benzer ilanlar bölümü bulunmuyor. AI destekli ilan karşılaştırma veya kullanıcı davranışına göre kişiselleştirilmiş öneri sistemi mevcut değil.
- Ana iletişim seçeneği `Arrange a Viewing` formu. Kullanıcının ilanla ilgili sorularına anlık cevap veren AI Chat Assistant bulunmuyor.
- Harita üzerinde mülkün konumu gösteriliyor. Bristol ve Bath'a ulaşım gibi bazı bilgiler ilan açıklamasında manuel olarak veriliyor ancak AI destekli Area Insights veya Commute Insights bulunmuyor.

## Değerleme

- Tahmini mülk değeri anında ekranda gösterilmiyor. ValPal değerleme sürecinde önce kullanıcının iletişim bilgileri alınıyor ve tahmini değer daha sonra iletiliyor.
- Değerlemenin hangi faktörlere göre hesaplandığını veya tahmini rakamın neden bu seviyede olduğunu açıklayan bir sistem bulunmuyor.
- Yüz yüze değerleme sürecinde AI destekli bir ön eleme yapılmıyor; form temel olarak iletişim bilgilerini ve tercih edilen tarihi alıyor.
- Mortgage veya Stamp Duty Calculator bulunmuyor; AI destekli finansal yorum veya öneri sunulmuyor.

## İletişim

- Anlık yanıt veren bir AI Chat Assistant bulunmuyor; kullanıcılar sorular için formlara veya telefon iletişimine yönlendiriliyor.
- Buy/Sell/Rent/Let seçimi ve Heads Up üzerinden toplanan bilgiler AI destekli Lead Qualification sistemine dönüşmüyor. Kullanıcılar genel olarak aynı iletişim akışından ilerliyor.
- Viewing taleplerinde müsaitlik doğrulaması veya AI destekli otomatik randevu planlama bulunmuyor.
- Mesai dışında otomatik yanıt sistemi bulunmuyor ve üç şube arasında otomatik yönlendirme yapılmıyor.

## Teknik / Genel

- İlan içerikleri `filter?search_type=sales` isteği üzerinden client-side olarak yükleniyor; içeriklerin oluşturulması veya yorumlanmasında görünür bir AI katmanı bulunmuyor.
- Neuron API'den gelen `property_types`, `property_styles` ve `tenure_types` gibi veriler standart arama/filtre parametreleri olarak kullanılıyor; AI tarafından yorumlanmıyor.
- `ice.js` ve Sentry kullanılıyor ancak bu verilerin kişiselleştirilmiş ilan önerilerine dönüştürüldüğüne dair bir kanıt bulunmuyor.
- Kaynak kodda `whatsapp-chatbot` tanımı bulunuyor ancak kullanıcı arayüzünde çalışan bir chatbot veya AI asistanı görünmüyor.

**Durum:** Yapıldı

### Tur 4 — Görkem

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

### Ortak Bulgular / Sentez (4 tur bitince doldurulur)

- Ortak eksik AI özellikleri:
- Öne çıkan fırsatlar:
- Görüş ayrılıkları / doğrulanması gerekenler:
