# 01 · kineticestateagents.co.uk

**URL:** https://kineticestateagents.co.uk/
**Group / Grup:** A

---

## English

This site is reviewed independently by 4 people across 4 rounds.

| Round | Reviewer | Status |
|---|---|---|
| 1 | Görkem | Done |
| 2 | Berkay | Done |
| 3 | Yasemin | Not done |
| 4 | Ayselin | Done |

> Fill in only your own round block; don't edit anyone else's.
> Write short, concrete sentences (not "yes/no" — say what it is).
> What to check: ../checklist.md · Terms: ../info/ai-feature-glossary.md

### Round 1 — Görkem

**Search:**
- Homepage is just a Buy/Rent toggle and one box. The real filtering only appears on `/properties`, and even there it's thin: price interval, min–max beds, and a location radius (+0 to +40 miles). No property-type filter, no keyword, no map — list view only.
- As someone genuinely browsing, I couldn't express "2-bed near Waddington under £250k" in one move; I had to set beds, guess a price band, then scroll. The missing **property-type filter is a plain UX gap, not an AI problem — fix that in the UI first.**
- Sort is Suggested / Highest / Lowest price / Newest / Oldest, but "Suggested" isn't explained; nothing tells me what's driving that order.
- No natural-language search at all. **AI opportunity (platform-level):** a free-text box that maps a sentence onto the existing filter API. Every Neuron tenant shares this exact filter set, so one component serves all 30+ agencies.

**Listing Detail:**
- Standard Neuron template: bullet "key features" up top, then a long hand-written narrative in sections ("Step Inside / Outside / Life in Navenby"). Quality rides entirely on whichever agent typed it.
- On the shared-ownership listing I opened there were only 4 photos, no EPC rating, and the material-information block said 3 beds while the headline said 2 — the kind of contradiction a buyer notices and quietly stops trusting.
- Floorplan present; no 360 tour or video on that listing. "Life in Navenby" area copy is prose only — no structured schools/transport/commute data, and the map tab is thin.
- No AI summary and no way to ask a question. **AI opportunity:** a summary + ask-a-question grounded in the listing's own data would help buyers skim, and could also surface the 2-vs-3-bed contradiction back to the agent (a data-quality win, not just a buyer feature).

