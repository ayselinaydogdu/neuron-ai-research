# 10 · roderickthomas.co.uk

**URL:** https://roderickthomas.co.uk/
**Group / Grup:** B

---

## English

This site is reviewed independently by 4 people across 4 rounds.

| Round | Reviewer | Status |
|---|---|---|
| 1 | Ayselin | Done |
| 2 | Görkem | Done |
| 3 | Berkay | Not done |
| 4 | Yasemin | Done |

> Fill in only your own round block; don't edit anyone else's.
> Write short, concrete sentences (not "yes/no" — say what it is).
> What to check: ../checklist.md · Terms: ../info/ai-feature-glossary.md

### Round 1 — Ayselin

## Search

- Location-based search (city, village, and postcode) is available.
- Standard filters such as price, bedrooms, and property type are available.
- Heads Up Property Alerts allow users to receive notifications based on their search criteria.
- Natural Language Search is not available.
- AI-powered smart search suggestions or query interpretation are not available.

## Property Details

- Property descriptions, photos, Floor Plans, Maps, and EPC certificates are available.
- An AI-generated Property Summary is not available.
- AI-powered Property Comparison is not available.
- AI-powered Area Insights and Commute Insights are not provided.
- EPC certificates and Floor Plans are not explained or summarized by AI.
- AI-powered Property Highlights and Lifestyle Matching are not available.
- AI-powered personalized similar property recommendations were not observed.

## Valuation

- Instant Valuation and Expert Valuation services are available.
- AI-powered property price analysis or valuation explanations are not available.
- Mortgage Calculator or AI-powered cost analysis was not observed.

## Contact

- Contact forms, telephone numbers, email addresses, and office information are available.
- No Live Chat or AI Chat Assistant is available.
- AI-powered viewing scheduling and lead qualification are not available.

## Technical / General

- The website has a modern and user-friendly interface.
- Heads Up Property Alerts allow users to receive automatic notifications based on their saved search criteria.
- Core real estate features function effectively.

**Status:** Done

### Round 2 — Görkem

**Search:**
- Same platform search under a very different, heritage brand ("50 years of experience", rural Somerset — Castle Cary, Somerton, Wells). The contrast is striking: a traditional, long-established agency running the exact same modern-but-thin Neuron search as the young challenger brands. No natural language, no map, no type filter.
- For rural/village stock this hurts more than in the towns: buyers think in villages and travel time, not radius circles, and there's no draw-on-map. **AI/area opportunity is strongest here** — village + commute insight suits an agency whose entire value proposition is deep local knowledge.

**Listing Detail:**
- Same Neuron template and gaps. A 50-year-old firm's real asset is local knowledge, yet the listing pages express none of it in structured form — same prose-description setup as everyone else, no AI summary/Q&A, thin map.

**Valuation:**
- Instant online estimate ("a starting point") + expert in-person. Same gated pattern across three regional offices.

**Contact:**
- Three regional phone numbers + contact form; no chat, no out-of-hours, no qualification.

**Technical / General:**
- Neuron/Iceberg, Vercel, S3 CDN. Google reviews, named team (Bridget/Lizzie/Harry), company reg — trust is solid and the heritage framing genuinely reassures.
- Main takeaway across the round: even the most established, local-expertise-driven brand in my ten is under-served by the platform's generic search and listing pages. The strongest tenants and the weakest all hit the same platform ceiling — which is precisely why the fixes belong in Neuron, not in any one site.

**Status:** Done

### Round 3 — Berkay

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

### Round 4 — Yasemin

## Search

- **Natural Language Search — No.** `4 bed eco home near Castle Cary under £700k` → **"Couldn't find the address"**. The box is a Google Places address autocomplete.
- **Smart Suggestions — Partial.** `Somertn` returns a Somerton suggestion, but it comes from Google Places. The property query itself is never interpreted.
- **Alerts — Yes.** The homepage makes a bold claim: *"We often match buyers with properties before they even hit the market."* No sign of AI matching in the form itself — it's criteria-based.
- **Sorting — Unclear.** The URL carries `sort=suggested`, but nothing explains what it sorts by.

---

## Property Detail

Example: `/properties/3-bedroom-house-...-blackthorn-way-somerton/521596` (£335,000)
Tabs: FEATURES / PROPERTY INFO / FLOOR PLANS / MAP

