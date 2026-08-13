# 12 · priceestateagents.uk

**URL:** https://priceestateagents.uk/
**Group / Grup:** C

---

## English

This site is reviewed independently by 4 people across 4 rounds.

| Round | Reviewer | Status |
|---|---|---|
| 1 | Yasemin | Done |
| 2 | Ayselin | Done |
| 3 | Görkem | Done |
| 4 | Berkay | Not done |

> Fill in only your own round block; don't edit anyone else's.
> Write short, concrete sentences (not "yes/no" — say what it is).
> What to check: ../checklist.md · Terms: ../info/ai-feature-glossary.md

### Round 1 — Yasemin

**Search:**

- Standard filter-based search is available (price, bedrooms, bathrooms, property type, etc.); no map view.
- Natural Language Search is not available. Queries such as "family home near schools" are interpreted as addresses rather than as criteria.
- Smart suggestion / query interpretation is partial; typos are corrected, but this is a feature of the location service, and no AI-assisted result refinement is provided.
- No intelligent narrowing for large result sets; all 58 listings are shown via "LOAD MORE" only.
- No personalised ranking; sorting options are limited to price and listing date, with Highest Price set as the default.
- Saved search / automated property alerts are available: "Heads Up Property Alerts".

**Property Detail:**

- Listing descriptions are manually written and vary in tone and level of detail from one listing to another; no AI-generated Property Summary.
- A photo gallery is available but there is no 360° virtual tour; the Floor Plan is shown on the page and the EPC is linked out to the gov.uk site, with neither explained by AI.
- The right-hand column lists only the newest properties; there are no personalised similar property recommendations, no Property Comparison and no lifestyle-oriented suggestions such as "Ideal for...".
- The contact CTA sits below the price, but the viewing form it opens requests more than ten fields; users cannot ask questions about a listing (no AI Property Q&A).
- Location is shown via Google Maps, but no school, transport or demographic data is provided; there is no AI-driven Area Insights or Commute Insights.

**Valuation:**

- Instant Valuation and a Mortgage Calculator are available.
- Instant Valuation runs in two steps; the figure is not displayed on screen and is sent by email in exchange for contact details.
- No AI-generated valuation explanation or personalisation; the tool runs on ValPal infrastructure.

**Contact:**

- No active AI Chat Assistant / Chatbot.
- The contact form requests first name, last name, phone, email, message and a Buy/Sell/Rent/Let selection; the selection does not alter the form, and no AI Lead Qualification is performed.
- Viewings and valuations are requested by typing a preferred day and time as free text; there is no calendar or AI-assisted automatic scheduling.
- Opening hours are listed on the site (weekdays 9:00–17:30, Saturday 9:00–16:00, closed Sunday), but no automated response is provided outside working hours.

**Technical/General:**

- No active chatbot or AI widget is present in the interface; a `whatsapp-chatbot` style definition appears in the source, but the component does not run on the page.
- The page is rendered server-side with Nuxt; listing content arrives with the HTML, and the Fetch/XHR traffic shows only Sentry and Google tracking requests, with no separate Neuron content API call.
- The layout adapts correctly on mobile; the gallery, tabs and forms remain usable on narrow screens.

**Status:** Done

### Round 2 — Ayselin

## Search

- A traditional search system is available with standard filters such as price, bedrooms, bathrooms, and property type; however, there is no map-based search view.
- Natural Language Search is not supported. Queries such as "family home near schools" are interpreted as address/location searches rather than being understood as user intent.
- Smart suggestions and query interpretation are partially available. Spelling mistakes can be corrected, but this appears to come from the underlying location service rather than an AI-powered property search feature.
- There is no AI-powered refinement when many results are returned. 58 listings are displayed progressively using a "LOAD MORE" option.
- Personalized result ranking is not available. Sorting options are based on price and listing date, with "Highest Price" set as the default.
- Saved searches and automatic property alerts are available through **Heads Up Property Alerts**.

## Property Details

