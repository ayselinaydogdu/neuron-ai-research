# 21 · courtyardhomes.co.uk

**URL:** https://courtyardhomes.co.uk/
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

- **Natural Language Search:** **Absent** — Property search uses structured Buy/Rent search controls and standard property criteria rather than free-sentence queries.
- **Smart Suggestions / Query Understanding:** **Partial** — Heads-Up Alerts match saved buyer or renter preferences against upcoming properties, but no natural-language query interpretation, typo handling, or conversational search was observed.
- **Saved Search / Alerts:** **Present** — Heads-Up Property Alerts match user preferences to upcoming listings and send notifications before properties appear on Rightmove or Zoopla.

## **Listing Detail:**

- **Property Summary (AI):** **Absent** — Property pages provide manually written descriptions and feature information, but no AI-generated 2–3 point summary was observed.
- **Property Q&A:** **Absent** — No free-form AI Q&A for individual listings was observed.
- **Property Highlights:** **Absent** — Listings contain manually written property features and descriptions, but no AI-extracted highlights were observed.
- **Lifestyle / "Ideal for…" Matching:** **Partial** — Property descriptions can explain suitability for families, first-time buyers or particular lifestyles, but no explicit AI-powered lifestyle matching was observed.
- **Property Comparison:** **Absent** — No AI-powered comparison of two or more properties was observed.
- **Similar Listings (personalised):** **Absent** — No behaviour-based personalised "you might also like" recommendations were observed.
- **Area Insights:** **Partial** — Property content and the Advice Hub provide local information about areas, schools, transport, amenities and local market conditions, but no AI-generated area commentary was observed.
- **Commute Insights:** **Partial** — Local transport connections and journey information are discussed in some property and area content, but there is no personalised commute-time analysis based on the user's destination.
- **Document Explanation (EPC / Floor Plan):** **Absent** — EPC information and floor plans can be provided with properties, but no AI-powered plain-language explanation of these documents was observed.

## **Valuation:**

- **Instant Valuation:** **Present** — The Quick Online Estimate provides a guide price in under 60 seconds using local property data.
- **AI Valuation Explanation:** **Absent** — The online estimate provides a general figure but no AI-generated explanation or personalised breakdown of the factors behind the valuation.
- **Mortgage / Stamp Duty Calculator:** **Absent** — No dedicated mortgage or Stamp Duty calculator with AI financial commentary was observed.

## **Contact:**

- **AI Chat Assistant / Chatbot:** **Absent** — No site-wide or property-level AI chat assistant was observed.
- **Lead Qualification:** **Partial** — Contact and valuation forms collect structured information, while the Heads-Up registration process captures buyer/renter preferences and circumstances. No AI-powered lead scoring or prioritisation was observed.
- **Automated Booking / Viewing Scheduling:** **Partial** — Properties allow users to book or arrange viewings, but no AI-driven appointment scheduling or automated qualification was observed.
- **Out-of-hours Response:** **Absent** — The site promotes direct communication with its personal agents and provides office contact details, but no automated out-of-hours AI chatbot or conversational response system was observed.

## **Technical / General:**

- **SSR vs CSR:** **Hybrid (SSR + CSR)** — Initial page load is server-side rendered, with core property and content information present directly in the delivered HTML. Client-side hydration then takes over for interactive elements and further navigation. 
- **API calls:** **Present** — The site is explicitly powered by Neuron / Iceberg Digital's "AI Operating System for Estate Agents". Property search results also expose the AI matching functionality through percentage-based match indicators. This verdict rests on vendor self-identification plus the observable match-% UI element; specific runtime API endpoints were not confirmed through Network-tab inspection.
- **Mobile behaviour:** **Present** — The responsive site provides access to property search, listings, alerts, valuation and contact functionality on mobile.

**Status:** Done

### Round 2 — Yasemin

**Search:**