- **AI Summary — No.** The PROPERTY INFO tab holds a long, hand-written room-by-room description. There's no 2–3 point summary anywhere to let a user get the gist quickly; the only alternative is reading the whole thing.
- **Q&A — No.** There's no field to ask a question about the listing. The only route is the 255-character message box inside the "BOOK A VIEWING" modal — meaning you have to fill in a booking form to ask a question, and the answer only comes back through a human.
- **Highlights — No.** The items in the FEATURES tab are a list the agent typed in, not standout features extracted from the description by AI. Details mentioned in the text but left off the list stay invisible to the user.
- **Lifestyle Matching — No.** The "who it suits" information appears as a sentence inside the copy (*"an excellent opportunity for those seeking a comfortable family home"*), not as structured matching or a filter.
- **Comparison — No.** No selection box or "compare" button on the listing cards; comparing two properties means opening two tabs and doing it by eye.
- **Similar Property Suggestions — No.** There is **no** similar-listings block at the bottom of the page; "Register to Property Alerts" and "Why Choose Us" CTAs sit there instead. When a user likes a listing, there's nowhere to go but off the site.
- **Area Insights — No.** No neighbourhood data at all — schools, crime, demographics. The MAP tab is a plain map showing the location.
- **Commute Insights — No.** The clearest manual example is here: the description opens with a hand-written distance block (*"Glastonbury 8 miles… Castle Cary 10 miles (Paddington 1.5 hours)… A303 3.5 miles (Distances & times approximate)"*). Data AI could generate automatically and keep current is typed out for every single listing — and the "approximate" note disclaims responsibility for it anyway.
- **Document Explanation — No.** The FLOOR PLANS tab is images only; reading the measurements is left to the user. **There isn't even an EPC tab** — the energy rating appears as a single line in the Features text.

**Note:** PROPERTY INFO does carry structured, icon-labelled data (type, tenure, council tax band, water/sewerage). The data sits there machine-readable, with no AI layer built on top of it.

---

## Valuation

- **Instant Valuation — Yes, but outsourced.** `valuation.roderickthomas.co.uk` is a separate subdomain, **"Powered by ValPal Network"**, with a design disconnected from the main site. Its own copy lowers expectations: *"Our algorithm tries to be as accurate as possible, yet we know this isn't always possible. For a more accurate valuation please call one of our experts."*
- **AI Valuation Explanation — No.** The screen says "algorithm" but never states what data it looks at, which comparable sales it uses, or how reliable the result is. The user can't interrogate the figure — only accept it and get pushed toward a phone call.
- **Mortgage / Stamp Duty Calculator — No.** Checked the listing page, `/blogs`, the footer and the menu; there's no calculator. Notably, the blog carries posts on rate cuts and the mortgage market — the interest is there, the tool isn't.

**Expert valuation:** For dates, just an empty free-text box — not even a calendar.

---

## Contact / Lead

- **AI Chat — No.** No chat bubble on any page; view-source still contains the `.whatsapp-chatbot` CSS, but no provider is wired up. The component ships with the theme and was never switched on.
- **Lead Qualification — Partial (not AI).** Every question Harris + Wood asks is here, plus "Do you require a mortgage in order to buy?". Even richer data, still nothing processing it.
- **Automated Booking — No.** The modal lets you pick a date and time, but states plainly underneath: *"This does not confirm the viewing."* No real availability is shown; the selection is passed on as a request.
- **Out-of-Hours Response — No.** Reviewed at night; no automated reply, banner or "we're closed" notice appeared. On top of that, **opening hours aren't published anywhere** — so the user can't even tell when to expect a response.

On the contact form the user picks the branch themselves (Castle Cary / Somerton / Wells); there's no automatic routing.

---

## Technical

- **SSR.** Nuxt 3 + Vercel, content present in the HTML source.
- **Theme `theme8`** (Harris + Wood runs `theme7`). Same `neuron.css`, same `IcebergTracker`.
- **API:** 6 of 84 requests are XHR. **Identical file names and the same UUID** as Harris + Wood — both sites run the same platform build.

**Status:** Done

### Findings / Synthesis (filled once all 4 rounds are done)

- Commonly missing AI features: Natural-language search, AI listing summaries, Property Q&A, AI lead scoring, out-of-hours automated response; there isn't even an EPC tab (energy rating appears as a single line of text).
- Standout opportunities: (1) A 50-year, local-knowledge-driven brand positioning exists, yet the site offers zero structured area data — the biggest gap between brand promise and product experience found in the study. (2) Commute/distance information is hand-typed into every listing ("Glastonbury 8 miles… Paddington 1.5 hours") — the clearest, most automatable example found. (3) The blog covers mortgage rate content but there's no calculator on the site.
- Disagreements / to verify: Confirmed technically to share the same platform build as site 09 (Harris & Wood) — identical file names and the same UUID — same underlying infrastructure, differences are branding-level only.

