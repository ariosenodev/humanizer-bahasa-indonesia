# Humanizer Bahasa Indonesia

A Claude skill that removes signs of AI-generated writing from Indonesian text, making it sound more natural and human.

Inspired by and based on [blader/humanizer](https://github.com/blader/humanizer) — a Claude Code skill for English text by [@blader](https://github.com/blader). This is an Indonesian-language adaptation that extends the original patterns with new ones specific to how AI writes in Bahasa Indonesia.

---

## Installation

### Option 1: Claude.ai Skills (Recommended)

1. Download `humanizer-id.skill` from the [Releases](../../releases) page
2. Go to **claude.ai → Settings → Skills**
3. Upload or drag the `.skill` file

### Option 2: Clone into Claude Code skills directory

```bash
mkdir -p ~/.claude/skills
git clone https://github.com/ariosenodev/humanizer-bahasa-indonesia.git ~/.claude/skills/humanizer-id
```

### Option 3: Manual install

```bash
mkdir -p ~/.claude/skills/humanizer-id
cp SKILL.md ~/.claude/skills/humanizer-id/
```

---

## Usage

In Claude Code:

```
/humanizer-id

[tempel teks kamu di sini]
```

Or ask Claude directly:

```
Tolong humanize teks ini: [teks kamu]
```

```
Buat teks ini terdengar lebih natural dan tidak seperti AI
```

---

## Overview

Based on [Wikipedia's "Signs of AI writing"](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing) guide (maintained by WikiProject AI Cleanup), adapted and extended for Bahasa Indonesia. The skill covers all 24 original English patterns, plus 9 new patterns specific to how AI writes in Indonesian.

> "LLMs use statistical algorithms to guess what should come next. The result tends toward the most statistically likely result that applies to the widest variety of cases."

Works across all writing contexts: articles/blogs, academic writing, business reports, and social media.

---

## Patterns Detected

### Universal Patterns (adapted from English)

| # | Pattern | Before | After |
|---|---------|--------|-------|
| 1 | **Significance inflation** | "menandai tonggak penting dalam evolusi..." | "didirikan pada 1989 untuk mengumpulkan statistik regional" |
| 2 | **Notability name-dropping** | "dikutip oleh Kompas, BBC, Financial Times" | "Dalam wawancara Kompas 2024, ia berpendapat..." |
| 3 | **Superficial -ing analyses** | "melambangkan... mencerminkan... menampilkan..." | Hapus atau ganti dengan sumber spesifik |
| 4 | **Promotional language** | "tersembunyi di kawasan Danau Toba yang menakjubkan" | "adalah desa di tepi Danau Toba" |
| 5 | **Vague attributions** | "Para ahli percaya sungai ini memainkan peran krusial" | "menurut survei 2019 oleh LIPI" |
| 6 | **Formulaic challenges section** | "Terlepas dari tantangan... terus berkembang" | Fakta spesifik tentang tantangan nyata |
| 7 | **AI vocabulary words** | "holistik, transformatif, krusial, lanskap, semarak" | Kata biasa yang lebih spesifik |
| 8 | **Copula avoidance** | "berfungsi sebagai... berperan sebagai... berdiri sebagai" | "adalah / merupakan" |
| 9 | **Negative parallelisms** | "Ini bukan hanya tentang X, ini tentang Y" | Langsung ke intinya |
| 10 | **Rule of three** | "inovasi, inspirasi, dan wawasan industri" | Jumlah item yang natural |
| 11 | **Synonym cycling** | "tokoh utama... protagonis... figur sentral... sang pahlawan" | Ulangi kata yang paling jelas |
| 12 | **False ranges** | "dari Big Bang hingga materi gelap" | Daftar topik langsung |
| 13 | **Em dash overuse** | "lembaga pemerintah—bukan masyarakat—namun terus berlanjut—" | Gunakan koma atau titik |
| 14 | **Boldface overuse** | "**OKR**, **KPI**, **BMC**" | "OKR, KPI, BMC" |
| 15 | **Inline-header lists** | "**Performa:** Performa meningkat..." | Ubah ke prosa |
| 16 | **Title Case headings** | "Negosiasi Strategis Dan Kemitraan Global" | "Negosiasi strategis dan kemitraan global" |
| 17 | **Emojis** | "🚀 Fase Peluncuran: 💡 Wawasan Kunci:" | Hapus emoji |
| 18 | **Chatbot artifacts** | "Pertanyaan bagus! Semoga membantu! Beritahu saya jika..." | Hapus seluruhnya |
| 19 | **Knowledge-cutoff disclaimers** | "Meskipun detail spesifisnya terbatas..." | Cari sumber atau hapus |
| 20 | **Sycophantic tone** | "Pertanyaan yang sangat bagus! Kamu benar sekali!" | Langsung ke substansi |
| 21 | **Filler phrases** | "Dalam rangka mencapai...", "Penting untuk dicatat bahwa" | "Untuk...", langsung ke klaimnya |
| 22 | **Excessive hedging** | "bisa jadi mungkin dapat diargumentasikan bahwa... mungkin" | "kemungkinan berdampak pada" |
| 23 | **Generic positive conclusions** | "Masa depan terlihat cerah. Waktu menggembirakan menanti..." | Rencana atau fakta spesifik |

### Indonesian-Specific Patterns

| # | Pattern | Before | After |
|---|---------|--------|-------|
| ID-1 | **Bureaucratic filler phrases** | "dalam rangka meningkatkan... guna memastikan... terkait dengan hal tersebut" | "untuk meningkatkan..." |
| ID-2 | **AI vocabulary in Indonesian** | "holistik, komprehensif, transformatif, tak terbantahkan, berkelanjutan (abstract)" | Kata konkret yang lebih spesifik |
| ID-3 | **"Tidak hanya... tetapi juga..." overuse** | "Ini tidak hanya X, tetapi juga Y. Bukan sekadar A, melainkan B." | Satu kalimat langsung |

---

## Full Example

**Before (AI-sounding):**

> Pertanyaan bagus! Pengkodean berbantuan AI merupakan bukti abadi dari potensi transformatif large language model, menandai momen penting dalam evolusi pengembangan perangkat lunak. Dalam lanskap teknologi yang terus berkembang pesat saat ini, alat-alat revolusioner ini—tersembunyi di persimpangan antara riset dan praktik—sedang membentuk ulang cara insinyur berideasi, menggarisbawahi peran vitalnya dalam alur kerja modern. Selain itu, kemampuan menghasilkan dokumentasi menampilkan bagaimana AI dapat berkontribusi pada hasil yang lebih baik, menyoroti keterkaitan intrinsik antara otomasi dan penilaian manusia. Dalam rangka mewujudkan potensi ini, tim harus sejalan dengan praktik terbaik. Masa depan terlihat cerah!

**After (Humanized):**

> Asisten koding AI bisa bikin kamu lebih cepat di bagian-bagian yang membosankan. Bukan semuanya. Apalagi untuk arsitektur sistem.
>
> Bagusnya untuk boilerplate: file konfigurasi, scaffolding tes, refactor berulang. Jeleknya, mereka juga jago terdengar benar padahal salah. Saya pernah asal terima saran yang dikompilasi, lolos lint, tapi tetap miss the point karena saya tidak lagi memperhatikan.
>
> Metrik produktivitasnya licin. Kalau tidak ada tes, kamu pada dasarnya nebak.

---

## References

- [blader/humanizer](https://github.com/blader/humanizer) — The original English humanizer skill this is based on
- [Wikipedia: Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing) — Primary source for all patterns
- [WikiProject AI Cleanup](https://en.wikipedia.org/wiki/Wikipedia:WikiProject_AI_Cleanup) — Maintaining organization

---

## License

MIT
