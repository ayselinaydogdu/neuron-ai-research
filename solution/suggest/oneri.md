# Çözüm Önerisi — Neuron Kernel

21 sitenin gap analizinden (`sites/01..21`) çıkan ürün önerisi.
Sunum: [`sunum.html`](sunum.html) — 36 sayfa, 21'i site bazlı.

---

## 1. Teşhis: 21 ayrı sorun değil, beş kalıp × 21 kez

21 sitenin tamamı aynı Neuron / Iceberg platformunda çalışıyor. Farklı olan tek
şey tema sürümü ve hangi bileşenin açık olduğu. Bu yüzden çözüm de tenant başına
entegrasyon değil, **platform seviyesinde tek bir katman**.

| # | Kalıp | Kanıt |
|---|---|---|
| 1 | **Uykuda bileşenler** — kod yükleniyor, özellik kapalı | `Chatbot`, `InstantValuation`, `StampDutyCalculator` üçü birden 20'de; `whatsapp-chatbot` / `live-search-container` 01, 04, 11, 12, 17'de |
| 2 | **Veri toplanıyor, hiç kullanılmıyor** | Heads-Up kalifikasyon soruları 21/21 tenant'ta; `ice.js` davranış izliyor (17); Virtual Valuation fotoğraf topluyor (15) |
| 3 | **Sahte kişiselleştirme** | "100% MATCH" rozeti: 02'de 44/44, 03'te 8/8, 04'te 9/9 ilan; 20'de hiç kriter girilmemişken bile %100 |
| 4 | **Arama = adres eşleştirme** | Serbest cümle → "Couldn't find the address". Otokomple yanıltıyor: "Paultn" → Paul Tann Ltd (18), "Sheilds" → SHEilds Ltd (19), "lin" → İskoçya (01) |
| 5 | **Rakam var, gerekçe yok** | Değerleme rakamı 02, 03, 16, 19, 21'de ekranda; hiçbirinde "neden" yok. Ajanslar itiraf ediyor: "only ever a guide" (04), "just a starting point" (08), "mülkünüzün benzersizliğini hesaba katmıyor" (19) |

**Tek cümlelik bulgu:** 21 sitenin ağ trafiğinde tek bir LLM çağrısı yok — platform
kendini "AI Operating System for Estate Agents" diye imzalamasına rağmen.

---

## 2. Ürün: Neuron Kernel

Platformun altına giren tek bir zekâ çekirdeği. İlanları indeksler, mevcut Neuron
API'sini tool-calling ile çağırır, her cevabı ilanın kendi verisine dayandırır,
tenant başına config ile açılır.

| Katman | Nerede | İş |
|---|---|---|
| 1 · Ingest & Index | **Yerel** | Neuron REST → normalize → embedding → vektör DB. + statik korpus (Advice Hub, bölge rehberleri) + harici veri (Land Registry, EPC kaydı, okul/ulaşım) |
| 2 · Enrichment | **Yerel, gece batch** | Özet, highlights, EPC açıklaması, veri kalitesi denetimi, alt-text. Üretilen **saklanır**, tekrar üretilmez |
| 3 · Serving | **Bulut API** | NL arama çözümlemesi, ilan Q&A, değerleme açıklaması, mesai dışı asistan |
| 4 · Tool katmanı | Ortak | Model bilgi üretmez, araç çağırır |
| 5 · Guardrail & log | Ortak | Kaynak alana dayanma zorunluluğu + her üretimin loglanması |
| 6 · Config / feature flag | Platform | Tenant başına modül aç/kapat — **mekanizma zaten var** |

### Tool sözleşmesi

```
search_properties(filters)      → mevcut Neuron REST filter uç noktası
get_property(id)                → tek ilanın tam kaydı (cevapların kaynağı)
get_comparables(postcode,...)   → Land Registry satış verisi        [M6 yakıtı]
get_area_insights(postcode)     → okul, ulaşım, sel riski, geniş bant
get_commute(from, to, mode)     → gerçek seyahat süresi
calc_stamp_duty(price, ...)     → ÜLKE-FARKINDA: SDLT / LBTT / LTT   [06'nın hatası]
book_viewing(property_id, slot) → Cal.com (03 ve 14'te zaten çalışıyor)
create_alert(criteria)          → Heads-Up kaydı
flag_data_issue(property_id)    → danışman kutusu                    [M3]
handoff_to_agent(context)       → emin değilse insana devret (varsayılan)
```

Uçtan uca örnek akış (thinking açık, gerçek site bulgularına dayalı):
[`tool-calling-example.md`](tool-calling-example.md).

**Test edilebilirlik:** NL arama böyle kurulduğunda çıktı serbest metin değil,
doğrulanabilir JSON. 200 örneklik altın küme ile her prompt değişikliği regresyon
testinden geçirilebilir.

---

## 3. Modüller ve öncelik