- No natural language search; entering a free-form sentence returns a "Couldn't find the address" response.
- Typos are corrected, but this is a feature of the address autocomplete; there is no AI-powered query interpretation.
- No personalised ranking; the "Suggested" default only reflects filter compliance.
- A 0.25 mile radius returns 27 results, but no suggestion is offered to widen the radius or relax the criteria.
- Results are only listed via "Load more properties"; no intelligent narrowing is applied at this volume.

**Property Detail:**

- The highlights list is written manually; no AI-generated summary (Property Summary) is extracted from the description.
- The user cannot ask questions about the listing (no AI Property Q&A).
- The gallery can be limited to a single image; there is no 360° virtual tour.
- No personalised similar listing recommendations or Property Comparison are offered.
- The map shows nearby amenities, but no AI-powered Area Insights or Commute Insights are produced.
- The Stamp Duty and Mortgage calculators return a figure and a fixed warning; no financial commentary tailored to the buyer's profile is produced.

**Valuation:**

- The Instant Valuation runs in two steps; after the postcode, bedroom count and property type are taken, the figure is not shown on screen but sent afterwards in exchange for contact details.
- It is not explained which comparable sale or property attribute the estimate is based on; information entered in the free-text field is not reflected in the figure either.
- A Stamp Duty and Mortgage Calculator are available but only return a figure; no AI financial commentary is provided.

**Contact:**

- No AI Chat Assistant providing instant responses; every enquiry is routed to a form or phone call.
- The Buy/Sell/Rent/Let selection, the free-text message and the Heads Up "Circumstances" answers collected are not turned into Lead Qualification.
- A date is picked from the calendar in the viewing request but availability is not confirmed; scheduling is handled manually.
- No automated response is provided outside office hours; the enquiry waits until the next working day.

**Technical/General:**

- The listing results are fed by a client-side `filter?search_type=sales` call; no layer intervenes to interpret the query.
- Network traffic contains only IcebergTracker, Sentry and Neuron REST endpoints; no AI service producing recommendations or content is called.
- Chatbot styles are loaded in the source, but no working assistant is active.
- The visit data collected is not turned into personalised content or recommendations.
- On mobile the filters are compressed into dropdown panels; no natural language input is offered to reduce the filtering burden on narrow screens.

**Status:** Done

### Round 3 — Ayselin

## **Search:**

- **Natural Language Search:** **No** — Property search relies on structured controls such as sale/rent selection, location, price, bedroom count, and other property filters. There is no free-text search where users can describe their needs in natural language.
- **Smart Suggestions / Query Understanding:** **Partial** — Search results are filtered based on the entered criteria, and location/address inputs may provide autocomplete-style assistance. However, no AI-based system was observed that understands user intent, automatically interprets requirements, or personalizes search results.
- **Saved Search / Alerts:** **Yes** — Users can use search and notification features based on specific property criteria. However, there is no clear evidence that alerts are intelligently personalized based on user behavior.

## **Property Details:**

- **AI Property Summary:** **No** — Property pages provide manually written descriptions, room information, and key features. There is no AI-generated short summary of the listing.
- **Property Q&A:** **No** — Users cannot ask an AI questions about a property, such as “Is this property suitable for a family?” or “How far is it from the nearest train station?”
- **Property Highlights:** **Partial** — Property pages display key features and descriptions, but there is no AI system that automatically extracts highlights such as “large garden,” “bright living room,” or “close to public transport.”
- **Lifestyle / “Ideal For” Matching:** **Partial** — Property descriptions may indicate suitability for families, couples, investors, or specific lifestyles. However, there is no AI-powered matching based on the user's personal preferences.
- **Property Comparison:** **No** — There is no AI-powered feature for comparing multiple properties based on price, location, bedrooms, features, advantages, and disadvantages.
- **Personalized Similar Properties:** **Partial** — Users may be directed to properties with similar criteria, but personalized recommendations based on browsing history, favorites, or user behavior are not observed.
- **Area Insights:** **Partial** — Location and basic information about nearby amenities are available. However, there is no AI-generated analysis combining factors such as schools, transport, shops, safety, and lifestyle suitability.
- **Commute Insights:** **Partial** — Map and location information can provide access to nearby transport points, but there is no personalized commute analysis based on a user's workplace, school, or selected destination.
- **Document Explanation (EPC / Floor Plan):** **No** — EPC information, floor plans, or other property documents may be available, but there is no AI feature that analyzes these documents and explains them in simple language.

