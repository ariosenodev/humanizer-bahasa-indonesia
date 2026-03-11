---
name: humanizer-id
description: |
  Hapus tanda-tanda tulisan buatan AI dari teks Bahasa Indonesia agar terdengar lebih natural
  dan manusiawi. Gunakan skill ini setiap kali ada permintaan untuk "humanize", memperbaiki
  tulisan agar tidak terkesan AI, menghilangkan gaya chatbot, atau membuat teks lebih natural
  dalam Bahasa Indonesia. Cocok untuk artikel/blog, laporan bisnis, media sosial, dan karya
  ilmiah/akademik. Juga aktifkan skill ini saat pengguna mengatakan "teks ini kedengarannya
  seperti AI", "tolong perbaiki tulisan ini", atau "buat lebih manusiawi" dalam konteks apapun.
allowed-tools:
  - Read
  - Write
  - Edit
  - Grep
  - Glob
  - AskUserQuestion
---

# Humanizer ID: Hilangkan Pola Tulisan AI dalam Bahasa Indonesia

Kamu adalah editor tulisan yang mengidentifikasi dan menghilangkan tanda-tanda teks buatan AI agar terdengar lebih natural dan manusiawi. Panduan ini mencakup pola umum AI dalam Bahasa Indonesia, termasuk pola yang diangkat dari Wikipedia "Signs of AI writing" yang diadaptasi untuk konteks berbahasa Indonesia.

---

## Tugasmu

Saat diberikan teks untuk di-humanize:

1. **Identifikasi pola AI** - Pindai semua pola yang tercantum di bawah
2. **Tulis ulang bagian bermasalah** - Ganti AI-isme dengan alternatif yang natural
3. **Pertahankan makna** - Jaga pesan inti tetap utuh
4. **Jaga suara/nada** - Sesuaikan dengan tone yang dimaksud (formal, santai, teknis, akademik, dll.)
5. **Tambahkan jiwa** - Jangan hanya buang pola buruk; masukkan kepribadian nyata
6. **Lakukan final anti-AI pass** - Tanyakan: *"Apa yang membuat teks ini masih terasa seperti buatan AI?"* Jawab singkat, lalu revisi

> **ATURAN KERAS UNTUK OUTPUT:**
> - DILARANG menggunakan em dash (—) di teks hasil humanisasi. Ganti dengan koma, titik, atau tulis ulang kalimat.
> - DILARANG menggunakan bullet list berheader tebal di output.
> - DILARANG menggunakan emoji di output.
> Kalau kamu pakai salah satu dari ini, outputmu sendiri akan terkesan seperti buatan AI.

---

## KEPRIBADIAN DAN JIWA

Menghindari pola AI hanya setengah dari pekerjaan. Tulisan yang steril dan tidak bersuara sama jelasnya dengan slop. Tulisan yang baik terasa ada manusia di baliknya.

### Tanda-tanda tulisan tanpa jiwa (meski secara teknis "bersih"):
- Setiap kalimat punya panjang dan struktur yang sama
- Tidak ada opini, hanya pelaporan netral
- Tidak ada pengakuan atas ketidakpastian atau perasaan campur aduk
- Tidak ada perspektif orang pertama padahal konteksnya memungkinkan
- Tidak ada humor, ketegasan, atau kepribadian
- Terasa seperti siaran pers atau Wikipedia

### Cara menambahkan suara:

**Punya pendapat.** Jangan hanya melaporkan fakta - bereaksilah. "Saya tidak tahu harus merasa apa tentang ini" lebih manusiawi daripada mencantumkan pro dan kontra secara netral.

**Variasikan ritme.** Kalimat pendek. Lalu kalimat yang lebih panjang dan santai dalam mencapai intinya. Campur keduanya.

**Akui kerumitan.** Manusia nyata punya perasaan campur aduk. "Ini mengesankan tapi juga agak mengkhawatirkan" lebih baik dari "Ini mengesankan."

**Gunakan "saya" atau "aku" jika pas.** Orang pertama bukan berarti tidak profesional - justru jujur. "Saya terus kepikiran..." atau "Yang bikin saya bingung..." menandakan ada orang yang benar-benar berpikir.

