# 02 · townandcityhomes.com

**URL:** https://townandcityhomes.com/
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
- Same Buy/Rent toggle + single box on the homepage; filtering lives on the properties page (price interval, min–max beds, location radius). No type/keyword, no natural language, list-only, no map — identical to the rest of Group A.
- What's different here is they push "Heads-Up alerts" hard on the homepage ("matched to your wishlist before it hits Rightmove"). Nice hook, but under the hood it's plain criteria matching against a registered saved search, not semantic matching.
- **AI opportunity (platform-level):** make Heads-Up genuinely smart — embed the buyer's own description + click behaviour and rank incoming stock by fit, not just filter equality. It's already wired into every tenant, so upgrading it once lifts all 30+.

**Listing Detail:**
- Standard Neuron listing template — bullet features + long hand-written narrative, floorplan, no 360. Description quality varies agent-to-agent. No AI summary, no ask-a-question, area info as prose only. Same gaps I saw on Kinetic.

**Valuation:**
- Two paths: a "Try this valuation" instant tool (`valuation.townandcityhomes.com`) plus book face-to-face. I stepped through the instant tool: postcode → beds → type → sales/lettings, then it gates on name/email/phone and does **not** show a figure on screen — the "valuation" is delivered later by contact.
- So "instant valuation" is really a lead-capture form wearing an instant-valuation label. That's a **trust risk**: a user expecting a number feels bait-and-switched. This is the shared platform pattern, so it repeats across the group.

**Contact:**
- Phone (01474), email, contact form; no chat/chatbot and no out-of-hours auto-reply. Same single generic form for everyone — no qualification.

**Technical / General:**
- Neuron/Iceberg, Vercel, Lifesycle CDN, separate valuation subdomain.
- Warm, human brand — mascot, real team (Nigel), strong Google reviews plus compliance badges (TPO, Money Shield). Trust is handled well; I'd comfortably leave my details here. The weak spot is the same search/listing thinness as its siblings.

**Status:** Done

### Round 2 — Berkay

## **Search:**

- **Natural Language Search:** **Absent** — Property search uses structured Buy/Rent controls and standard property criteria rather than free-sentence queries.
- **Smart Suggestions / Query Understanding:** **Absent** — Listing pages show a "100% MATCH" badge on every property (44/44 checked, anonymous visitor, no saved criteria). All listings displaying identical 100% values regardless of profile indicates this is a rule-based match against basic search parameters (location, price, beds, property type) rather than an AI/NLP-driven suggestion or query-understanding feature. No evidence of intelligent or personalised matching logic was observed.
- **Saved Search / Alerts:** **Present** — Heads-Up Property Alerts allow users to register detailed buying or renting requirements and receive tailored property updates, including properties before they reach Rightmove or Zoopla. Alerts can be delivered through WhatsApp or email.

## **Listing Detail:**

- **Property Summary (AI):** **Absent** — Property pages provide manually written descriptions and property features, but no AI-generated 2–3 point summary was observed.
- **Property Q&A:** **Absent** — No free-form AI Q&A for individual listings was observed.
- **Property Highlights:** **Partial** — Listings contain concise feature/highlight text alongside the main description, but no evidence that these highlights are AI-generated was observed.
- **Lifestyle / "Ideal for…" Matching:** **Partial** — Property descriptions can explain suitability and local lifestyle benefits, while the matching system connects properties with buyer requirements. However, no explicit AI-generated lifestyle commentary was observed.
- **Property Comparison:** **Absent** — No AI-powered comparison of two or more properties was observed.
- **Similar Listings (personalised):** **Absent** — There is a “Latest Properties” section at the bottom of the property detail pages; however, the properties displayed do not show any similarity to the current listing in terms of price, number of bedrooms, location, or property type. It appears to be the same static “latest listings” content shown on the website’s homepage. No personalized or listing-specific similarity matching was observed, and no match percentage is displayed in this section.
- **Area Insights:** **Partial** — The site provides local information about Gravesend, Dartford and surrounding areas, including community information and local property context, but no dedicated AI-generated neighbourhood analysis covering demographics, crime or similar data was observed.
- **Commute Insights:** **Partial** — Property and local content can mention transport connections and proximity to stations, but no personalised commute-time analysis based on the user's workplace or school was observed.
- **Document Explanation (EPC / Floor Plan):** **Absent** — EPC information and floor plans may be available on listings, but no AI-powered plain-language explanation of these documents was observed.