---

## Türkçe

Bu siteyi 4 tur boyunca 4 farklı kişi bağımsız inceler.

| Tur | İnceleyen | Durum |
|---|---|---|
| 1 | Ayselin | Yapıldı |
| 2 | Görkem | Yapıldı |
| 3 | Berkay | Yapılmadı |
| 4 | Yasemin | Yapıldı |

> Sadece kendi tur bloğunuzu doldurun; başkasının bloğunu değiştirmeyin.
> Kısa, somut cümleler yazın ("Var/Yok" değil, ne olduğunu yazın).
> Neye bakılacağı: ../checklist.md · Terimler: ../info/ai-feature-glossary.md

### Tur 1 — Ayselin

## Arama

- Konum (şehir, köy ve postcode) bazlı arama mevcut.
- Fiyat, oda sayısı ve property type filtreleri bulunuyor.
- Heads Up Property Alerts ile kullanıcılar arama kriterlerine göre ilan bildirimi oluşturabiliyor.
- Doğal dil araması bulunmuyor.
- AI destekli akıllı arama önerileri veya sorgu yorumlama bulunmuyor.

## İlan Detay

- Property açıklamaları, fotoğraflar, Floor Plan, Map ve EPC belgeleri mevcut.
- AI destekli Property Summary bulunmuyor.
- AI Property Comparison özelliği bulunmuyor.
- AI destekli Area Insights ve Commute Insights sunulmuyor.
- EPC ve Floor Plan belgeleri AI tarafından açıklanmıyor.
- AI destekli Property Highlights veya Lifestyle Matching bulunmuyor.
- AI destekli kişiselleştirilmiş benzer ilan önerileri gözlemlenmedi.

## Değerleme

- Instant Valuation ve Expert Valuation hizmetleri mevcut.
- AI destekli fiyat analizi veya valuation açıklamaları bulunmuyor.
- Mortgage Calculator veya AI destekli maliyet analizi gözlemlenmedi.

## İletişim

- İletişim formu, telefon, e-posta ve ofis bilgileri mevcut.
- Live Chat veya AI Chat Assistant bulunmuyor.
- AI destekli randevu planlama ve lead qualification sistemi bulunmuyor.

## Teknik / Genel

- Modern ve kullanıcı dostu bir arayüze sahip.
- Heads Up Property Alerts ile kullanıcılar arama kriterlerine göre otomatik ilan bildirimi alabiliyor.
- Temel emlak fonksiyonları başarılı şekilde çalışıyor.

**Durum:** Yapıldı

### Tur 2 — Görkem

**Arama:**
- Aynı platform araması, ama çok farklı bir köklü marka altında ("50 yıllık deneyim", kırsal Somerset — Castle Cary, Somerton, Wells). Kontrast çarpıcı: geleneksel, uzun soluklu bir acente, genç meydan-okuyucu markalarla birebir aynı modern-ama-zayıf Neuron aramasını çalıştırıyor. Doğal dil yok, harita yok, type filtresi yok.
- Kırsal/köy stoğu için bu, kasabalardan daha çok canını yakıyor: alıcılar yarıçap daireleriyle değil köyler ve seyahat süresiyle düşünüyor ve haritaya-çizme yok. **AI/bölge fırsatı burada en güçlüsü** — köy + commute içgörüsü, tüm değer önermesi derin yerel bilgi olan bir acenteye yakışır.

**İlan Detay:**
- Aynı Neuron şablonu ve açıkları. 50 yıllık bir firmanın gerçek varlığı yerel bilgi, ama ilan sayfaları bunun hiçbirini yapılandırılmış biçimde ifade etmiyor — herkesle aynı düz-yazı-açıklama düzeni, AI özet/Q&A yok, zayıf harita.

**Değerleme:**
- Anlık online tahmin ("bir başlangıç noktası") + uzman yüz yüze. Üç bölgesel ofiste aynı kapı-tutan kalıp.

**İletişim:**
- Üç bölgesel telefon numarası + iletişim formu; chat yok, mesai dışı yok, kalifikasyon yok.

**Teknik/Genel:**
- Neuron/Iceberg, Vercel, S3 CDN. Google yorumları, isimli ekip (Bridget/Lizzie/Harry), şirket kaydı — güven sağlam ve köklülük çerçevesi gerçekten güven veriyor.
- Turun ana çıkarımı: on sitem içindeki en köklü, yerel-uzmanlığa dayalı marka bile platformun jenerik arama ve ilan sayfalarınca yetersiz hizmet alıyor. En güçlü tenant'lar da en zayıflar da aynı platform tavanına çarpıyor — düzeltmelerin neden herhangi bir sitede değil, Neuron'da olması gerektiğinin tam nedeni bu.

