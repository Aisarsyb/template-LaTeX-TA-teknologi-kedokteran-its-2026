# Template LaTeX Seminar Proposal (Sempro) — Teknologi Kedokteran ITS 2026

[![GitHub repo](https://img.shields.io/badge/GitHub-Aisarsyb-181717.svg?logo=github)](https://github.com/Aisarsyb/template-Latex-sempro-teknologi-kedokteran-its-2026)
[![LaTeX](https://img.shields.io/badge/LaTeX-pdflatex-008080.svg?logo=latex)](https://www.latex-project.org/)
[![ITS](https://img.shields.io/badge/Institusi-ITS%20Surabaya-003366.svg)](https://www.its.ac.id/)
[![Departemen](https://img.shields.io/badge/Departemen-Teknologi%20Kedokteran-crimson.svg)](https://www.its.ac.id/)
[![Fakultas](https://img.shields.io/badge/Fakultas-Kedokteran%20dan%20Kesehatan%20(FKK)-blue.svg)](https://www.its.ac.id/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)

Template [LaTeX](https://www.latex-project.org/) resmi untuk penulisan **Seminar Proposal (Sempro) Tugas Akhir** yang telah dikonfigurasi khusus untuk mahasiswa **Departemen Teknologi Kedokteran**, **Fakultas Kedokteran dan Kesehatan (FKK)**, **Institut Teknologi Sepuluh Nopember (ITS) Surabaya** tahun 2026.

Template ini mencakup struktur inti Sempro: **Bab I (Pendahuluan)**, **Bab II (Tinjauan Pustaka)**, **Bab III (Metodologi)**, serta **Daftar Pustaka** dan lembar administrasi resmi (Sampul & Lembar Pengesahan Proposal). Format mengacu pada pedoman tugas akhir ITS (*SK Rektor ITS No. 280 Tahun 2022*) dengan layout naskah terkini.

---

## ✨ Kepatuhan Terhadap Pedoman Resmi ITS (SK Rektor No. 280/2022)

1. **Preset Lengkap Departemen & Program Studi**:
   - Program Studi: `Teknologi Kedokteran`
   - Departemen: `Teknologi Kedokteran`
   - Fakultas: `Kedokteran dan Kesehatan` (`FKK`)
   - Kode Mata Kuliah: `KT234801` (Proposal Tugas Akhir)
2. **Sampul Resmi Proposal Sempro (Lampiran 1)**:
   - Menggunakan format dasar kertas putih dengan pita biru horizontal khas ITS 10 mm (`sampul-luar-tipis.tex`).
   - Menyediakan opsi peralihan mudah jika ingin digunakan untuk *Buku Tugas Akhir Final Hardcover* (`sampul-luar.tex` / Lampiran 6).
3. **Format Judul Bab Terstandar (Subbab 3.2.i)**:
   - Judul bab dicetak tebal, simetris di tengah (*centered*), dengan nomor bab angka Romawi di baris pertama dan judul bab di baris berikutnya (dua baris terpisah sesuai pedoman).
4. **Penomoran Halaman Presisi (Subbab 2.1 & 3.2.f)**:
   - Nomor halaman Romawi kecil (`ii, iii, ...`) di kanan bawah dimulai dari Lembar Pengesahan (halaman sampul terhitung halaman `i` tanpa dicetak).
   - Penomoran angka Arab (`1, 2, ...`) di kanan bawah dimulai dari Bab I Pendahuluan.
5. **Format Caption Gambar & Tabel**:
   - Penomoran dua bagian (**Gambar 3.1.** / **Tabel 3.1.**) dengan judul tabel di atas dan judul gambar di bawah.
6. **Manajemen Sitasi & Bibliografi Standar APA Edisi ke-7**:
   - Menggunakan `biblatex` dengan backend `biber` dan format resmi APA 7th edition (`style=apa`).
7. **Dukungan Lingkungan Kerja Lengkap**:
   - Siap pakai di **Visual Studio Code** dengan ekstensi *LaTeX Workshop* (konfigurasi `.vscode/settings.json` sudah disediakan).
   - Mendukung kompilasi otomatis melalui **GitHub Actions** CI/CD (`.github/workflows/ci.yaml`).
   - Dapat diimpor langsung ke **Overleaf**.

---

## 📁 Struktur Direktori

```text
template-ta-teknologi-kedokteran-its/
├── .github/workflows/       # Otomasi build GitHub Actions (CI/CD)
├── .vscode/                 # Konfigurasi ekstensi LaTeX Workshop VS Code
├── abstrak/                 # Berkas abstrak (Indonesia & Inggris)
│   ├── abstrak-id.tex
│   └── abstrak-en.tex
├── bab/                     # Berkas isi bab naskah
│   ├── 1-pendahuluan.tex
│   ├── 2-tinjauan-pustaka.tex
│   ├── 3-metodologi.tex
│   ├── 4-pengujian-analisis.tex
│   └── 5-penutup.tex
├── gambar/                  # Berkas grafik, diagram, dan foto
├── lainnya/                 # Lembar pengesahan, kata pengantar, dll.
│   ├── lembar-pengesahan.tex
│   └── lembar-pengesahan-en.tex
├── program/                 # Berkas kode sumber lampiran (Python/C++)
├── pustaka/                 # Daftar pustaka & konfigurasi variabel
│   ├── pustaka.bib          # Basis data referensi BibTeX
│   ├── tanda-hubung.tex     # Penyesuaian pemenggalan kata Indonesia
│   └── variables.tex        # DATA PRIBADI (Nama, NRP, Dosen, Judul)
├── sampul/                  # Halaman sampul luar & dalam
├── .gitignore               # Mengabaikan berkas build (*.aux, *.log, *.pdf, dll)
├── LICENSE                  # Lisensi MIT
├── main.tex                 # Berkas utama dokumen LaTeX
└── README.md                # Dokumentasi petunjuk penggunaan
```

---

## 🚀 Panduan Penggunaan Cepat

### Langkah 1: Kloning Repositori
```bash
git clone https://github.com/Aisarsyb/template-Latex-sempro-teknologi-kedokteran-its-2026.git
cd template-Latex-sempro-teknologi-kedokteran-its-2026
```

### Langkah 2: Sesuaikan Variabel Dokumen
Buka berkas [`pustaka/variables.tex`](./pustaka/variables.tex) dan ubah data berikut sesuai data Anda:
- `\name{...}`: Nama lengkap mahasiswa
- `\nrp{...}`: Nomor Pokok Mahasiswa (NRP)
- `\advisor{...}` & `\advisornip{...}`: Nama dan NIP Dosen Pembimbing Utama
- `\coadvisor{...}` & `\coadvisornip{...}`: Nama dan NIP Dosen Pembimbing Kedua
- `\tatitle{...}`: Judul naskah dalam Bahasa Indonesia
- `\engtatitle{...}`: Judul naskah dalam Bahasa Inggris

### Langkah 3: Menulis Isi Naskah
Tuliskan isi naskah Anda pada berkas-berkas di folder [`bab/`](./bab/):
- **Bab I**: Latar Belakang, Rumusan Masalah, Batasan Masalah, Tujuan, Manfaat, Sistematika Penulisan.
- **Bab II**: Tinjauan Pustaka, Penelitian Terdahulu, Dasar Teori.
- **Bab III**: Diagram Alir Penelitian, Perancangan Sistem / Alat, Protokol Pengujian.
- **Bab IV**: Hasil Pengujian dan Analisis.
- **Bab V**: Kesimpulan dan Saran.

### Langkah 4: Menambahkan Referensi
Masukkan referensi sitasi dalam format BibTeX ke dalam berkas [`pustaka/pustaka.bib`](./pustaka/pustaka.bib). Sitasi di naskah menggunakan perintah `\textcite{kunci_sitasi}` atau `\parencite{kunci_sitasi}`.

---

## 🛠️ Cara Kompilasi Dokumen

### 1. Menggunakan Visual Studio Code (Sangat Disarankan)
1. Pasang ekstensi **LaTeX Workshop** dari James-Yu.
2. Buka folder template ini di VS Code.
3. Buka berkas `main.tex`.
4. Tekan `Ctrl + Alt + B` untuk mengompilasi naskah (resep `pdflatex ➞ biber ➞ pdflatex × 2` akan berjalan otomatis).
5. Tekan `Ctrl + Alt + V` untuk membuka pratinjau PDF.

### 2. Menggunakan Terminal / CLI
Jalankan perintah berikut di dalam direktori proyek:
```bash
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
```

### 3. Menggunakan Overleaf
1. Unduh seluruh folder repositori ini sebagai berkas `.zip`.
2. Buka [Overleaf](https://www.overleaf.com/) dan pilih **New Project** > **Upload Project**.
3. Pastikan pengaturan *Compiler* diatur ke **pdfLaTeX** dan *TeX Live version* terbaru.

---

## 💡 Tips & Panduan Penulisan

- **Menyisipkan Gambar**:
  Gunakan penentu posisi `[H]` agar posisi gambar tidak berpindah mendahului subbab berikutnya:
  ```latex
  \begin{figure}[H]
    \centering
    \includegraphics[width=0.8\textwidth]{gambar/nama-gambar.png}
    \caption{Keterangan Gambar Anda}
    \label{fig:labelgambar}
  \end{figure}
  ```
- **Istilah Asing**: Gunakan perintah `\emph{istilah}` untuk memformat teks miring (*italic*).
- **Tanda Hubung Dokter–Pasien**: Gunakan `dokter--pasien` (dua strip) untuk tanda pisah en-dash yang rapi.

---

## 📄 Lisensi

Berkas template ini dilisensikan di bawah [MIT License](./LICENSE). Silakan gunakan, bagikan, dan kembangkan untuk kebutuhan akademik mahasiswa Departemen Teknologi Kedokteran ITS.