## **Valuation:**

- **Instant Valuation:** **Present** — The site provides an Instant Valuation option using online property valuation tools. It presents this as a starting-point estimate based on sold-price and postcode data.
- **AI Valuation Explanation:** **Absent** — The instant valuation does not provide an AI-generated explanation of the valuation factors. Town & City instead emphasises that its face-to-face valuation adds local knowledge, property presentation, pricing and strategy.
- **Mortgage / Stamp Duty Calculator:** **Absent** — The site offers access to independent mortgage brokers, but no dedicated mortgage or Stamp Duty calculator with AI financial commentary was observed.

## **Contact:**

- **AI Chat Assistant / Chatbot:** **Absent** — No site-wide or property-level AI chat assistant was observed.
- **Lead Qualification:** **Partial** — Heads-Up registration collects detailed buyer and renter circumstances. Rental registration asks about moving timeframe, applicant type, total income, maximum rent, children, pets, adverse credit and current tenancy notice. This provides structured lead information, but no AI-powered lead scoring or prioritisation was observed.
- **Automated Booking / Viewing Scheduling:** **Partial** — The site states that viewings can be booked quickly and property pages provide viewing/contact options, but no AI-driven appointment scheduling or conversational booking assistant was observed.
- **Out-of-hours Response:** **Absent** — The site states that it is available 24/7 and promotes direct communication and WhatsApp updates, but this appears to be human/direct communication rather than an AI-powered out-of-hours chatbot or automated conversational response system.

## **Technical / General:**

- **SSR vs CSR:** **Hybrid (SSR + CSR)** — Initial page load is server-side rendered, with core property and content information present directly in the delivered HTML. Client-side hydration then takes over for interactive elements and further navigation. 
- **API calls:** **Present** — The site explicitly identifies itself as powered by Neuron / Iceberg Digital's "AI Operating System for Estate Agents," and property results expose an observable AI-style match-percentage element in the UI. 
- **Mobile behaviour:** **Partial** — The responsive website provides access to property search, listings, alerts and contact/valuation forms on mobile, but detailed usability of every filter and form requires direct device testing.

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

## **Search:**

- **Natural Language Search:** **Absent** — The homepage uses a Buy/Rent toggle with a basic search field, while the main filtering options are available on the properties page. Users can filter by price, bedrooms and location radius, but there is no property-type filter, keyword search, map-based search or natural-language input. A query such as “2-bed house near Gravesend under £300k” cannot be entered directly.

- **Smart Suggestions / Query Understanding:** **Absent** — The website strongly promotes its Heads-Up Alerts feature, which notifies users about properties matching their saved requirements. However, the current system appears to rely on predefined criteria rather than understanding the meaning or context of a user's request. The “100% MATCH” indicator was also displayed consistently across listings, including when browsing anonymously without saved criteria, suggesting that it is not currently providing meaningful personalised AI matching.  
  **AI opportunity:** Heads-Up could become a genuinely intelligent recommendation system by combining saved requirements with user behaviour, property interactions and free-text preferences. New properties could then be ranked according to overall suitability rather than simple filter matches. As this functionality is part of the shared Neuron infrastructure, the improvement could potentially benefit multiple agencies.

- **Saved Search / Alerts:** **Present** — Heads-Up Property Alerts allow buyers and renters to register their requirements and receive notifications when matching properties become available. Alerts can be delivered through email or WhatsApp, including notifications for properties before they appear on major property portals.

---

## **Listing Detail:**

- **Property Summary (AI):** **Absent** — Property pages contain manually prepared descriptions and feature lists, but no AI-generated summary was observed to help users quickly understand the most important aspects of a listing.

- **Property Q&A:** **Absent** — There is no property-specific AI assistant that allows users to ask questions and receive answers based on the listing's available information.

- **Property Highlights:** **Partial** — Listings include short feature descriptions and key points, but these appear to be manually entered by the agency rather than dynamically generated or personalised by AI.

- **Lifestyle / "Ideal for…" Matching:** **Partial** — Property descriptions sometimes explain who a property could suit and provide local lifestyle information. However, there is no dedicated AI system that analyses a user's preferences and explains why a particular property may be suitable for them.