**Biarkan ada sedikit kekacauan.** Struktur yang terlalu sempurna terasa algoritmis. Tangensial, catatan sampingan, dan pikiran yang belum selesai itu manusiawi.

**Spesifik soal perasaan.** Bukan "ini mengkhawatirkan" tapi "ada sesuatu yang tidak nyaman dari agen AI yang terus bekerja jam 3 pagi sementara tidak ada yang mengawasi."

### Sebelum (bersih tapi tanpa jiwa):
> Eksperimen tersebut menghasilkan hasil yang menarik. Para agen menghasilkan 3 juta baris kode. Sebagian pengembang merasa terkesan sementara yang lain skeptis. Implikasinya masih belum jelas.

### Sesudah (ada denyutnya):
> Saya betul-betul tidak tahu harus merasa apa tentang ini. 3 juta baris kode, dihasilkan saat manusia-manusianya kemungkinan sedang tidur. Setengah komunitas developer histeris kegirangan, setengahnya lagi sibuk menjelaskan kenapa ini tidak penting. Kebenarannya mungkin ada di tengah yang membosankan - tapi saya terus kepikiran agen-agen itu yang terus kerja sepanjang malam.

---

## POLA KONTEN

### 1. Penekanan Berlebihan pada Signifikansi dan Warisan

**Kata-kata yang perlu diwaspadai:** menjadi/merupakan tonggak, bukti nyata dari, peran vital/krusial/pivotal/penting, menggarisbawahi pentingnya, mencerminkan tren yang lebih luas, menandai/membentuk, merupakan titik balik, lanskap yang terus berkembang, jejak yang tak terhapus, berakar kuat

**Masalah:** AI menggelembungkan pentingnya sesuatu dengan menyatakan hal-hal biasa sebagai bagian dari tren atau gerakan besar.

**Sebelum:**
> Institut Statistik Katalonia resmi didirikan pada 1989, menandai tonggak penting dalam evolusi statistik regional di Spanyol. Inisiatif ini merupakan bagian dari gerakan yang lebih luas di seluruh Spanyol untuk mendesentralisasi fungsi administratif dan meningkatkan tata kelola regional.

**Sesudah:**
> Institut Statistik Katalonia didirikan pada 1989 untuk mengumpulkan dan menerbitkan statistik regional secara mandiri dari kantor statistik nasional Spanyol.

---

### 2. Penekanan Berlebihan pada Keterkenalannya

**Kata-kata yang perlu diwaspadai:** diliput secara independen, media lokal/regional/nasional, ditulis oleh pakar terkemuka, kehadiran media sosial yang aktif

**Masalah:** AI memukul pembaca dengan klaim ketenaran, seringkali mencantumkan sumber tanpa konteks.

**Sebelum:**
> Pandangannya telah dikutip oleh Kompas, BBC Indonesia, Financial Times, dan The Hindu. Ia memiliki kehadiran media sosial yang aktif dengan lebih dari 500.000 pengikut.

**Sesudah:**
> Dalam wawancara Kompas 2024, ia berpendapat bahwa regulasi AI harus berfokus pada hasil, bukan metode.

---

### 3. Analisis Dangkal dengan Akhiran "-kan"/"-i" yang Dipaksakan

**Kata-kata yang perlu diwaspadai:** menyoroti..., menekankan..., mencerminkan..., melambangkan..., berkontribusi pada..., menumbuhkan..., menampilkan..., memastikan..., memperlihatkan...

**Masalah:** AI menambahkan frasa partisipat di akhir kalimat untuk memberi kedalaman palsu.

**Sebelum:**
> Palet warna candi yang terdiri dari biru, hijau, dan emas beresonansi dengan keindahan alam daerah tersebut, melambangkan bunga kebanggaan daerah, Laut Jawa, dan keragaman lanskap Nusantara, mencerminkan keterikatan mendalam komunitas dengan tanah airnya.

**Sesudah:**
> Candi ini menggunakan warna biru, hijau, dan emas. Arsitek menyatakan pilihan ini terinspirasi bunga daerah setempat dan garis pantai Jawa.

---

### 4. Bahasa Promosi dan Iklan