- Property descriptions are manually written, with the writing style and level of detail varying between listings. An AI-generated Property Summary is not available.
- A photo gallery is available, but there is no 360° virtual tour. Floor Plans are provided on the property page, while EPC information is provided through a link to the gov.uk website. None of these materials are explained or summarized by AI.
- The sidebar mainly displays the newest listings. Personalized similar-property recommendations, AI-powered Property Comparison, and lifestyle-based suggestions such as "Ideal for..." are not available.
- A contact CTA is placed below the property price. The viewing form contains more than 10 fields, and there is no AI Property Q&A feature for asking questions about the listing.
- Google Maps is used to display the property location, but no school, transport, or demographic information is provided. AI-powered Area Insights and Commute Insights are not available.

## Valuation

- Instant Valuation and Mortgage Calculator services are available.
- The Instant Valuation process consists of two steps. The estimated value is not displayed directly on screen; users need to provide their contact details and receive the result by email.
- AI-powered valuation explanations or personalized valuation insights are not available.
- The valuation tool operates through the ValPal platform.

## Contact

- There is no active AI Chat Assistant or chatbot visible on the website.
- The contact form asks for first name, last name, phone number, email, message, and a Buy/Sell/Rent/Let selection. However, selecting an option does not change the form or trigger different processing, and there is no AI-powered Lead Qualification.
- Viewing and valuation requests require users to enter their preferred date and time as free text. There is no calendar showing real-time availability or AI-powered automated appointment scheduling.
- Opening hours are listed as 09:00–17:30 on weekdays, 09:00–16:00 on Saturdays, and closed on Sundays. No automated out-of-hours response or AI-powered customer support is provided.

## Technical / General

- No active chatbot or AI widget is visible in the user interface. A `whatsapp-chatbot`-related style definition is present in the source code, but the component does not appear to be active.
- The website uses Nuxt and is server-side rendered (SSR). Property content is delivered directly within the HTML.
- Fetch/XHR traffic shows Sentry and Google tracking requests, but no separate Neuron content API call was observed.
- The website is responsive on mobile devices, with the gallery, tabs, and forms remaining usable on smaller screens.

**Status:** Done

### Round 3 — Görkem

**Search:**
- Standard platform search again (price / beds / baths / type, no map). One thing genuinely annoyed me as a shopper: the default sort is **"Highest Price"**. So a first-time buyer lands on the most expensive homes first — exactly backwards for most people's budgets. That's a one-line config choice hurting real users, not an AI problem.
- "family home near schools" is read as an address, not intent. 58 results dumped behind "LOAD MORE" with no way to narrow smartly.
- **AI opportunity (platform-level):** the free-text → filter layer I keep flagging; every site in this group shares the identical filter set, so it's write-once. But before that, just flip the default sort to something sane.

**Listing Detail:**
- Hand-written descriptions whose tone/detail swing wildly from listing to listing — the quality-floor problem I've seen on every tenant. Photo gallery, floor plan on-page, EPC linked out to gov.uk; no 360 tour.
- Right column is only "newest properties" — not personalised, not related. No summary, no Q&A.
- **AI opportunity:** a summary would paper over the uneven human copy (some listings are three lines, some three paragraphs); grounded Q&A would answer the questions the thinner descriptions leave open.

**Valuation:**
- Instant Valuation runs two steps and, per the platform pattern, hands the figure over **by email in exchange for contact details** — nothing on screen. Runs on **ValPal**, same as Cope & Co.
- A **Mortgage Calculator is present** here, which not every site has — but it only spits a number, no commentary. **AI opportunity:** turn that raw number into "what this means for your budget" (an explanation layer, the same idea as AI valuation explanation).

**Contact:**
- Form takes name/phone/email/message + Buy/Sell/Rent/Let; the selection changes nothing. Viewings/valuations are booked by **typing a preferred day/time as free text** — no calendar, no availability.
- Opening hours are listed (wkdays 9–17:30, Sat 9–16, Sun closed) but nothing answers out of hours. An out-of-hours qualifier grounded in their own stock is the obvious platform-level fill.

**Technical / General:**
- Nuxt SSR; content in the HTML. Fetch/XHR shows only Sentry + Google — **no separate Neuron content API call** here either (matches Cope & Co, differs from Group D). `whatsapp-chatbot` present-but-inactive again — the dormant chatbot slot is clearly a platform-wide default.
- Responsive; forms not submitted, no real-device test.