- **Property Comparison:** **Absent** — No AI-powered tool was observed for comparing multiple properties based on price, bedrooms, location, features or suitability.

- **Similar Listings (personalised):** **Absent** — A “Latest Properties” section is displayed on property pages, but the properties shown do not appear to be specifically selected based on the current listing. They seem to represent general recent listings rather than personalised recommendations. No similarity score or property-specific recommendation logic was observed.

- **Area Insights:** **Partial** — The website provides local information about areas such as Gravesend and Dartford, including community and property-related information. However, there is no AI-generated neighbourhood analysis covering factors such as schools, demographics, crime, amenities or lifestyle suitability.

- **Commute Insights:** **Partial** — Transport links and nearby stations may be mentioned within property or area information, but there is no personalised commute analysis based on a user's workplace, school or preferred destination.

- **Document Explanation (EPC / Floor Plan):** **Absent** — EPC information and floor plans are available where provided, but there is no AI-powered feature that explains these documents in simple language or highlights important information for the user.

---

## **Valuation:**

- **Instant Valuation:** **Present** — The website provides an online valuation tool where users enter information such as postcode, bedroom count, property type and whether they are interested in selling or letting. However, the process requests personal contact details before providing the result, and no valuation figure is immediately displayed on the screen. As a result, the “instant” valuation functions partly as a lead-generation process rather than a fully instant valuation experience.

- **AI Valuation Explanation:** **Absent** — No AI-generated explanation of the estimated property value or the factors influencing it was observed. The website instead highlights the additional value of a face-to-face valuation, including local knowledge, pricing strategy and property presentation.  
  **AI opportunity:** The online tool could provide an indicative price range immediately and explain the main factors behind the estimate, while still encouraging users to arrange a professional valuation with an agent.

- **Mortgage / Stamp Duty Calculator:** **Absent** — The website provides access to mortgage-related services and independent brokers, but no dedicated mortgage or Stamp Duty calculator with AI-generated financial guidance was observed.

---

## **Contact:**

- **AI Chat Assistant / Chatbot:** **Absent** — No AI-powered chatbot was observed on either the main website or individual property pages.

- **Lead Qualification:** **Partial** — The Heads-Up registration process collects useful information about buyers and renters, including moving timeframe, financial situation and other requirements. Rental enquiries can also include information such as income, affordability, pets, children and current tenancy status. However, there is no evidence of AI-powered lead scoring or automatic prioritisation.

- **Automated Booking / Viewing Scheduling:** **Partial** — Users can request property viewings through the website, but there is no conversational AI assistant or fully automated scheduling system managing the process.

- **Out-of-hours Response:** **Absent** — Although the agency promotes direct communication and WhatsApp updates, no AI-powered out-of-hours assistant was observed that could answer questions or qualify leads automatically.

---

## **Technical / General:**

- **SSR vs CSR:** **Hybrid (SSR + CSR)** — The initial page content is server-rendered, with important property and website information available in the delivered HTML. Client-side JavaScript is then used for interactive components and navigation.

- **API calls:** **Present** — The website is built on the Neuron / Iceberg Digital platform and uses its property, matching and alert infrastructure. The visible “100% MATCH” element suggests that matching information is integrated into the property interface, although the exact underlying API logic was not independently verified.

- **Mobile behaviour:** **Partial** — The website is responsive and provides access to property search, alerts, valuation and contact features on mobile devices. However, the usability of the more detailed filters and forms should be validated through testing on a physical mobile device.

- **Overall UX:** **Good** — The website has a warm and human-oriented identity, supported by a visible team, customer reviews and industry/compliance badges. Trust and brand presentation are strong. The main weakness is the relatively basic property discovery and listing experience.

- **AI Opportunity:** **High** — The site already has a strong foundation through Neuron's matching and alert infrastructure, but most of the customer-facing experience remains rule-based. The biggest opportunities are improving Heads-Up with intelligent matching, introducing natural-language search, adding property Q&A and summaries, providing personalised recommendations and making the valuation process more transparent.