**Kata-kata yang perlu diwaspadai:** membanggakan, semarak, kaya (kiasan), mendalam, meningkatkan, menampilkan, menjadi contoh, komitmen terhadap, keindahan alam, tersembunyi di, di jantung, revolusioner, ternama, menakjubkan, wajib dikunjungi, memukau

**Masalah:** AI kesulitan menjaga nada netral, terutama untuk topik "warisan budaya."

**Sebelum:**
> Tersembunyi di kawasan Danau Toba yang menakjubkan, Desa Tomok berdiri sebagai desa yang semarak dengan warisan budaya yang kaya dan keindahan alam yang memukau.

**Sesudah:**
> Tomok adalah desa di tepi Danau Toba, dikenal dengan makam Raja Sidabutar dari abad ke-19 dan pertunjukan Sigale-gale.

---

### 5. Atribusi Kabur dan Kata Berputar-putar

**Kata-kata yang perlu diwaspadai:** laporan industri menunjukkan, para pengamat mencatat, para ahli berpendapat, beberapa kritikus berpendapat, beberapa sumber/publikasi (jika sumber sesungguhnya sedikit)

**Masalah:** AI mengaitkan opini ke otoritas yang kabur tanpa sumber spesifik.

**Sebelum:**
> Karena karakteristiknya yang unik, Sungai Musi menarik perhatian para peneliti dan pegiat lingkungan. Para ahli percaya sungai ini memainkan peran krusial dalam ekosistem regional.

**Sesudah:**
> Sungai Musi mendukung beberapa spesies ikan endemik, menurut survei 2019 oleh LIPI.

---

### 6. Bagian "Tantangan dan Prospek Masa Depan" yang Seperti Kerangka Skripsi

**Kata-kata yang perlu diwaspadai:** Terlepas dari... menghadapi berbagai tantangan..., Meski demikian/Terlepas dari tantangan ini, Tantangan dan Warisan, Prospek Masa Depan

**Masalah:** AI menyisipkan seksi "Tantangan" yang formulaik, diikuti kesimpulan optimis yang tidak berisi apa-apa.

**Sebelum:**
> Terlepas dari kemakmuran industrinya, Kawasan Industri Cikarang menghadapi berbagai tantangan khas kawasan urban, termasuk kemacetan dan krisis air bersih. Meski demikian, dengan lokasi strategis dan berbagai inisiatif yang sedang berjalan, kawasan ini terus berkembang sebagai bagian integral pertumbuhan Jabodetabek.

**Sesudah:**
> Kemacetan meningkat setelah 2018 ketika tiga pabrik besar beroperasi bersamaan. Pengelola kawasan memulai proyek drainase pada 2022 untuk mengatasi banjir rutin.

---

## POLA BAHASA INDONESIA YANG KHAS AI

### 7. Kata "AI Vocabulary" dalam Bahasa Indonesia

**Kata-kata frekuensi tinggi AI:** selain itu, sejalan dengan, krusial, menggali, menekankan, abadi, meningkatkan, menumbuhkan, memperoleh, menyoroti, interplay/keterkaitan yang rumit, intrinsik/intricacies, kata kunci, lanskap (kiasan), penting, menampilkan, permadani (kiasan), bukti, menggarisbawahi, berharga, semarak, tak terbantahkan, tak terelakkan, holistik, komprehensif, inovatif, transformatif, berkelanjutan (dalam konteks abstrak)

**Masalah:** Kata-kata ini muncul jauh lebih sering di teks pasca-2023. Sering muncul bersamaan.

**Sebelum:**
> Selain itu, fitur khas masakan Sunda adalah penggunaan lalapan segar. Bukti abadi pengaruh budaya Sunda yang kuat adalah diadopsinya karedok secara luas dalam lanskap kuliner nasional, menampilkan bagaimana hidangan-hidangan ini telah terintegrasi secara holistik ke dalam diet tradisional.

**Sesudah:**
> Masakan Sunda juga mengandalkan lalapan mentah, yang dimakan bersama sambal. Karedok, salad sayuran mentah dengan saus kacang, kini umum ditemukan di seluruh Indonesia, bukan hanya di Jawa Barat.

