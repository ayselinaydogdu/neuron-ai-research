# 13 · keysandlee.co.uk

**URL:** https://keysandlee.co.uk/
**Group / Grup:** C

---

## English

This site is reviewed independently by 4 people across 4 rounds.

| Round | Reviewer | Status |
|---|---|---|
| 1 | Yasemin | Not done |
| 2 | Ayselin | Done |
| 3 | Görkem | Done |
| 4 | Berkay | Not done |

> Fill in only your own round block; don't edit anyone else's.
> Write short, concrete sentences (not "yes/no" — say what it is).
> What to check: ../checklist.md · Terms: ../info/ai-feature-glossary.md

### Round 1 — Yasemin

**Search:**

- Classic filter-based search is available (price, bedrooms, bathrooms, property type, etc.); no map view.
- No Natural Language Search. Queries such as "family home near schools under £400k" are interpreted as an address rather than as criteria.
- No smart suggestions / query interpretation (typo correction, synonym understanding or AI-assisted result refinement).
- No personalised ranking; SUGGESTED is the default but the options are limited to price and listing date, and the "100% MATCH" badge only reflects an exact match against the criteria entered.
- No smart narrowing when there are many results; listings are only revealed via "LOAD MORE". Saved search / automatic property alerts are available: "Heads Up Property Alerts".

**Property Detail:**

- Property descriptions are written manually, long and structured room by room; no AI-generated summary (Property Summary). Users cannot ask questions about a listing (no AI Property Q&A).
- A gallery, walkthrough video and Video Tour are available, but there is no 360° virtual tour.
- The right-hand column only lists "Latest Properties"; no personalised similar-property recommendations and no Property Comparison.
- The contact CTA sits in the right-hand column (Book a Viewing, Get in Touch); the form asks for first name, surname, phone, email, a Buy/Sell/Rent/Let selection and a message, with no chat or open question field.
- Location and nearby schools are shown via Google Maps, but no AI-assisted Area Insights or Commute Insights; the Features list includes distance details such as "0.8 miles to Clockhouse primary school", entered by the agent.
- Floor Plan and EPC are embedded in the page, but neither is explained in plain language by AI.

**Valuation:**

- An Instant Valuation and a face-to-face valuation form are available.
- The Instant Valuation runs in two steps; after asking for postcode, number of bedrooms, property type and valuation type, it requests name, email and phone, and the estimated figure is never displayed on screen.
- No AI-generated valuation explanation or personalisation; the tool runs on ValPal Network infrastructure.
- The face-to-face valuation form asks for suitable times as free text; no calendar or automated appointment scheduling.
- No Mortgage or Stamp Duty Calculator on property pages.

**Contact:**

- No AI Chat Assistant / Chatbot, either site-wide or per listing.
- Forms consist of fixed fields; the Book a Viewing form asks for name, message, email, phone, address and whether the user has a property to sell or let, while the Heads Up Alerts registration asks about moving timescale, solicitors and mortgage status — but the form does not branch based on those answers, so there is no AI Lead Qualification.
- The viewing form includes a calendar and time picker, but available slots are not shown and a notice states the selection does not confirm the viewing; no AI-assisted automated scheduling.
- Opening hours are listed on the page (weekdays 9:00–17:30, Saturday 9:00–15:30, closed Sunday), but there is no automated out-of-hours response.

**Technical/General:**

- No active chatbot or AI widget in the interface; a `whatsapp-chatbot` style definition exists in the source code, but the component does not run on the page.
- Pages are server-side rendered with Nuxt; listing content arrives with the HTML, and Fetch/XHR traffic shows a `filter` request for search results alongside Sentry and Google tracking calls.
- The layout adapts cleanly on mobile; gallery, filters and forms remain usable on narrow screens.

**Status:** Done

### Round 2 — Ayselin

## Search