---

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
- Ana sayfada yine Buy/Rent toggle + tek kutu; filtreleme properties sayfasında (price interval, min–max beds, konum yarıçapı). Type/keyword yok, doğal dil yok, sadece liste, harita yok — Grup A'nın geri kalanıyla aynı.
- Buradaki fark: "Heads-Up alerts" ana sayfada güçlü şekilde öne çıkarılıyor ("Rightmove'a düşmeden wishlist'inle eşleşir"). Güzel bir kanca, ama arkada sadece kayıtlı bir aramaya karşı kriter eşleşmesi, semantik eşleşme değil.
- **AI fırsatı (platform seviyesi):** Heads-Up'ı gerçekten akıllı yap — alıcının kendi açıklamasını + tıklama davranışını embed edip gelen stoğu filtre eşitliğine göre değil uygunluğa göre sırala. Zaten her tenant'ta bağlı olduğu için tek seferlik geliştirme 30+ acenteyi birden yükseltir.

**İlan Detay:**
- Standart Neuron ilan şablonu — madde madde features + uzun elle yazılmış anlatı, floorplan, 360 yok. Açıklama kalitesi danışmandan danışmana değişiyor. AI özet yok, soru-cevap yok, bölge bilgisi sadece düz yazı. Kinetic'te gördüğüm aynı açıklar.

**Değerleme:**
- İki yol: "Try this valuation" anlık aracı (`valuation.townandcityhomes.com`) + yüz yüze randevu. Anlık aracı adım adım denedim: postcode → beds → type → sales/lettings, sonra name/email/phone ile kapı tutuyor ve ekranda **rakam göstermiyor** — "valuation" sonradan iletişimle veriliyor.
- Yani "instant valuation" aslında instant-valuation etiketi takmış bir lead-capture formu. Bu bir **güven riski**: rakam bekleyen kullanıcı kandırılmış hissediyor. Bu paylaşılan platform kalıbı, dolayısıyla grup boyunca tekrarlıyor.

**İletişim:**
- Telefon (01474), e-posta, iletişim formu; chat/chatbot yok, mesai dışı otomatik yanıt yok. Herkese aynı tek tip form — kalifikasyon yok.

**Teknik/Genel:**
- Neuron/Iceberg, Vercel, Lifesycle CDN, ayrı valuation subdomain.
- Sıcak, insani marka — maskot, gerçek ekip (Nigel), güçlü Google yorumları ve uyum rozetleri (TPO, Money Shield). Güven iyi yönetilmiş; bilgilerimi rahatça bırakırdım. Zayıf nokta kardeş sitelerdeki aynı arama/ilan zayıflığı.

**Durum:** Yapıldı

### Tur 2 — Berkay

## **Arama:**

- **Doğal Dil Araması:** **Yok** — Mülk araması yapılandırılmış Satın Alma/Kiralama kontrolleri ve standart mülk kriterlerini kullanıyor; serbest cümleyle arama bulunmuyor.
- **Akıllı Öneriler / Sorgu Anlama:** **Yok** — İlan sayfalarında her mülkün yanında bir "100% MATCH" rozeti görünüyor (anonim ziyaretçi, kayıtlı kriter yokken kontrol edilen 44/44 ilan). Profil fark etmeksizin tüm ilanların aynı şekilde %100 göstermesi, bunun yapay zeka/NLP destekli bir öneri veya sorgu anlama özelliği değil, temel arama parametrelerine (lokasyon, fiyat, oda sayısı, mülk tipi) dayalı kural tabanlı bir eşleştirme olduğunu gösteriyor. Akıllı veya kişiselleştirilmiş bir eşleştirme mantığına dair kanıt gözlemlenmedi.
- **Kayıtlı Arama / Uyarılar:** **Var** — Heads-Up Mülk Uyarıları ile kullanıcılar ayrıntılı satın alma veya kiralama gereksinimlerini kaydedebiliyor ve Rightmove veya Zoopla'ya çıkmadan önceki ilanlar da dahil olmak üzere uygun mülkler hakkında bildirim alabiliyor. Bildirimler WhatsApp veya e-posta üzerinden gönderilebiliyor.

## **İlan Detay:**

