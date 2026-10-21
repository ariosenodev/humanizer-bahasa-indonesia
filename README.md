# Humanizer Bahasa Indonesia

> Sunting teks berbahasa Indonesia agar terdengar alami, jelas, dan tetap setia pada maksud penulis.

Humanizer Bahasa Indonesia adalah skill untuk Claude Code dan Codex CLI. Skill ini membantu mengenali pola tulisan yang terasa generik atau seperti keluaran AI, lalu menyuntingnya tanpa mengarang fakta atau menghapus suara penulis.

**Deskripsi GitHub:** Skill Claude Code dan Codex CLI untuk menyunting teks berbahasa Indonesia agar lebih alami, jelas, dan tetap mempertahankan makna serta suara penulis.

## Fitur

- Mencakup 21 pola tulisan, termasuk bahasa promosi, atribusi kabur, frasa birokratis, pengulangan sinonim, pengisi, dan hedging berlebihan.
- Menyesuaikan hasil dengan konteks dan nada yang diminta, seperti formal, santai, akademik, atau bisnis.
- Mempertahankan makna dan fakta. Skill tidak menambahkan detail yang tidak ada di teks sumber.
- Menggunakan aturan yang sama di Claude Code dan Codex CLI.

Pola-pola ini merupakan panduan editorial, bukan alat pendeteksi AI. Sebuah pola tidak otomatis berarti teks ditulis oleh AI.

## Instalasi

### Claude Code

Salin folder skill ke folder skill pribadi Claude Code:

```bash
mkdir -p ~/.claude/skills/humanizer-id
cp .claude/skills/humanizer-id/SKILL.md ~/.claude/skills/humanizer-id/SKILL.md
```

Untuk mengaktifkannya hanya pada repo ini, gunakan file yang sudah tersedia di `.claude/skills/humanizer-id/SKILL.md`.

### Codex CLI

Salin folder skill ke folder skill pribadi Codex:

```bash
mkdir -p ~/.agents/skills/humanizer-id
cp .agents/skills/humanizer-id/SKILL.md ~/.agents/skills/humanizer-id/SKILL.md
```

Untuk mengaktifkannya hanya pada repo ini, gunakan file yang sudah tersedia di `.agents/skills/humanizer-id/SKILL.md`.

## Penggunaan

Minta secara langsung, misalnya:

> Sunting teks ini agar lebih natural dalam Bahasa Indonesia. Pertahankan makna dan nada formalnya.

Atau, jika skill sudah terpasang:

```text
$humanizer-id
```

Tempelkan teks yang ingin disunting dan sebutkan konteks atau nada yang diinginkan. Jika tidak disebutkan, skill akan mengikuti nada teks sumber.

## Contoh hasil

**Sebelum**

> Dalam rangka meningkatkan kualitas layanan, sistem ini memiliki kemampuan untuk memproses permohonan dengan lebih cepat.

**Sesudah**

> Sistem ini memproses permohonan lebih cepat.

Contoh ini menunjukkan penyederhanaan kalimat tanpa mengubah inti pesannya.

## Pola yang dicakup

Skill ini membahas 21 pola editorial. Pola adalah petunjuk untuk menyunting, bukan bukti bahwa sebuah teks ditulis oleh AI.

