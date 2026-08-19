# Neuron AI Katmanı — Mimari ve Ürün Önerisi

**Hazırlayan:** Ayselin
**Kaynak:** 21 Neuron sitesinin 4 tur bağımsız incelemesi + canlı doğrulama
**Amaç:** "Neuron AI Özellikleri Araştırması" raporundaki fikirlerin nasıl hayata geçirilebileceğine dair teknik/ürünsel bir öneri

---

## 1. Teşhis — Neden Tek Tek Değil, Tek Katman

21 sitenin incelemesinde ortaya çıkan tablo şu: bu 21 site aslında **21 ayrı sorun değil, aynı platformun (Neuron/Iceberg) üzerinde 21 kez tekrarlanan aynı birkaç kalıp.** Farklı olan sadece tema sürümü ve hangi bileşenin o tenant için açık/kapalı olduğu.

| # | Kalıp | Kanıt (canlı doğrulanmış) |
|---|---|---|
| 1 | **Kapalı bileşenler** — kod var, özellik pasif | `.whatsapp-chatbot`, `.live-search-container` sınıfları 5+ sitede kaynak kodunda bulundu ama hiçbirinde aktif değil |
| 2 | **Veri toplanıyor, işlenmiyor** | Heads-Up Alerts formu 21/21 sitede zengin veri topluyor (taşınma zamanı, mortgage durumu) ama hiçbiri sıralama/önceliklendirmeye gitmiyor |
| 3 | **Sahte kişiselleştirme** | "100% MATCH" rozeti — kayıtsız, hiç kriter girmemiş kullanıcıya bile her ilanda %100 gösteriliyor (birden fazla sitede doğrulandı) |
| 4 | **Arama = sadece adres eşleştirme** | Serbest cümle → "Couldn't find the address" hatası; otomatik tamamlama yanlış yönlendiriyor (örn. "Paultn" → "Paul Tann Ltd") |
| 5 | **Rakam var, gerekçe yok** | Değerleme akışlarının çoğunda bir sayı üretiliyor ama hiçbir yerde "neden bu rakam" açıklaması yok; bazı acenteler kendi aracına güvenmediğini açıkça yazıyor |

**Tek cümlelik bulgu:** İncelenen sitelerin ağ trafiğinde hiçbir AI/LLM servis çağrısı tespit edilmedi — platform kendini "AI Operating System for Estate Agents" olarak tanıtmasına rağmen.

**Bunun sonucu:** Çözüm de tenant başına ayrı entegrasyon değil, **platform seviyesinde tek bir katman** olmalı — bir kez inşa edilip config ile açılıp kapatılabilmeli.

---

## 2. Önerilen Yaklaşım — Genel Hatlarıyla

Aşağıdaki öneri üç katmanlı düşünülebilir:

1. **Veri hazırlığı** — ilanların ve platform içeriğinin AI'nın anlayabileceği/kullanabileceği hale getirilmesi
2. **Servis katmanı** — kullanıcının gerçek zamanlı etkileşime girdiği kısım (arama, soru-cevap, değerleme açıklaması)
3. **Kontrol katmanı** — her AI çıktısının gerçek veriye dayanmasını zorunlu kılan, agent onayı ve loglama içeren güvenlik ağı

Bu üç katman, tek bir yerde inşa edilip her acente sitesinde ayrı ayrı **açılıp kapatılabilir** — böylece platformun mevcut "her tenant kendi teması/config'i" mantığıyla uyumlu çalışır.

---

## 3. Modül Bazlı Öneri

Aşağıdaki modüller, ana rapordaki 5 fikri daha uygulanabilir parçalara ayırır ve her biri gerçek site kanıtına dayanır.

| Modül | İş | Kanıt / Pilot Aday |
|---|---|---|
| **A · Güven Onarımı** *(AI değil, önkoşul)* | Sahte rozet düzeltme/kaldırma, yanlış vergi hesabı (SDLT/LBTT karışıklığı), hatalı harita, footer hataları | Doğrulanan bug'lar: 01, 06, 07 |
| **B · Doğal Dil Arama** | Serbest metni mevcut filtre parametrelerine çeviren katman | 21/21 sitede eksik; filtre şeması ağ trafiğinde zaten görünür durumda |
| **C · İlan Zekası** | Özet üretimi (önceden, ilan başına bir kez) + soru-cevap (gerçek zamanlı) | 21/21 sitede eksik; açıklama kalitesi acenteden acenteye çok değişken |
| **D · Veri Kalitesi Denetimi** | Yayın öncesi ilan içi çelişkileri (başlık vs detay) yakalama | 3 bağımsız incelemeci aynı ilanda bağımsız olarak çelişki bulmuştu |
| **E · Değerleme Açıklama Katmanı** | Var olan rakamın üzerine "neden" açıklaması | Rakam birçok sitede zaten üretiliyor, açıklama hiçbir yerde yok |
| **F · Lead Ön-Değerlendirme / Mesai Dışı Asistan** | Toplanan form verisini işleyip önceliklendirme, basit soruları mesai dışı yanıtlama | Hiçbir sitede mesai dışı otomatik yanıt yok; form verisi zaten zengin |

*Not: Bu modüller ana rapordaki 5 fikirle birebir eşleşir (B=arama, C=ilan detay 1. fikir, D=ilan detay 2. fikir, E=değerleme, F=iletişim); burada sadece "nasıl" sorusuna daha fazla ayrıntı eklenmiştir.*

---

## 4. Teknik Yaklaşım — Model Nasıl Kullanılmalı

Üç farklı AI yaklaşımı var; hangisinin nerede kullanılacağı önemli bir tercih:

| Yaklaşım | Ne İşe Yarar | Bu Projede Rolü |
|---|---|---|
| **Tool-calling** (modelin gerçek API'leri çağırması) | Model bilgi uydurmaz, var olan sisteme (Neuron'un filtre API'si gibi) bir fonksiyon çağrısı yapar | **Önerilen ana yaklaşım.** Doğal dil arama zaten bir "cümleyi fonksiyon parametresine çevirme" problemi; halüsinasyon riski en düşük yöntem |
| **RAG / veri dayanaklı üretim** | Her cevap, ilanın kendi verisine veya tenant'ın kendi metnine dayandırılır, kaynak gösterilir | İlan Q&A ve değerleme açıklaması için gerekli — model asla ilan dışı bilgi uydurmamalı |
| **Fine-tune** (modeli özel eğitmek) | Modelin belirli bir üslup/tonu öğrenmesi veya maliyeti düşürmek için küçük modele damıtma | **Şimdilik önerilmiyor.** Sebep: (a) eksik olan bilgi değil erişim — fiyat/ilan verisi sürekli değişiyor, modele "ezberletmek" bunu bayatlatır; (b) henüz yeterli etiketli veri yok; (c) mevcut modeller bu görevleri zaten yeterince iyi yapıyor |

**Öneri:** İlk fazda sadece tool-calling + RAG kullanılsın. Fine-tune, sistem birkaç ay çalışıp yeterli veri (agent onayları, düzeltmeler) biriktikten sonra — hem üslup tutarlılığı hem maliyet optimizasyonu için — ikinci fazda değerlendirilebilir.

---

## 5. Nerede Çalışmalı — Arka Plan İşler vs Anlık İşler

Her AI işlemi aynı yerde/hızda çalışmak zorunda değil. İkiye ayırmak faydalı olur:

**Önceden / arka planda yapılabilecekler:**
- İlan özeti üretimi (ilan yayınlandığında bir kez üretilip saklanır)
- Veri kalitesi kontrolü (ilan kaydedilirken çalışır)
- Değerleme rakamının hazır olduğu durumlarda açıklama metninin önceden üretilmesi

**Kullanıcı beklerken, anlık yapılması gerekenler:**
- Doğal dil arama sorgusu çevirme (kullanıcı "ara" dediği an cevap bekliyor)
- İlan soru-cevap asistanı (kullanıcı soru sorduğu an)
- Mesai dışı asistan (kullanıcı mesaj yazdığı an)

**Neden bu ayrım önemli:** Önceden üretilebilen işler (özet gibi) bir kez yapılıp saklandığı için trafik arttıkça maliyet artmaz — sadece anlık işler (arama, soru-cevap) her kullanımda maliyet üretir. Bu, sistemin ölçeklenebilirliğini doğrudan etkiler.

---

## 6. Güvenlik ve Doğruluk İlkeleri

Emlak verisiyle çalışırken en büyük risk **yanlış beyan** (misdescription) — yani AI'nın bir ilan hakkında yanlış veya olmayan bir bilgi söylemesi. Bu riski azaltmak için üç temel kural önerilir:

1. **Her cevap kaynağa dayanmalı.** Model, ilanın kendi verisinde olmayan bir şeyi asla üretmemeli; bilmiyorsa "bu bilgi ilanda yer almıyor, agent'a danışın" demeli.
2. **Değerleme dili tavsiye değil açıklama olmalı.** "Bu fiyata satın alın" değil, "bu tahmini şu üç faktör etkiledi, kesin bilgi için yerinde inceleme gerekir."
3. **Yayına giden hiçbir AI-üretimi metin, agent onayı olmadan canlıya çıkmamalı** (en azından ilk fazda) — bu hem hata riskini azaltır hem de ileride fine-tune için gereken "onaylı örnek" veri setini oluşturur.

---

## 7. Basit Bir Öncelik/Yol Haritası Önerisi

Detaylı bir proje planı bu doküman kapsamında değil, ama kabaca bir sıralama önerilebilir:

1. **Önce:** Güven onarımı (Modül A) — AI'dan bağımsız, en düşük efor, en acil
2. **Sonra:** Doğal dil arama (Modül B) — platform-geneli, tek yazılıp her yerde kullanılabilir
3. **Paralel:** Değerleme açıklama katmanı (Modül E) — rakam zaten var, düşük ek efor
4. **Daha sonra:** İlan zekası (Modül C) ve veri kalitesi denetimi (Modül D) — biraz daha fazla altyapı (özet üretim pipeline'ı) gerektiriyor
5. **En son:** Lead/mesai dışı asistan (Modül F) — en çok sorumluluk taşıyan modül (gerçek müşteri iletişimi), bu yüzden diğerleri oturduktan sonra

Bu sıralama, ana rapordaki Top 3 önceliğiyle (Güven Onarımı → Doğal Dil Arama → Değerleme Açıklaması) tutarlıdır; burada sadece kalan modüllerin nereye oturacağı eklenmiştir.

---

## 8. Bu Doküman Neyi Kapsamıyor

Netlik için: bu öneri bir **başlangıç çerçevesi**dir, aşağıdakiler kasıtlı olarak dışarıda bırakılmıştır ve mühendislik/ürün ekibinin kararına bırakılmalıdır:
- Kesin API sözleşmeleri / fonksiyon isimleri
- Hangi AI sağlayıcısının (Claude, Gemini, vb.) kullanılacağı ve maliyet karşılaştırması
- Detaylı fiyatlandırma/paketleme modeli
- Hafta bazlı proje takvimi ve kaynak planlaması

Bu kararlar, mühendislik ekibinin mevcut altyapıyı (Nuxt 3, API'ler, hosting) daha yakından bildiği ve iş gereksinimlerini (bütçe, zaman çizelgesi) belirleyeceği bir sonraki aşamada netleştirilmelidir.