**Valuation:**
- "Book a Valuation" only — Kinetic deliberately leans human ("valuations start with a conversation, no script"). No instant number anywhere.
- That fits their anti-corporate brand, but a seller who just wants a ballpark at 11pm gets nothing. A midpoint (instant range + AI explanation of what it's based on) would keep the human close without the dead end.

**Contact:**
- Phone + email + a "Book a Viewing" button on the listing; the enquiry itself is a generic form (I didn't submit it). No live chat, nothing out-of-hours.
- No lead qualification — every enquiry lands looking identical to the agency.

**Technical / General:**
- Powered by Neuron | Iceberg Digital (Vercel image optimization, Lifesycle S3 CDN), API-driven modern build. The footer literally reads "AI Operating System for Estate Agents", which is ironic given there's zero user-facing AI.
- First impression is genuinely strong: energetic, anti-corporate tone, 20+ named testimonials. Trust isn't the problem here — discovery friction is.
- Couldn't properly test mobile gestures by inspection; layout is responsive, but the radius/price filter UX on a phone deserves a real-device check.

**Status:** Done

### Round 2 — Berkay

## **Search:**

- **Natural Language Search:** **Absent** — Property search uses structured Buy/Rent filters and location criteria rather than free-sentence queries.
- **Smart Suggestions / Query Understanding:** **Absent** — Property matching is based on structured saved criteria (price, beds, location, radius) entered via the Heads Up Alerts form, functioning as a rule-based saved-search match rather than AI-driven query understanding or smart suggestions. No evidence of NLP-based interpretation or intelligent recommendation logic was observed on the site itself.
- **Saved Search / Alerts:** **Present** — Heads Up Property Alerts let buyers and renters save detailed requirements and receive tailored alerts for suitable properties, including properties before they reach Rightmove.

## **Listing Detail:**

- **Property Summary (AI):** **Absent** — Property pages contain manually written descriptions and property information, but no AI-generated 2–3 point summary was observed.
- **Property Q&A:** **Absent** — No free-form AI Q&A for individual listings was observed.
- **Property Highlights:** **Partial** — Listings provide a dedicated Features section with concise property highlights, but there is no evidence that these highlights are AI-generated.
- **Lifestyle / "Ideal for…" Matching:** **Partial** — Property descriptions can explain who a property may suit, but no explicit AI-generated lifestyle matching commentary was observed.
- **Property Comparison:** **Absent** — No AI-powered comparison of multiple properties was observed.
- **Similar Listings (personalised):** **Absent** — No "similar properties" or personalised recommendation section was observed on individual property pages. The Heads Up Alerts system is a separate, user-initiated saved-search feature, not an on-page similar-listings widget.
- **Area Insights:** **Partial** — Property descriptions and local content provide information about locations, amenities and transport, but no AI-generated neighbourhood analysis covering demographics, crime or similar data was observed.
- **Commute Insights:** **Partial** — Transport links and travel connections are included in some property information, but there is no personalised commute-time analysis based on the user's destination.
- **Document Explanation (EPC / Floor Plan):** **Absent** — EPC information and floor plans are provided, but no AI-powered plain-language explanation of these documents was observed.

## **Valuation:**

- **AI Valuation Explanation:** **Absent** — The valuation process focuses on agent advice and local knowledge rather than an AI-generated valuation explanation.
- **Mortgage / Stamp Duty Calculator:** **Absent** — No dedicated mortgage or Stamp Duty calculator with AI financial commentary was observed.

## **Contact:**

- **AI Chat Assistant / Chatbot:** **Absent** — No site-wide or property-level AI chat assistant was observed.
- **Lead Qualification:** **Partial** — Property alert registration collects detailed buyer circumstances, including moving timeframe, solicitor status, whether the user needs to sell, and mortgage requirements. Rental registration collects additional affordability and applicant information. No AI lead scoring or prioritisation was observed.
- **Automated Booking / Viewing Scheduling:** **Partial** — Property pages provide a "BOOK A VIEWING" option, but the process can require pre-qualification and agent contact rather than AI-driven scheduling.
- **Out-of-hours Response:** **Absent** — No automated out-of-hours AI chatbot or conversational response system was observed.

## **Technical / General:**

- **SSR vs CSR:** **SSR** — The site delivers fully rendered property content (descriptions, features, pricing, floor plans) in the initial HTML response without requiring client-side JavaScript execution, confirming a server-side rendering (or static/prerendered) architecture rather than a pure CSR single-page app.
- **API calls:** **Present** — The site is powered by Neuron / Iceberg Digital and uses its property-alert and matching infrastructure, but the specific runtime API calls were not confirmed through Network-tab inspection.
- **Mobile behaviour:** **Present** — The responsive site provides access to property search, listings, alerts and contact forms on mobile, but detailed usability of every filter and form requires direct device testing.

**Status:** Done

### Round 3 — Yasemin

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

### Round 4 — Ayselin

## Search:

- **Natural Language Search:** **Absent** — Homepage provides a simple Buy/Rent selection and a basic search box. More detailed filters are available on the `/properties` page, including price range, number of bedrooms and location radius. However, users cannot enter natural-language queries such as “2-bed near Waddington under £250k.”  
  **AI opportunity:** A natural-language search layer could convert free-text queries into the existing Neuron property filters, making the feature reusable across multiple Neuron-powered agencies.

- **Smart Suggestions / Query Understanding:** **Absent** — Property matching is based on structured criteria such as price, bedrooms, location and radius. The Heads Up Property Alerts feature can match saved requirements with suitable properties, but there is no evidence of AI-based query understanding or intelligent property recommendations.

- **Saved Search / Alerts:** **Present** — Heads Up Property Alerts allows buyers and renters to save detailed requirements and receive alerts for suitable properties. The service also promotes access to properties before they reach Rightmove.

- The search experience is functional but relatively limited. Important filters such as property type and keyword search are missing. Sorting includes Suggested, Highest Price, Lowest Price, Newest and Oldest, but the logic behind the “Suggested” option is not clearly explained.

---

## Listing Detail:

- **Property Summary (AI):** **Absent** — Property pages contain manually written descriptions, feature lists and property information, but there is no AI-generated summary that allows users to quickly understand the main points of a listing.

- **Property Q&A:** **Absent** — There is no AI assistant that allows users to ask questions about an individual property.  
  **AI opportunity:** A property-specific Q&A assistant could answer questions using the property's description, features, floor plan and other verified listing data.

- **Property Highlights:** **Partial** — Listings contain a dedicated Features section with concise property highlights, but these appear to be manually provided rather than AI-generated.

- **Lifestyle / "Ideal for…" Matching:** **Partial** — Property descriptions sometimes indicate who the property may be suitable for, but there is no explicit AI-powered lifestyle matching system that connects property characteristics with individual user preferences.

- **Property Comparison:** **Absent** — No AI-powered comparison feature was observed for comparing multiple properties based on price, bedrooms, location, features or overall suitability.

- **Similar Listings (personalised):** **Absent** — No personalised “similar properties” or recommendation section was observed on individual property pages. Heads Up Alerts is a saved-search feature rather than an on-page personalised recommendation system.

- **Area Insights:** **Partial** — Property descriptions include information about local areas, amenities and transport, but there is no AI-generated structured neighbourhood analysis covering factors such as schools, transport, amenities or lifestyle suitability.

- **Commute Insights:** **Partial** — Some listings provide information about transport connections and nearby routes, but there is no personalised commute-time analysis based on a user's workplace or chosen destination.

- **Document Explanation (EPC / Floor Plan):** **Absent** — EPC information and floor plans may be available, but there is no AI-powered explanation that converts these documents into simple, user-friendly information.

- **Data Quality:** **Improvement opportunity** — Property information can contain inconsistencies between different sections of a listing. For example, a listing was observed with different bedroom counts in separate parts of the page. An AI-powered validation layer could detect these contradictions and notify the agent before they affect the customer experience.

---

## Valuation:

- **AI Valuation Explanation:** **Absent** — The website focuses on its “Book a Valuation” process and emphasises direct communication with the agent. There is no instant valuation estimate or AI-generated explanation of how a potential property value could be determined.  
  **AI opportunity:** An indicative valuation range with an explanation of the main factors could provide users with an initial estimate while still directing them toward a professional agent valuation.

- **Mortgage / Stamp Duty Calculator:** **Absent** — No dedicated mortgage or Stamp Duty calculator with AI-generated financial commentary was observed.

---

## Contact:

- **AI Chat Assistant / Chatbot:** **Absent** — No site-wide or property-level AI chatbot was observed.

- **Lead Qualification:** **Partial** — Heads Up Alerts collects detailed information about buyers and renters, including moving timeframe, solicitor status, mortgage requirements and whether the user needs to sell another property. However, there is no evidence of AI-based lead scoring or prioritisation.

- **Automated Booking / Viewing Scheduling:** **Partial** — Property pages include a “BOOK A VIEWING” option, but the process still depends largely on agent interaction rather than automated AI scheduling.

- **Out-of-hours Response:** **Absent** — No AI-powered out-of-hours assistant was observed for answering questions or handling enquiries outside normal business hours.

---

## Technical / General:

- **SSR vs CSR:** **SSR** — Property content such as descriptions, features, pricing and floor plans is delivered as rendered HTML without requiring the entire page to be generated through client-side JavaScript, indicating a server-rendered or prerendered architecture.

- **API calls:** **Present** — The website is powered by Neuron / Iceberg Digital and uses its property and alert infrastructure. However, the specific runtime API calls were not independently confirmed through detailed Network-tab inspection.

- **Mobile behaviour:** **Present** — The website is responsive and provides access to property search, listings, alerts and contact forms on mobile devices. However, the usability of filters such as price range and location radius should be tested directly on a physical mobile device.

- **Overall UX:** **Good** — The website has a distinctive, energetic and anti-corporate brand identity, supported by numerous testimonials. The main weakness is property discovery rather than trust or branding. Users have limited ways to search, understand and compare properties intelligently.

- **AI Opportunity:** **High** — Although the Neuron platform describes itself as an “AI Operating System for Estate Agents,” Kinetic Estate Agents currently has very limited visible customer-facing AI functionality. The strongest opportunities are natural-language search, AI property summaries, property Q&A, data-quality checking, personalised recommendations and AI-assisted lead qualification.


**Status:** Done

### Findings / Synthesis (filled once all 4 rounds are done)

- Commonly missing AI features:
- Standout opportunities:
- Disagreements / to verify:

---

## Türkçe

Bu siteyi 4 tur boyunca 4 farklı kişi bağımsız inceler.

| Tur | İnceleyen | Durum |
|---|---|---|
| 1 | Görkem | Yapıldı |
| 2 | Berkay | Yapıldı |
| 3 | Yasemin | Yapılmadı |
| 4 | Ayselin | Yapıldı |

> Sadece kendi tur bloğunuzu doldurun; başkasının bloğunu değiştirmeyin.
> Kısa, somut cümleler yazın ("Var/Yok" değil, ne olduğunu yazın).
> Neye bakılacağı: ../checklist.md · Terimler: ../info/ai-feature-glossary.md

### Tur 1 — Görkem

**Arama:**
- Ana sayfa yalnızca Buy/Rent toggle ve tek bir kutu. Gerçek filtreleme sadece `/properties` sayfasında çıkıyor, o da zayıf: price interval, min–max beds ve konum yarıçapı (+0 ila +40 mil). Property-type filtresi yok, keyword yok, harita yok — sadece liste görünümü.
- Gerçekten ev arıyormuş gibi baktığımda "Waddington yakınında £250k altı 2+1" diyemedim; önce beds, sonra tahmini bir fiyat aralığı seçip kaydırmam gerekti. Eksik **property-type filtresi düz bir UX açığı, AI problemi değil — önce arayüzde çözülmeli.**
- Sıralama Suggested / Highest / Lowest price / Newest / Oldest, ama "Suggested" açıklanmıyor; bu sıralamayı neyin belirlediği belli değil.
- Doğal dil araması hiç yok. **AI fırsatı (platform seviyesi):** bir cümleyi mevcut filtre API'sine çeviren serbest metin kutusu. Her Neuron tenant'ı aynı filtre setini paylaştığı için tek bir bileşen 30+ acentenin hepsine hizmet eder.

**İlan Detay:**
- Standart Neuron şablonu: üstte madde madde "key features", altında bölümlere ayrılmış uzun elle yazılmış anlatı ("Step Inside / Outside / Life in Navenby"). Kalite tamamen ilanı yazan danışmana bağlı.
- Açtığım shared-ownership ilanında sadece 4 fotoğraf vardı, EPC rating yoktu ve material-information bloğu 3 yatak odası derken başlık 2 diyordu — alıcının fark edip sessizce güvenini kaybettiği türden bir çelişki.
- Floorplan var; 360 tur veya video yok. "Life in Navenby" bölge metni sadece düz yazı — yapılandırılmış okul/ulaşım/commute verisi yok, map sekmesi zayıf.
- AI özet yok, soru sorma imkânı yok. **AI fırsatı:** ilanın kendi verisine dayalı özet + soru-cevap alıcının hızlı taramasına yardım eder ve 2-vs-3 yatak odası çelişkisini danışmana geri bildirebilir (sadece alıcı özelliği değil, veri kalitesi kazancı).

**Değerleme:**
- Yalnızca "Book a Valuation" — Kinetic bilinçli olarak insana yaslanıyor ("valuations start with a conversation, no script"). Hiçbir yerde anlık rakam yok.
- Bu anti-kurumsal markaya uyuyor, ama gece 11'de sadece kabaca bir rakam isteyen satıcıya hiçbir şey vermiyor. Bir ara nokta (anlık aralık + AI açıklaması) insan ilişkisini bozmadan bu çıkmazı kapatırdı.

**İletişim:**
- Telefon + e-posta + ilanda "Book a Viewing" butonu; enquiry düz bir form (göndermedim). Canlı sohbet yok, mesai dışı hiçbir şey yok.
- Lead qualification yok — her enquiry acenteye aynı görünüyor.

**Teknik/Genel:**
- Neuron | Iceberg Digital (Vercel image optimization, Lifesycle S3 CDN), API tabanlı modern yapı. Footer düpedüz "AI Operating System for Estate Agents" yazıyor, ama sitede kullanıcıya dönük sıfır AI olması ironik.
- İlk izlenim gerçekten güçlü: enerjik, anti-kurumsal ton, 20+ isimli testimonial. Buradaki sorun güven değil — keşif sürtünmesi.
- Mobil hareketleri inceleyerek test edemedim; layout responsive ama telefonda yarıçap/fiyat filtresi UX'i gerçek cihazda kontrol edilmeli.

**Durum:** Yapıldı

### Tur 2 — Berkay

## **Arama:**

- **Doğal Dil Araması:** **Yok** — Mülk araması serbest cümleler yerine Satın Alma/Kiralama filtreleri ve konum kriterleri kullanıyor.
- **Akıllı Öneriler / Sorgu Anlama:** **Yok** — Mülk eşleştirmesi, Heads Up Alerts formu üzerinden girilen yapılandırılmış kriterlere (fiyat, oda sayısı, lokasyon, yarıçap) dayanıyor; bu, yapay zeka destekli sorgu anlama veya akıllı öneri değil, kural tabanlı bir kayıtlı arama eşleştirmesi. Sitede NLP tabanlı yorumlama veya akıllı öneri mantığına dair bir kanıt gözlemlenmedi.
- **Kayıtlı Arama / Uyarılar:** **Var** — Heads Up Mülk Uyarıları ile alıcılar ve kiracılar ayrıntılı kriterlerini kaydedebiliyor ve uygun ilanlar hakkında, Rightmove'a çıkmadan önceki ilanlar da dahil olmak üzere, kişiselleştirilmiş bildirimler alabiliyor.

## **İlan Detay:**

- **Mülk Özeti (YZ):** **Yok** — İlan sayfalarında manuel olarak hazırlanmış açıklamalar ve mülk bilgileri bulunuyor; yapay zeka tarafından oluşturulan 2–3 maddelik özet gözlemlenmedi.
- **Mülk Soru-Cevap:** **Yok** — İlan hakkında serbest biçimde soru sorulabilen yapay zeka destekli Q&A özelliği gözlemlenmedi.
- **Mülkün Öne Çıkan Özellikleri:** **Kısmi** — İlanlarda kısa mülk özelliklerini içeren ayrı bir Özellikler bölümü bulunuyor; ancak bu özelliklerin yapay zeka tarafından oluşturulduğuna dair kanıt bulunmuyor.
- **Yaşam Tarzı / "... için ideal" Eşleştirmesi:** **Kısmi** — İlan açıklamalarında mülkün kimlere uygun olabileceği anlatılabiliyor; ancak açık bir yapay zeka destekli yaşam tarzı eşleştirmesi veya yorumu gözlemlenmedi.
- **Mülk Karşılaştırma:** **Yok** — Birden fazla mülkü yapay zeka ile karşılaştırma özelliği gözlemlenmedi.
- **Benzer İlanlar (kişiselleştirilmiş):** **Yok** — İlan detay sayfalarında "benzer mülkler" veya kişiselleştirilmiş öneri bölümü gözlemlenmedi. Heads Up Alerts sistemi, kullanıcının kendi başlattığı ayrı bir kayıtlı arama özelliğidir; sayfa içi benzer ilan widget'ı değildir.
- **Bölge İçgörüleri:** **Kısmi** — İlan açıklamalarında ve yerel içeriklerde bölgeler, olanaklar ve ulaşım hakkında bilgiler bulunuyor; ancak demografi, suç oranı ve benzeri verileri yapay zeka ile yorumlayan özel bir bölge analizi bulunmuyor.
- **Ulaşım İçgörüleri:** **Kısmi** — Bazı mülk bilgilerinde ulaşım bağlantıları ve seyahat bilgileri veriliyor; ancak kullanıcının belirlediği hedefe göre kişiselleştirilmiş ulaşım süresi analizi bulunmuyor.
- **Belge Açıklaması (EPC / Kat Planı):** **Yok** — EPC bilgileri ve kat planları sunuluyor; ancak bu belgeleri sade bir dille açıklayan yapay zeka özelliği bulunmuyor.

## **Değerleme:**

- **Yapay Zeka Değerleme Açıklaması:** **Yok** — Değerleme süreci yapay zeka tarafından oluşturulan bir açıklama yerine danışman tavsiyesi ve yerel bilgiye dayanıyor.
- **Mortgage / Damga Vergisi Hesaplayıcısı:** **Yok** — yapay zeka destekli finansal yorum içeren özel bir mortgage veya Stamp Duty hesaplayıcısı gözlemlenmedi.

## **İletişim:**

- **Yapay Zeka Sohbet Asistanı / Chatbot:** **Yok** — Site genelinde veya ilan seviyesinde yapay zeka destekli sohbet asistanı gözlemlenmedi.
- **Müşteri Adayı Nitelendirme:** **Kısmi** — Mülk Uyarısı kayıt süreci; taşınma zamanı, solicitor durumu, mevcut mülkün satılması gerekip gerekmediği ve mortgage ihtiyacı gibi ayrıntılı bilgiler topluyor. Kiralama kaydı ise karşılanabilirlik ve başvuru sahibi hakkında ek bilgiler topluyor. Ancak yapay zeka destekli müşteri adayı puanlama veya önceliklendirme bulunmuyor.
- **Otomatik Rezervasyon / Görüntüleme Planlama:** **Kısmi** — İlan sayfalarında "BOOK A VIEWING" seçeneği bulunuyor; ancak süreç bazı ilanlarda ön eleme ve danışman iletişimi gerektiriyor ve yapay zeka destekli randevu planlama kullanılmıyor.
- **Mesai Dışı Yanıt:** **Yok** — Mesai dışı AI sohbet botu veya otomatik konuşma tabanlı yanıt sistemi gözlemlenmedi.

## **Teknik/Genel:**

- **SSR ve CSR:** **SSR** — Site, mülk içeriğini (açıklamalar, özellikler, fiyat, kat planı) istemci tarafında JavaScript çalıştırmaya gerek kalmadan, ilk HTML yanıtında tam olarak render edilmiş şekilde sunuyor. Bu, saf bir CSR (tek sayfa uygulama) mimarisi yerine sunucu taraflı render (veya statik/prerender) mimarisini doğruluyor.
- **API Çağrıları:** **Var** — Site Neuron / Iceberg Digital altyapısını kullanıyor ve property alert/matching sistemlerinden yararlanıyor.
- **Mobil Davranış:** **Var** — Responsive site üzerinden mülk arama, ilanlar, alertler ve iletişim formlarına mobil erişim sağlanıyor.

**Durum:** Yapıldı

### Tur 3 — Yasemin

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

### Tur 4 — Ayselin

## Arama:

- **Doğal Dil Araması:** **Yok** — Ana sayfada Buy/Rent seçimi ve basit bir arama kutusu bulunuyor. Daha detaylı filtreler `/properties` sayfasında mevcut; fiyat aralığı, yatak odası sayısı ve konum yarıçapı gibi kriterler kullanılabiliyor. Ancak kullanıcılar “Waddington yakınında 250 bin £ altı 2 yatak odalı ev” gibi doğal dilde sorgular giremiyor.  
  **AI fırsatı:** Doğal dil arama katmanı, kullanıcıların serbest metin sorgularını mevcut Neuron mülk filtrelerine dönüştürebilir. Böylece aynı özellik Neuron kullanan birden fazla emlak sitesinde yeniden kullanılabilir.

- **Akıllı Öneriler / Sorgu Anlama:** **Yok** — Mülk eşleştirme; fiyat, yatak odası, konum ve yarıçap gibi yapılandırılmış kriterlere dayanıyor. Heads Up Property Alerts, kullanıcıların kaydettiği kriterlere uygun mülkleri eşleştirebiliyor ancak AI tabanlı sorgu anlama veya akıllı mülk önerileri bulunmuyor.

- **Kayıtlı Arama / Uyarılar:** **Mevcut** — Heads Up Property Alerts, alıcı ve kiracıların detaylı kriterlerini kaydetmesine ve uygun mülkler hakkında bildirim almasına olanak sağlıyor. Sistem ayrıca Rightmove'a ulaşmadan önce bazı mülklere erişim sunuyor.

- Arama deneyimi işlevsel ancak oldukça sınırlı. Property Type ve keyword gibi önemli filtreler bulunmuyor. Sıralama seçenekleri Suggested, Highest Price, Lowest Price, Newest ve Oldest şeklinde; ancak “Suggested” seçeneğinin hangi mantığa göre çalıştığı açık değil.

---

## İlan Detayı:

- **Mülk Özeti (AI):** **Yok** — İlan sayfalarında manuel olarak hazırlanmış açıklamalar, özellik listeleri ve mülk bilgileri bulunuyor ancak kullanıcıların ilanı hızlıca anlamasını sağlayacak AI tarafından oluşturulmuş kısa bir özet bulunmuyor.

- **Mülk Soru-Cevap:** **Yok** — Kullanıcıların belirli bir mülk hakkında soru sorabileceği bir AI asistanı bulunmuyor.  
  **AI fırsatı:** Mülke özel bir Q&A asistanı; ilan açıklaması, özellikler, kat planı ve diğer doğrulanmış ilan verilerini kullanarak kullanıcı sorularını cevaplayabilir.

- **Mülk Öne Çıkan Özellikleri:** **Kısmi** — İlanlarda kısa mülk özelliklerinin yer aldığı ayrı bir Features bölümü bulunuyor ancak bu özelliklerin AI tarafından oluşturulduğuna dair bir kanıt yok; manuel olarak giriliyor.

- **Yaşam Tarzı / “Kimler İçin Uygun?” Eşleştirmesi:** **Kısmi** — İlan açıklamalarında mülkün kimler için uygun olabileceğine dair bilgiler zaman zaman veriliyor. Ancak mülk özelliklerini kullanıcının kişisel tercihleriyle eşleştiren açık bir AI sistemi bulunmuyor.

- **Mülk Karşılaştırma:** **Yok** — Birden fazla mülkü fiyat, yatak odası, konum, özellikler veya genel uygunluk açısından karşılaştıran AI destekli bir özellik gözlemlenmedi.

- **Benzer İlanlar (kişiselleştirilmiş):** **Yok** — İlan sayfalarında kişiselleştirilmiş “benzer mülkler” veya önerilen mülkler bölümü gözlemlenmedi. Heads Up Alerts, sayfa üzerindeki kişiselleştirilmiş önerilerden ziyade kayıtlı arama kriterlerine dayalı bir sistem.

- **Bölge İçgörüleri:** **Kısmi** — İlan açıklamalarında bölge, çevredeki olanaklar ve ulaşım hakkında bilgiler bulunuyor ancak okullar, ulaşım, olanaklar veya yaşam tarzına uygunluk gibi konuları yapılandırılmış şekilde analiz eden AI destekli bir bölge analizi bulunmuyor.

- **Ulaşım / İşe Gidiş İçgörüleri:** **Kısmi** — Bazı ilanlarda ulaşım bağlantıları ve yakın güzergâhlar hakkında bilgi veriliyor ancak kullanıcının iş yeri veya belirlediği hedef noktaya göre kişiselleştirilmiş ulaşım süresi analizi bulunmuyor.

- **Belge Açıklama (EPC / Kat Planı):** **Yok** — EPC bilgileri ve kat planları bulunabiliyor ancak bu belgeleri daha anlaşılır bir dile dönüştüren AI destekli bir açıklama sistemi bulunmuyor.

- **Veri Kalitesi:** **Geliştirme fırsatı** — İlanın farklı bölümlerinde aynı mülke ait bilgiler arasında tutarsızlıklar oluşabiliyor. Örneğin bir ilanda farklı bölümlerde farklı yatak odası sayıları gösterildiği gözlemlendi. AI destekli bir doğrulama katmanı bu tür çelişkileri tespit ederek yayınlanmadan önce veya sonrasında emlak danışmanını uyarabilir.

---

## Değerleme:

- **AI Değerleme Açıklaması:** **Yok** — Web sitesi “Book a Valuation” sürecine ve doğrudan emlak danışmanıyla iletişime geçmeye odaklanıyor. Anlık bir değer tahmini veya bir mülkün tahmini değerinin hangi faktörlere göre belirlendiğini açıklayan AI sistemi bulunmuyor.  
  **AI fırsatı:** Kullanıcıya başlangıç niteliğinde bir fiyat aralığı ve bu tahmini etkileyen temel faktörlerin açıklaması sunulabilir. Aynı zamanda kullanıcı profesyonel değerleme için emlak danışmanına yönlendirilebilir.

- **Mortgage / Stamp Duty Calculator:** **Yok** — AI destekli finansal yorumlarla birlikte çalışan özel bir mortgage veya Stamp Duty hesaplayıcısı gözlemlenmedi.

---

## İletişim:

- **AI Chat Assistant / Chatbot:** **Yok** — Site genelinde veya belirli bir mülk sayfasında AI destekli chatbot bulunmuyor.

- **Lead Qualification:** **Kısmi** — Heads Up Alerts sistemi; taşınma zamanı, solicitor durumu, mortgage gereksinimleri ve kullanıcının mevcut mülkünü satması gerekip gerekmediği gibi detaylı bilgileri topluyor. Ancak AI tabanlı lead scoring veya önceliklendirme sistemi bulunmuyor.

- **Otomatik Rezervasyon / Viewing Scheduling:** **Kısmi** — İlan sayfalarında “BOOK A VIEWING” seçeneği bulunuyor ancak süreç büyük ölçüde emlak danışmanının iletişimine bağlı. AI destekli otomatik randevu planlama sistemi bulunmuyor.

- **Mesai Dışı Yanıt:** **Yok** — Mesai saatleri dışında kullanıcı sorularını yanıtlayan veya talepleri yöneten AI destekli bir asistan bulunmuyor.

---

## Teknik / Genel:

- **SSR vs CSR:** **SSR** — Açıklamalar, özellikler, fiyatlar ve kat planları gibi mülk içerikleri, tüm sayfanın client-side JavaScript tarafından oluşturulmasını gerektirmeden render edilmiş HTML olarak sunuluyor. Bu durum server-side rendering veya prerendered bir mimariye işaret ediyor.

- **API çağrıları:** **Mevcut** — Web sitesi Neuron / Iceberg Digital tarafından destekleniyor ve mülk ile alert altyapısını kullanıyor. Ancak spesifik runtime API çağrıları detaylı Network-tab incelemesiyle bağımsız olarak doğrulanmadı.

- **Mobil davranış:** **Mevcut** — Web sitesi responsive yapıya sahip ve mobil cihazlarda mülk arama, ilanlar, uyarılar ve iletişim formlarına erişim sağlıyor. Ancak fiyat aralığı ve konum yarıçapı gibi filtrelerin kullanım kolaylığı gerçek bir mobil cihaz üzerinde ayrıca test edilmeli.

- **Genel UX:** **İyi** — Web sitesi kendine özgü, enerjik ve anti-kurumsal bir marka kimliğine sahip ve çok sayıda müşteri yorumu ile destekleniyor. Temel problem güven veya marka algısı değil, mülk keşif deneyiminin sınırlı olması. Kullanıcıların mülkleri akıllı bir şekilde arama, anlama ve karşılaştırma seçenekleri oldukça sınırlı.

- **AI Fırsatı:** **Yüksek** — Neuron platformu kendisini “AI Operating System for Estate Agents” olarak konumlandırmasına rağmen Kinetic Estate Agents sitesinde kullanıcıya doğrudan sunulan AI özellikleri oldukça sınırlı. En güçlü fırsatlar; doğal dil araması, AI mülk özetleri, mülk Q&A, veri kalitesi kontrolü, kişiselleştirilmiş öneriler ve AI destekli lead qualification alanlarında bulunuyor.


**Durum:** Yapıldı

### Ortak Bulgular / Sentez (4 tur bitince doldurulur)

- Ortak eksik AI özellikleri:
- Öne çıkan fırsatlar:
- Görüş ayrılıkları / doğrulanması gerekenler:
