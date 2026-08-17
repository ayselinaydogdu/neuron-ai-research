# 09 · harrisandwood.co.uk

**URL:** https://harrisandwood.co.uk/
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

- Location-based search (city, area, or postcode) is available.
- Standard filters such as price, bedrooms, and property type are available.
- Natural Language Search is not available.
- AI-powered smart search suggestions or query interpretation are not available.
- Property Alerts are available, allowing users to receive email notifications for properties matching their search criteria.

## Property Details

- Property descriptions are detailed, but an AI-generated Property Summary is not available.
- Floor Plans, Maps, and EPC certificates are provided where available.
- AI-powered Property Highlights and Lifestyle Matching features are not available.
- AI-powered Property Comparison is not available.
- AI-powered Area Insights and Commute Insights are not provided.
- EPC certificates and Floor Plans are not summarized or explained by AI.
- Personalized AI-powered similar property recommendations were not observed.

## Valuation

- An Online Property Valuation service is available.
- Mortgage Calculator and Stamp Duty Calculator were not observed during the inspection.
- AI-powered financial analysis, valuation explanations, or personalized recommendations are not available.

## Contact

- Contact forms, telephone numbers, and email addresses are available.
- Information for multiple office locations is provided.
- No Live Chat or AI Chat Assistant is available.
- AI-powered lead qualification and automated viewing scheduling are not available.

## Technical / General

- The website has a modern and user-friendly interface.
- Core real estate features (property search, property listings, valuation, and contact services) function effectively.
- No customer-facing AI features were observed during the inspection.

**Status:** Done

### Round 2 — Görkem

**Search:**
- Same platform search. Essex (Colchester/Witham/Tendring), black branding, and an unusually strong social presence (TikTok, YouTube, Instagram). But the search itself is still the default price/beds/radius — no type, no free text, no map. The marketing energy on social doesn't translate into a smarter on-site search.

**Listing Detail:**
- Same Neuron template and same gaps. Award badges (gold winners) and heavy social proof are a homepage/brand strength, not a listing-page one — the listings are the usual bullet-features + narrative, no AI summary/Q&A.

**Valuation:**
- Instant tool (`valuation.harrisandwood.co.uk`) + book. Same gated instant pattern.

**Contact:**
- Four department phone lines + `team@` email + form; no chat, no out-of-hours. The multi-branch phone list is thorough but leaves the user with a "which number is actually mine?" decision.
- Mostly a **UX/routing fix** (a pick-your-branch selector, no AI needed). The lightweight AI version would be a postcode-based router that sends the enquiry to the right branch automatically.

**Technical / General:**
- Neuron/Iceberg, Vercel, Lifesycle.
- Trust is well covered (awards, CMP, ICO reg, TPOS) and the brand is polished and marketing-savvy. It's the most social-media-fluent tenant of my ten, which makes the plain, un-personalised search feel like the biggest missed opportunity here.

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

- **Natural Language Search — No.** `2 bed flat near Gilberd School under £200k` → **"Couldn't find the address"**. The box isn't a search engine, it's a Google Places address autocomplete. The "Find Your Dream Home" heading sets the wrong expectation.
- **Smart Suggestions / Query Interpretation — Partial.** `Colchster` returns a Colchester suggestion, but that comes from Google Places. Typo tolerance exists only in the location field; the property query itself is never interpreted.
- **Saved Search / Alerts — Yes.** "Heads Up Alerts". Criteria-based (location + radius, type, beds, price); no AI matching claimed.
- **Sorting — Unclear.** A `SUGGESTED` option exists, but nothing on the site explains what it sorts by.

Filters are extensive but entirely dropdowns and checkboxes.

---

## Property Detail

Example: `/properties/6-bedroom-house-...-co2/538132` (£900,000)

- **Property Summary (AI Summary) — No.** Description sits inside an accordion, 8–10 hand-written paragraphs.
- **Property Q&A — No.** No way to ask a question; the only channel is the 255-character message box in the viewing form.
- **Property Highlights — No.** The "Features" list is manually entered by the agent.
- **Lifestyle Matching — No.** "Ideal for first-time buyers, professionals, investors" is written into the copy by hand.
- **Property Comparison — No.**
- **Similar Property Suggestions — No.** The "Latest Properties" block at the bottom is identical for everyone — not even similarity-based.
- **Area Insights — No.** School, hospital, A12 and Park & Ride details are buried in the description text. A textbook "could be done with AI, done manually instead" case.
- **Commute Insights — No.**
- **Document Explanation (EPC / Floor Plan) — No.** Both are images only.

**Note:** Some listings are blurred as "Pre-Market Property" and require registration to view. A registration wall instead of personalisation.

---

## Valuation

- **Instant Valuation — Yes.** `/instant-valuation`, "Takes about 60 seconds". ⚠️ Result screen not verified — is the figure shown on screen or held behind an email capture?
- **AI Valuation Explanation — No (likely).** The only justification is a generic line: "We use recent local sales + property data."
- **Mortgage / Stamp Duty Calculator — No.**

The in-person valuation form is fully manual; no availability display.

---

## Contact / Lead

- **AI Chat Assistant — Partial (key finding).** No chat bubble on the page, **but** view-source shows `.whatsapp-chatbot` CSS and the `cdn.msgboxx.io` bundle loaded. The infrastructure ships with the theme; it just isn't switched on for this site.
- **Lead Qualification — Partial (not AI).** The alerts registration asks a serious set of questions: moving timeline, solicitors arranged, property to sell, how they heard about the agency. Rich data, but a rule-based form — no scoring or prioritisation.
- **Automated Booking — No.** The form lets you pick a date and time but states plainly: *"This does not confirm the viewing."* It's a request, not a real slot.
- **Out-of-Hours Response — No.** Closed Sundays; reviewed on a Sunday evening and got no automated reply, banner or chat of any kind.

---

## Technical

- **SSR.** Nuxt 3 + Vercel; content present in the HTML source.
- **API:** Very little XHR traffic (6 of 105 requests), data arrives via SSR. No visible Neuron REST API traffic.
- **Traces:** `neuron.css`, `theme7`, `window.IcebergTracker`, images served from the Lifesycle CRM CDN.

**Status:** Done

### Findings / Synthesis (filled once all 4 rounds are done)

- Commonly missing AI features: Natural-language search, AI listing summaries, Property Q&A, AI lead scoring, out-of-hours automated response, area/commute insight.
- Standout opportunities: (1) A strong social-media presence (TikTok, YouTube, Instagram) is never reflected in on-site search — the biggest gap between brand energy and product experience seen in the study. (2) Four separate department phone lines require the user to guess which to call — postcode-based automatic routing could resolve this. (3) Some listings are blurred as "Pre-Market Property" and require registration — a registration wall rather than personalisation.
- Disagreements / to verify: Whether the instant valuation result screen actually displays a figure was not verified (flagged as "not verified" in round 4) — needs live testing.

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

- Konum (şehir, bölge veya posta kodu) bazlı arama mevcut.
- Fiyat, oda sayısı ve emlak türü gibi klasik filtreler bulunuyor.
- Doğal dil araması (Natural Language Search) bulunmuyor.
- AI destekli akıllı arama önerileri veya sorgu yorumlama bulunmuyor.
- Property Alerts özelliği mevcut. Kullanıcılar belirledikleri kriterlere uygun yeni ilanlar için e-posta bildirimi alabiliyor.

## İlan Detay

- Property açıklamaları detaylı ancak AI destekli Property Summary (özet) bulunmuyor.
- Floor Plan, Map ve EPC belgeleri mevcut.
- AI destekli Property Highlights veya Lifestyle Matching özellikleri bulunmuyor.
- AI Property Comparison özelliği bulunmuyor.
- AI destekli Area Insights ve Commute Insights sunulmuyor.
- EPC ve Floor Plan belgeleri AI tarafından özetlenmiyor veya açıklanmıyor.
- AI destekli kişiselleştirilmiş benzer ilan önerileri gözlemlenmedi.

## Değerleme

- Online Property Valuation hizmeti mevcut.
- İnceleme sırasında Mortgage Calculator veya Stamp Duty Calculator gözlemlenmedi.
- AI destekli maliyet analizi, değerleme açıklamaları veya kişiselleştirilmiş finansal öneriler sunulmuyor.

## İletişim

- İletişim formu, telefon ve e-posta bilgileri mevcut.
- Birden fazla ofis bilgisi sunuluyor.
- Live Chat veya AI Chat Assistant bulunmuyor.
- AI destekli lead qualification (ön değerlendirme) ve otomatik viewing planlama bulunmuyor.

## Teknik / Genel

- Site modern ve kullanıcı dostu bir arayüze sahip.
- Temel emlak fonksiyonları (arama, ilan detayları, değerleme ve iletişim) başarılı şekilde çalışıyor.
- İnceleme sırasında kullanıcıya yönelik AI özellikleri gözlemlenmedi.