- The website provides traditional property search with standard filters such as price, bedrooms, bathrooms, and property type; however, there is no map-based search view.
- Natural Language Search is not supported. Queries such as `"family home near schools under £400k"` are interpreted as address/location searches rather than being understood as user intent.
- There are no smart search or query interpretation features such as spelling correction, synonym understanding, or AI-powered result improvement.
- Personalized ranking is not available. Although `SUGGESTED` is selected by default, the other sorting options are based on price and listing date. The `100% MATCH` badge indicates how well a property matches the entered criteria rather than AI-based personalization.
- There is no AI-powered refinement when many results are returned; listings are displayed using `LOAD MORE`. Saved searches and automated property alerts are available through **Heads Up Property Alerts**.

## Property Details

- Property descriptions are manually written and generally consist of long, room-by-room paragraphs. There is no AI-generated Property Summary or Property Q&A feature for asking questions about the listing.
- A photo gallery, walkthrough videos, and Video Tour content are available, but there is no 360° virtual tour.
- The sidebar displays `Latest Properties`. Personalized similar-property recommendations and AI-powered Property Comparison are not available.
- `Book a Viewing` and `Get in Touch` CTAs remain visible in the sidebar. The contact form asks for first name, last name, phone number, email, Buy/Sell/Rent/Let selection, and a message; there is no AI chat or free-form property Q&A functionality.
- Google Maps displays the property location and nearby schools, but there are no AI-powered Area Insights or Commute Insights. Distance information such as `"0.8 miles to Clockhouse primary school"` appears in the Features section and is manually provided by the agent.
- Floor Plans and EPC information are embedded on the property page, but neither is simplified or explained in plain language by AI.

## Valuation

- Both Instant Valuation and in-person valuation services are available.
- The Instant Valuation process has two stages. Users first provide their postcode, number of bedrooms, property type, and valuation type, followed by their name, email, and phone number. The estimated value is not displayed directly on the screen.
- There is no AI-powered valuation explanation or personalized valuation analysis. The Instant Valuation tool operates using the ValPal Network infrastructure.
- The in-person valuation form asks users to provide their preferred date and time as free text. There is no calendar showing real-time availability or automated appointment scheduling.
- Mortgage Calculator and Stamp Duty Calculator are not available on the property pages.

## Contact

- There is no active AI Chat Assistant or chatbot available across the website or on individual property pages.
- The forms consist of predefined fields. The `Book a Viewing` form asks for name, message, email, phone number, address, and whether the property is for sale or rent. The Heads Up Alerts registration also collects information such as moving timeframe, solicitor status, and mortgage status. However, the form does not dynamically branch based on the answers, and there is no AI-powered Lead Qualification.
- The viewing form includes date and time fields, but actual availability is not displayed. After selecting a time, a notice indicates that the appointment will not be automatically confirmed. Therefore, AI-powered automated viewing scheduling is not available.
- Opening hours are listed as 09:00–17:30 on weekdays, 09:00–15:30 on Saturdays, and closed on Sundays. There is no automated out-of-hours response or AI-powered support system.

## Technical / General

- No active chatbot or AI widget is visible in the user interface. A `whatsapp-chatbot`-related style definition exists in the source code, but the component does not appear to be active.
- The website uses Nuxt and is server-side rendered (SSR). Property content is delivered directly within the HTML. Network traffic shows a `filter` request for search results along with Sentry and Google tracking requests.
- The mobile layout is responsive, with the gallery, filters, and forms remaining usable on smaller screens.

**Status:** Done

### Round 3 — Görkem

**Search:**
- Same filter set, no map, no natural language ("family home near schools under £400k" is treated as an address). What's new here is a **"100% MATCH" badge** on cards — and it's important not to be fooled: it only means the listing satisfies the exact filters I typed. It's a *filter-compliance* label dressed up as personalisation, not AI ranking.
- I flag it because the same badge reappears (and gets called "AI" by the vendor) on the Group-D sites — so it's worth being precise: this is the platform's built-in match indicator, and at this tenant it's plainly just exact-match.
- 49-odd results behind "LOAD MORE", "Suggested" default unexplained. Real gap is still expressing intent + a way to say "close to *my* school/work".