**Durum:** Yapıldı

### Tur 3 — Berkay

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

### Tur 4 — Yasemin

## Arama

- **Doğal Dil Araması — Yok.** `4 bed eco home near Castle Cary under £700k` → **"Couldn't find the address"**. Kutu Google Places adres autocomplete'i.
- **Akıllı Öneri — Kısmen var.** `Somertn` → Somerton önerisi geliyor, ama Google Places kaynaklı. İlan sorgusu yorumlanmıyor.
- **Alerts — Var.** Ana sayfa iddialı: *"We often match buyers with properties before they even hit the market."* Formda AI eşleştirmeye dair iz yok, kriter tabanlı.
- **Sıralama — Belirsiz.** URL'de `sort=suggested`, neye göre sıraladığı açıklanmıyor.

---

## İlan Detay

Örnek: `/properties/3-bedroom-house-...-blackthorn-way-somerton/521596` (£335,000)
Sekmeler: FEATURES / PROPERTY INFO / FLOOR PLANS / MAP

- **AI Özet — Yok.** PROPERTY INFO sekmesinde oda oda ilerleyen, elle yazılmış uzun bir metin var. Kullanıcının hızlı fikir edinmesini sağlayacak 2-3 maddelik bir özet hiçbir yerde yok; tek alternatif metnin tamamını okumak.
- **Q&A — Yok.** İlan hakkında soru sorulabilecek bir alan yok. Tek yol "BOOK A VIEWING" modalındaki 255 karakterlik serbest mesaj kutusu — yani soru sormak için randevu formu doldurmak gerekiyor, cevap da ancak insan dönüşüyle geliyor.
- **Highlights — Yok.** FEATURES sekmesindeki maddeler emlakçının elle girdiği liste; ilan metninden AI ile çıkarılmış öne çıkan özellikler değil. Metinde geçen ama listeye girmemiş detaylar kullanıcıya görünmüyor.
- **Lifestyle Eşleştirme — Yok.** "Kimin için uygun" bilgisi metnin içinde cümle olarak geçiyor (*"an excellent opportunity for those seeking a comfortable family home"*), yapılandırılmış bir eşleştirme veya filtre olarak değil.
- **Comparison — Yok.** İlan kartlarında seçim kutusu veya "compare" butonu yok; iki ilanı karşılaştırmak için kullanıcının iki sekme açıp kendi gözüyle kıyaslaması gerekiyor.
- **Benzer İlan Önerisi — Yok.** Sayfa altında benzer ilan bloğu **hiç yok**; yerine "Register to Property Alerts" ve "Why Choose Us" CTA'ları konmuş. Kullanıcı bir ilanı beğendiğinde siteden çıkmak dışında gidecek yeri yok.
- **Area Insights — Yok.** Okul, suç, demografi gibi mahalle verisi hiç yok. MAP sekmesi sadece konumu gösteren düz bir harita.
- **Commute Insights — Yok.** En net manuel örnek burada: açıklamanın başında elle yazılmış bir mesafe bloğu var (*"Glastonbury 8 miles… Castle Cary 10 miles (Paddington 1.5 hours)… A303 3.5 miles (Distances & times approximate)"*). AI'ın otomatik ve güncel üretebileceği veri, her ilan için tek tek yazılıyor — üstelik "approximate" notuyla sorumluluk da reddediliyor.
- **Belge Açıklama — Yok.** FLOOR PLANS sekmesi sadece görsel; ölçüleri okumak kullanıcıya kalmış. **EPC için sekme bile yok**, enerji sınıfı sadece Features metninde bir satır olarak geçiyor.

**Not:** PROPERTY INFO'da ikonlu yapılandırılmış veri var (tip, tenure, council tax band, su/kanalizasyon). Veri makine-okunabilir halde duruyor, üstüne hiçbir AI katmanı kurulmamış.

---

## Değerleme

- **Instant Valuation — Var, ama dışarıya taşeronlanmış.** `valuation.roderickthomas.co.uk` ayrı subdomain, **"Powered by ValPal Network"**. Ana siteden kopuk tasarım. Kendi metni beklentiyi düşürüyor: *"Our algorithm tries to be as accurate as possible, yet we know this isn't always possible. For a more accurate valuation please call one of our experts."*
- **AI Valuation Açıklaması — Yok.** Ekranda "algorithm" deniyor ama hangi verilere baktığı, hangi benzer satışların kullanıldığı, sonucun ne kadar güvenilir olduğu hiçbir yerde belirtilmiyor. Kullanıcı çıkan rakamı sorgulayamıyor, sadece kabul edip telefona yönlendiriliyor.
- **Mortgage / Stamp Duty Calculator — Yok.** İlan sayfası, `/blogs`, footer ve menü tarandı; hesaplayıcı yok. İlginç olan, blogda faiz indirimi ve mortgage piyasası üzerine yazılar olması — konuya ilgi var, araç yok.