| Modül | İş | Pilot tenant (kanıta dayalı) |
|---|---|---|
| **M0 · Güven onarımı** (AI değil, önkoşul) | Sahte rozet; İskoçya'da İngiliz SDLT (06); 600 km yanlış harita (06); çift footer / "Company Number: NaN" (01, 07); varsayılan "Highest Price" (12); 0,25 mil yarıçap (11) | — |
| **M1 · Doğal dil arama + sorgu anlama** | Cümle → filtre JSON. Otokomple hatasını da çözer. Boş sonuçta kriter gevşetme | **16 Beercocks** (515 ilan, 11 şube) + **14 Nicholsons** (şema telde görünür) |
| **M2 · İlan zekâsı** | Özet, highlights, Q&A, EPC/kat planı açıklaması. İlan başına bir kez batch | **20 By Design** (en iyi kaynak metin) + **08 Jacksons** (Advice Hub) |
| **M3 · Veri kalitesi & uyumluluk** | Yayın öncesi çelişki yakalama (01: başlık 2 yatak, material info 3) | **01 Kinetic** + **06 Property Connections** |
| **M4 · Bölge & ulaşım zekâsı** | Elle yazılan mesafeleri doğrulanmış veriye çevir; Londra'da yarıçap yerine ulaşım süresi | **04 Lloyds** (Londra) + **10 Roderick Thomas** (kırsal) |
| **M5 · Lead zekâsı & mesai dışı asistan** | Girdi zaten toplanıyor: skorla, önceliklendir, yönlendir. Tool-calling ile gerçek randevu | **19 Browns** (altyapı hazır) + **14 Nicholsons** (canlı WhatsApp) |
| **M6 · Değerleme açıklama katmanı** | AVM inşa etme — "neden"i inşa et. İnsan-only markalarda (01, 20) "randevu öncesi brifing" | **16** / **21** (rakam ekranda) + **15 No.86** (3 rota) |
| **M7 · Danışman içerik stüdyosu** | Tek girdi → site metni + portal ilanı + sosyal post + alt-text | **05 Property Cloud** (aynı içerik 3× elle) |

---

## 4. Yerel makine vs bulut

Ayrım: **hacimli ve tekrarlı iş yerelde, kullanıcının beklediği iş bulutta.**

**Yerelde:**
- Embedding üretimi (tüm korpus + her düzenlemede yeniden) — en yüksek hacimli iş
- Reranking
- Gece enrichment (özet, highlights, EPC, veri kalitesi) — 7B–30B sınıfı yeterli
- Vektör DB + ingestion pipeline
- **Eval harness** — 21 siteden ~200 gerçek sorgudan altın küme; en çok atlanan, en çok işe yarayan parça
- İleride LoRA fine-tune

**Bulutta:**
- NL arama çözümlemesi (küçük/hızlı model, structured output, agresif cache)
- İlan Q&A ve sohbet (kullanıcı önünde, kalite pazarlık konusu değil)
- Değerleme açıklaması (az sayıda, yüksek değerli çağrı)

**Neden canlı trafik yerelde değil:** 21 sitenin trafiğini tek makineye bağlamak tek
noktadan arıza demek; SLA veremezsiniz, bakım penceresi siteleri düşürür.
**Yerelin ikinci avantajı:** lead verisi ve danışman içeriği dışarı çıkmadan
işlenebilir — GDPR / veri ikameti tarafında somut koz.

---

## 5. Fine-tune mi, RAG mı, tool-calling mi?

| Sıra | Yaklaşım | Karar |
|---|---|---|
| 1 | **Tool-calling + structured output** | **Omurga.** NL arama zaten bir fonksiyon çağrısı problemi. Model bilgi üretmiyor, API çağırıyor. Halüsinasyon riski en düşük, test edilebilirliği en yüksek |
| 2 | **RAG / grounding** | **İkinci katman.** Her cevap ilanın kendi alanına ya da tenant'ın kendi metnine dayanacak ve kaynağı gösterecek. Kaynak yoksa cevap yok |
| 3 | **Fine-tune** | **Şimdi değil.** (a) Eksik olan bilgi değil, *erişim* — fiyat/ilan/EPC sürekli değişiyor, ağırlığa gömülen olgu bayatlar ve kaynak gösteremez. (b) Etiketli veri yok. (c) Baz modeller bu işleri zaten yapıyor |

