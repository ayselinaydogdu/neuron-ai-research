# 11 · copeandco.co.uk

**URL:** https://copeandco.co.uk/
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
- Classic filter-based search is available: location + radius, price, number of
bedrooms, property type. No map view. Default radius is very narrow at 0.25 miles.
- Natural Language Search is not available; input is interpreted as an address.
"big house" → places containing those words in their name.
- Smart suggestions / query understanding are partial: typos are corrected, but this
comes from the location service and suggestions are not ranked by property context.
- No smart narrowing when there are many results; 49 results are listed via "LOAD MORE".
- No recovery on zero results; no radius expansion or nearest-listing suggestion is
offered, the only exit is Heads Up registration.
- No personalised ranking. The default "Suggested" order is unexplained; other options
are price and listing date.
- Saved search / automatic property alerts are available: "Heads Up Property Alerts",
with criteria-based matching.
- Search state is not synced with the URL; switching tabs or refreshing resets the
criteria, and changing location can produce a false "0 results".
- Sold/let properties (SSTC / Let Agreed) are included in results by default.

**Listing Detail:**
- Property descriptions are hand-written and quite long; no AI-generated summary
(Property Summary).
- Users cannot ask questions about a listing (no AI Property Q&A).
- Features are listed as bullet points, but these are agent-entered fields; no
AI-powered Property Highlights.
- No lifestyle-oriented suggestions such as "Ideal for..." and no Property Comparison.
- No personalised similar-listing recommendations; the page runs straight into the footer.
- Location is shown via Google Maps, but no AI-powered Area Insights or Commute Insights.
- Documents such as EPC and Floor Plan are available but not explained by AI.
- A gallery and a Giraffe360 360° virtual tour are available, but the content is
presented raw.
- The contact CTA sits below the price, but the form that opens asks for more than 10
fields and the calendar does not show available slots.

**Valuation:**
- Instant Valuation is available but the result is not shown on screen; name, email and
phone are required to receive the figure.
- The tool does not belong to Neuron; it is provided by ValPal Network on a separate
subdomain.
- No AI-powered valuation explanation or personalised recommendation.
- No Mortgage or Stamp Duty Calculator.

**Contact:**
- A contact form and viewing request are available; the form has 7 required fields and
intent is separated only by a Buy/Sell/Rent/Let checkbox.
- No AI chatbot or AI-powered customer assistant.
- No AI-powered lead qualification; the Heads Up registration asks for income and moving
timeframe, but the screening is form-based.
- No AI-powered automatic viewing scheduling; the calendar does not show available slots.
- No out-of-hours automatic response system.

**Technical / General:**
- The `whatsapp-chatbot` and `BlendedFeeCalculator` components are loaded in the source
code but are not active on the site.
- The site is server-rendered with Nuxt (Vue) and no Neuron API calls are visible in the
Network tab.
- Filters and forms work without issues on mobile.

**Status:** Done

### Round 2 — Ayselin

## Search

- A traditional filter-based search is available, including location with radius, price, number of bedrooms, and property type. There is no map-based search view, and the default search radius is only 0.25 miles.
- Natural Language Search is not available. Search input is interpreted as an address/location query. For example, searching for "big house" returns properties with those words in their names rather than understanding the user's intent.
- Smart query interpretation is partially available: spelling mistakes are corrected, but this appears to be a feature of the underlying location service rather than a property-specific AI search capability. Suggestions are not ranked according to real estate context.
- There is no intelligent refinement when too many results are returned. For example, 49 results are simply displayed using a "LOAD MORE" option.
- No recovery mechanism is provided when there are no results. The system does not automatically expand the search radius or suggest nearby properties; the main alternative is to register for Heads Up alerts.
- Personalized result ranking is not available. The default "Suggested" sorting is not clearly explained, while other sorting options include price and listing date.
- Saved searches and automatic property alerts are available through **Heads Up Property Alerts**, which match properties based on user-defined criteria.
- Search parameters are not consistently synchronized with the URL. Switching tabs or refreshing the page can reset the selected criteria, and changing the location can sometimes result in an incorrect "0 results" state.
- Sold and let-agreed properties (SSTC / Let Agreed) are included in the search results by default.

## Property Details

