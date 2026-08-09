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
| 4 | Ayselin | Not done |

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

| Tur | İnceleyen | Durum |
|---|---|---|
| 1 | Görkem | Yapıldı |
| 2 | Berkay | Yapıldı |
| 3 | Yasemin | Yapılmadı |
| 4 | Ayselin | Yapılmadı |

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
