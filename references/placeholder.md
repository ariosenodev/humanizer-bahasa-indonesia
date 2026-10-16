# Placeholder: cara menandai bagian yang butuh isi user

Saat membuat dokumen untuk user, ada bagian yang TIDAK BISA diisi oleh
assistant (logo kampus, tanda tangan, data pribadi, hasil penelitian nyata).
JANGAN mengarang isinya, dan JANGAN diam-diam mengosongkan. Pakai placeholder
visual yang jelas, supaya user langsung tahu bagian mana yang harus dia isi.

## Aturan

1. Bagian yang butuh isi user = kotak putus-putus merah dengan teks italic.
2. Teks di dalamnya WAJIB menjelaskan apa yang harus diisi, bukan cuma "diisi".
3. Setiap dokumen placeholder diakhiri catatan singkat: daftar bagian yang
   masih placeholder.
4. Setelah user mengirim isi penggantinya, placeholder diganti permanen.
5. Jangan lebih dari 3-4 placeholder per dokumen. Kalau lebih, dokumen itu
   berarti belum layak diserahkan; tanya user lebih dulu.

## CSS standar

```css
.ph {
  border: 2px dashed #b32020;
  background: #fff5f5;
  color: #b32020;
  text-align: center;
  font-size: 11px;
  padding: 10px 8px;
  border-radius: 6px;
  margin: 8px 0;
  font-style: italic;
}
```

## Contoh pemakaian

```html
<!-- Logo sampul -->
<div class="ph" style="width:120px;height:120px;margin:0 auto 10px;line-height:120px;padding:0">
  isi disini<br>logo universitasmu
</div>

<!-- Tanda tangan -->
<div class="ph">tanda tangan + nama pembimbing diisi manual setelah print</div>

<!-- Data yang tidak assistant ketahui -->
<div class="ph">abstrak / bagian yang gue gatau isinya → diisi user</div>
```

## Kapan placeholder vs bertanya

- Data yang WAJIB dan cuma user yang tahu (NIM, nama dosen, logo) → pakai
  placeholder dulu, serahkan dokumen, user isi kapan saja. Jangan blokir.
- Data yang mengubah SELURUH isi dokumen (jenis tugas salah paham, topik
  salah) → bertanya sebelum membuat, jangan placeholder.

## Kapan TIDAK boleh placeholder

- Hasil eksekusi kode: jalankan beneran, jangan placeholder.
- Angka analisis: hitung, jangan placeholder.
- Kesimpulan: tulis, jangan placeholder.
Placeholder hanya untuk data yang secara prinsip berada di luar jangkauan
assistant (aset fisik, identitas, data lapangan user).