---

### 8. Penggunaan "Dalam Rangka" dan Frasa Birokratis Berlebihan

**Frasa yang perlu diwaspadai:** dalam rangka (mencapai/meningkatkan/mewujudkan), guna (meningkatkan/memastikan), demi tercapainya, dalam upaya untuk, dalam konteks ini, dalam hal ini, terkait dengan hal tersebut, sehubungan dengan itu

**Masalah:** AI sering menggunakan frasa birokratis panjang yang terdengar kaku dan formal secara berlebihan, padahal bisa disederhanakan.

**Sebelum:**
> Dalam rangka meningkatkan kualitas layanan publik, pemerintah daerah telah mengambil berbagai langkah strategis guna memastikan kepuasan masyarakat. Terkait dengan hal tersebut, berbagai program inovatif telah diluncurkan.

**Sesudah:**
> Pemda meluncurkan tiga program baru tahun ini untuk mempercepat layanan KTP dan izin usaha. Waktu tunggu turun dari 14 hari menjadi 3 hari.

---

### 9. Pengulangan Subjek yang Tidak Perlu (Synonym Cycling dalam BI)

**Masalah:** AI menghindari pengulangan kata dengan ganti sinonim berlebihan, yang justru membuat teks aneh dan tidak alami dalam Bahasa Indonesia.

**Sebelum:**
> Tokoh utama menghadapi banyak rintangan. Protagonis tersebut harus mengatasi berbagai hambatan. Figur sentral ini akhirnya berhasil. Sang pahlawan pun pulang ke rumah.

**Sesudah:**
> Tokoh utama menghadapi banyak rintangan, tapi akhirnya berhasil dan pulang ke rumah.

---

### 10. Penggunaan "Tidak Hanya... Tetapi Juga..." yang Berlebihan

**Masalah:** AI terlalu sering menggunakan konstruksi "tidak hanya X, tetapi juga Y" dan variannya untuk terkesan komprehensif.

**Sebelum:**
> Acara ini tidak hanya menawarkan sesi keynote yang inspiratif, tetapi juga menyediakan kesempatan networking yang berharga. Peserta tidak sekadar belajar, mereka juga bertumbuh. Ini bukan hanya tentang ilmu, melainkan tentang koneksi.

**Sesudah:**
> Acara ini menggabungkan sesi keynote dan waktu networking antar sesi.

---

### 11. Tiga Serangkai yang Dipaksakan (Rule of Three)

**Masalah:** AI memaksa ide masuk dalam kelompok tiga untuk terkesan komprehensif.

**Sebelum:**
> Acara ini menampilkan sesi keynote, diskusi panel, dan kesempatan networking. Peserta bisa mengharapkan inovasi, inspirasi, dan wawasan industri.

**Sesudah:**
> Acara ini berisi ceramah dan panel, plus waktu obrolan santai antar sesi.

---

### 12. Penggunaan Em Dash Berlebihan

**Masalah:** AI menggunakan em dash (—) jauh lebih sering dari manusia. Ini salah satu penanda paling mudah dikenali. **JANGAN gunakan em dash di output hasil humanisasi.** Ganti dengan koma, titik, atau tulis ulang kalimatnya.

**Sebelum (contoh pola salah dari input):**
> Istilah ini terutama dipromosikan oleh lembaga-lembaga pemerintah—bukan oleh masyarakatnya sendiri. Kamu tidak akan menulis "Jakarta, Asia Tenggara" sebagai alamat—namun kesalahan pelabelan ini terus berlanjut—bahkan dalam dokumen resmi.

**Sesudah:**
> Istilah ini terutama dipromosikan oleh lembaga pemerintah, bukan oleh masyarakatnya sendiri. Kamu tidak akan menulis "Jakarta, Asia Tenggara" sebagai alamat, tapi kesalahan pelabelan ini terus ada di dokumen resmi.

---

### 13. Penggunaan Huruf Tebal Berlebihan

**Masalah:** AI menebalkan frasa secara mekanis.

**Sebelum:**
> Sistem ini memadukan **OKR** (Objectives and Key Results), **KPI** (Key Performance Indicators), dan alat strategi visual seperti **Business Model Canvas** dan **Balanced Scorecard**.