- **Mülk Özeti (YZ):** **Yok** — İlan sayfalarında manuel olarak hazırlanmış açıklamalar ve mülk özellikleri bulunuyor; yapay zeka tarafından oluşturulan 2–3 maddelik özet gözlemlenmedi.
- **Mülk Soru-Cevap:** **Yok** — İlan hakkında serbest biçimde soru sorulabilen yapay zeka destekli Q&A özelliği gözlemlenmedi.
- **Mülkün Öne Çıkan Özellikleri:** **Kısmi** — İlanlarda ana açıklamanın yanında kısa özellik/öne çıkan bilgi alanları bulunuyor; ancak bunların yapay zeka tarafından oluşturulduğuna dair kanıt bulunmuyor.
- **Yaşam Tarzı / "... için ideal" Eşleştirmesi:** **Kısmi** — İlan açıklamalarında mülkün uygunluğu ve yerel yaşam avantajları anlatılabiliyor; matching sistemi de mülkleri alıcı gereksinimleriyle eşleştiriyor. Ancak açık bir yapay zeka tarafından oluşturulmuş yaşam tarzı yorumu gözlemlenmedi.
- **Mülk Karşılaştırma:** **Yok** — İki veya daha fazla mülkü yapay zeka ile karşılaştırma özelliği gözlemlenmedi.
- **Benzer İlanlar (kişiselleştirilmiş):** **Yok** — İlan detay sayfalarının altında "Latest Properties" bölümü var, ancak bu bölüm o anki ilanla fiyat, oda sayısı, lokasyon veya mülk tipi açısından herhangi bir benzerlik göstermiyor — sitenin ana sayfasındaki genel "son eklenenler" listesiyle aynı, statik bir içerik. Kişiselleştirilmiş veya o ilana özgü bir benzerlik hesaplaması gözlemlenmedi; ayrıca bu bölümde eşleşme yüzdesi de gösterilmiyor.
- **Bölge İçgörüleri:** **Kısmi** — Site Gravesend, Dartford ve çevre bölgeler hakkında topluluk bilgileri ve yerel mülk bağlamı sağlıyor; ancak demografi, suç oranı ve benzeri verileri yapay zeka ile analiz eden özel bir bölge içgörü sistemi gözlemlenmedi.
- **Ulaşım İçgörüleri:** **Kısmi** — İlan ve yerel içeriklerde ulaşım bağlantıları ve istasyonlara yakınlık gibi bilgiler bulunabiliyor; ancak kullanıcının iş veya okul konumuna göre kişiselleştirilmiş ulaşım süresi analizi bulunmuyor.
- **Belge Açıklaması (EPC / Kat Planı):** **Yok** — EPC bilgileri ve kat planları ilanlarda bulunabiliyor; ancak bu belgeleri sade bir dille açıklayan yapay zeka özelliği gözlemlenmedi.

## **Değerleme:**

- **Anlık Değerleme:** **Var** — Site, anlık (instant) online mülk değerleme aracı sunuyor. Bu değerleme, satılan mülk fiyatları ve posta kodu verilerine dayanan başlangıç niteliğinde bir tahmin olarak sunuluyor.
- **Yapay Zeka Değerleme Açıklaması:** **Yok** — Anlık değerleme sonucunun arkasındaki faktörleri açıklayan yapay zeka yorumu bulunmuyor. Town & City bunun yerine yüz yüze değerlemede yerel bilgi, mülk sunumu, fiyatlandırma ve strateji bilgisinin eklenmesini vurguluyor.
- **Mortgage / Damga Vergisi Hesaplayıcısı:** **Yok** — Site bağımsız mortgage brokerlarına yönlendirme yapıyor; ancak yapay zeka destekli finansal yorum içeren özel bir mortgage veya Stamp Duty hesaplayıcısı gözlemlenmedi.

## **İletişim:**

