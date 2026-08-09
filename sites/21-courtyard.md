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
