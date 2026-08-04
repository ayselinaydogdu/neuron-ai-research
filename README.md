# Neuron AI Feature Research / Neuron AI Özellik Araştırması

## English

We review the **21 live estate-agent websites** on the Neuron platform and record
their current UX (search, listing detail, valuation, contact). These notes are the
raw data for the "current state / gap analysis" section of an AI-feature-proposals
report.

Team: **Görkem · Ayselin · Yasemin · Berkay**

### Folder structure

| Path | Contents |
|---|---|
| `info/` | Project context and AI feature glossary (each file has EN + TR sections) |
| `checklist.md` | Checklist of what to look at in every category |
| `site-assignments.md` | **Rotation home page** — the 4-round assignment matrix |
| `assignments/round-1..4.md` | Each round's checkable assignment list (4 copies) |
| `sites/01..21-*.md` | Each site's own schema file — the 4 round blocks get filled |

### How it works — rotation

The 21 sites are split into 4 groups (A: 01–05, B: 06–10, C: 11–15, D: 16–21).
Assignments run over **4 rounds** and the groups rotate between people across rounds:

| Group | Round 1 | Round 2 | Round 3 | Round 4 |
|---|---|---|---|---|
| A (01–05) | Görkem | Berkay | Yasemin | Ayselin |
| B (06–10) | Ayselin | Görkem | Berkay | Yasemin |
| C (11–15) | Yasemin | Ayselin | Görkem | Berkay |
| D (16–21) | Berkay | Yasemin | Ayselin | Görkem |

Result: each round everyone gets 5–6 sites, and **after 4 rounds every site has
been reviewed independently by 4 different people**. No separate cross-check phase
is needed — verification is built into the rotation.

### Flow

1. **Read the context:** [info/project-context.md](info/project-context.md) and
   [info/ai-feature-glossary.md](info/ai-feature-glossary.md).
2. **Open your round:** your current round's list (`assignments/round-N.md`) shows
   the 5–6 sites assigned to you.
3. **Review + fill:** for each site, open its file under `sites/`, actually use the
   site ([checklist.md](checklist.md)) and fill in **your own round block**. When
   done, set `Status: Done`.
4. **Check + commit:** tick your box (`[x]`) in the round list, and commit in small,
   frequent commits (e.g. "Görkem: 03 round-1 notes").
5. **Synthesis:** once all 4 rounds are done, the **"Findings / Synthesis"** section
   at the bottom of each site file is filled in together.

### Rules

- Short, concrete observations — no long paragraphs.
- Not "yes / no" but **what it is** (e.g. "Dropdown filters only, no natural-language search").
- Edit **only your own round block**; don't delete or change anyone else's notes.
- Use the shared vocabulary for terms (`info/`).

---

## Türkçe

Neuron platformundaki **21 canlı emlak sitesini** inceleyip mevcut UX'i (arama,
ilan detay, değerleme, iletişim) not alıyoruz. Bu notlar, AI özellik önerileri
raporunun "mevcut durum / gap analizi" bölümünün ham verisi olacak.

Ekip: **Görkem · Ayselin · Yasemin · Berkay**

### Klasör yapısı

| Yol | İçerik |
|---|---|
| `info/` | Proje bağlamı ve AI özellik sözlüğü (her dosyada EN + TR bölümü) |
| `checklist.md` | Her kategoride neye bakılacağını gösteren checklist |
| `site-assignments.md` | **Rotasyon ana sayfası** — 4 turluk atama matrisi |
| `assignments/round-1..4.md` | Her turun işaretlenebilir atama listesi (4 kopya) |
| `sites/01..21-*.md` | Her sitenin kendi şematik dosyası — 4 tur bloğu doldurulur |

### Nasıl çalışır — rotasyon

21 site 4 gruba (A: 01–05, B: 06–10, C: 11–15, D: 16–21) bölündü. Atamalar **4 tur**
hâlinde yapılır ve gruplar turlar arasında kişiler üzerinde döner:

| Grup | Tur 1 | Tur 2 | Tur 3 | Tur 4 |
|---|---|---|---|---|
| A (01–05) | Görkem | Berkay | Yasemin | Ayselin |
| B (06–10) | Ayselin | Görkem | Berkay | Yasemin |
| C (11–15) | Yasemin | Ayselin | Görkem | Berkay |
| D (16–21) | Berkay | Yasemin | Ayselin | Görkem |

Sonuç: her turda herkese 5–6 site düşer ve **4 tur sonunda her site 4 farklı kişi
tarafından bağımsız incelenmiş** olur. Ayrı bir çapraz kontrol aşamasına gerek
yok — doğrulama rotasyonun içinde.

### Akış

1. **Bağlamı oku:** [info/project-context.md](info/project-context.md) ve
   [info/ai-feature-glossary.md](info/ai-feature-glossary.md).
2. **Turunu aç:** İçinde bulunduğun turun listesi (`assignments/round-N.md`) sana
   düşen 5–6 siteyi gösterir.
3. **İncele + doldur:** Her site için `sites/` altındaki dosyayı aç, siteyi
   gerçekten kullan ([checklist.md](checklist.md)) ve **kendi tur bloğunu** doldur.
   Bitince `Durum: Yapıldı` yap.
4. **İşaretle + commit:** Tur listesindeki kutucuğu (`[x]`) işaretle, küçük ve sık
   commit at (ör. "Görkem: 03 round-1 notları").
5. **Sentez:** 4 tur bitince her site dosyasının altındaki **"Findings / Synthesis"**
   kısmı birlikte doldurulur.

### Kurallar

- Kısa, somut gözlemler — uzun paragraf yok.
- "Var / Yok" değil, **ne olduğunu** yaz (ör. "Sadece dropdown filtre, doğal dil
  arama yok").
- Sadece **kendi tur bloğunu** düzenle; başkasının notunu silme/değiştirme.
- Terimlerde ortak sözlüğü kullan (`info/`).