**Listing Detail:**
- A relative highlight: proper **walk-through video and a Video Tour** are present (no 360). Descriptions are long and structured room-by-room — good raw material, badly digestible.
- The Features list carries hand-typed distances like **"0.8 miles to Clockhouse primary school"** — exactly the commute/area info buyers want, but it's manual, unstructured and only as good as the agent who typed it. **AI opportunity:** structure this consistently (and, later, verify it against a maps API) instead of leaving it to prose.
- No AI summary, no ask-a-question; right column is "Latest Properties", not related. The room-by-room copy is the perfect thing for a summary to compress.

**Valuation:**
- Instant Valuation, two steps, **ValPal** — postcode/beds/type/valuation-type then name/email/phone, and **the figure never shows on screen**. Face-to-face form asks for suitable times as free text. No mortgage/stamp-duty calculator.
- Same instant-labelled lead capture I've now confirmed as the platform norm.

**Contact:**
- No chatbot. The viewing form actually **has a calendar and time picker**, but available slots aren't shown and a notice admits the pick **"does not confirm the viewing"** — so it looks like scheduling without being scheduling. That mismatch is its own small trust hit.
- Heads Up registration asks moving timescale / solicitor / mortgage status, but the form never branches on the answers — data collected, never used. That's a **ready-made lead-qualification input sitting idle.**

**Technical / General:**
- Nuxt SSR, but here I did see a **`filter` request** for the search results in Fetch/XHR (alongside Sentry/Google) — so this tenant *does* hit the REST search endpoint, unlike Cope & Co / Price where content came inline. Same platform, differing render/fetch config per tenant.
- Responsive; forms not submitted; no real-device test.

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
- Doğal dil araması (Natural Language Search) bulunmuyor. "family home near schools under £400k" gibi sorgular kriter olarak değil adres olarak yorumlanıyor.
- Akıllı öneri / sorgu yorumlama (yazım hatası düzeltme, eş anlamlı anlama veya AI destekli sonuç iyileştirme) bulunmuyor.
- Kişiselleştirilmiş sıralama bulunmuyor; SUGGESTED varsayılan olsa da seçenekler fiyat ve ilan tarihinden ibaret, "100% MATCH" rozeti girilen kriterlere birebir uyumu gösteriyor.
- Çok sonuçta akıllı daraltma bulunmuyor; ilanlar yalnızca "LOAD MORE" ile listeleniyor. Kayıtlı arama / otomatik ilan bildirimleri mevcut: "Heads Up Property Alerts".

**İlan Detay:**


- İlan açıklamaları elle yazılmış, uzun ve oda oda ilerleyen paragraflardan oluşuyor; AI destekli özet (Property Summary) bulunmuyor. Kullanıcı ilan hakkında soru soramıyor (AI Property Q&A yok).
- Galeri, walkthrough videosu ve Video Tour mevcut ancak 360° sanal tur bulunmuyor.
- Sağ sütunda yalnızca "Latest Properties" listeleniyor; kişiselleştirilmiş benzer ilan önerisi ve Property Comparison bulunmuyor.
- İletişim CTA'sı sağ sütunda sabit duruyor (Book a Viewing, Get in Touch); form ad, soyad, telefon, e-posta, Buy/Sell/Rent/Let seçimi ve mesaj istiyor, chat veya serbest soru alanı sunulmuyor.
- Google Maps ile konum ve çevredeki okullar gösteriliyor ancak AI destekli Area Insights veya Commute Insights sunulmuyor; Features listesinde "0.8 miles to Clockhouse primary school" gibi mesafe bilgisi yer alıyor, bu emlakçı girişi.
- Floor Plan ve EPC sayfaya gömülü olarak sunuluyor ancak hiçbiri AI tarafından sade dille açıklanmıyor.