- Property descriptions are manually written and often lengthy; no AI-generated Property Summary is provided.
- Users cannot ask questions about a property in natural language (AI Property Q&A is not available).
- Property features are presented as bullet points, but these are manually entered by the estate agent rather than AI-generated Property Highlights.
- Lifestyle recommendations such as "Ideal for..." and AI-powered Property Comparison are not available.
- No personalized similar-property recommendations are provided; the property page leads directly to the footer instead.
- Google Maps is used to display the property location, but AI-powered Area Insights and Commute Insights are not provided.
- EPC certificates and Floor Plans are available, but they are not explained or simplified by AI.
- Property galleries and Giraffe360 360° virtual tours are available, although the content is presented without AI-generated interpretation.
- A contact CTA is displayed below the property price, but the form contains more than 10 fields and does not provide available appointment times through a calendar.

## Valuation

- An Instant Valuation service is available, but the estimated value is not displayed directly on the results page. Users must provide their name, email address, and phone number to receive the valuation.
- The valuation tool is provided by ValPal Network through a separate subdomain rather than directly by Neuron.
- No AI-powered valuation explanation or personalized valuation recommendations are provided.
- No Mortgage Calculator or Stamp Duty Calculator is available.

## Contact

- Contact and viewing request forms are available. The contact form contains seven required fields, while the user's intent is categorized only through Buy/Sell/Rent/Let checkboxes.
- No AI chatbot or AI-powered customer assistant is available.
- AI-powered lead qualification is not available. Although the Heads Up registration form asks about income and moving timeframe, the qualification process remains form-based rather than AI-driven.
- No AI-powered viewing scheduling is available. A calendar with available appointment times is not provided.
- No automated out-of-hours response system is available.

## Technical / General

- The source code loads components named `whatsapp-chatbot` and `BlendedFeeCalculator`, but these components do not appear to be active or visible on the website.
- The website uses Nuxt (Vue) with server-side rendering (SSR).
- No Neuron API requests were observed in the Network tab during the inspection.
- The website is responsive, and filters and forms can be used smoothly on mobile devices.

**Status:** Done

### Round 3 — Görkem

**Search:**
- Same platform default I've now met eleven times, but two things bit me as a real user. The default radius is **0.25 miles** — absurdly tight; I searched a town and got a near-empty page until I widened it by hand, and nothing prompted me to. Typing "big house" was read as an address, not intent.
- Worse, it's flaky: switching tabs and coming back reset my criteria and briefly threw a false "0 results". That's a **plain state/URL-sync bug, not an AI gap** — fix it in the front-end before anything clever goes on top.
- SSTC / Let Agreed listings sit in results by default, padding the page with things I can't actually buy; there's no "hide sold" toggle.
- Sort is Suggested / price / date with "Suggested" unexplained. A natural-language layer would help here as everywhere, but the honest first fixes are the radius default, the refresh bug and a property-type-aware "still available" filter.

**Listing Detail:**
- One genuine bright spot versus my earlier groups: a **Giraffe360 360° virtual tour** is actually present — the first real immersive media I've hit across all my sites. Credit where due.
- But it sits there raw. No AI summary, no ask-a-question, and after the description the page runs straight into the footer — no "similar homes" at all. So even the most media-rich listing I've seen hits the exact same understanding ceiling.
- EPC and floor plan are embedded but unexplained. **AI opportunity:** summary + grounded Q&A would finally let a buyer skim; the 360 tour is wasted if I still can't ask "does the garden face south?".

**Valuation:**
- "Instant Valuation" is the familiar bait — it's **ValPal on a subdomain**, collects name/email/phone and shows **no number on screen**. This is the same instant-labelled lead form I documented first-hand on Town & City back in Round 1.
- No mortgage/stamp-duty calculator. The pattern holds: the platform promises "instant", delivers a call-back.

**Contact:**
- Contact form asks 7+ fields and the viewing calendar shows no real availability; intent is a single Buy/Sell/Rent/Let checkbox that changes nothing downstream.
- Telling detail: a `whatsapp-chatbot` component is **loaded in the source but switched off**. The platform ships a chatbot slot nobody has turned on — the AI hooks exist and sit dormant.