## **Valuation:**

- **Instant Valuation:** **Yes** — An online valuation process is available, allowing users to provide property information and receive an estimated property value.
- **AI Valuation Explanation:** **No** — Although an estimated value can be provided, there is no AI-generated explanation showing which property characteristics, local data, or comparable properties contributed to the valuation.
- **Mortgage / Stamp Duty Calculator:** **Partial** — Mortgage or purchasing-cost calculation tools may be available, but there is no AI-powered financial commentary based on the user's income, budget, or purchasing scenario.

## **Communication:**

- **AI Chat Assistant / Chatbot:** **No** — There is no AI-powered chatbot that allows users to ask questions about the website or properties 24/7.
- **Lead Qualification:** **Partial** — Contact, valuation, and viewing forms collect user information. However, there is no AI system that analyzes these details, scores lead quality, or prioritizes prospects for the sales team.
- **Automated Booking / Viewing Scheduling:** **Partial** — Users can request property viewings, but there is no AI-powered system that automatically checks availability, matches preferences, and schedules appointments.
- **After-Hours Response:** **No** — Contact forms and agent communication channels are available, but there is no AI-based system providing automated responses outside business hours.

## **Technical / General:**

- **SSR and CSR:** **Partial** — Core property and content pages are accessible, but the exact SSR/CSR architecture cannot be conclusively verified through external inspection alone.
- **API Calls:** **Partial** — Backend services/APIs are used for property and user interactions, but no separate AI API layer responsible for recommendations, NLP, or generative content could be confirmed through page-level inspection.
- **Mobile Behavior:** **Yes** — The website is responsive and supports property search, property detail viewing, and communication on mobile devices. However, there is no natural-language search or AI-powered quick filtering to reduce the filtering effort on smaller screens.

### **Overall AI Opportunities**

The main AI opportunities identified for Courtyard Homes are:

1. **Natural Language Property Search** — Convert users' natural-language requirements into structured property filters.
2. **AI Property Summary** — Generate concise summaries from long property descriptions.
3. **AI Property Q&A** — Answer user questions instantly using property data.
4. **Lifestyle Matching** — Analyze user requirements and prioritize the most suitable properties.
5. **AI Area & Commute Insights** — Interpret area and transport data based on the user's destinations and lifestyle.
6. **AI Valuation Explanation** — Explain the factors behind the estimated property value.
7. **AI Lead Qualification** — Analyze enquiry forms and prioritize leads for agents.
8. **AI Viewing Assistant** — Match user and agent availability and automate the viewing process.


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

- **Doğal Dil Araması:** **Yok** — Mülk araması, Satın Alma/Kiralama seçimleri ve standart mülk kriterleri gibi yapılandırılmış arama kontrollerini kullanıyor; serbest cümleyle arama bulunmuyor.
- **Akıllı Öneriler / Sorgu Anlama:** **Kısmi** — Heads-Up Uyarıları, kayıtlı alıcı veya kiracı tercihlerini yaklaşan ilanlarla eşleştiriyor; ancak doğal dil sorgu yorumlama, yazım hatası yönetimi veya konuşma tabanlı arama gözlemlenmedi.
- **Kayıtlı Arama / Uyarılar:** **Var** — Heads-Up Mülk Uyarıları, kullanıcı tercihlerini yaklaşan ilanlarla eşleştirerek Rightmove veya Zoopla'da yayınlanmadan önce bildirim gönderiyor.

## **İlan Detay:**