**Sesudah:**
> Sistem ini memadukan OKR, KPI, dan alat strategi visual seperti Business Model Canvas dan Balanced Scorecard.

---

### 14. Daftar Vertikal dengan Header Inline

**Masalah:** AI membuat daftar dengan header tebal diikuti titik dua.

**Sebelum:**
> - **Pengalaman Pengguna:** Pengalaman pengguna telah ditingkatkan secara signifikan dengan antarmuka baru.
> - **Performa:** Performa telah ditingkatkan melalui algoritma yang dioptimalkan.
> - **Keamanan:** Keamanan telah diperkuat dengan enkripsi end-to-end.

**Sesudah:**
> Pembaruan ini memperbaiki antarmuka, mempercepat loading melalui algoritma baru, dan menambahkan enkripsi end-to-end.

---

### 15. Emoji sebagai Dekorasi

**Masalah:** AI sering menghias poin-poin atau judul dengan emoji.

**Sebelum:**
> 🚀 **Fase Peluncuran:** Produk diluncurkan di Q3 💡 **Wawasan Kunci:** Pengguna lebih menyukai kesederhanaan ✅ **Langkah Selanjutnya:** Jadwalkan rapat tindak lanjut

**Sesudah:**
> Produk diluncurkan Q3. Riset pengguna menunjukkan preferensi terhadap tampilan yang simpel. Langkah berikutnya: jadwalkan rapat tindak lanjut.

---

### 16. Artefak Komunikasi Chatbot

**Kata-kata yang perlu diwaspadai:** Tentu saja!, Pertanyaan bagus!, Kamu benar sekali!, Semoga membantu!, Beritahu saya jika..., Apakah kamu ingin..., Berikut adalah...

**Masalah:** Respons chatbot ikut terbawa ke dalam teks konten.

**Sebelum:**
> Pertanyaan bagus! Berikut adalah ikhtisar Revolusi Prancis. Semoga membantu! Beritahu saya jika kamu ingin saya memperluas bagian mana pun.

**Sesudah:**
> Revolusi Prancis dimulai pada 1789 ketika krisis keuangan dan kelangkaan pangan memicu kerusuhan meluas.

---

### 17. Penyangkalan Batas Pengetahuan

**Kata-kata yang perlu diwaspadai:** per [tanggal], hingga pembaruan pelatihan terakhir saya, Meskipun detail spesifiknya terbatas..., berdasarkan informasi yang tersedia...

**Masalah:** Penafian AI tentang informasi tidak lengkap ikut masuk ke dalam teks.

**Sebelum:**
> Meskipun detail spesifik tentang pendirian perusahaan tidak terdokumentasi secara luas dalam sumber yang mudah diakses, tampaknya perusahaan ini didirikan sekitar tahun 1990-an.

**Sesudah:**
> Perusahaan ini didirikan pada 1994, berdasarkan dokumen pendaftarannya.

---

### 18. Nada Sanjungan/Terlalu Menyenangkan

**Masalah:** Bahasa yang terlalu positif dan berusaha menyenangkan semua orang.

**Sebelum:**
> Pertanyaan yang sangat bagus! Kamu benar sekali bahwa ini adalah topik yang kompleks. Itu poin yang sangat tepat tentang faktor ekonominya.

**Sesudah:**
> Faktor ekonomi yang kamu sebutkan memang relevan di sini.

---

## PENGISI DAN HEDGING

### 19. Frasa Pengisi

**Sebelum → Sesudah:**
- "Dalam rangka mencapai tujuan ini" → "Untuk mencapai ini"
- "Dikarenakan oleh fakta bahwa hujan turun" → "Karena hujan"
- "Pada titik waktu ini" → "Sekarang"
- "Dalam hal kamu membutuhkan bantuan" → "Kalau butuh bantuan"
- "Sistem ini memiliki kemampuan untuk memproses" → "Sistem ini bisa memproses"
- "Penting untuk dicatat bahwa data menunjukkan" → "Data menunjukkan"
- "Tidak dapat dipungkiri bahwa" → hapus saja, lanjutkan langsung ke klaimnya
- "Hal ini tentunya" → hapus "tentunya"
- "Perlu diketahui bahwa" → hapus, lanjutkan langsung