**Technical / General:**
- Nuxt SSR; interestingly the listing content arrives in the HTML and I saw **no separate Neuron content-API call** in the Network tab here (only tracking) — this differs from the Group-D sites where I later watched a REST `filter` call fire. Noting it, not overclaiming.
- `BlendedFeeCalculator` is another component present-but-inactive. Mobile layout is fine; I didn't submit any form and couldn't test touch gestures on a real device.

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

- Commonly missing AI features: Natural-language search, AI listing summaries, Property Q&A, personalised similar-listing recommendations, AI-powered area/commute insight, EPC/floor plan explanation, AI lead scoring, out-of-hours automated response.
- Standout opportunities: (1) The default search radius is absurdly tight (0.25 miles), producing near-empty results with no prompt to widen — a UX bug, but a natural-language search layer would sidestep the radius mental model entirely. (2) A genuine Giraffe360 360° virtual tour is present — the richest media found in the study so far — yet sits completely unexplained, with no AI summary or Q&A layered on top and no "similar homes" section at all after it. (3) SSTC/Let Agreed listings are included in results by default with no "hide sold" toggle — a filtering fix, but relevant context for any AI-ranking feature built later.
- Disagreements / to verify: Switching tabs and returning resets search criteria and can trigger a false "0 results" state — a state/URL-sync bug that should be fixed before any AI layer is added on top, needs confirming as reproducible. Source code loads `whatsapp-chatbot` and `BlendedFeeCalculator` components but neither is active — consistent with the pattern seen on other sites where platform-level AI hooks exist but are switched off. One reviewer (Round 3) found no separate Neuron content-API call in the Network tab (only tracking calls), differing from Group D sites where a REST `filter` call was observed — worth confirming whether this is a genuine platform/build difference or a one-off observation gap.
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
- Klasik filtre tabanlı arama mevcut: konum + yarıçap, fiyat, oda sayısı,
mülk tipi. Harita görünümü yok. Varsayılan yarıçap 0.25 mil ile çok dar.
- Doğal dil araması (Natural Language Search) bulunmuyor; girdi adres
olarak yorumlanıyor. "big house" → adında bu kelimeler geçen yerler.
- Akıllı öneri / sorgu yorumlama kısmi: yazım hatası düzeltiliyor ama bu
konum servisinin özelliği, öneriler emlak bağlamına göre sıralanmıyor.
- Çok sonuçta akıllı daraltma yok; 49 sonuç "LOAD MORE" ile listeleniyor.
- Sıfır sonuçta kurtarma yok; yarıçap genişletme veya en yakın ilan önerisi
sunulmuyor, tek çıkış Heads Up kaydı.
- Kişiselleştirilmiş sıralama yok. Varsayılan "Suggested" açıklanmıyor;
diğer seçenekler fiyat ve ilan tarihi.
- Kayıtlı arama / otomatik ilan bildirimleri (Alerts) mevcut: "Heads Up
Property Alerts", kriter tabanlı eşleştirme.
- Arama durumu URL ile senkron değil; sekme değişimi ve sayfa yenileme
kriterleri sıfırlıyor, konum değişiminde yanlış "0 results" üretebiliyor.
- Satılmış/kiralanmış ilanlar (SSTC / Let Agreed) varsayılan olarak
sonuçlara dahil ediliyor.

**İlan Detay:**
- Property açıklamaları elle yazılmış ve oldukça uzun; AI destekli özet (Property Summary) bulunmuyor.
- Kullanıcı ilan hakkında soru soramıyor (AI Property Q&A yok).
- Özellikler madde madde listeleniyor ancak bunlar emlakçının girdiği alanlar; AI destekli Property Highlights bulunmuyor.
- "Ideal for..." gibi yaşam tarzına yönelik öneriler ve Property Comparison bulunmuyor.
- Kişiselleştirilmiş benzer ilan önerisi sunulmuyor; sayfa doğrudan footer'a bağlanıyor.
- Google Maps ile konum gösteriliyor ancak AI destekli Area Insights veya Commute Insights sunulmuyor.
- EPC ve Floor Plan gibi belgeler mevcut ancak AI tarafından açıklanmıyor.
- Galeri ve Giraffe360 ile 360° sanal tur mevcut, ancak içerikler ham haliyle sunuluyor.
- İletişim CTA'sı fiyatın altında yer alıyor ancak açılan form 10'dan fazla alan istiyor ve takvimde müsait saatler gösterilmiyor.