**Değerleme:**

- Instant Valuation ve yüz yüze değerleme formu mevcut.
- Instant Valuation iki adımda ilerliyor; postcode, oda sayısı, mülk tipi ve değerleme türü sorulduktan sonra isim, e-posta ve telefon isteniyor, tahmini değer ekranda gösterilmiyor.
- AI destekli valuation açıklaması veya kişiselleştirme bulunmuyor; araç ValPal Network altyapısıyla çalışıyor.
- Yüz yüze değerleme formu uygun saatleri serbest metinle soruyor; takvim veya otomatik randevu planlama bulunmuyor.
- İlan sayfalarında Mortgage veya Stamp Duty Calculator bulunmuyor.

**İletişim:**

- Site genelinde veya ilan bazlı AI Chat Assistant / Chatbot bulunmuyor.
- Formlar sabit alanlardan oluşuyor; Book a Viewing formu ad, mesaj, e-posta, telefon, adres ve satılık/kiralık mülk durumu soruyor, Heads Up Alerts kaydında ise taşınma zamanı, avukat ve mortgage durumu gibi sorular yer alıyor ancak verilen cevaba göre form dallanmıyor, AI Lead Qualification yapılmıyor.
- Viewing formunda takvim ve saat seçimi mevcut ancak müsait saatler gösterilmiyor, seçim sonrası "bu görüşmeyi onaylamaz" uyarısı çıkıyor; AI destekli otomatik randevu planlama bulunmuyor.
- Çalışma saatleri sayfada listeleniyor (hafta içi 9:00–17:30, cumartesi 9:00–15:30, pazar kapalı) ancak mesai dışında otomatik yanıt sunulmuyor.

**Teknik/Genel:**

- Aktif bir chatbot veya AI widget arayüzde bulunmuyor; kaynak kodda `whatsapp-chatbot` stil tanımı yer alıyor ancak bileşen sayfada çalışmıyor.
- Sayfa Nuxt ile sunucu tarafında render ediliyor; ilan içeriği HTML ile birlikte geliyor, Fetch/XHR trafiğinde arama sonuçları için bir `filter` isteği ile Sentry ve Google izleme çağrıları görünüyor.
- Mobilde düzen sorunsuz uyarlanıyor; galeri, filtreler ve formlar dar ekranda kullanılabilir durumda.

**Durum:** Yapıldı

### Tur 2 — Ayselin

## Arama

- Site, fiyat, bedroom, bathroom ve property type gibi standart filtrelerle klasik arama sunuyor; ancak arama sonuçlarında harita görünümü bulunmuyor.
- Natural Language Search desteği yok. Örneğin, `"family home near schools under £400k"` gibi doğal dilde yazılan sorgular kullanıcı niyeti olarak yorumlanmak yerine adres/konum araması şeklinde değerlendiriliyor.
- Yazım hatalarını düzeltme, eş anlamlı kelimeleri algılama veya sonuçları AI ile iyileştirme gibi akıllı arama ve query interpretation özellikleri bulunmuyor.
- Kişiye özel bir sonuç sıralama sistemi mevcut değil. Varsayılan olarak `SUGGESTED` seçili olsa da diğer sıralama seçenekleri fiyat ve ilan tarihine dayanıyor. `100% MATCH` etiketi ise AI tabanlı kişiselleştirme yerine girilen arama kriterleriyle eşleşmeyi ifade ediyor.
- Çok sayıda sonuç olduğunda kullanıcıya AI destekli daraltma önerisi sunulmuyor; ilanlar `LOAD MORE` seçeneğiyle devam ediyor. Kullanıcıların kriterlerine göre otomatik bildirim almasını sağlayan **Heads Up Property Alerts** sistemi mevcut.

## İlan Detay