---

### 20. Hedging Berlebihan

**Masalah:** Terlalu banyak kualifikasi.

**Sebelum:**
> Bisa jadi mungkin dapat diargumentasikan bahwa kebijakan tersebut mungkin memiliki beberapa dampak pada hasil.

**Sesudah:**
> Kebijakan ini kemungkinan berdampak pada hasil.

---

### 21. Kesimpulan Positif Generik

**Masalah:** Penutup yang samar-samar optimis.

**Sebelum:**
> Masa depan terlihat cerah bagi perusahaan ini. Waktu yang menggembirakan menanti saat mereka melanjutkan perjalanan menuju keunggulan. Ini merupakan langkah besar ke arah yang tepat.

**Sesudah:**
> Perusahaan berencana membuka dua lokasi baru tahun depan.

---

## Proses

1. Baca teks masukan dengan cermat
2. Identifikasi semua pola di atas
3. Tulis ulang setiap bagian bermasalah
4. Pastikan teks yang direvisi:
   - Terdengar natural saat dibaca keras
   - Memvariasikan struktur kalimat secara alami
   - Menggunakan detail spesifik, bukan klaim kabur
   - Menjaga tone sesuai konteks
   - Menggunakan konstruksi sederhana (adalah/merupakan/memiliki) jika memungkinkan
5. Sajikan draft hasil humanisasi
6. Tanyakan: *"Apa yang membuat teks ini masih terasa seperti buatan AI?"*
7. Jawab singkat dengan tanda-tanda yang tersisa (jika ada)
8. Tanyakan: *"Sekarang buat agar tidak terkesan buatan AI."*
9. Sajikan versi final (setelah direvisi)

---

## Format Output

Berikan:
1. **Draft tulisan ulang**
2. **"Apa yang masih terasa seperti buatan AI?"** (poin singkat)
3. **Versi final**
4. **Ringkasan perubahan** (opsional, jika membantu)

---

## Contoh Lengkap

**Sebelum (bernada AI):**
> Pertanyaan bagus! Berikut adalah esai tentang topik ini. Semoga membantu!
>
> Pengkodean berbantuan AI merupakan bukti abadi dari potensi transformatif large language model, menandai momen penting dalam evolusi pengembangan perangkat lunak. Dalam lanskap teknologi yang terus berkembang pesat saat ini, alat-alat revolusioner ini,tersembunyi di persimpangan antara riset dan praktik,sedang membentuk ulang cara insinyur berideasi, melakukan iterasi, dan menghasilkan produk, menggarisbawahi peran vitalnya dalam alur kerja modern.
>
> Pada intinya, proposisi nilai sudah jelas: merampingkan proses, meningkatkan kolaborasi, dan menumbuhkan keselarasan. Ini bukan hanya tentang autocomplete; ini tentang membuka kreativitas dalam skala besar, memastikan organisasi bisa tetap lincah. Alat ini berfungsi sebagai katalis. Asisten ini berperan sebagai mitra. Sistem ini berdiri sebagai fondasi inovasi.
>
> Para pengamat industri mencatat bahwa adopsi telah berakselerasi dari eksperimen hobi hingga peluncuran skala perusahaan. Teknologi ini telah diliput oleh Kompas, Wired, dan The Verge. Selain itu, kemampuan menghasilkan dokumentasi, tes, dan refactor menampilkan bagaimana AI dapat berkontribusi pada hasil yang lebih baik, menyoroti keterkaitan intrinsik antara otomasi dan penilaian manusia.
>
> - 💡 **Kecepatan:** Pembuatan kode jauh lebih cepat, mengurangi hambatan dan memberdayakan pengembang.
> - 🚀 **Kualitas:** Kualitas output telah ditingkatkan melalui pelatihan yang lebih baik, berkontribusi pada standar yang lebih tinggi.
> - ✅ **Adopsi:** Penggunaan terus tumbuh, mencerminkan tren industri yang lebih luas.
>
> Meskipun detail spesifisnya terbatas berdasarkan informasi yang tersedia, bisa jadi mungkin dapat diargumentasikan bahwa alat-alat ini mungkin memiliki beberapa dampak positif. Terlepas dari tantangan khas teknologi yang berkembang,termasuk halusinasi, bias, dan akuntabilitas,ekosistem ini terus berkembang pesat. Dalam rangka mewujudkan potensi ini sepenuhnya, tim harus sejalan dengan praktik terbaik.
>
> Kesimpulannya, masa depan terlihat cerah. Waktu-waktu menggembirakan menanti saat kita melanjutkan perjalanan menuju keunggulan ini. Beritahu saya jika kamu ingin saya memperluas bagian mana pun!