**Durum:** Yapıldı

### Tur 2 — Görkem

**Arama:**
- Aynı platform araması. Essex (Colchester/Witham/Tendring), siyah marka ve alışılmadık derecede güçlü sosyal medya varlığı (TikTok, YouTube, Instagram). Ama aramanın kendisi hâlâ varsayılan price/beds/radius — type yok, serbest metin yok, harita yok. Sosyaldeki pazarlama enerjisi site içi daha akıllı bir aramaya dönüşmüyor.

**İlan Detay:**
- Aynı Neuron şablonu ve aynı açıklar. Ödül rozetleri (gold winners) ve yoğun sosyal kanıt ana sayfa/marka gücü, ilan sayfası gücü değil — ilanlar yine bullet-features + anlatı, AI özet/Q&A yok.

**Değerleme:**
- Anlık araç (`valuation.harrisandwood.co.uk`) + randevu. Aynı kapı-tutan anlık kalıp.

**İletişim:**
- Dört departman telefon hattı + `team@` e-posta + form; chat yok, mesai dışı yok. Çok şubeli telefon listesi kapsamlı ama kullanıcıyı "hangi numara benim?" kararıyla baş başa bırakıyor.
- Çoğunlukla bir **UX/yönlendirme düzeltmesi** (şube-seç seçici, AI gerekmez). Hafif AI versiyonu, enquiry'yi otomatik doğru şubeye gönderen postcode tabanlı bir router olurdu.

**Teknik/Genel:**
- Neuron/Iceberg, Vercel, Lifesycle.
- Güven iyi kapsanmış (ödüller, CMP, ICO kaydı, TPOS) ve marka cilalı, pazarlama-zeki. On sitem içinde sosyal medyaya en hâkim tenant, bu da sade ve kişiselleştirilmemiş aramayı buradaki en büyük kaçırılmış fırsat gibi gösteriyor.

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

- **Doğal Dil Araması — Yok.** `2 bed flat near Gilberd School under £200k` → **"Couldn't find the address"**. Kutu arama motoru değil, Google Places adres autocomplete'i. Başlık "Find Your Dream Home" olduğu için kullanıcıda yanlış beklenti yaratıyor.
- **Akıllı Öneri / Sorgu Yorumlama — Kısmen var.** `Colchster` → Colchester önerisi geliyor, ama bu Google Places'ten. Yazım hatası toleransı sadece konum alanında; ilan sorgusu yorumlanmıyor.
- **Kayıtlı Arama / Alerts — Var.** "Heads Up Alerts". Kriter tabanlı (konum + yarıçap, tip, oda, fiyat); AI eşleştirme iddiası yok.
- **Sıralama — Belirsiz.** `SUGGESTED` seçeneği var ama neye göre sıraladığı hiçbir yerde yazmıyor.

Filtreler zengin ama tamamı dropdown + checkbox.

---

## İlan Detay

Örnek: `/properties/6-bedroom-house-...-co2/538132` (£900,000)

- **Property Summary (AI Özet) — Yok.** Açıklama akordeon içinde, elle yazılmış 8-10 paragraf.
- **Property Q&A — Yok.** Soru sorulacak alan yok; tek yol viewing formundaki 255 karakterlik mesaj kutusu.
- **Property Highlights — Yok.** "Features" listesi emlakçının elle girdiği maddeler.
- **Lifestyle Eşleştirme — Yok.** "Ideal for first-time buyers, professionals, investors" metne elle yazılmış.
- **Property Comparison — Yok.**
- **Benzer İlan Önerisi — Yok.** Alttaki "Latest Properties" herkese aynı; benzerlik bazlı bile değil.
- **Area Insights — Yok.** Okul, hastane, A12, Park & Ride bilgisi açıklama metnine gömülü. Klasik "AI ile yapılabilir ama elle yapılmış" örneği.
- **Commute Insights — Yok.**
- **Belge Açıklama (EPC / Floor Plan) — Yok.** İkisi de sadece görsel.

**Not:** Bazı ilanlar "Pre-Market Property" olarak bulanık; görmek için kayıt zorunlu. Kişiselleştirme yerine kayıt duvarı.

---

## Değerleme

- **Instant Valuation — Var.** `/instant-valuation`, "Takes about 60 seconds". ⚠️ Sonuç ekranı doğrulanmadı — rakam ekranda mı, e-posta arkasında mı?
- **AI Valuation Açıklaması — Yok (muhtemelen).** Tek dayanak ifadesi genel bir cümle: "We use recent local sales + property data."
- **Mortgage / Stamp Duty Calculator — Yok.**

