# 20 · bydesignhomes.com

**URL:** https://bydesignhomes.com/
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

- **Natural Language Search:** **Absent** — Property search uses structured filters (buy/rent toggle, distance radius, price range, bedroom range) rather than free-sentence queries.
- **Smart Suggestions / Query Understanding:** **Present** — Every listing on the search results page displays a "100% MATCH" badge with a "Match Score" tooltip: "This is a prediction of what our software thinks you may find an interesting property, based on the unique search criteria that you gave us. You can improve the relevance of your match score by adjusting and saving your search criteria."
- **Saved Search / Alerts:** **Present** — Heads Up Property Alerts let users build a detailed saved profile (locations via towns/villages/postcodes/schools/pubs, property type, price range, bedrooms/bathrooms/receptions, new-homes/retirement/shared-ownership/investment toggles) and receive suggested properties and price-reduction alerts.

## **Listing Detail:**

- **Property Summary (AI):** **Absent** — Listings contain long, hand-written narrative descriptions (including a "Seller's Story" section written in first person), but no separate AI-generated 2–3 point summary was observed.
- **Property Q&A:** **Absent** — No free-form AI Q&A for individual listings was observed.
- **Property Highlights:** **Absent** — Listings present a manually written bullet list of key selling points above the description, but no AI-extracted highlights module was observed.
- **Lifestyle / "Ideal for…" Matching:** **Absent** — Descriptions mention nearby schools, sport and leisure suitable for a lifestyle (e.g. "Mount Kelly in Tavistock... provide strong independent education options"), but this is manually written editorial copy, not AI-generated lifestyle matching.
- **Property Comparison:** **Absent** — No AI-powered comparison of two or more properties was observed.
- **Similar Listings (personalised):** **Absent** — The listing page reviewed did not show a "similar properties" or "you might also like" module; the site's personalisation is expressed through the search-results Match Score rather than on individual listing pages.
- **Area Insights:** **Partial** — Listings include a hand-written "Location" section describing schools, amenities, restaurants and access, but this is editorial copy, not an AI-generated neighbourhood analysis with data (demographics, crime, etc.).
- **Commute Insights:** **Absent** — Descriptions mention distances/road access in prose (e.g. "7 miles from Ashburton with excellent access to the A38"), but there is no dedicated commute-time calculator or AI commentary.
- **Document Explanation (EPC / Floor Plan):** **Absent** — Multiple floor plans and EPC certificates are provided as images/PDF-style graphics, but no AI-powered plain-language explanation of them was observed.

## **Valuation:**

- **Instant Valuation:** **Absent** — Unlike other sites on the same platform, the Valuation page offers only a "Face to Face Valuation" booking option; no instant/online self-serve valuation tool was found on this site.
- **AI Valuation Explanation:** **Absent** — N/A given no instant valuation tool is offered; no AI-generated valuation explanation exists on the site.
- **Mortgage / Stamp Duty Calculator:** **Absent** — The property listing reviewed (a £4.5m estate) has no mortgage or stamp duty calculator widget; only "What's MY property worth?" and direct call/email CTAs are shown.

## **Contact:**

- **AI Chat Assistant / Chatbot:** **Absent** — No site-wide or property-level AI chat assistant or live-chat widget was observed.
- **Lead Qualification:** **Partial** — The Heads Up Alerts registration form collects detailed buyer circumstances (reason for buying, moving timeframe, solicitor status, whether they need to sell an existing property, mortgage/cash status, how they heard about By Design), enabling structured lead segmentation, but no AI-powered lead scoring or prioritisation was observed.
- **Automated Booking / Viewing Scheduling:** **Partial** — Listings provide an "ARRANGE A VIEWING" call-to-action plus a named agent's direct phone/email, but no AI-driven scheduling or automated qualification flow was observed.
- **Out-of-hours Response:** **Absent** — No out-of-hours chatbot or automated response system was observed; contact is via direct agent phone/email or a general enquiry route.

## **Technical / General:**

- **SSR vs CSR:** **Hybrid (SSR + CSR)** — Initial page load is server-side rendered, with core property and content information present directly in the delivered HTML. Client-side hydration then takes over for interactive elements and further navigation. 
- **API calls:** **Present** — The site is explicitly powered by Neuron / Iceberg Digital's "AI Operating System for Estate Agents". Property search results also expose the AI matching functionality through percentage-based match indicators. This verdict rests on vendor self-identification plus the observable match-% UI element; specific runtime API endpoints were not confirmed through Network-tab inspection.
- **Mobile behaviour:** **Present** — The responsive site provides access to property search, listings, alerts, valuation and contact functionality on mobile.
**Status:** Done

