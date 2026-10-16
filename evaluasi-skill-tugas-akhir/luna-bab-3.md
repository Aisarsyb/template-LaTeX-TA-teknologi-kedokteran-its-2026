# BAB III METODOLOGI

> **Konteks simulasi:** Naskah ini menguji penerapan skill penulisan, bukan melaporkan penelitian nyata. Data empat pengukuran berpasangan yang dicantumkan merupakan data simulasi eksplisit. Bab 1–3 diposisikan sebagai rancangan; bila contoh hasil ditampilkan pada Bab 4–5, hasil itu harus tetap diberi label simulasi dan tidak boleh diperlakukan sebagai bukti klinis.

## Diagram Alir Penelitian

Penelitian dirancang sebagai evaluasi teknis deskriptif terhadap selisih pembacaan saturasi oksigen perifer (SpO₂) antara purwarupa dan alat pembanding pada kondisi diam. Alur kerja yang direncanakan ialah penetapan protokol dan kelengkapan alat, pencatatan pembacaan berpasangan, pemeriksaan kelengkapan pasangan, penghitungan selisih setiap pasangan, lalu penafsiran hasil sesuai batas pengujian teknis. Alur tersebut tidak mencakup penilaian diagnosis, keselamatan pasien, atau manfaat klinis.

**Alur rancangan:** protokol dan alat ditetapkan → pembacaan purwarupa dan pembanding dicatat berpasangan pada kondisi diam → pasangan data diperiksa → selisih pembacaan dihitung → hasil deskriptif ditafsirkan dengan batas pengujian teknis.

Data yang tersedia untuk simulasi terdiri atas empat pasangan. Jumlah peserta maupun sumber setiap pasangan tidak diketahui, sehingga empat pasangan tidak dapat disebut sebagai empat peserta atau mewakili kelompok tertentu. Prosedur perekrutan, pengulangan pembacaan, urutan penggunaan alat, dan cara memastikan kondisi diam perlu ditetapkan sebelum pelaksanaan nyata.

## Bahan dan Peralatan

Bahan pengukuran yang disebut dalam rancangan ialah pembacaan SpO₂ dari purwarupa dan alat pembanding. Jenis dan spesifikasi sensor purwarupa, model serta status kalibrasi alat pembanding, perangkat pencatat, perangkat lunak, dan kondisi lingkungan pengukuran belum tersedia. Informasi tersebut tidak diisi dengan perkiraan karena dapat memengaruhi keterulangan dan penafsiran hasil.

Untuk penelitian nyata, kedua alat perlu diidentifikasi hingga model dan spesifikasinya, termasuk sumber keluaran SpO₂ dan satuan tampilannya. Tanpa informasi itu, uraian ini hanya menetapkan jenis data yang dibandingkan, belum menjadi petunjuk teknis yang cukup untuk mereplikasi pengukuran.

## Perancangan Sistem

### Arsitektur dan Diagram Blok Sistem

Evaluasi ini tidak merancang sistem klinis baru; objek yang dibandingkan ialah keluaran SpO₂ purwarupa dan alat pembanding. Secara konseptual, kedua keluaran dicatat sebagai satu pasangan pada setiap pengukuran, kemudian pasangan dianalisis menggunakan selisih absolut. Alur konseptualnya adalah: **purwarupa dan alat pembanding → pencatatan nilai berpasangan → penghitungan selisih → ringkasan deskriptif**. Tidak tersedia rincian antarmuka, jalur akuisisi sinyal, atau pengolahan internal purwarupa, sehingga komponen tersebut tidak diasumsikan.

### Tahapan Implementasi

Rancangan pengujian menetapkan kondisi diam agar perbandingan dilakukan pada kondisi yang dinyatakan sama untuk semua pasangan. Pada pelaksanaan nyata, protokol harus menjelaskan definisi operasional kondisi diam, cara memasang sensor, waktu tunggu sebelum pencatatan, cara menyelaraskan waktu pembacaan kedua alat, dan penanganan pembacaan yang tidak terbaca. Rincian tersebut belum diberikan; karena itu, naskah ini tidak menetapkan durasi, posisi sensor, atau aturan pengulangan.