**Status:** Done

### Round 4 — Berkay

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
| 1 | Yasemin | Yapıldı |
| 2 | Ayselin | Yapıldı |
| 3 | Görkem | Yapıldı |
| 4 | Berkay | Yapılmadı |

> Sadece kendi tur bloğunuzu doldurun; başkasının bloğunu değiştirmeyin.
> Kısa, somut cümleler yazın ("Var/Yok" değil, ne olduğunu yazın).
> Neye bakılacağı: ../checklist.md · Terimler: ../info/ai-feature-glossary.md

### Tur 1 — Yasemin

**Arama:**

- Klasik filtre tabanlı arama mevcut (price, bedrooms, bathrooms, property type vb.); harita görünümü bulunmuyor.
- Doğal dil araması (Natural Language Search) bulunmuyor. "family home near schools" gibi sorgular kriter olarak değil adres olarak yorumlanıyor.
- Akıllı öneri / sorgu yorumlama kısmi; yazım hatası düzeltiliyor ancak bu konum servisinin özelliği, AI destekli sonuç iyileştirme bulunmuyor.
- Çok sonuçta akıllı daraltma bulunmuyor; 58 ilan yalnızca "LOAD MORE" ile listeleniyor.
- Kişiselleştirilmiş sıralama bulunmuyor; seçenekler fiyat ve ilan tarihinden ibaret, varsayılan Highest Price olarak ayarlanmış.
- Kayıtlı arama / otomatik ilan bildirimleri (Alerts) mevcut: "Heads Up Property Alerts".

**İlan Detay:**

- İlan açıklamaları elle yazılmış ve ilandan ilana üslup/detay seviyesi değişiyor; AI destekli özet (Property Summary) bulunmuyor.
- Fotoğraf galerisi mevcut ancak 360° sanal tur bulunmuyor; Floor Plan sayfada yer alıyor, EPC gov.uk sitesine link olarak veriliyor, hiçbiri AI tarafından açıklanmıyor.
- Sağ sütunda yalnızca en yeni ilanlar listeleniyor; kişiselleştirilmiş benzer ilan önerisi, Property Comparison ve "Ideal for..." gibi yaşam tarzına yönelik öneriler bulunmuyor.
- İletişim CTA'sı fiyatın altında yer alıyor ancak açılan viewing formu 10'dan fazla alan istiyor; kullanıcı ilan hakkında soru soramıyor (AI Property Q&A yok).
- Google Maps ile konum gösteriliyor ancak okul, ulaşım veya demografi verisi sunulmuyor; AI destekli Area Insights ve Commute Insights bulunmuyor.

**Değerleme:**

- Instant Valuation ve Mortgage Calculator mevcut.
- Instant Valuation iki adımda ilerliyor; rakam ekranda gösterilmiyor, iletişim bilgisi karşılığında e-posta ile iletiliyor.
- AI destekli valuation açıklaması veya kişiselleştirme bulunmuyor; araç ValPal altyapısıyla çalışıyor.

**İletişim:**

- Aktif bir AI Chat Assistant / Chatbot bulunmuyor.
- İletişim formu ad, soyad, telefon, e-posta, mesaj ve Buy/Sell/Rent/Let seçimini istiyor; seçim forma göre bir değişiklik yaratmıyor, AI Lead Qualification yapılmıyor.
- Viewing ve değerleme randevuları serbest metinle uygun gün/saat yazılarak talep ediliyor; takvim veya AI destekli otomatik planlama bulunmuyor.
- Çalışma saatleri sayfada listeleniyor (hafta içi 9:00–17:30, cumartesi 9:00–16:00, pazar kapalı) ancak mesai dışında otomatik yanıt sunulmuyor.

**Teknik/Genel:**

- Aktif bir chatbot veya AI widget arayüzde bulunmuyor; kaynak kodda `whatsapp-chatbot` stil tanımı yer alıyor ancak bileşen sayfada çalışmıyor.
- Sayfa Nuxt ile sunucu tarafında render ediliyor; ilan içeriği HTML ile birlikte geliyor, Fetch/XHR trafiğinde yalnızca Sentry ve Google izleme istekleri görünüyor, ayrı bir Neuron içerik API çağrısı yapılmıyor.
- Mobilde düzen sorunsuz uyarlanıyor; galeri, sekmeler ve formlar dar ekranda kullanılabilir durumda.