In-person valuation formu tamamen manuel; müsaitlik gösterimi yok.

---

## İletişim / Lead

- **AI Chat Assistant — Kısmen (kritik bulgu).** Sayfada chat balonu yok, **ama** view-source'ta `.whatsapp-chatbot` CSS'i ve `cdn.msgboxx.io` bundle'ı yüklü. Altyapı temada var, bu sitede devrede değil.
- **Lead Qualification — Kısmen var (AI değil).** Alerts kaydında ciddi soru seti: taşınma zamanı, avukat durumu, satılacak mülk var mı, bizi nereden duydunuz. Veri zengin ama kural tabanlı form; skorlama/önceliklendirme yok.
- **Otomatik Randevu — Yok.** Takvim + saat seçtiriyor ama açıkça yazıyor: *"This does not confirm the viewing"*. Gerçek slot değil, talep.
- **Mesai Dışı Yanıt — Yok.** Pazar kapalı, Pazar akşamı incelendi; hiçbir otomatik yanıt/banner/chat yok.

---

## Teknik

- **SSR.** Nuxt 3 + Vercel; içerik HTML kaynağında mevcut.
- **API:** XHR trafiği çok az (6/105 request), veri SSR ile geliyor. Açık bir Neuron REST API trafiği görünmüyor.
- **İzler:** `neuron.css`, `theme7`, `window.IcebergTracker`, görseller Lifesycle CRM CDN'inden.

**Durum:** Yapıldı

### Ortak Bulgular / Sentez (4 tur bitince doldurulur)

- Ortak eksik AI özellikleri: Doğal dil arama, AI ilan özeti, Property Q&A, AI lead scoring, mesai dışı otomatik yanıt, area/commute insight.
- Öne çıkan fırsatlar: (1) Güçlü sosyal medya varlığı (TikTok, YouTube, Instagram) var ama site aramasına hiç yansımamış — marka enerjisi ile ürün deneyimi arasında en büyük kopukluk. (2) 4 farklı departman telefon hattı var, kullanıcı hangisini arayacağını kendi bulmak zorunda — postal kod bazlı otomatik yönlendirme yapılabilir. (3) Bazı ilanlar "Pre-Market" olarak bulanıklaştırılmış, kayıt gerektiriyor — kişiselleştirme yerine sadece bir kayıt duvarı.
- Görüş ayrılıkları / doğrulananlar: ✅ **Yasemin tarafından doğrulandı (canlı kontrol, Ağustos 2026):** Round 4'te "not verified" işaretlenen instant valuation sonuç ekranı canlı test edildi (`CO4 6AZ` → 13 Cordelia Drive). İki katmanlı sonuç çıktı. **(1) Rakam iletişim duvarının arkasında:** akış `#2 "Almost Finished"` adımında ad, soyad, e-posta ve telefonu **zorunlu** tutuyor ("Show My Valuation Results"). "Takes about 60 seconds. No obligation." diyen araç, sonucu göstermeden önce lead topluyor. **(2) Form son adımda kırık:** geçerli UK mobil numaraları defalarca denendi, hepsinde "Please enter a valid phone number" hatası alındı. Konsol sebebi gösteriyor: `Uncaught (in promise) SyntaxError: Failed to execute 'querySelector' on 'Document': '#2' is not a valid selector` (`DGx-v1bZ.js:4:13837`, `scrollBehavior`). URL hash'i (`#2`) CSS selector olarak kullanılıyor; CSS'te ID rakamla başlayamayacağı için hata düşüyor ve gönderim zinciri kesiliyor. **Yani instant valuation sonucu hiç gösterilmiyor — çünkü akış tamamlanamıyor.** Bu, sitedeki en yüksek maliyetli hata: değerleme sayfasının tek amacı lead toplamak, lead formu çalışmıyor.

**Ek bulgu — veri zenginleştirme var:** Adres seçilince form otomatik doluyor (4 yatak, 2 banyo, Flats/Apartments, Flat, Freehold, 132 sq mt). İncelenen üç site içinde görülen tek otomatik doldurma davranışı; ancak seçilen adres için bu kombinasyon tutarsız görünüyor, gerçek veri mi varsayılan mı belirsiz.

**Ek bulgu — form validasyonu:** Telefon alanı `+44` seçiliyken baştaki `0`'ı normalize etmiyor; UK'de yaygın olan `07...` yazımı doğrudan reddediliyor.