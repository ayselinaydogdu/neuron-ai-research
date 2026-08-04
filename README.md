# Neuron AI Özellik Araştırması

Bu klasör, Neuron platformu için AI özellik fırsatlarını araştırma görevimizin
saha çalışması materyallerini içerir.

## Amaç

21 canlı Neuron web sitesini inceleyip mevcut UX'i (arama, ilan detay,
değerleme, iletişim) not almak. Bu notlar, AI özellik önerileri raporunun
"mevcut durum / gap analizi" bölümünün ham verisi olacak.

## Dosyalar

| Dosya | İçerik |
|---|---|
| `kontrol-listesi.md` | Her kategori için nelere bakılacağını gösteren referans checklist |
| `site-atamalari.md` | 21 sitenin 4 kişiye bölüşümü + çapraz kontrol ataması |
| `site-incelemeleri.md` | Asıl doldurulacak bulgu dosyası — hem bireysel notlar hem çapraz kontrol notları |

## Süreç — 2 aşama

### 1. Bireysel inceleme
1. `site-atamalari.md` dosyasında size atanmış siteleri bulun.
2. Her siteyi ziyaret edin: arama yapın, bir ilana girin, değerleme formunu
   deneyin, iletişim formuna bakın. Neye bakacağınız için `kontrol-listesi.md`'ye
   bakın.
3. `site-incelemeleri.md` dosyasında kendi sitelerinizin "Notlar" kısmını
   doldurun (kısa, somut cümleler).
4. Bitirince ilgili sitenin "Durum" satırını `Tamamlandı` yapın, commit+push
   edin.

### 2. Çapraz kontrol
5. Herkes bireysel incelemesini bitirince, ekip içinde sırayla/rastgele kim
   kimin sitelerine bakacağı belirlenir ve `site-atamalari.md`'deki tabloya
   yazılır (kimse kendi incelediğine bakmaz).
6. Size atanan çapraz kontrol sitelerini tekrar ziyaret edin, arkadaşınızın
   notlarını okuyup eksik/yanlış bir şey var mı kontrol edin.
7. `site-incelemeleri.md`'de ilgili sitenin "Çapraz Kontrol Notları" kısmını
   doldurun, "Durum"u `Çapraz Kontrol Tamamlandı` yapın, commit+push edin.

## Kurallar

- Uzun paragraf yazmayın — kısa, somut gözlemler.
- "Var / Yok" değil, ne olduğunu yazın (örn. "Sadece dropdown filtre, doğal
  dil arama yok" — "Yok" tek başına yeterli değil).
- Sadece kendi bölümünüzü (kendi notlarınız veya size atanan çapraz kontrol)
  düzenleyin, başkasının yazdığını silmeyin/değiştirmeyin.
- Küçük, sık commit'ler tercih edilir (örn. "Kişi 2: site 6 notları eklendi").