Data simulasi disusun sebagai pasangan nilai berikut. Tabel ini hanya memperlihatkan data simulasi yang diberikan, bukan hasil pengukuran nyata.

| Pasangan simulasi | Alat pembanding (% SpO₂) | Purwarupa (% SpO₂) | Selisih absolut (poin persentase) |
|---:|---:|---:|---:|
| 1 | 96 | 95 | 1 |
| 2 | 97 | 97 | 0 |
| 3 | 98 | 97 | 1 |
| 4 | 99 | 100 | 1 |

## Prosedur Pengujian dan Evaluasi

Tujuan evaluasi ialah menilai besar selisih pembacaan SpO₂ purwarupa terhadap alat pembanding dan menetapkan batas makna hasil sebagai pengujian teknis. Untuk setiap pasangan, selisih absolut dihitung sebagai nilai mutlak pembacaan purwarupa dikurangi pembacaan alat pembanding. Rerata selisih absolut dihitung dengan menjumlahkan selisih absolut seluruh pasangan lalu membaginya dengan jumlah pasangan. Ukuran ini dipilih untuk merangkum besar perbedaan tanpa membiarkan arah positif dan negatif saling meniadakan; satuannya ialah poin persentase SpO₂.

Pada data simulasi yang diberikan, selisih absolut tiap pasangan adalah 1, 0, 1, dan 1 poin persentase, sehingga reratanya 0,75 poin persentase. Angka tersebut merupakan ringkasan aritmetika dari empat pasangan simulasi, bukan estimasi hasil penelitian nyata. Analisis deskriptif ini sesuai untuk menggambarkan data contoh yang tersedia; empat pasangan tanpa informasi peserta, spesifikasi alat, dan prosedur terverifikasi tidak cukup untuk menyimpulkan ketepatan klinis, kesetaraan alat, kinerja pada populasi, atau kelayakan pemakaian pada pasien. Tidak ditetapkan ambang penerimaan karena sumber atau dasar klinis untuk ambang tersebut tidak tersedia.

Dalam pelaksanaan nyata, pencatatan harus mempertahankan pasangan nilai dan satuan yang sama, serta menyimpan informasi yang diperlukan untuk mengaudit sumber data tanpa mencantumkan identitas pasien pada naskah. Status izin etik dan persetujuan belum diketahui; status tersebut tidak dapat dinyatakan telah diperoleh ataupun tidak diperlukan. Kebutuhan izin, persetujuan, dan perlindungan data harus ditentukan berdasarkan sumber data serta ketentuan institusi sebelum pengumpulan data nyata.

## Jadwal Kegiatan

Tanggal dan rentang pelaksanaan belum tersedia, sehingga jadwal bertanggal tidak dapat disusun secara faktual. Urutan kegiatan yang perlu dijadwalkan setelah protokol dan persyaratan etik ditetapkan meliputi penelaahan sumber, penetapan protokol dan spesifikasi alat, pelaksanaan pengukuran, pemeriksaan serta analisis data, dan penyusunan laporan. Urutan ini adalah kerangka kegiatan, bukan catatan bahwa kegiatan tersebut telah dilakukan.

## Fakta yang Belum Tersedia

Jumlah peserta dan sumber empat pasangan pengukuran; kriteria inklusi; status serta kebutuhan izin etik dan persetujuan; spesifikasi sensor dan purwarupa; identitas, spesifikasi, dan status kalibrasi alat pembanding; rincian protokol pengukuran dan pencatatan; sumber studi relevan untuk Bab 2; tanggal dan jadwal pelaksanaan; serta data pasien tidak tersedia. Karena sumber literatur relevan belum diberikan, Bab 2 tidak boleh menyatakan dukungan penelitian terdahulu atau ambang klinis tertentu tanpa verifikasi sumber. Data simulasi di atas tidak memuat dan tidak boleh ditafsirkan sebagai data pasien.