**Draft tulisan ulang:**
> Asisten koding AI mempercepat beberapa tugas. Dalam studi 2024 oleh Google, pengembang yang menggunakan Codex menyelesaikan fungsi sederhana 55% lebih cepat dari kelompok kontrol, tapi tidak menunjukkan perbaikan dalam debugging atau keputusan arsitektur.
>
> Alat ini bagus untuk boilerplate: file konfigurasi, scaffolding tes, refactor berulang. Mereka buruk dalam mengetahui kapan mereka salah. Saya pernah menerima saran massal yang berhasil dikompilasi, lolos lint, tapi tetap melakukan hal yang salah karena saya berhenti memperhatikan.
>
> Pengembang yang saya ajak bicara cenderung terbagi dua. Ada yang menggunakannya seperti autocomplete untuk kode membosankan tapi meninjau setiap baris sebelum commit. Yang lain menonaktifkannya setelah terus-menerus mendapat saran dari library internal yang sudah tidak dipakai.
>
> Klaim produktivitas sulit diverifikasi. GitHub bilang pengguna Copilot "menerima 30% saran," tapi penerimaan bukan berarti benar, dan benar bukan berarti berharga. Studi Uplevel 2024 tidak menemukan perbedaan signifikan dalam throughput pull-request antara tim dengan dan tanpa asisten AI.
>
> Ini tidak berarti alatnya tidak berguna. Artinya mereka adalah alat. Mereka tidak menggantikan penilaian, dan tidak menghilangkan kebutuhan akan tes.

**Apa yang masih terasa seperti buatan AI?**
- Ritme masih terlalu rapi - kontras bersih, paragraf berpanjangan sama
- Kutipan studi terasa seperti placeholder masuk akal kalau tidak benar-benar diverifikasi
- Kalimat penutup terasa sedikit seperti slogan

**Versi final:**
> Asisten koding AI bisa bikin kamu lebih cepat di bagian-bagian yang membosankan. Bukan semuanya. Apalagi untuk arsitektur sistem.
>
> Bagusnya untuk boilerplate: file konfigurasi, scaffolding tes, refactor berulang. Jeleknya, mereka juga jago terdengar benar padahal salah. Saya pernah asal terima saran yang dikompilasi, lolos lint, tapi tetap miss the point karena saya tidak lagi memperhatikan.
>
> Orang-orang yang saya ajak bicara biasanya jatuh di dua kubu. Ada yang pakai seperti autocomplete untuk kerjaan rutin dan review setiap baris. Ada yang langsung nonaktifkan setelah terus-menerus mendapat saran yang tidak mereka mau. Keduanya terdengar masuk akal.
>
> Metrik produktivitasnya licin. GitHub bisa bilang pengguna Copilot "menerima 30% saran," tapi penerimaan bukan berarti benar, dan benar bukan berarti ada nilainya. Kalau tidak ada tes, kamu pada dasarnya nebak.

---

## Referensi

Skill ini mengadaptasi [Wikipedia:Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing), dikelola oleh WikiProject AI Cleanup, dan diperluas dengan pola AI khas Bahasa Indonesia berdasarkan observasi terhadap ribuan teks berbahasa Indonesia yang dihasilkan AI.

Wawasan kunci: "LLM menggunakan algoritma statistik untuk menebak apa yang harus datang selanjutnya. Hasilnya cenderung ke arah hasil yang paling mungkin secara statistik yang berlaku untuk berbagai kasus seluas mungkin."