**Değerleme:**
- Instant Valuation mevcut ancak sonuç ekranda gösterilmiyor; rakamı almak için ad, e-posta ve telefon zorunlu tutuluyor.
- Araç Neuron'a ait değil; ayrı bir subdomain üzerinde ValPal Network tarafından sağlanıyor.
- AI destekli valuation açıklaması veya kişiselleştirilmiş öneri bulunmuyor.
- Mortgage veya Stamp Duty Calculator bulunmuyor.

**İletişim:**
- İletişim formu ve viewing talebi mevcut; form 7 zorunlu alan içeriyor ve niyet yalnızca Buy/Sell/Rent/Let checkbox'ı ile ayrıştırılıyor.
- AI chatbot veya AI destekli müşteri asistanı bulunmuyor.
- AI destekli lead qualification bulunmuyor; Heads Up kaydında gelir ve taşınma zamanı soruluyor ancak eleme form tabanlı.
- AI destekli otomatik viewing planlama bulunmuyor; takvimde müsait saatler gösterilmiyor.
- Mesai dışı otomatik yanıt sistemi bulunmuyor.

**Teknik/Genel:**
- Kaynak kodda `whatsapp-chatbot` ve `BlendedFeeCalculator` bileşenleri yükleniyor ancak sitede aktif değil.
- Site Nuxt (Vue) ile sunucuda render ediliyor ve Network'te Neuron API çağrısı görünmüyor.
- Mobilde filtreler ve formlar sorunsuz kullanılabiliyor.

**Durum:** Yapıldı

### Tur 2 — Ayselin

## Arama

- Konum ve yarıçap, fiyat, oda sayısı ve mülk tipi gibi klasik filtre tabanlı arama mevcut. Harita üzerinden arama özelliği bulunmuyor ve varsayılan arama yarıçapı yalnızca 0.25 mil.
- Doğal dil araması (Natural Language Search) bulunmuyor. Arama girdileri adres/konum sorgusu olarak yorumlanıyor. Örneğin, "big house" araması kullanıcı niyetini anlamak yerine adında bu kelimeler geçen mülkleri getiriyor.
- Akıllı sorgu yorumlama kısmen mevcut: Yazım hataları düzeltiliyor ancak bunun emlak odaklı bir AI özelliğinden ziyade kullanılan konum servisinin özelliği olduğu görülüyor. Öneriler emlak bağlamına göre sıralanmıyor.
- Çok fazla sonuç olduğunda akıllı daraltma yapılmıyor. Örneğin 49 sonuç yalnızca "LOAD MORE" seçeneğiyle listeleniyor.
- Hiç sonuç bulunmadığında herhangi bir kurtarma mekanizması sunulmuyor. Sistem arama yarıçapını otomatik olarak genişletmiyor veya yakınlardaki ilanları önermiyor; temel alternatif Heads Up bildirimi oluşturmak.
- Kişiselleştirilmiş sonuç sıralaması bulunmuyor. Varsayılan "Suggested" sıralamasının nasıl belirlendiği açıklanmıyor; diğer sıralama seçenekleri fiyat ve ilan tarihine göre.
- Kayıtlı arama ve otomatik ilan bildirimleri **Heads Up Property Alerts** üzerinden mevcut. Sistem, kullanıcı tarafından belirlenen kriterlere uygun ilanları eşleştiriyor.
- Arama kriterleri URL ile tutarlı şekilde senkronize edilmiyor. Sekme değiştirme veya sayfayı yenileme seçilen kriterlerin sıfırlanmasına neden olabiliyor; konum değiştirildiğinde zaman zaman hatalı şekilde "0 results" gösterilebiliyor.
- Satılmış ve kiralanmış ilanlar (SSTC / Let Agreed) varsayılan olarak arama sonuçlarına dahil ediliyor.

## İlan Detay