- **Mülk Özeti (YZ):** **Yok** — İlan sayfalarında manuel olarak hazırlanmış açıklamalar ve özellik bilgileri bulunuyor; yapay zeka tarafından oluşturulan 2–3 maddelik özet gözlemlenmedi.
- **Mülk Soru-Cevap:** **Yok** — İlan hakkında serbest biçimde soru sorulabilen yapay zeka destekli Q&A özelliği gözlemlenmedi.
- **Mülkün Öne Çıkan Özellikleri:** **Yok** — İlanlarda manuel olarak hazırlanmış özellikler ve açıklamalar bulunuyor; yapay zeka tarafından çıkarılmış öne çıkan özellikler bulunmuyor.
- **Yaşam Tarzı / "... için ideal" Eşleştirmesi:** **Kısmi** — İlan açıklamalarında aileler, ilk kez ev alacaklar veya belirli yaşam tarzları için uygunluk belirtilebiliyor; ancak açık bir yapay zeka destekli yaşam tarzı eşleştirmesi gözlemlenmedi.
- **Mülk Karşılaştırma:** **Yok** — İki veya daha fazla mülkü yapay zeka ile karşılaştırma özelliği gözlemlenmedi.
- **Benzer İlanlar (kişiselleştirilmiş):** **Yok** — Kullanıcı davranışına göre kişiselleştirilmiş "benzer ilanlar" önerisi gözlemlenmedi.
- **Bölge İçgörüleri:** **Kısmi** — İlan içerikleri ve Advice Hub; bölgeler, okullar, ulaşım, olanaklar ve yerel piyasa koşulları hakkında bilgi sağlıyor, ancak yapay zeka tarafından oluşturulan bölge yorumu bulunmuyor.
- **Ulaşım İçgörüleri:** **Kısmi** — Bazı ilan ve bölge içeriklerinde ulaşım bağlantıları ve yolculuk bilgileri bulunuyor; ancak kullanıcının belirlediği hedefe göre kişiselleştirilmiş ulaşım süresi analizi bulunmuyor.
- **Belge Açıklaması (EPC / Kat Planı):** **Yok** — EPC bilgileri ve kat planları ilanlarla birlikte sunulabiliyor; ancak bunları sade bir dille açıklayan yapay zeka özelliği bulunmuyor.

## **Değerleme:**

- **Anlık Değerleme:** **Var** — Quick Online Estimate, yerel mülk verilerini kullanarak 60 saniyeden kısa sürede tahmini bir değer sunuyor.
- **Yapay Zeka Değerleme Açıklaması:** **Yok** — Online tahmin genel bir değer sağlıyor; ancak değerin arkasındaki faktörleri açıklayan yapay zeka destekli veya kişiselleştirilmiş bir analiz bulunmuyor.
- **Mortgage / Damga Vergisi Hesaplayıcısı:** **Yok** — yapay zeka destekli finansal yorum içeren özel bir mortgage veya Stamp Duty hesaplayıcısı gözlemlenmedi.

## **İletişim:**

- **Yapay Zeka Sohbet Asistanı / Chatbot:** **Yok** — Site genelinde veya ilan seviyesinde yapay zeka destekli sohbet asistanı gözlemlenmedi.
- **Müşteri Adayı Nitelendirme:** **Kısmi** — İletişim ve değerleme formları yapılandırılmış bilgiler topluyor; Heads-Up kayıt süreci de alıcı/kiracı tercihleri ve durumları hakkında bilgi topluyor. Ancak yapay zeka destekli müşteri adayı puanlama veya önceliklendirme bulunmuyor.
- **Otomatik Rezervasyon / Görüntüleme Planlama:** **Kısmi** — İlanlar üzerinden görüntüleme ayarlanabiliyor; ancak yapay zeka destekli randevu planlama veya otomatik ön eleme gözlemlenmedi.
- **Mesai Dışı Yanıt:** **Yok** — Site kişisel danışman iletişimini ve ofis iletişim bilgilerini öne çıkarıyor; ancak mesai dışı otomatik AI sohbet botu veya konuşma tabanlı yanıt sistemi gözlemlenmedi.

## **Teknik/Genel:**

