# Project Context / Proje Bağlamı

## English

### Goal
Review 21 live estate-agent websites built on the Neuron platform and record their
current user experience (search, listing detail, valuation, contact). These notes
are the raw input for the **"current state / gap analysis"** section of an
AI-feature-opportunities report.

### What we are looking for
Things these sites do **manually today that AI could do better**. Typical gaps:
- Search is dropdown/filter only; no natural-language search.
- Listing descriptions are hand-written and inconsistent; no AI summary.
- Valuation is a "we'll call you" form; no instant smart estimate.
- Contact is a single generic form; no chatbot / lead qualification.

Full term list: [ai-feature-glossary.md](ai-feature-glossary.md).

### Method
- Actually use each site: run a search, open a listing, try the valuation form,
  inspect the contact path. What to check: [../checklist.md](../checklist.md).
- Don't write **Yes/No** — write *what* it is. ("Dropdown filters only, no natural
  language" > "No").
- Short, concrete sentences. No long paragraphs.
- If possible, look technical: SSR vs CSR, which APIs appear in the Network tab
  (is the Neuron API visible), mobile behaviour.

### Rotation logic
The 21 sites are split into 4 groups; across 4 rounds the groups rotate between
people. As a result **every site is reviewed independently by all 4 people** —
this provides verification without needing a separate cross-check phase. Details:
[../site-assignments.md](../site-assignments.md).

### Output
Once all 4 round blocks in a site file are filled, the **"Findings / Synthesis"**
section at the bottom is completed together. These syntheses feed the gap analysis
in the final report.

---

## Türkçe

### Amaç
Neuron platformunda yayında olan 21 emlak (estate agent) web sitesini inceleyip
mevcut kullanıcı deneyimini (arama, ilan detay, değerleme, iletişim) not almak.
Bu notlar, **AI özellik önerileri raporunun** "mevcut durum / gap analizi"
bölümünün ham verisidir.

### Neyi arıyoruz
Sitelerin bugün **AI ile yapılabilecek ama yapmadığı** şeyleri arıyoruz. Yani
klasik/manuel çözülmüş ama AI ile daha iyi olabilecek noktaları. Örnek boşluklar:
- Arama sadece dropdown/filtre; doğal dil araması yok.
- İlan açıklamaları elle yazılmış, tutarsız; AI özet yok.
- Değerleme "sizi arayacağız" formu; anlık akıllı tahmin yok.
- İletişim tek tip form; chatbot / lead kalifikasyonu yok.

Terimlerin tam listesi: [ai-feature-glossary.md](ai-feature-glossary.md).

### Yöntem
- Her siteyi gerçekten kullan: arama yap, bir ilana gir, değerleme formunu dene,
  iletişim yolunu incele. Neye bakılacağı: [../checklist.md](../checklist.md).
- **Var/Yok** yazma — ne olduğunu yaz. ("Sadece dropdown filtre, doğal dil yok"
  > "Yok").
- Kısa, somut cümleler. Uzun paragraf yok.
- Mümkünse teknik bak: SSR mi CSR mi, Network tab'de hangi API'ler (Neuron API
  görünüyor mu), mobil davranış.

### Rotasyon mantığı
21 site 4 gruba bölündü; 4 tur boyunca gruplar kişiler arasında döner. Sonuçta
**her site 4 farklı kişi tarafından bağımsız incelenir** — bu, ayrı bir çapraz
kontrol aşamasına gerek bırakmadan doğrulama sağlar. Detay:
[../site-assignments.md](../site-assignments.md).

### Çıktı
Her site dosyasında 4 tur bloğu dolunca, en altta **"Findings / Synthesis"**
birlikte doldurulur. Bu sentezler nihai raporun gap analizini besler.
