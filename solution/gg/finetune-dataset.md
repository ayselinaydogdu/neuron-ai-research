# Fine-tune Örnek Veri Seti — Neuron Kernel

Dosya: [`finetune-dataset.jsonl`](finetune-dataset.jsonl) — **14 örnek**, her satır bir
eğitim örneği. Üreteç ve gerekçe: [`oneri.md`](oneri.md) §5, tam trace mantığı:
[`tool-calling-example.md`](tool-calling-example.md).

Bu, fine-tune'un **1. günden** başlaması gereken şeyin somut hâli: müşteri–asistan
diyaloğu, asistan önce **düşünür** (`thinking`), sonra **araç çağırır** (`tool_use`),
cevabını yalnızca aracın döndürdüğüne (`tool_result`) dayandırır. Fine-tune veri
setiniz ürünün kendi kullanımından doğsun — bu 14 örnek o akışın tohumu.

## Format

Anthropic Messages API sözleşmesine birebir uyar. Roller yalnızca `user` ve
`assistant`; bir tool sonucu, `tool_result` bloğu taşıyan bir `user` mesajıdır
(ayrı "tool" rolü yoktur). Her satır:

```json
{ "system": "...guardrail kuralları...", "messages": [ /* user / assistant turns */ ] }
```

Her `assistant` mesajı sırayla: `thinking` (görünür akıl yürütme) → `text` (opsiyonel)
→ bir veya daha çok `tool_use`. Paralel araç çağrıları tek `assistant` mesajında,
sonuçları tek `user` mesajında döner.

## 14 örnek ve hedeflediği gerçek bulgu

| # | Senaryo | Kapatılan gap |
|---|---|---|
| 1 | NL arama + boş sonuçta kriter gevşetme + gerçek commute | 16 Beercocks — "Couldn't find the address" |
| 2 | Ülke-farkında damga vergisi — İskoçya **LBTT** | 06 — Scottish property'de İngiliz SDLT |
| 3 | Ülke-farkında damga vergisi — Galler **LTT** + ek konut | 06 — aynı bug sınıfı, Wales |
| 4 | Kendiyle çelişen ilan → `flag_data_issue` + `handoff` | 01 Kinetic — başlık 2 yatak, material info 3 |
| 5 | Otokomple yanıltması → netleştir, uydurma | 19 Browns "Sheilds"→şirket; 01 "lin"→İskoçya |
| 6 | Değerleme = **açıklama**, tavsiye değil; comparables | 16/21 rakam ekranda, "neden" yok; 01/20 insan-only |
| 7 | Cal.com randevu — önce slot kontrol, sonra onay | 03/14 booking altyapısı zaten çalışıyor |
| 8 | Heads-Up alarmını sohbetin içinden kur | Heads-Up 21/21 tenant'ta toplanıyor |
| 9 | Bölge zekâsı — okul + sel riski (harici veri) | M4 — bölge/ulaşım zekâsı |
| 10 | Sahte kişiselleştirmeyi reddet | 02/03/04/20 — herkese "100% MATCH" |
| 11 | Londra'da yarıçap yerine **ulaşım süresi** | 04 Lloyds — radius yanlış |
| 12 | Mesai dışı asistan — emin değil → handoff + callback | 21/21 — mesai dışı yanıt yok |
| 13 | Eksik alan (EPC maliyeti null) → dürüst sınır | M2 grounding — absence ≠ negatif cevap |
| 14 | Kirada NL arama — parking must-have, alan farkını göster | genel NL arama + grounding |

## İki amaçlı kullanım

Aynı set hem **eğitim verisi** hem **regresyon altın kümesi**. Çıktı serbest metin
değil doğrulanabilir yapı olduğu için, her prompt/model değişikliğinde emitlenen
`tool_use` argümanlarını karşılaştırırsınız — prozayı değil. `oneri.md` §5'teki
"~1.000 danışman-onaylı örnek" hedefine giden yol bu 14 örnekle başlar; gerçek
danışman düzeltmeleri biriktikçe genişler.

> **Not:** `signature` alanları placeholder'dır. Gerçek eğitimde thinking blokları
> modelin döndürdüğü imzayla birlikte, değiştirilmeden loglanır.
