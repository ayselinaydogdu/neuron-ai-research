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
| 3     | Ayselin  | Not done |
| 4     | Görkem   | Not done |

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