**Fine-tune ne zaman evet:** ~1.000 danışman-onaylı örnekten sonra, iki amaçla —
**üslup** (her ajansın kendi ses tonunda ilan metni; By Design'ın "Seller's Story"
tonu ile Kinetic'in anti-kurumsal tonu aynı modelden çıkmamalı) ve **maliyet**
(büyük modelin çıktısıyla küçük modeli damıtıp yüksek hacimli işi ucuzlatmak).

→ **1. günden itibaren her üretimi ve her danışman düzeltmesini loglayın.**
Fine-tune veri setiniz ürünün kendi kullanımından doğsun.

**Model seçimi:** Gemini API makul bir başlangıç (Flash sınıfı, yüksek hacimli ucuz
iş, uzun bağlam). Ama mimariyi sağlayıcıya kilitlemeyin: tek bir `LLMProvider`
arayüzü, tüm çağrılar structured output + araç şeması üzerinden. Zor yolda güçlü
model, kolay yolda küçük model.

---

## 6. İş modeli — "ilan başına ek ücret" değerlendirmesi

**Sayaç yanlış.** Üç nedenle:

1. İlan başına ücret, teşvik etmek istediğiniz davranışı (platforma daha çok ilan
   koymak) cezalandırır.
2. Maliyet ilan sayısıyla ölçeklenmiyor. Özet/highlight ilan başına bir kez üretilir
   (kuruşluk iş); asıl maliyet Q&A ve sohbet — yani **alıcı trafiği**, danışmanın
   kontrol etmediği şey.
3. Emlakçı "AI" için değil **sonuç** için öder: daha çok viewing, daha çok market
   appraisal, daha az boşa giden lead.

### Önerilen üç katman

| Katman | Sayaç | İçerik | Gerekçe |
|---|---|---|---|
| **Core** | Lisansa dahil | NL arama, ilan özeti + highlights, veri kalitesi denetçisi | Paywall'a koymayın. Dönüşümü her tenant için yükseltir, önceden üretildiği için ucuzdur, "AI OS" iddiasını nihayet doğru kılar. Bu sattığınız şey değil, **farkınız** |
| **Pro** | **Şube / ay** | Q&A asistanı, mesai dışı asistan + gerçek randevu, lead skorlama, bölge/ulaşım zekâsı | Fiyatı *kaçırılan lead* üzerinden çerçeveleyin: mesai dışında yakalanan tek bir market appraisal aylık ücreti karşılar. 21 tenant'ın hiçbirinde mesai dışı yanıt yok |
| **Eklentiler** | **Birim başına** | İçerik Paketi (ilan başına), AI Değerleme Raporu | **"İlan başına ücret" fikrinin doğru yeri burası** — tetikleyen de faydalanan da danışman, çıktı elle tutulur |

**Maliyet kontrolü:** ön-üretim + agresif cache (ilan başına özet bir kez); şube
başına aylık Q&A kotası; kota aşımında küçük modele düş, **kesme**. 500 ilanlık bir
tenant'ın tüm korpusunu özetlemek tek seferlik birkaç dolarlık iş — değişken
maliyetin tamamı sohbette.

---

## 7. Yol haritası

| Hafta | İş |
|---|---|
| 0–4 | M0 güven onarımı + ingest/index pipeline + **eval harness** (200 sorguluk altın küme) |
| 4–10 | M1 + M2, iki pilot tenant (16, 20), tenant içi A/B |
| 10–16 | M3 + M6 + danışman onay paneli — buradan itibaren **eğitim verisi üretilmeye başlar** |
| 16–24 | M5 + M4, tool-calling ile gerçek Cal.com rezervasyonu |
| 24+ | M7 + ilk LoRA fine-tune — takvimle değil, **veri birikimiyle** tetiklenir |

**Ölçüm:** her pilotta tek birincil metrik — arama→ilan görüntüleme (M1),
ilan→enquiry (M2), mesai dışı yakalanan lead (M5), değerleme formu tamamlama (M6).

---

## 8. Riskler ve korkuluklar

- **Yanlış beyan (misdescription) en büyük hukuki risk.** Kural üçlüsü: her cevap
  ilanın kendi alanına dayanacak, alan gösterilecek, bilinmiyorsa "bilmiyorum +
  danışmana yönlendir". Mimari zorunluluk, tercih değil.
- **Yayına giden hiçbir metin danışman onayı olmadan çıkmasın** (M7). Onay ekranı
  aynı zamanda eğitim verisi toplama noktanız.
- **Değerleme dili tavsiye değil, açıklama.** "Şu fiyata satın" değil, "bu tahmini
  şu üç faktör sürüklüyor, kesinlik için yerinde inceleme gerekir".
- **Lead skorlama GDPR kapsamında otomatik karar.** Skor insanı yönlendirsin,
  kapıyı kapatmasın; düşük skorlu lead sıraya alınır, elenmez.
- **Sıra riski:** "100% MATCH" düzeltilmeden AI eklenirse, güven kırıldığında AI'ı
  da beraberinde götürür.
- **Regresyon:** eval harness olmadan prompt değişikliği sessiz bozulma demektir.

---

## 9. Tek cümle

Eksik olan 21 ayrı AI özelliği değil — hepsinin altına giren **tek bir çekirdek**.
Bir kez inşa edin, 21 kez açın; platforma katılan her yeni ajansta sıfır ek işle
tekrar.