| # | Pola | Contoh sebelum | Arah penyuntingan |
| --- | --- | --- | --- |
| 1 | Signifikansi dan warisan yang dibesar-besarkan | “menandai tonggak penting dalam evolusi...” | Sebutkan fungsi atau fakta konkretnya. |
| 2 | Klaim keterkenalan tanpa konteks | “dikutip oleh berbagai media ternama” | Sebut sumber dan konteks kutipannya bila relevan. |
| 3 | Analisis dangkal di akhir kalimat | “..., mencerminkan tren yang lebih luas” | Hapus tafsir kabur atau dukung dengan sumber yang ada. |
| 4 | Bahasa promosi | “tersembunyi di kawasan yang menakjubkan” | Gunakan deskripsi netral dan spesifik. |
| 5 | Atribusi kabur | “para ahli percaya...” | Cantumkan sumber yang jelas atau hilangkan atribusinya. |
| 6 | Bagian tantangan dan prospek yang formulaik | “meski menghadapi tantangan, terus berkembang” | Fokus pada tantangan atau rencana yang benar-benar disebut. |
| 7 | Kosakata AI yang generik | “holistik, transformatif, lanskap” | Pilih kata konkret sesuai maksud. |
| 8 | Frasa birokratis | “dalam rangka..., guna memastikan...” | Ringkas menjadi bahasa langsung. |
| 9 | Pengulangan sinonim untuk subjek yang sama | “tokoh utama, protagonis, figur sentral...” | Gunakan istilah yang paling jelas secara konsisten. |
| 10 | “Tidak hanya..., tetapi juga...” berlebihan | “Ini tidak hanya X, tetapi juga Y” | Sampaikan hubungan antargagasan secara lugas. |
| 11 | Tiga serangkai yang dipaksakan | “inovasi, inspirasi, dan wawasan” | Gunakan jumlah unsur yang memang diperlukan. |
| 12 | Em dash berlebihan | “lembaga pemerintah—bukan masyarakat—...” | Ganti dengan tanda baca atau susun ulang kalimat. |
| 13 | Huruf tebal berlebihan | “**OKR**, **KPI**, **BMC**” | Gunakan format biasa kecuali ada alasan penekanan. |
| 14 | Daftar dengan header inline berulang | “**Performa:** Performa meningkat...” | Ringkas menjadi prosa atau daftar yang memang dibutuhkan. |
| 15 | Emoji dekoratif | “🚀 Fase peluncuran: 💡 wawasan kunci” | Hapus emoji yang tidak membawa makna. |
| 16 | Artefak chatbot | “Pertanyaan bagus! Semoga membantu!” | Hapus basa-basi chatbot dari teks. |
| 17 | Penyangkalan batas pengetahuan | “berdasarkan informasi yang tersedia...” | Cari dan gunakan sumber yang tersedia; jangan menebak. |
| 18 | Nada terlalu memuji | “Kamu benar sekali, poin yang sangat bagus!” | Tanggapi substansi dengan wajar. |
| 19 | Frasa pengisi | “Penting untuk dicatat bahwa...” | Langsung ke informasi utamanya. |
| 20 | Hedging berlebihan | “bisa jadi mungkin dapat...” | Pertahankan tingkat kepastian yang didukung sumber. |
| 21 | Kesimpulan positif generik | “masa depan terlihat cerah” | Akhiri dengan fakta atau rencana spesifik yang tersedia. |

## Contoh lengkap

Contoh berikut bersifat ilustratif untuk menunjukkan jenis penyuntingan yang dilakukan. Detail orang pertama merupakan bagian dari contoh, bukan klaim tentang penulis repo ini.

**Sebelum**

> Pertanyaan bagus! Pengkodean berbantuan AI merupakan bukti abadi dari potensi transformatif large language model, menandai momen penting dalam evolusi pengembangan perangkat lunak. Dalam lanskap teknologi yang terus berkembang pesat saat ini, alat-alat revolusioner ini, tersembunyi di persimpangan antara riset dan praktik, sedang membentuk ulang cara insinyur berideasi, menggarisbawahi peran vitalnya dalam alur kerja modern. Selain itu, kemampuan menghasilkan dokumentasi menampilkan bagaimana AI dapat berkontribusi pada hasil yang lebih baik, menyoroti keterkaitan intrinsik antara otomasi dan penilaian manusia. Dalam rangka mewujudkan potensi ini, tim harus sejalan dengan praktik terbaik. Masa depan terlihat cerah!

**Sesudah**

> Asisten koding AI bisa bikin kamu lebih cepat di bagian-bagian yang membosankan. Bukan semuanya. Apalagi untuk arsitektur sistem.
>
> Bagusnya untuk boilerplate: file konfigurasi, scaffolding tes, refactor berulang. Jeleknya, mereka juga jago terdengar benar padahal salah. Saya pernah asal terima saran yang dikompilasi, lolos lint, tapi tetap meleset karena saya tidak lagi memperhatikan.
>
> Metrik produktivitasnya licin. Kalau tidak ada tes, kamu pada dasarnya menebak.

Contoh ini mempertahankan nada santai. Saat menyunting teks lain, sesuaikan pilihan kata dengan suara dan konteks penulisnya.

## Batasan

- Humanisasi adalah penyuntingan gaya, bukan verifikasi fakta atau pemeriksaan plagiarisme.
- Teks yang diubah tetap perlu ditinjau penulis, terutama untuk penggunaan akademik, profesional, atau publikasi.
- Skill tidak menjamin dan tidak dirancang untuk mengelabui detektor AI.

## Sumber

- [Wikipedia: Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing), sebagai salah satu rujukan pola umum.
- [blader/humanizer](https://github.com/blader/humanizer), inspirasi untuk adaptasi berbahasa Indonesia ini.

## Lisensi

MIT. Lihat [`LICENSE`](LICENSE).
