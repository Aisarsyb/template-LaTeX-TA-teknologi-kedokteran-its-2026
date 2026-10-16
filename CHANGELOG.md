# Changelog

## Unreleased

### Distribusi skill
- Sumber template dipindah ke `skills/tugas-akhir/template/` agar pengguna dapat memasang skill dan membuat proyek di folder kerja sendiri tanpa clone manual.
- Skill meminta izin sebelum menyalin template, membantu penulisan berbasis data pengguna, dan membangun PDF setelah satu permintaan penulisan selesai.
- README dan CI mengikuti lokasi baru; panduan instalasi serta contoh pemakaian ditambahkan.

### Abstrak
- Identitas abstrak Indonesia dan Inggris memakai tabel tanpa border, seluruh teks tebal, dengan jarak 1ex antarbaris.
- Nama pembimbing ditampilkan sebagai placeholder pembimbing utama; isi kata kunci dicetak tebal dan miring.
- Token `\paragraphtextstyle` diterapkan pada isi abstrak kedua bahasa; teks abstrak Inggris menggunakan gaya normal, bukan miring.
- Token paragraf juga diterapkan secara eksplisit pada Bab 1–5 dan daftar pustaka di semua dokumen utama.
- Jarak 1ex setelah heading abstrak; jarak setelah judul, setelah tabel identitas, dan sebelum kata kunci memakai `\baselineskip`.

### Daftar berpoin
- Token `\listtextstyle` meniadakan jarak sebelum daftar dan antarbutir, lalu mempertahankan jarak paragraf setelah daftar.

### Sampul
- Sampul luar dan sampul dalam bahasa Indonesia kini memakai satu sumber konten, `sampul/konten-id.tex`; duplikat `sampul/konten-luar.tex` dihapus. Sampul bahasa Inggris di `sampul/konten-en.tex` diselaraskan dengan susunan yang sama.
- Tipografi sampul memakai bobot normal sebagai dasar; baris yang perlu tebal ditandai secara khusus.
- Teks sampul luar dan dalam menggunakan Trebuchet MS lewat XeLaTeX; empat berkas `.ttf` tersedia di `fonts/` tanpa memerlukan pemasangan font sistem.

### Lembar pengesahan
- Lembar pengesahan bahasa Indonesia dan Inggris disusun ulang agar menampilkan judul, informasi mahasiswa, keterangan persetujuan, lima baris pihak yang menyetujui, dan lokasi serta tanggal.
- Tabel lima baris tidak memakai border; jarak antarbaris dan posisi kolom dirapatkan.
- Nama mahasiswa dicetak tebal dan huruf kapital. Label `Oleh:`, `By:`, dan NRP tetap normal.

### Token gaya teks
- Definisi Heading 1–4, caption Gambar dan Tabel, serta paragraf dipusatkan di `pustaka/gaya-teks.tex` dan digunakan oleh `main.tex`, `sempro.tex`, serta `buku-ta.tex`.
- Heading 1 menggunakan 14 pt tebal, kapital, dan rata tengah; Heading 2 memakai 13 pt tebal; Heading 3–4 memakai 12 pt tebal.
- Caption Gambar dan Tabel menggunakan 10 pt normal, rata tengah, dengan jarak setelah caption.
- Token `\paragraphtextstyle` menetapkan teks normal 12 pt, indentasi baris pertama, perataan kiri-kanan, dan jarak setelah paragraf. Teks utama memakai Times New Roman dari `fonts/`; `txfonts` tetap menyediakan simbol matematika.

### Daftar awal
- `pustaka/daftar-awal.tex` menyatukan daftar isi, daftar gambar, daftar tabel, dan daftar simbol. Ketiga dokumen utama memakai berkas yang sama.
- Isi daftar menggunakan 11 pt normal, dengan jarak setelah entri; daftar simbol mencantumkan gaya, kecepatan, dan waktu dari persamaan contoh.
- Lembar pengesahan ditambahkan sebagai entri daftar isi.