- İlan açıklamaları manuel olarak hazırlanmış ve genellikle uzun, oda bazında ilerleyen metinlerden oluşuyor. AI tarafından oluşturulan Property Summary bulunmuyor ve ilan hakkında doğal dilde soru sorulabilecek bir Property Q&A sistemi mevcut değil.
- Fotoğraf galerisine ek olarak walkthrough videoları ve Video Tour içerikleri sunuluyor; ancak 360° virtual tour özelliği bulunmuyor.
- Sayfanın sağ tarafındaki bölümde `Latest Properties` gösteriliyor. Kullanıcı davranışına göre kişiselleştirilmiş Similar Properties önerileri veya AI Property Comparison özelliği bulunmuyor.
- `Book a Viewing` ve `Get in Touch` CTA'ları sağ tarafta sabit şekilde yer alıyor. İletişim formunda ad, soyad, telefon, e-posta, Buy/Sell/Rent/Let seçimi ve mesaj bilgileri isteniyor; AI chat veya ilanla ilgili serbest biçimde soru sorulabilecek bir alan sunulmuyor.
- Google Maps üzerinden konum ve yakın çevredeki okullar gösteriliyor. Ancak AI destekli Area Insights veya Commute Insights bulunmuyor. Features bölümündeki `"0.8 miles to Clockhouse primary school"` gibi mesafe bilgileri AI tarafından oluşturulmuyor, emlakçı tarafından girilen bilgiler olarak sunuluyor.
- Floor Plan ve EPC içerikleri sayfaya entegre edilmiş durumda; ancak bu belgeleri AI kullanarak sade bir dille açıklayan veya özetleyen herhangi bir özellik bulunmuyor.

## Değerleme

- Hem Instant Valuation hem de yüz yüze valuation hizmeti sunuluyor.
- Instant Valuation iki aşamalı bir form üzerinden ilerliyor. Öncelikle postcode, bedroom sayısı, property type ve valuation type bilgileri alınıyor; ardından isim, e-posta ve telefon bilgileri isteniyor. Tahmini değer doğrudan ekranda gösterilmiyor.
- Valuation sürecinde AI destekli fiyat açıklaması veya kullanıcıya özel valuation analizi bulunmuyor. Instant Valuation aracı ValPal Network altyapısını kullanıyor.
- Yüz yüze valuation talebinde kullanıcıdan uygun gün/saat bilgisini serbest metin şeklinde girmesi isteniyor. Gerçek zamanlı müsaitlik gösteren bir takvim veya otomatik randevu planlama sistemi bulunmuyor.
- Property sayfalarında Mortgage Calculator veya Stamp Duty Calculator bulunmuyor.

## İletişim

- Web sitesinde genel veya property-specific olarak çalışan bir AI Chat Assistant / Chatbot bulunmuyor.
- Formlar önceden belirlenmiş alanlardan oluşuyor. `Book a Viewing` formunda ad, mesaj, e-posta, telefon, adres ve mülkün satılık/kiralık durumuyla ilgili bilgiler isteniyor. Heads Up Alerts kayıt sürecinde ise taşınma zamanı, solicitor ve mortgage durumu gibi ek bilgiler alınıyor. Ancak verilen cevaplara göre dinamik bir lead qualification süreci oluşmuyor ve AI destekli ön eleme yapılmıyor.
- Viewing formunda tarih ve saat seçimi için alan bulunuyor ancak gerçek müsaitlik bilgileri gösterilmiyor. Seçim sonrasında randevunun otomatik olarak onaylanmayacağına dair bir uyarı gösteriliyor. Dolayısıyla AI destekli otomatik viewing scheduling mevcut değil.
- Çalışma saatleri hafta içi 09:00–17:30, cumartesi 09:00–15:30 ve pazar günü kapalı olarak belirtiliyor. Mesai dışında otomatik yanıt veren bir chatbot veya AI destek sistemi bulunmuyor.

## Teknik / Genel