- **Yapay Zeka Sohbet Asistanı / Chatbot:** **Yok** — Site genelinde veya ilan seviyesinde yapay zeka destekli sohbet asistanı gözlemlenmedi.
- **Müşteri Adayı Nitelendirme:** **Kısmi** — Heads-Up kayıt süreci ayrıntılı alıcı ve kiracı bilgileri topluyor. Kiralama kaydında taşınma zamanı, başvuru sahibi tipi, toplam gelir, maksimum kira, çocuklar, evcil hayvanlar, olumsuz kredi geçmişi ve mevcut kiralık mülk için bildirim süresi gibi bilgiler isteniyor. Bu yapılandırılmış lead bilgisi sağlıyor ancak yapay zeka destekli müşteri adayı puanlama veya önceliklendirme bulunmuyor.
- **Otomatik Rezervasyon / Görüntüleme Planlama:** **Kısmi** — Site görüntülemelerin hızlı şekilde ayarlanabildiğini belirtiyor ve ilanlarda görüntüleme/iletişim seçenekleri bulunuyor; ancak yapay zeka destekli randevu planlama veya konuşma tabanlı rezervasyon asistanı gözlemlenmedi.
- **Mesai Dışı Yanıt:** **Yok** — Site 24/7 ulaşılabilir olduğunu belirtiyor ve doğrudan iletişim ile WhatsApp güncellemelerini öne çıkarıyor; ancak bu, yapay zeka destekli bir mesai dışı sohbet botu veya otomatik konuşma tabanlı yanıt sistemi değil, insan/direkt iletişim hizmeti olarak görünüyor.

## **Teknik/Genel:**

- **SSR ve CSR:** **Hibrit (SSR + CSR)** — İlk sayfa yüklemesi sunucu tarafında render ediliyor; temel ilan ve içerik bilgileri doğrudan teslim edilen HTML içinde yer alıyor. Ardından etkileşimli öğeler ve sonraki gezinmeler için istemci tarafı hydration devreye giriyor. 
- **API Çağrıları:** **Var** — Site kendisini Neuron / Iceberg Digital'in "Estate Agentlar için Yapay Zeka İşletim Sistemi" altyapısıyla güçlendirilmiş olarak tanımlıyor ve ilan sonuçlarında gözlemlenebilir yapay zeka tipi eşleşme yüzdesi arayüz öğesi bulunuyor.
- **Mobil Davranış:** **Var** — Responsive site üzerinden mülk arama, ilanlar, alertler ve iletişim/değerleme formlarına mobil erişim sağlanıyor.

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

## **Arama:**

- **Doğal Dil Araması:** **Yok** — Ana sayfada Buy/Rent seçimi ve temel bir arama alanı bulunuyor; asıl filtreleme seçenekleri ise properties sayfasında yer alıyor. Kullanıcılar fiyat, yatak odası ve konum yarıçapına göre filtreleme yapabiliyor ancak mülk tipi, anahtar kelime, harita tabanlı arama veya doğal dil ile arama seçenekleri bulunmuyor. Örneğin “Gravesend yakınında 300 bin £ altı 2 yatak odalı ev” gibi bir sorgu doğrudan girilemiyor.

- **Akıllı Öneriler / Sorgu Anlama:** **Yok** — Web sitesi Heads-Up Alerts özelliğini güçlü şekilde öne çıkarıyor. Bu özellik, kullanıcıların kaydettiği kriterlere uygun mülkler hakkında bildirim gönderiyor. Ancak mevcut sistem, kullanıcının sorgusunun anlamını veya bağlamını anlamaktan ziyade önceden belirlenmiş kriterlere göre çalışıyor gibi görünüyor. Ayrıca “100% MATCH” göstergesinin kayıtlı kriterleri olmayan anonim kullanıcılarda da ilanlar arasında sürekli gösterilmesi, bunun gerçek anlamda kişiselleştirilmiş bir AI eşleştirme sistemi olmadığını düşündürüyor.  
  **AI fırsatı:** Heads-Up, kayıtlı kriterlerin yanı sıra kullanıcının davranışlarını, ilanlarla etkileşimlerini ve serbest metinle belirttiği tercihleri analiz ederek gerçekten akıllı bir öneri sistemine dönüştürülebilir. Yeni ilanlar yalnızca filtrelerin eşleşmesine göre değil, kullanıcının genel ihtiyaçlarına ne kadar uygun olduğuna göre sıralanabilir. Bu özellik Neuron altyapısının ortak bir parçası olduğu için yapılacak geliştirme birden fazla emlak sitesine uygulanabilir.

- **Kayıtlı Arama / Uyarılar:** **Mevcut** — Heads-Up Property Alerts, alıcı ve kiracıların ihtiyaçlarını kaydetmesine ve uygun yeni mülkler hakkında bildirim almasına olanak sağlıyor. Bildirimler e-posta veya WhatsApp üzerinden gönderilebiliyor. Ayrıca bazı mülkler büyük emlak portallarında yayınlanmadan önce kullanıcılara bildirilebiliyor.