**Durum:** Yapıldı

### Tur 2 — Ayselin

## Arama

- Fiyat, bedrooms, bathrooms ve property type gibi standart filtrelerle klasik arama yapılabiliyor; ancak harita tabanlı bir arama görünümü bulunmuyor.
- Natural Language Search desteklenmiyor. Örneğin, "family home near schools" gibi bir sorgu kullanıcı niyeti olarak yorumlanmak yerine adres/konum araması şeklinde ele alınıyor.
- Akıllı öneri ve sorgu yorumlama kısmen mevcut. Yazım hataları düzeltilebiliyor ancak bu davranış konum servisinden kaynaklanıyor; emlak odaklı AI destekli sonuç iyileştirmesi bulunmuyor.
- Çok sayıda sonuç olduğunda kullanıcıya AI tabanlı filtreleme veya daraltma önerisi sunulmuyor. 58 ilan "LOAD MORE" seçeneğiyle aşamalı olarak gösteriliyor.
- Sonuçların kişiselleştirilmiş şekilde sıralandığı bir sistem bulunmuyor. Fiyat ve ilan tarihi bazlı sıralama seçenekleri mevcut ve varsayılan sıralama "Highest Price" olarak ayarlanmış.
- Kayıtlı arama ve otomatik ilan bildirimleri **Heads Up Property Alerts** üzerinden sunuluyor.

## İlan Detay

- İlan açıklamaları manuel olarak hazırlanmış ve içerik ile detay seviyesi ilanlara göre farklılık gösteriyor. AI destekli Property Summary özelliği bulunmuyor.
- Fotoğraf galerisi mevcut ancak 360° sanal tur bulunmuyor. Floor Plan ilan sayfasında yer alırken EPC bilgisi gov.uk sitesine yönlendiren bir bağlantı olarak sunuluyor. Bu içeriklerin hiçbiri AI tarafından açıklanmıyor veya özetlenmiyor.
- Sağ taraftaki bölümde yalnızca en yeni ilanlar gösteriliyor. Kişiselleştirilmiş benzer ilan önerileri, AI Property Comparison ve "Ideal for..." gibi Lifestyle Matching özellikleri bulunmuyor.
- Fiyat bilgisinin altında iletişim CTA'sı yer alıyor. Viewing formu 10'dan fazla alan içeriyor ve kullanıcıların ilanla ilgili doğal dilde soru sorabileceği bir AI Property Q&A özelliği bulunmuyor.
- Google Maps üzerinden konum gösteriliyor ancak okul, ulaşım veya demografik bilgiler sunulmuyor. AI destekli Area Insights ve Commute Insights özellikleri bulunmuyor.

## Değerleme

- Instant Valuation ve Mortgage Calculator hizmetleri mevcut.
- Instant Valuation süreci iki aşamadan oluşuyor. Tahmini değer doğrudan ekranda gösterilmiyor; kullanıcı iletişim bilgilerini sağladıktan sonra sonuç e-posta üzerinden iletiliyor.
- AI destekli valuation açıklaması veya kişiselleştirilmiş değerleme özelliği bulunmuyor.
- Valuation aracı ValPal altyapısı üzerinden çalışıyor.

## İletişim

- Kullanıcı arayüzünde aktif bir AI Chat Assistant veya chatbot bulunmuyor.
- İletişim formunda ad, soyad, telefon, e-posta ve mesaj bilgilerinin yanı sıra Buy/Sell/Rent/Let seçenekleri sunuluyor. Ancak seçilen kategori forma göre farklı bir işlem veya yönlendirme oluşturmuyor; AI destekli Lead Qualification bulunmuyor.
- Viewing ve valuation taleplerinde kullanıcıdan uygun gün ve saatini serbest metin olarak belirtmesi isteniyor. Gerçek zamanlı müsaitlik gösteren bir takvim veya AI destekli otomatik randevu planlama sistemi bulunmuyor.
- Çalışma saatleri hafta içi 09:00–17:30, cumartesi 09:00–16:00 ve pazar günü kapalı olarak belirtilmiş. Mesai saatleri dışında otomatik yanıt veya AI destekli müşteri hizmeti bulunmuyor.