- **SSR ve CSR:** **Kısmi** — Temel ilan ve içerik sayfaları teslim edilen sayfada erişilebilir durumda; ancak kesin SSR/CSR yapısı doğrudan Geliştirici Araçları incelemesi olmadan doğrulanamadı.
- **API Çağrıları:** **Kısmi** — Site harici mülk/alert altyapıları kullanıyor; ancak spesifik çalışma zamanı API çağrıları ve Neuron API kullanımı sayfa seviyesindeki incelemeden doğrulanamadı.
- **Mobil Davranış:** **Var** — Responsive arayüz üzerinden mülk arama, ilanlar, alertler ve iletişim formlarına mobil erişim sağlanıyor.

**Durum:** Yapıldı

### Tur 2 — Yasemin

**Arama:**

- Doğal dil araması bulunmuyor; serbest cümle girildiğinde "Couldn't find the address" yanıtı dönüyor.
- Yazım hatası düzeltiliyor ancak bu adres tamamlamanın özelliği; AI destekli sorgu yorumlama bulunmuyor.
- Kişiselleştirilmiş sıralama bulunmuyor; "Suggested" varsayılanı yalnızca filtre uyumunu yansıtıyor.
- 0.25 mil yarıçapta 27 sonuç dönüyor ama yarıçapı genişletme veya kriter gevşetme önerisi sunulmuyor.
- Sonuçlar yalnızca "Load more properties" ile listeleniyor; bu hacimde akıllı daraltma yapılmıyor.

**İlan Detay:**

- Öne çıkanlar listesi elle yazılmış; açıklamadan AI destekli özet (Property Summary) çıkarılmıyor.
- Kullanıcı ilan hakkında soru soramıyor (AI Property Q&A yok).
- Galeri tek görselle sınırlı kalabiliyor; 360° sanal tur bulunmuyor.
- Kişiselleştirilmiş benzer ilan önerisi ve Property Comparison sunulmuyor.
- Harita çevredeki tesisleri gösteriyor ama AI destekli Area Insights veya Commute Insights üretilmiyor.
- Stamp Duty ve Mortgage hesaplayıcıları rakam ve sabit uyarı veriyor; alıcının profiline göre finansal yorum üretilmiyor.

**Değerleme:**

- Instant Valuation iki adımda ilerliyor; postcode, oda sayısı ve mülk tipi alındıktan sonra rakam ekranda gösterilmiyor, iletişim bilgisi karşılığında sonradan iletiliyor.
- Tahminin hangi karşılaştırmalı satışa veya mülk özelliğine dayandığı açıklanmıyor; serbest metin alanına yazılan bilgi de rakama yansımıyor.
- Stamp Duty ve Mortgage Calculator mevcut ancak yalnızca rakam veriyor; AI finansal yorum sunulmuyor.

**İletişim:**

- Anlık yanıt veren AI Chat Assistant bulunmuyor; her soru forma veya telefona yönleniyor.
- Toplanan Buy/Sell/Rent/Let seçimi, serbest mesaj ve Heads Up "Circumstances" yanıtları Lead Qualification'a dönüşmüyor.
- Viewing talebinde takvimden tarih seçiliyor fakat müsaitlik teyit edilmiyor; planlama elle yapılıyor.
- Mesai dışında otomatik yanıt sunulmuyor; talep bir sonraki iş gününe kalıyor.

**Teknik/Genel:**

- İlan listesi client-side `filter?search_type=sales` çağrısıyla besleniyor; sorguyu yorumlayan bir katman araya girmiyor.
- Ağ trafiğinde yalnızca IcebergTracker, Sentry ve Neuron REST uçları var; öneri veya içerik üreten bir AI servisi çağrılmıyor.
- Kaynakta chatbot stilleri yükleniyor ama çalışan bir asistan devrede değil.
- Toplanan ziyaret verisi kişiselleştirilmiş içerik veya öneriye dönüşmüyor.
- Mobilde filtreler açılır panellere sıkışıyor; dar ekranda filtre yükünü azaltacak doğal dil girişi sunulmuyor.

**Durum:** Yapıldı

### Tur 3 — Ayselin

## **Arama:**