### Round 2 — Yasemin

**Search:**
- No natural language search; entering a free-form sentence returns a "Couldn't find the address" response.
- Typos are corrected, but this is a feature of the address autocomplete; there is no AI-powered query interpretation.
- No personalised ranking; the "Suggested" default and the "100% MATCH" badge only reflect filter compliance.
- Every listing shows "100% MATCH" even when no criteria have been entered; the badge is not calculated per user.
- When the result count is high or zero, no intelligent narrowing or alternative area suggestion is offered.

**Property Detail:**

- The highlights list is written manually; there is no AI-generated summary (Property Summary) of the long description.
- The user cannot ask questions about the listing (no AI Property Q&A).
- A gallery and a YouTube tour video are present, but there is no 360° virtual tour.
- No personalised similar listing recommendations or Property Comparison are offered.
- Map, Floor Plan and EPC tabs are present, but there are no AI-powered Area Insights, Commute Insights or document explanations.

**Valuation:**

- No Instant Valuation is offered; there is no flow that attempts to produce a figure.
- Valuation is reduced to an appointment form alone; the user leaves without seeing any estimate on screen.
- The form does not ask about the property's condition or attributes; no data beyond the entered address is collected.
- A date is selected but availability is not confirmed; appointment scheduling is handled manually.
- No Stamp Duty or Mortgage calculator is available; no financial commentary or recommendation is provided.

**Contact:**

- Chatbot styles are loaded in the source, but no working AI Chat Assistant is active; every enquiry is routed to a form or phone call.
- The moving timeframe, solicitor status and property-to-sell answers in the Heads Up form are not turned into Lead Qualification.
- The office list is left to the user; there is no routing to the right branch based on location or enquiry type.
- A date is selected in the appointment form but availability is not confirmed; scheduling is handled manually.
- No automated response is provided outside office hours; enquiries wait until the next working day.

**Technical/General:**

- The listing results are fed by a client-side `filter?search_type=sales` call; no layer intervenes to interpret the query.
- Network traffic contains only IcebergTracker, Sentry and Neuron REST endpoints; no AI service producing recommendations or content is called.
- Chatbot, InstantValuation and StampDutyCalculator components are loaded in the source, but none of them have been activated.
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

- **Doğal Dil Araması:** **Yok** — Mülk araması, serbest cümle yerine yapılandırılmış filtreler kullanıyor (buy/rent seçici, mesafe yarıçapı, fiyat aralığı, oda sayısı aralığı).
- **Akıllı Öneriler / Sorgu Anlama:** **Var** — Arama sonuçları sayfasındaki her ilanda "100% MATCH" rozeti ve şu metni içeren bir "Eşleşme Skoru" tooltip'i bulunuyor: "This is a prediction of what our software thinks you may find an interesting property, based on the unique search criteria that you gave us. You can improve the relevance of your match score by adjusting and saving your search criteria."
- **Kayıtlı Arama / Uyarılar:** **Var** — Heads Up Mülk Uyarıları, kullanıcının konum (kasaba/köy/posta kodu/okul/pub bazlı), mülk tipi, fiyat aralığı, oda/banyo/salon sayısı ve yeni ev/emeklilik/ortak mülkiyet/yatırım gibi seçenekleri içeren ayrıntılı bir kayıtlı profil oluşturmasına izin veriyor ve buna göre önerilen ilan ile fiyat düşüşü bildirimleri gönderiyor.

## **İlan Detay:**