## Teknik / Genel

- Kullanıcı arayüzünde aktif bir chatbot veya AI widget bulunmuyor. Kaynak kodda `whatsapp-chatbot` ile ilişkili bir stil tanımı görülmesine rağmen bileşen aktif olarak çalışmıyor.
- Site Nuxt kullanıyor ve sayfalar server-side rendering (SSR) ile sunuluyor. İlan içeriği doğrudan HTML içerisinde geliyor.
- Fetch/XHR trafiğinde Sentry ve Google tracking istekleri görülüyor; ayrı bir Neuron içerik API çağrısı gözlemlenmiyor.
- Mobil görünüm responsive şekilde çalışıyor. Galeri, sekmeler ve formlar dar ekranlarda kullanılabilir durumda.

**Durum:** Yapıldı

### Tur 3 — Görkem

**Arama:**
- Yine standart platform araması (fiyat / oda / banyo / tip, harita yok). Alıcı olarak gerçekten sinir bozan bir şey: varsayılan sıralama **"Highest Price"**. Yani ilk kez ev alan biri en pahalı evlerle karşılaşıyor — çoğu bütçe için tam ters. Bu, gerçek kullanıcıyı zorlayan tek satırlık bir config tercihi, AI problemi değil.
- "family home near schools" niyet değil adres olarak okunuyor. 58 sonuç "LOAD MORE" arkasına yığılmış, akıllıca daraltma yolu yok.
- **AI fırsatı (platform seviyesi):** sürekli işaret ettiğim serbest metin → filtre katmanı; bu gruptaki her site aynı filtre setini paylaştığı için bir kez yazılır. Ama ondan önce, varsayılan sıralamayı mantıklı bir şeye çevirin.

**İlan Detay:**
- Ton/detayı ilandan ilana savrulan elle yazılmış açıklamalar — her tenant'ta gördüğüm kalite-tabanı problemi. Foto galeri, sayfada kat planı, EPC gov.uk'e link; 360 tur yok.
- Sağ sütun sadece "en yeni ilanlar" — kişiselleştirilmiş değil, ilişkili değil. Özet yok, Q&A yok.
- **AI fırsatı:** özet, dengesiz insan metnini örter (bazı ilanlar üç satır, bazıları üç paragraf); veriye dayalı Q&A ise zayıf açıklamaların bıraktığı soruları cevaplar.

**Değerleme:**
- Instant Valuation iki adım ve platform kalıbına uygun olarak rakamı **iletişim bilgisi karşılığında e-posta ile** veriyor — ekranda hiçbir şey yok. **ValPal** ile çalışıyor, Cope & Co gibi.
- Burada bir **Mortgage Calculator var**, ki her sitede yok — ama sadece rakam üretiyor, yorum yok. **AI fırsatı:** o çıplak rakamı "bunun bütçen için anlamı" haline getirmek (açıklama katmanı, AI valuation explanation ile aynı fikir).

**İletişim:**
- Form ad/telefon/e-posta/mesaj + Buy/Sell/Rent/Let alıyor; seçim hiçbir şey değiştirmiyor. Viewing/değerleme **tercih edilen gün/saati serbest metinle yazarak** ayarlanıyor — takvim yok, müsaitlik yok.
- Çalışma saatleri listeli (hafta içi 9–17:30, Cmt 9–16, Paz kapalı) ama mesai dışı hiçbir şey yanıtlamıyor. Kendi stoklarına dayalı mesai-dışı bir qualifier bariz platform seviyesi dolgusu.

**Teknik/Genel:**
- Nuxt SSR; içerik HTML'de. Fetch/XHR yalnızca Sentry + Google — burada da **ayrı Neuron içerik API çağrısı yok** (Cope & Co ile aynı, Grup D'den farklı). `whatsapp-chatbot` yine mevcut-ama-inaktif — uykudaki chatbot yuvası açıkça platform geneli varsayılan.
- Responsive; form gönderilmedi, gerçek cihaz testi yok.

**Durum:** Yapıldı

### Tur 4 — Berkay

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