- Kullanıcı arayüzünde aktif bir chatbot veya AI widget bulunmuyor. Kaynak kodunda `whatsapp-chatbot` ile ilişkili bir stil tanımı bulunmasına rağmen ilgili bileşen aktif olarak kullanılmıyor.
- Site Nuxt kullanıyor ve sayfalar server-side rendering (SSR) ile oluşturuluyor. Property içerikleri doğrudan HTML içerisinde sunuluyor. Network tarafında arama sonuçları için bir `filter` isteğinin yanı sıra Sentry ve Google tracking çağrıları görülüyor.
- Mobil görünüm responsive şekilde çalışıyor. Galeri, filtreleme seçenekleri ve formlar küçük ekranlarda da kullanılabilir durumda.

**Durum:** Yapıldı

### Tur 3 — Görkem

**Arama:**
- Aynı filtre seti, harita yok, doğal dil yok ("family home near schools under £400k" adres sanılıyor). Buradaki yenilik kartlardaki **"100% MATCH" rozeti** — ve aldanmamak önemli: yalnızca ilanın yazdığım kesin filtrelere uyduğunu gösteriyor. Bu, kişiselleştirme kılığına sokulmuş bir *filtre-uyumu* etiketi, AI sıralaması değil.
- Bunu vurguluyorum çünkü aynı rozet (ve satıcının "AI" dediği hali) Grup-D sitelerinde tekrar çıkıyor — o yüzden net olmakta fayda var: bu platformun yerleşik eşleşme göstergesi ve bu tenant'ta düpedüz kesin-eşleşme.
- 49 civarı sonuç "LOAD MORE" arkasında, "Suggested" açıklanmıyor. Gerçek açık hâlâ niyeti ifade etmek + "*benim* okuluma/işime yakın" diyebilmek.

**İlan Detay:**
- Göreli bir artı: düzgün **walk-through video ve Video Tour** var (360 yok). Açıklamalar uzun ve oda-oda yapılandırılmış — iyi ham malzeme, kötü sindirilebilir.
- Features listesi **"0.8 miles to Clockhouse primary school"** gibi elle yazılmış mesafeler taşıyor — tam da alıcının istediği commute/bölge bilgisi, ama manuel, yapısız ve yazan danışman kadar iyi. **AI fırsatı:** bunu prose'a bırakmak yerine tutarlı biçimde yapılandır (ve sonra bir harita API'siyle doğrula).
- AI özet yok, soru sorma yok; sağ sütun "Latest Properties", ilişkili değil. Oda-oda metin, bir özetin sıkıştıracağı ideal içerik.

**Değerleme:**
- Instant Valuation, iki adım, **ValPal** — postcode/oda/tip/değerleme-türü sonra ad/e-posta/telefon ve **rakam asla ekranda çıkmıyor**. Yüz yüze form uygun saatleri serbest metinle soruyor. Mortgage/stamp-duty hesaplayıcı yok.
- Artık platform normu olarak doğruladığım instant-etiketli lead toplama.

**İletişim:**
- Chatbot yok. Viewing formunun aslında **takvim ve saat seçici var**, ama müsait saatler gösterilmiyor ve bir uyarı seçimin **"bu görüşmeyi onaylamaz"** olduğunu itiraf ediyor — yani planlama gibi görünüp planlama olmuyor. Bu uyumsuzluk kendi başına küçük bir güven kaybı.
- Heads Up kaydı taşınma zamanı / avukat / mortgage durumu soruyor ama form yanıtlara göre dallanmıyor — veri toplanıyor, hiç kullanılmıyor. Bu, **atıl duran hazır bir lead-qualification girdisi.**

**Teknik/Genel:**
- Nuxt SSR ama burada arama sonuçları için Fetch/XHR'de bir **`filter` isteği** gördüm (Sentry/Google yanında) — yani bu tenant REST arama ucuna *vuruyor*, içeriğin inline geldiği Cope & Co / Price'ın aksine. Aynı platform, tenant başına farklı render/fetch config.
- Responsive; form gönderilmedi; gerçek cihaz testi yok.

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
