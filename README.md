# Humanizer Bahasa Indonesia

Skill untuk Claude Code dan Codex CLI yang menyunting teks berbahasa Indonesia agar terdengar alami dan jelas, tanpa mengarang fakta dan tanpa menghapus suara penulis.

**Sebelum**

> Dalam rangka meningkatkan kualitas layanan, sistem ini memiliki kemampuan untuk memproses permohonan dengan lebih cepat.

**Sesudah**

> Sistem ini memproses permohonan lebih cepat.

Maknanya sama. Yang hilang hanya kata-kata yang tidak bekerja.

## Daftar isi

- [Kenapa skill ini ada](#kenapa-skill-ini-ada)
- [Fitur](#fitur)
- [Mulai cepat](#mulai-cepat)
- [Instalasi](#instalasi)
- [Penggunaan](#penggunaan)
- [Contoh lengkap](#contoh-lengkap)
- [21 pola yang dicakup](#21-pola-yang-dicakup)
- [Batasan](#batasan)
- [Sumber](#sumber)
- [Lisensi](#lisensi)

## Kenapa skill ini ada

Teks yang dibantu AI sering terbaca generik: kalimat panjang yang berputar-putar, kata-kata megah tanpa isi, pujian di awal, kesimpulan optimis di akhir. Skill ini membantu mengenali pola-pola tersebut lalu menyuntingnya menjadi tulisan yang langsung dan spesifik.

Pola-pola ini adalah panduan editorial, bukan alat pendeteksi AI. Sebuah pola tidak otomatis berarti teks ditulis oleh AI. Manusia juga menulis begitu.

## Fitur

- **21 pola tulisan**, termasuk bahasa promosi, atribusi kabur, frasa birokratis, pengulangan sinonim, kata pengisi, dan hedging berlebihan.
- **Menyesuaikan nada**: formal, santai, akademik, atau bisnis. Jika tidak disebutkan, skill mengikuti nada teks sumber.
- **Setia pada isi**: makna dan fakta dipertahankan, tidak ada detail yang ditambahkan dari luar teks.
- **Satu aturan, dua alat**: perilaku yang sama di Claude Code dan Codex CLI.

## Mulai cepat

1. Pasang skill (lihat [Instalasi](#instalasi)).
2. Tempelkan teks Anda dan minta:

   > Sunting teks ini agar lebih natural dalam Bahasa Indonesia. Pertahankan makna dan nada formalnya.

3. Tinjau hasilnya sebelum dipakai.

## Instalasi

### Claude Code

Salin folder skill ke folder skill pribadi:

```bash
mkdir -p ~/.claude/skills/humanizer-id
cp .claude/skills/humanizer-id/SKILL.md ~/.claude/skills/humanizer-id/SKILL.md
```

Untuk mengaktifkannya hanya di repo ini, pakai file yang sudah ada di `.claude/skills/humanizer-id/SKILL.md`.

### Codex CLI

```bash
mkdir -p ~/.agents/skills/humanizer-id
cp .agents/skills/humanizer-id/SKILL.md ~/.agents/skills/humanizer-id/SKILL.md
```

Untuk mengaktifkannya hanya di repo ini, pakai file yang sudah ada di `.agents/skills/humanizer-id/SKILL.md`.

## Penggunaan

Minta secara langsung, atau panggil skill-nya:

```text
$humanizer-id
```

Lalu tempelkan teks dan sebutkan konteks atau nada yang diinginkan.

Contoh permintaan:

| Kebutuhan | Contoh perintah |
| --- | --- |
| Umum | "Sunting teks ini agar lebih natural." |
| Formal | "Humanize teks ini, tetap formal untuk laporan bisnis." |
| Santai | "Buat lebih santai untuk postingan media sosial." |
| Akademik | "Rapikan paragraf ini untuk skripsi, jangan ubah argumennya." |

## Contoh lengkap

Contoh ini ilustratif, untuk menunjukkan jenis penyuntingan yang dilakukan. Detail orang pertama adalah bagian dari contoh, bukan klaim tentang penulis repo ini.

**Sebelum**

> Pertanyaan bagus! Pengkodean berbantuan AI merupakan bukti abadi dari potensi transformatif large language model, menandai momen penting dalam evolusi pengembangan perangkat lunak. Dalam lanskap teknologi yang terus berkembang pesat saat ini, alat-alat revolusioner ini, tersembunyi di persimpangan antara riset dan praktik, sedang membentuk ulang cara insinyur berideasi, menggarisbawahi peran vitalnya dalam alur kerja modern. Selain itu, kemampuan menghasilkan dokumentasi menampilkan bagaimana AI dapat berkontribusi pada hasil yang lebih baik, menyoroti keterkaitan intrinsik antara otomasi dan penilaian manusia. Dalam rangka mewujudkan potensi ini, tim harus sejalan dengan praktik terbaik. Masa depan terlihat cerah!

**Sesudah**

> Asisten koding AI bisa bikin kamu lebih cepat di bagian-bagian yang membosankan. Bukan semuanya. Apalagi untuk arsitektur sistem.
>
> Bagusnya untuk boilerplate: file konfigurasi, scaffolding tes, refactor berulang. Jeleknya, mereka juga jago terdengar benar padahal salah. Saya pernah asal terima saran yang dikompilasi, lolos lint, tapi tetap meleset karena saya tidak lagi memperhatikan.
>
> Metrik produktivitasnya licin. Kalau tidak ada tes, kamu pada dasarnya menebak.

Nada santai dipertahankan. Saat menyunting teks lain, pilihan kata menyesuaikan suara dan konteks penulisnya.

## 21 pola yang dicakup

Pola dikelompokkan menurut jenisnya. Ingat: pola adalah petunjuk untuk menyunting, bukan bukti bahwa teks ditulis oleh AI.

### Isi

| # | Pola | Contoh sebelum | Arah penyuntingan |
| --- | --- | --- | --- |
| 1 | Signifikansi dan warisan yang dibesar-besarkan | "menandai tonggak penting dalam evolusi..." | Sebutkan fungsi atau fakta konkretnya. |
| 2 | Klaim keterkenalan tanpa konteks | "dikutip oleh berbagai media ternama" | Sebut sumber dan konteks kutipannya bila relevan. |
| 3 | Analisis dangkal di akhir kalimat | "..., mencerminkan tren yang lebih luas" | Hapus tafsir kabur atau dukung dengan sumber yang ada. |
| 4 | Bahasa promosi | "tersembunyi di kawasan yang menakjubkan" | Gunakan deskripsi netral dan spesifik. |
| 5 | Atribusi kabur | "para ahli percaya..." | Cantumkan sumber yang jelas atau hilangkan atribusinya. |
| 6 | Bagian tantangan dan prospek yang formulaik | "meski menghadapi tantangan, terus berkembang" | Fokus pada tantangan atau rencana yang benar-benar disebut. |

### Bahasa dan struktur kalimat

| # | Pola | Contoh sebelum | Arah penyuntingan |
| --- | --- | --- | --- |
| 7 | Kosakata AI yang generik | "holistik, transformatif, lanskap" | Pilih kata konkret sesuai maksud. |
| 8 | Frasa birokratis | "dalam rangka..., guna memastikan..." | Ringkas menjadi bahasa langsung. |
| 9 | Pengulangan sinonim untuk subjek yang sama | "tokoh utama, protagonis, figur sentral..." | Gunakan istilah yang paling jelas secara konsisten. |
| 10 | "Tidak hanya..., tetapi juga..." berlebihan | "Ini tidak hanya X, tetapi juga Y" | Sampaikan hubungan antargagasan secara lugas. |
| 11 | Tiga serangkai yang dipaksakan | "inovasi, inspirasi, dan wawasan" | Gunakan jumlah unsur yang memang diperlukan. |

### Gaya dan format

| # | Pola | Contoh sebelum | Arah penyuntingan |
| --- | --- | --- | --- |
| 12 | Em dash berlebihan | "lembaga pemerintah—bukan masyarakat—..." | Ganti dengan tanda baca atau susun ulang kalimat. |
| 13 | Huruf tebal berlebihan | "**OKR**, **KPI**, **BMC**" | Pakai format biasa kecuali ada alasan penekanan. |
| 14 | Daftar dengan header inline berulang | "**Performa:** Performa meningkat..." | Ringkas menjadi prosa atau daftar yang memang dibutuhkan. |
| 15 | Emoji dekoratif | "🚀 Fase peluncuran: 💡 wawasan kunci" | Hapus emoji yang tidak membawa makna. |

### Komunikasi

| # | Pola | Contoh sebelum | Arah penyuntingan |
| --- | --- | --- | --- |
| 16 | Artefak chatbot | "Pertanyaan bagus! Semoga membantu!" | Hapus basa-basi chatbot dari teks. |
| 17 | Penyangkalan batas pengetahuan | "berdasarkan informasi yang tersedia..." | Cari dan gunakan sumber yang tersedia; jangan menebak. |
| 18 | Nada terlalu memuji | "Kamu benar sekali, poin yang sangat bagus!" | Tanggapi substansi dengan wajar. |

### Pengisi dan penutup

| # | Pola | Contoh sebelum | Arah penyuntingan |
| --- | --- | --- | --- |
| 19 | Frasa pengisi | "Penting untuk dicatat bahwa..." | Langsung ke informasi utamanya. |
| 20 | Hedging berlebihan | "bisa jadi mungkin dapat..." | Pertahankan tingkat kepastian yang didukung sumber. |
| 21 | Kesimpulan positif generik | "masa depan terlihat cerah" | Akhiri dengan fakta atau rencana spesifik yang tersedia. |

## Batasan

- Humanisasi adalah penyuntingan gaya, bukan verifikasi fakta atau pemeriksaan plagiarisme.
- Hasil tetap perlu ditinjau penulis, terutama untuk penggunaan akademik, profesional, atau publikasi.
- Skill ini tidak menjamin dan tidak dirancang untuk mengelabui detektor AI.

## Sumber

- [Wikipedia: Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing), salah satu rujukan pola umum.
- [blader/humanizer](https://github.com/blader/humanizer), inspirasi untuk adaptasi berbahasa Indonesia ini.

## Lisensi

MIT. Lihat [`LICENSE`](LICENSE).