---

## **İlan Detayı:**

- **Mülk Özeti (AI):** **Yok** — İlan sayfalarında manuel olarak hazırlanmış açıklamalar ve özellik listeleri bulunuyor ancak kullanıcının ilanı hızlıca anlamasını sağlayacak AI tarafından oluşturulmuş bir özet bulunmuyor.

- **Mülk Soru-Cevap:** **Yok** — Kullanıcıların belirli bir mülk hakkında soru sorarak ilan bilgilerinden cevap alabileceği mülke özel bir AI asistanı bulunmuyor.

- **Mülk Öne Çıkan Özellikleri:** **Kısmi** — İlanlarda kısa özellik açıklamaları ve önemli noktalar bulunuyor ancak bunların AI tarafından dinamik olarak oluşturulduğuna veya kişiselleştirildiğine dair bir kanıt bulunmuyor.

- **Yaşam Tarzı / "Kimler İçin Uygun?" Eşleştirmesi:** **Kısmi** — İlan açıklamalarında mülkün kimler için uygun olabileceği ve bölgedeki yaşam hakkında bilgiler verilebiliyor. Ancak kullanıcının tercihlerini analiz ederek belirli bir mülkün neden kullanıcıya uygun olduğunu açıklayan özel bir AI sistemi bulunmuyor.

- **Mülk Karşılaştırma:** **Yok** — Birden fazla mülkü fiyat, yatak odası, konum, özellikler veya kullanıcıya uygunluk açısından karşılaştıran AI destekli bir araç gözlemlenmedi.

- **Benzer İlanlar (kişiselleştirilmiş):** **Yok** — İlan sayfalarında “Latest Properties” bölümü bulunuyor ancak burada gösterilen mülklerin mevcut ilanla özel olarak eşleştirildiğine dair bir kanıt yok. Bölüm daha çok genel olarak en son eklenen ilanları gösteriyor gibi görünüyor. Kişiselleştirilmiş öneri veya benzerlik skoru bulunmuyor.

- **Bölge İçgörüleri:** **Kısmi** — Web sitesi Gravesend ve Dartford gibi bölgeler hakkında topluluk ve emlak bilgileri sunuyor. Ancak okullar, demografi, suç oranları, olanaklar veya yaşam tarzına uygunluk gibi faktörleri analiz eden AI destekli bir bölge analizi bulunmuyor.

- **Ulaşım / İşe Gidiş İçgörüleri:** **Kısmi** — İlan veya bölge açıklamalarında ulaşım bağlantıları ve yakın istasyonlardan bahsedilebiliyor ancak kullanıcının iş yeri, okulu veya belirlediği hedef noktaya göre kişiselleştirilmiş ulaşım süresi analizi bulunmuyor.

- **Belge Açıklama (EPC / Kat Planı):** **Yok** — EPC bilgileri ve kat planları mevcut olduğunda ilanlarda sunuluyor ancak bu belgeleri basit bir dille açıklayan veya önemli noktaları öne çıkaran AI destekli bir özellik bulunmuyor.

---

## **Değerleme:**

- **Anlık Değerleme:** **Mevcut** — Web sitesinde kullanıcıların posta kodu, yatak odası sayısı, mülk tipi ve satış/kiralama tercihi gibi bilgileri girdiği online bir değerleme aracı bulunuyor. Ancak sonuç aşamasından önce kullanıcıdan iletişim bilgileri isteniyor ve değerleme sonucu ekranda anında gösterilmiyor. Bu nedenle “instant valuation” özelliği tamamen anlık bir değerleme deneyiminden ziyade kısmen lead toplama süreci olarak çalışıyor.

- **AI Değerleme Açıklaması:** **Yok** — Tahmini mülk değerini veya bu değeri etkileyen faktörleri açıklayan AI destekli bir sistem gözlemlenmedi. Bunun yerine web sitesi yüz yüze değerlemenin yerel bilgi, fiyatlandırma stratejisi ve mülk sunumu gibi ek avantajlarını öne çıkarıyor.  
  **AI fırsatı:** Online araç, kullanıcıya anında tahmini bir fiyat aralığı gösterebilir ve bu tahminin arkasındaki temel faktörleri açıklayabilir. Aynı zamanda profesyonel değerleme için emlak danışmanıyla görüşmeye yönlendirme yapılabilir.