- **Mülk Özeti (YZ):** **Yok** — İlanlarda uzun, elle yazılmış anlatı tarzında açıklamalar bulunuyor (birinci ağızdan yazılmış bir "Satıcının Hikayesi" bölümü dahil), ancak ayrı bir yapay zeka tarafından oluşturulmuş 2–3 maddelik özet gözlemlenmedi.
- **Mülk Soru-Cevap:** **Yok** — İlan hakkında serbest biçimde soru sorulabilen yapay zeka destekli Q&A özelliği gözlemlenmedi.
- **Mülkün Öne Çıkan Özellikleri:** **Yok** — İlanlarda açıklamanın üstünde manuel yazılmış öne çıkan özellikler listesi bulunuyor, ancak yapay zeka tarafından çıkarılmış bir highlights modülü gözlemlenmedi.
- **Yaşam Tarzı / "... için ideal" Eşleştirmesi:** **Yok** — Açıklamalarda yakın okullar, spor ve boş zaman aktiviteleri gibi yaşam tarzına uygun bilgiler geçiyor (ör. "Mount Kelly in Tavistock... provide strong independent education options"), ancak bu manuel yazılmış editoryal metin, yapay zeka destekli yaşam tarzı eşleştirmesi değil.
- **Mülk Karşılaştırma:** **Yok** — İki veya daha fazla mülkü yapay zeka ile karşılaştırma özelliği gözlemlenmedi.
- **Benzer İlanlar (kişiselleştirilmiş):** **Yok** — İncelenen ilan sayfasında "benzer mülkler" veya "bunlar da ilginizi çekebilir" modülü bulunmuyor; sitenin kişiselleştirmesi ilan sayfası düzeyinde değil, arama sonuçlarındaki Eşleşme Skoru üzerinden ifade ediliyor.
- **Bölge İçgörüleri:** **Kısmi** — İlanlarda okullar, olanaklar, restoranlar ve ulaşımı anlatan elle yazılmış bir "Location" bölümü bulunuyor, ancak bu editoryal metin; demografi, suç oranı gibi verilerle desteklenen yapay zeka destekli bir bölge analizi değil.
- **Ulaşım İçgörüleri:** **Yok** — Açıklamalarda mesafe/yol erişimi düz metinle belirtiliyor (ör. "7 miles from Ashburton with excellent access to the A38"), ancak özel bir ulaşım süresi hesaplayıcısı veya yapay zeka yorumu bulunmuyor.
- **Belge Açıklaması (EPC / Kat Planı):** **Yok** — Birden fazla kat planı ve EPC sertifikası görsel/PDF formatında sunuluyor, ancak bunları sade bir dille açıklayan yapay zeka özelliği gözlemlenmedi.

## **Değerleme:**