- **Doğal Dil Araması:** **Yok** — Mülk araması; satış/kiralama seçimi, konum, fiyat, oda sayısı ve diğer yapılandırılmış filtreler üzerinden ilerliyor. Kullanıcının “şehir merkezine yakın, bahçeli ve aile için uygun bir ev” gibi serbest metinle arama yapmasını sağlayan doğal dil özelliği bulunmuyor.
- **Akıllı Öneriler / Sorgu Anlama:** **Kısmi** — Arama sonuçları girilen kriterlere göre filtreleniyor ve konum/adres girişinde otomatik tamamlama benzeri yardımcı özellikler bulunabiliyor; ancak kullanıcı niyetini anlayan, kriterleri otomatik yorumlayan veya sonuçları kişiselleştiren AI tabanlı bir sistem gözlemlenmiyor.
- **Kayıtlı Arama / Uyarılar:** **Var** — Kullanıcıların belirli mülk kriterlerine göre arama ve bildirim özelliklerinden yararlanabildiği görülüyor. Ancak uyarıların kullanıcı davranışını analiz ederek akıllı şekilde kişiselleştirildiğine dair bir AI özelliği bulunmuyor.

## **İlan Detay:**

- **Mülk Özeti (YZ):** **Yok** — İlanlarda mülk açıklaması, oda bilgileri ve temel özellikler manuel içerik olarak sunuluyor. Uzun ilan açıklamasını otomatik olarak kısa ve anlaşılır bir AI özetine dönüştüren özellik bulunmuyor.
- **Mülk Soru-Cevap:** **Yok** — Kullanıcının ilanla ilgili “Bu ev çocuklu aile için uygun mu?” veya “Tren istasyonuna ne kadar uzak?” gibi soruları doğrudan AI'a sorabileceği bir sistem bulunmuyor.
- **Mülkün Öne Çıkan Özellikleri:** **Kısmi** — İlanlarda temel özellikler ve açıklamalar listeleniyor; ancak AI'ın açıklamadan otomatik olarak “geniş bahçe”, “aydınlık salon”, “ulaşıma yakın” gibi öne çıkan noktaları çıkardığı bir yapı bulunmuyor.
- **Yaşam Tarzı / "... için ideal" Eşleştirmesi:** **Kısmi** — İlan açıklamalarında aileler, çiftler, yatırımcılar veya belirli kullanıcı profilleri için uygunluk manuel olarak ifade edilebiliyor. Ancak kullanıcı profiline göre AI destekli yaşam tarzı eşleştirmesi bulunmuyor.
- **Mülk Karşılaştırma:** **Yok** — Kullanıcının birden fazla ilanı seçerek fiyat, konum, oda sayısı, özellikler ve avantaj/dezavantajlar açısından AI destekli karşılaştırabileceği bir özellik gözlemlenmiyor.
- **Benzer İlanlar (kişiselleştirilmiş):** **Kısmi** — Benzer kriterlere sahip başka ilanlara yönlendirme yapılabiliyor; ancak kullanıcının görüntüleme geçmişi, favorileri veya davranışlarına göre kişiselleştirilmiş AI önerileri bulunmuyor.
- **Bölge İçgörüleri:** **Kısmi** — İlanlarda konum ve çevredeki olanaklara ilişkin temel bilgiler sunuluyor. Ancak okul, ulaşım, market, güvenlik veya yaşam kalitesi gibi verileri birleştirerek AI tarafından oluşturulan kişiselleştirilmiş bölge analizi bulunmuyor.
- **Ulaşım İçgörüleri:** **Kısmi** — Harita ve konum bilgileri üzerinden çevredeki ulaşım noktaları görülebiliyor; ancak kullanıcının belirlediği iş yeri, okul veya başka bir hedefe göre otomatik yolculuk süresi ve ulaşım analizi sunulmuyor.
- **Belge Açıklaması (EPC / Kat Planı):** **Yok** — EPC, kat planı veya benzeri mülk dokümanları mevcut olduğunda kullanıcı bunları inceleyebiliyor; ancak AI'ın bu belgeleri analiz edip sade bir dille açıklaması bulunmuyor.

## **Değerleme:**