**Expert valuation:** Tarih için sadece boş bir serbest metin kutusu — takvim bile yok.

---

## İletişim / Lead

- **AI Chat — Yok.** Hiçbir sayfada chat balonu yok; view-source'ta `.whatsapp-chatbot` CSS'i duruyor ama sağlayıcı bağlı değil. Yani bileşen tema ile geliyor, açılmamış.
- **Lead Qualification — Kısmen var (AI değil).** Harris + Wood'daki soruların hepsi var, artı "Do you require a mortgage in order to buy?". Veri daha da zengin, işleyen AI yok.
- **Otomatik Randevu — Yok.** Modal takvim ve saat seçtiriyor ama altında açıkça yazıyor: *"This does not confirm the viewing."* Gerçek müsaitlik gösterilmiyor, seçim sadece bir talep olarak iletiliyor.
- **Mesai Dışı Yanıt — Yok.** Gece incelendi, hiçbir otomatik yanıt, banner veya "şu an kapalıyız" uyarısı çıkmadı. Üstelik **çalışma saatleri hiçbir yerde yayınlanmamış** — kullanıcı ne zaman dönüş alacağını da bilemiyor.

Contact formunda şubeyi (Castle Cary / Somerton / Wells) kullanıcı seçiyor; otomatik yönlendirme yok.

---

## Teknik

- **SSR.** Nuxt 3 + Vercel, içerik HTML kaynağında.
- **Tema `theme8`** (Harris + Wood `theme7`). Aynı `neuron.css`, aynı `IcebergTracker`.
- **API:** 6/84 request XHR. Harris + Wood'la **birebir aynı dosya adları ve aynı UUID** — iki site de aynı platform build'i.

**Durum:** Yapıldı

### Ortak Bulgular / Sentez (4 tur bitince doldurulur)

- Ortak eksik AI özellikleri: Doğal dil arama, AI ilan özeti, Property Q&A, AI lead scoring, mesai dışı otomatik yanıt; EPC sekmesi bile yok (sadece Features metninde tek satır).
- Öne çıkan fırsatlar: (1) 50 yıllık, yerel bilgiye dayalı marka konumlandırması var ama site sıfır yapılandırılmış alan verisi sunuyor — marka vaadi ile ürün deneyimi arasındaki en büyük uçurum bu sitede görüldü. (2) Commute/mesafe bilgisi ilanlarda elle yazılıyor ("Glastonbury 8 miles… Paddington 1.5 hours") — otomatikleştirmeye en uygun, en açık örnek. (3) Blog'da mortgage/faiz oranı içeriği var ama hesap makinesi yok.
- Görüş ayrılıkları / doğrulananlar: ✅ **Yasemin tarafından doğrulandı (canlı kontrol, 17 Ağustos 2026):** 09 · Harris + Wood ile aynı platform build'ini paylaştığı **kesin olarak doğrulandı.** Her iki sitenin HTML `<head>` bölümündeki Sentry release hash'i birebir aynı: `fa3a1c21fbc31083c37fb3f41928c0c10c23476f`. Release hash doğrudan kaynak kodun commit SHA'sı olduğu için bu, dosya adı/UUID benzerliğinden çok daha güçlü bir kanıt — iki site aynı git commit'inden deploy edilmiş. Ayrıca her ikisi de aynı Sentry projesine rapor ediyor (`org_id=4511222927065088`, `public_key=275a5eb4f79d0e2b5c93a588858cfc0e`), yani ayrı siteler değil tek bir uygulamanın örnekleri.

**Ek bulgu — kademeli deploy:** 08 · Jacksons farklı release hash'te (`9ce27bec7a14fa785eb9fd8d36c531fc71808b27`) ve farklı tema (`theme3`). Yani Neuron tüm tenant'ları aynı anda güncellemiyor; site grupları farklı sürümlerde kalabiliyor. Bu, ekipte daha önce tartışılan "hata bazı sitelerde var bazılarında yok" gözlemlerinin muhtemel açıklaması: sorun tenant'a özgü değil, o tenant'ın hangi build'de olduğuna bağlı. **Not: release hash zamanla değişir, bu ölçüm 17 Ağustos 2026 tarihlidir.**