- İlan açıklamaları manuel olarak hazırlanmış ve genellikle uzun; AI destekli Property Summary bulunmuyor.
- Kullanıcılar ilan hakkında doğal dilde soru soramıyor (AI Property Q&A bulunmuyor).
- İlan özellikleri madde halinde listeleniyor ancak bunlar emlak danışmanı tarafından giriliyor; AI tarafından oluşturulan Property Highlights özelliği bulunmuyor.
- "Ideal for..." gibi yaşam tarzı önerileri ve AI destekli Property Comparison bulunmuyor.
- Kişiselleştirilmiş benzer ilan önerileri sunulmuyor; ilan sayfası doğrudan footer bölümüne yöneliyor.
- Google Maps ile mülk konumu gösteriliyor ancak AI destekli Area Insights veya Commute Insights sunulmuyor.
- EPC ve Floor Plan belgeleri mevcut ancak AI tarafından açıklanmıyor veya sadeleştirilmiyor.
- İlan galerisi ve Giraffe360 360° sanal tur mevcut ancak içerikler AI tarafından yorumlanmadan sunuluyor.
- İlan fiyatının altında iletişim CTA'sı bulunuyor ancak açılan form 10'dan fazla alan içeriyor ve takvim üzerinden müsait randevu saatleri gösterilmiyor.

## Değerleme

- Instant Valuation hizmeti mevcut ancak tahmini değer sonuç ekranında doğrudan gösterilmiyor. Değeri alabilmek için ad, e-posta ve telefon bilgilerinin girilmesi gerekiyor.
- Değerleme aracı Neuron tarafından değil, ayrı bir subdomain üzerinden ValPal Network tarafından sağlanıyor.
- AI destekli valuation açıklaması veya kişiselleştirilmiş değerleme önerileri bulunmuyor.
- Mortgage Calculator veya Stamp Duty Calculator bulunmuyor.

## İletişim

- İletişim ve viewing talep formları mevcut. İletişim formunda yedi zorunlu alan bulunuyor ve kullanıcı niyeti yalnızca Buy/Sell/Rent/Let seçenekleriyle belirleniyor.
- AI chatbot veya AI destekli müşteri asistanı bulunmuyor.
- AI destekli lead qualification bulunmuyor. Heads Up kayıt formunda gelir ve taşınma zamanı gibi bilgiler sorulsa da değerlendirme süreci AI yerine form tabanlı ilerliyor.
- AI destekli viewing planlama bulunmuyor. Takvim üzerinden müsait randevu saatleri sunulmuyor.
- Mesai dışı otomatik yanıt sistemi bulunmuyor.

## Teknik / Genel

- Kaynak kodda `whatsapp-chatbot` ve `BlendedFeeCalculator` isimli bileşenler yükleniyor ancak bu bileşenler sitede aktif veya kullanıcıya görünür durumda değil.
- Site Nuxt (Vue) kullanıyor ve server-side rendering (SSR) ile sunuluyor.
- İnceleme sırasında Network sekmesinde Neuron API çağrısı gözlemlenmedi.
- Site responsive yapıda; filtreler ve formlar mobil cihazlarda sorunsuz kullanılabiliyor.

**Durum:** Yapıldı

### Tur 3 — Görkem

**Arama:**
- Artık on birinci kez gördüğüm platform varsayılanı, ama gerçek kullanıcı olarak iki şey canımı yaktı. Varsayılan yarıçap **0.25 mil** — saçma derecede dar; bir kasabayı arayınca elle genişletene kadar neredeyse boş sayfa geldi ve beni uyaran hiçbir şey yoktu. "big house" yazınca niyet değil adres olarak yorumlandı.
- Dahası kırılgan: sekme değiştirip döndüğümde kriterler sıfırlandı ve kısa süre yanlış "0 results" gösterdi. Bu **düz bir durum/URL-senkron hatası, AI açığı değil** — akıllı bir şey eklenmeden önce arayüzde düzeltilmeli.
- SSTC / Let Agreed ilanları varsayılan olarak sonuçlarda; satın alamayacağım şeylerle sayfayı dolduruyor, "satılanı gizle" seçeneği yok.
- Sıralama Suggested / fiyat / tarih, "Suggested" açıklanmıyor. Doğal dil katmanı burada da yardım eder ama dürüst ilk düzeltmeler yarıçap varsayılanı, yenileme hatası ve ev-tipine duyarlı "hâlâ müsait" filtresi.