- **Anlık Değerleme:** **Var** — Kullanıcıların mülk bilgilerini girerek çevrimiçi değer tahmini alabileceği bir valuation süreci bulunuyor.
- **Yapay Zeka Değerleme Açıklaması:** **Yok** — Tahmini değer sunulsa da bu değerin hangi özellikler, bölgesel veriler veya benzer satışlar dikkate alınarak oluşturulduğunu açıklayan AI destekli bir analiz bulunmuyor.
- **Mortgage / Damga Vergisi Hesaplayıcısı:** **Kısmi** — Mortgage veya satın alma maliyetleriyle ilgili hesaplama araçları bulunabiliyor; ancak sonuçları kullanıcının gelirine, bütçesine veya satın alma senaryosuna göre yorumlayan AI destekli finansal danışmanlık bulunmuyor.

## **İletişim:**

- **Yapay Zeka Sohbet Asistanı / Chatbot:** **Yok** — Kullanıcıların site veya ilan hakkında 7/24 soru sorabileceği AI destekli bir sohbet asistanı bulunmuyor.
- **Müşteri Adayı Nitelendirme:** **Kısmi** — İletişim, valuation ve viewing formları kullanıcıdan çeşitli bilgiler topluyor. Ancak bu bilgileri AI kullanarak analiz eden, lead kalitesini puanlayan veya satış ekibine önceliklendirilmiş adaylar sunan bir sistem bulunmuyor.
- **Otomatik Rezervasyon / Görüntüleme Planlama:** **Kısmi** — Kullanıcılar ilan üzerinden viewing talebinde bulunabiliyor; ancak müsaitlikleri otomatik kontrol eden, kullanıcı tercihleriyle eşleştiren ve randevuyu AI ile planlayan bir sistem gözlemlenmiyor.
- **Mesai Dışı Yanıt:** **Yok** — İletişim formları ve danışman iletişim kanalları mevcut; ancak mesai dışında kullanıcı sorularını otomatik olarak yanıtlayan AI tabanlı bir sistem bulunmuyor.

## **Teknik/Genel:**

- **SSR ve CSR:** **Kısmi** — Temel ilan ve içerik sayfaları erişilebilir durumda; ancak sayfaların SSR/CSR mimarisi yalnızca dışarıdan yapılan incelemeyle kesin olarak doğrulanamıyor.
- **API Çağrıları:** **Kısmi** — İlan ve kullanıcı etkileşimleri için arka planda servis/API kullanımı bulunuyor; ancak sayfa incelemesi üzerinden AI öneri, NLP veya generatif içerik üreten ayrı bir AI API katmanı doğrulanamıyor.
- **Mobil Davranış:** **Var** — Site responsive yapıda ve mobil cihazlarda ilan arama, ilan detaylarını görüntüleme ve iletişim işlemleri gerçekleştirilebiliyor. Ancak mobil kullanıcı deneyiminde doğal dil araması veya AI destekli hızlı filtreleme bulunmuyor.

### **Genel AI Fırsatları**

Courtyard Homes için en belirgin AI geliştirme alanları:

1. **Natural Language Property Search** — Kullanıcının günlük dilde yazdığı ihtiyaçları filtrelere dönüştürme.
2. **AI Property Summary** — Uzun ilan açıklamalarından kısa ve anlaşılır özet oluşturma.
3. **AI Property Q&A** — İlan verileri üzerinden kullanıcı sorularını anlık yanıtlama.
4. **Lifestyle Matching** — Kullanıcı ihtiyaçlarını analiz ederek uygun ilanları önceliklendirme.
5. **AI Area & Commute Insights** — Bölge ve ulaşım verilerini kullanıcının hedeflerine göre yorumlama.
6. **AI Valuation Explanation** — Tahmini mülk değerinin hangi faktörlere dayandığını açıklama.
7. **AI Lead Qualification** — Formlardan gelen adayları analiz ederek satış ekibi için önceliklendirme.
8. **AI Viewing Assistant** — Kullanıcı ve danışman müsaitliklerini eşleştirerek görüntüleme sürecini otomatikleştirme.

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