- **Anlık Değerleme:** **Yok** — Aynı platformdaki diğer sitelerin aksine, Valuation sayfası yalnızca "Yüz Yüze Değerleme" randevu seçeneği sunuyor; sitede anlık/online kendi kendine değerleme aracı bulunamadı.
- **Yapay Zeka Değerleme Açıklaması:** **Yok** — Anlık değerleme aracı sunulmadığı için bu madde de geçerli değil; sitede yapay zeka destekli bir değerleme açıklaması bulunmuyor.
- **Mortgage / Damga Vergisi Hesaplayıcısı:** **Yok** — İncelenen ilanda (4,5 milyon £'luk bir malikane) mortgage veya stamp duty hesaplayıcı widget'ı yok; sadece "What's MY property worth?" ve doğrudan arama/e-posta çağrı'ları gösteriliyor.

## **İletişim:**

- **Yapay Zeka Sohbet Asistanı / Chatbot:** **Yok** — Site genelinde veya ilan seviyesinde yapay zeka destekli sohbet asistanı veya canlı sohbet widget'ı gözlemlenmedi.
- **Müşteri Adayı Nitelendirme:** **Kısmi** — Heads Up Uyarıları kayıt formu; alım nedeni, taşınma zamanlaması, avukat/solicitor durumu, mevcut mülkün satılması gerekip gerekmediği, mortgage/nakit durumu ve By Design'ı nereden duyduğu gibi ayrıntılı bilgiler topluyor; bu, yapılandırılmış müşteri adayı segmentasyonu sağlıyor, ancak yapay zeka destekli müşteri adayı puanlama veya önceliklendirme gözlemlenmedi.
- **Otomatik Rezervasyon / Görüntüleme Planlama:** **Kısmi** — İlanlarda "ARRANGE A VIEWING" çağrısı ve ilgili danışmanın doğrudan telefon/e-posta bilgisi bulunuyor, ancak yapay zeka destekli randevu planlama veya otomatik ön eleme akışı gözlemlenmedi.
- **Mesai Dışı Yanıt:** **Yok** — Mesai dışı sohbet botu veya otomatik yanıt sistemi gözlemlenmedi; iletişim doğrudan danışman telefonu/e-postası veya genel bir iletişim formu üzerinden sağlanıyor.

## **Teknik/Genel:**

- **SSR ve CSR:** **Hibrit (SSR + CSR)** — İlk sayfa yüklemesi sunucu tarafında render ediliyor; temel ilan ve içerik bilgileri doğrudan teslim edilen HTML içinde yer alıyor. Ardından etkileşimli öğeler ve sonraki gezinmeler için istemci tarafı hydration devreye giriyor. 
- **API Çağrıları:** **Var** — Site açıkça Neuron / Iceberg Digital'in "Estate Agentlar için Yapay Zeka İşletim Sistemi" altyapısını kullanıyor. Property search sonuçlarında yapay zeka eşleştirme sistemi yüzde bazlı eşleşme göstergeleriyle görünür durumda. 
- **Mobil Davranış:** **Var** — Responsive site üzerinden mülk arama, ilanlar, alertler, değerleme ve iletişim özelliklerine mobil erişim sağlanıyor.

**Durum:** Yapıldı

### Tur 2 — Yasemin

**Arama:**

- Doğal dil araması bulunmuyor; serbest cümle girildiğinde "Couldn't find the address" yanıtı dönüyor.
- Yazım hatası düzeltiliyor ancak bu adres tamamlamanın özelliği; AI destekli sorgu yorumlama bulunmuyor.
- Kişiselleştirilmiş sıralama bulunmuyor; "Suggested" varsayılanı ve "100% MATCH" rozeti yalnızca filtre uyumunu gösteriyor.
- Kriter girilmemişken bile her ilan "100% MATCH" gösteriyor; rozet kişiye göre hesaplanmıyor.
- Sonuç sayısı çok ya da sıfır olduğunda akıllı daraltma veya alternatif bölge önerisi sunulmuyor.

**İlan Detay:**

- Öne çıkanlar listesi elle yazılmış; uzun açıklamadan AI destekli özet (Property Summary) bulunmuyor.
- Kullanıcı ilan hakkında soru soramıyor (AI Property Q&A yok).
- Galeri ve YouTube tanıtım videosu mevcut ancak 360° sanal tur bulunmuyor.
- Kişiselleştirilmiş benzer ilan önerisi ve Property Comparison sunulmuyor.
- Harita, Floor Plan ve EPC sekmeleri mevcut ancak AI destekli Area Insights, Commute Insights veya belge açıklaması bulunmuyor.

**Değerleme:**

- Instant Valuation hiç sunulmuyor; rakam üretmeye çalışan bir akış bulunmuyor.
- Değerleme yalnızca randevu formuna indirgenmiş; kullanıcı ekranda hiçbir tahmin görmeden ayrılıyor.
- Formda mülkün durumu veya nitelikleri sorulmuyor; girilen adres dışında veri toplanmıyor.
- Tarih seçiliyor fakat müsaitlik teyit edilmiyor; randevu planlaması elle yapılıyor.
- Stamp Duty ve Mortgage hesaplayıcısı bulunmuyor; finansal yorum veya öneri sunulmuyor.

**İletişim:**

- Kaynakta chatbot stilleri yükleniyor ama çalışan bir AI Chat Assistant devrede değil; her soru forma veya telefona yönleniyor.
- Heads Up formundaki taşınma zamanı, avukat durumu ve satılacak mülk cevapları Lead Qualification'a dönüşmüyor.
- Ofis listesi kullanıcıya bırakılmış; konuma veya talebe göre doğru şubeye yönlendirme yapılmıyor.
- Randevu formunda tarih seçiliyor fakat müsaitlik teyit edilmiyor; planlama elle yapılıyor.
- Mesai dışında otomatik yanıt sunulmuyor; gelen talep ertesi iş gününe kadar bekliyor.

**Teknik/Genel:**

- İlan listesi client-side `filter?search_type=sales` çağrısıyla besleniyor; sorguyu yorumlayan bir katman araya girmiyor.
- Ağ trafiğinde yalnızca IcebergTracker, Sentry ve Neuron REST uçları var; öneri veya içerik üreten bir AI servisi çağrılmıyor.
- Kaynakta chatbot, InstantValuation ve StampDutyCalculator bileşenleri yükleniyor ama hiçbiri devreye alınmamış.
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