**İlan Detay:**
- Önceki gruplarıma göre gerçek bir parlak nokta: **Giraffe360 360° sanal tur** gerçekten var — tüm sitelerim içinde çarptığım ilk gerçek immersive medya. Hakkını vereyim.
- Ama ham duruyor. AI özet yok, soru sorma yok ve açıklamadan sonra sayfa doğrudan footer'a iniyor — hiç "benzer evler" yok. Yani gördüğüm en medya-zengini ilan bile tam olarak aynı anlama tavanına çarpıyor.
- EPC ve kat planı gömülü ama açıklanmıyor. **AI fırsatı:** özet + veriye dayalı Q&A nihayet alıcının taramasını sağlar; "bahçe güneye mi bakıyor?" diye soramıyorsam 360 tur boşa gidiyor.

**Değerleme:**
- "Instant Valuation" tanıdık yem — **subdomain'de ValPal**, ad/e-posta/telefon topluyor ve **ekranda rakam göstermiyor**. Bu, Round 1'de Town & City'de bizzat belgelediğim instant-etiketli lead formunun aynısı.
- Mortgage/stamp-duty hesaplayıcı yok. Kalıp tutuyor: platform "instant" vaat ediyor, geri-arama veriyor.

**İletişim:**
- İletişim formu 7+ alan istiyor, viewing takvimi gerçek müsaitlik göstermiyor; niyet tek bir Buy/Sell/Rent/Let checkbox'ı, sonrasında hiçbir şeyi değiştirmiyor.
- Anlamlı detay: bir `whatsapp-chatbot` bileşeni **kaynakta yüklü ama kapalı**. Platform kimsenin açmadığı bir chatbot yuvası taşıyor — AI kancaları var, uykuda bekliyor.

**Teknik/Genel:**
- Nuxt SSR; ilginç şekilde ilan içeriği HTML ile geliyor ve burada Network'te **ayrı bir Neuron içerik-API çağrısı görmedim** (yalnızca tracking) — bu, sonradan REST `filter` çağrısının çalıştığını izlediğim Grup-D sitelerinden farklı. Not düşüyorum, abartmıyorum.
- `BlendedFeeCalculator` da mevcut-ama-inaktif başka bir bileşen. Mobil düzen iyi; hiçbir form göndermedim ve gerçek cihazda dokunmatik test edemedim.

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

- Ortak eksik AI özellikleri: Doğal dil arama, AI ilan özeti, Property Q&A, kişiselleştirilmiş benzer ilan önerisi, AI destekli alan/commute analizi, EPC/floor plan açıklaması, AI lead scoring, mesai dışı otomatik yanıt.
- Öne çıkan fırsatlar: (1) Varsayılan arama yarıçapı absürt derecede dar (0.25 mil), neredeyse boş sonuç veriyor ve kullanıcıyı genişletmeye yönlendiren hiçbir uyarı yok — bir UX hatası, ama doğal dil arama katmanı bu yarıçap zihinsel modelini tamamen atlayabilir. (2) Gerçek bir Giraffe360 360° sanal tur mevcut — bu çalışmada şimdiye kadar bulunan en zengin medya — ama tamamen ham halde duruyor, üstüne AI özeti veya soru-cevap yok, ve ardından hiçbir "benzer evler" bölümü de yok. (3) SSTC/Let Agreed (satılmış/kiralanmış) ilanlar varsayılan olarak sonuçlara dahil ediliyor, "satılanları gizle" seçeneği yok — bir filtreleme düzeltmesi, ama ileride kurulacak herhangi bir AI sıralama özelliği için önemli bir bağlam.
- Görüş ayrılıkları / doğrulanması gerekenler: Sekme değiştirip geri dönmek arama kriterlerini sıfırlıyor ve bazen sahte bir "0 sonuç" durumu tetikliyor — herhangi bir AI katmanı eklenmeden önce düzeltilmesi gereken bir state/URL-senkronizasyon hatası, tekrarlanabilir olduğu doğrulanmalı. Kaynak kodda `whatsapp-chatbot` ve `BlendedFeeCalculator` bileşenleri yükleniyor ama ikisi de aktif değil — diğer sitelerde görülen "platform seviyesinde AI altyapısı var ama kapalı" örüntüsüyle tutarlı. Bir incelemeci (Round 3) Network sekmesinde ayrı bir Neuron content-API çağrısı görmemiş (sadece tracking çağrıları), bu Group D sitelerinde gözlemlenen REST `filter` çağrısından farklı — bunun gerçek bir platform/build farkı mı yoksa tek seferlik bir gözlem eksikliği mi olduğu doğrulanmalı.