- **Mortgage / Stamp Duty Calculator:** **Yok** — Web sitesinde mortgage ile ilgili hizmetler ve bağımsız brokerlara erişim bulunuyor ancak AI destekli finansal yönlendirme sağlayan özel bir mortgage veya Stamp Duty hesaplayıcısı gözlemlenmedi.

---

## **İletişim:**

- **AI Chat Assistant / Chatbot:** **Yok** — Ana web sitesinde veya bireysel ilan sayfalarında AI destekli chatbot bulunmuyor.

- **Lead Qualification:** **Kısmi** — Heads-Up kayıt süreci alıcı ve kiracılar hakkında taşınma zamanı, finansal durum ve diğer ihtiyaçlar gibi faydalı bilgiler topluyor. Kiralama sürecinde gelir, bütçe, evcil hayvan, çocuk ve mevcut kira sözleşmesi gibi bilgiler de alınabiliyor. Ancak AI destekli lead scoring veya otomatik önceliklendirme sistemi bulunmuyor.

- **Otomatik Rezervasyon / Viewing Scheduling:** **Kısmi** — Kullanıcılar web sitesi üzerinden mülk görüntüleme talebinde bulunabiliyor ancak süreci yöneten konuşma tabanlı bir AI asistanı veya tamamen otomatik bir randevu planlama sistemi bulunmuyor.

- **Mesai Dışı Yanıt:** **Yok** — Web sitesi doğrudan iletişimi ve WhatsApp üzerinden güncellemeleri desteklese de, mesai saatleri dışında kullanıcı sorularını otomatik olarak cevaplayan veya lead bilgilerini toplayan AI destekli bir asistan gözlemlenmedi.

---

## **Teknik / Genel:**

- **SSR vs CSR:** **Hibrit (SSR + CSR)** — Sayfanın ilk yüklenmesinde temel içerikler server-side olarak oluşturuluyor ve önemli mülk bilgileri doğrudan HTML içerisinde bulunuyor. Daha sonra client-side JavaScript etkileşimli bileşenleri ve navigasyonu yönetiyor.

- **API çağrıları:** **Mevcut** — Web sitesi Neuron / Iceberg Digital platformu üzerinde çalışıyor ve mülk, eşleştirme ve alert altyapısını kullanıyor. Arayüzde görülen “100% MATCH” göstergesi, eşleştirme bilgilerinin ilan deneyimine entegre edildiğini gösteriyor; ancak bu sistemin arkasındaki kesin API mantığı bağımsız olarak doğrulanmadı.

- **Mobil davranış:** **Kısmi** — Web sitesi responsive yapıya sahip ve mobil cihazlarda mülk arama, uyarılar, değerleme ve iletişim özelliklerine erişim sağlıyor. Ancak detaylı filtrelerin ve formların kullanım kolaylığının gerçek bir mobil cihaz üzerinde ayrıca test edilmesi gerekiyor.

- **Genel UX:** **İyi** — Web sitesi sıcak ve insan odaklı bir marka kimliğine sahip. Gerçek ekip üyeleri, müşteri yorumları ve sektör/uyumluluk rozetleri güven duygusunu destekliyor. Temel problem güven veya marka algısı değil, mülk keşif ve ilan deneyiminin nispeten basit kalması.

- **AI Fırsatı:** **Yüksek** — Site, Neuron'un eşleştirme ve alert altyapısı sayesinde güçlü bir temel oluşturmuş durumda ancak kullanıcıya sunulan deneyimin büyük bölümü hâlâ kural tabanlı çalışıyor. En önemli fırsatlar Heads-Up sisteminin akıllı eşleştirmeye dönüştürülmesi, doğal dil aramasının eklenmesi, mülk Q&A ve özetlerinin sunulması, kişiselleştirilmiş önerilerin geliştirilmesi ve değerleme sürecinin daha şeffaf hale getirilmesi.

---

**Durum:** Yapıldı

### Ortak Bulgular / Sentez (4 tur bitince doldurulur)

- Ortak eksik AI özellikleri:
- Öne çıkan fırsatlar:
- Görüş ayrılıkları / doğrulanması gerekenler:
