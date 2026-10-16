# BAB 4 HASIL DAN PEMBAHASAN

Bab ini menyajikan hasil pengujian simulasi perbandingan pembacaan saturasi oksigen ($SpO_2$) antara purwarupa instrumen dan alat pembanding, serta analisis batas makna teknis dari data yang diperoleh. Seluruh data dan angka yang disajikan merupakan hasil studi simulasi eksplisit untuk menguji kerangka metodologi penelitian tugas akhir, bukan hasil uji klinis nyata pada manusia ataupun pasien di fasilitas pelayanan kesehatan. Pembahasan diarahkan secara kritis dari sudut pandang medis untuk menilai deviasi pengukuran perangkat pada kondisi statis serta menguraikan keterbatasan mendasar hasil pengujian laboratorium terhadap klaim diagnostik klinis.

## 4.1 Skenario Pengujian

Skenario pengujian dirancang untuk mengevaluasi konsistensi pembacaan purwarupa instrumen oksimeter nadi secara langsung terhadap alat pembanding melalui metode pengukuran berpasangan (*paired measurement*). Pengujian dilakukan pada empat titik pengukuran berpasangan dalam kondisi diam (*resting condition*). Kondisi diam dipilih secara sengaja dalam skenario awal ini untuk mengeliminasi gangguan gerak (*motion artifact*) dan fluktuasi hemodinamika jaringan perifer yang kerap memicu pergeseran posisi sensor optik maupun perubahan aliran pulsasi kapiler darah. Dengan meniadakan gerakan subjek, pengujian dapat berfokus murni pada evaluasi respons teknis elektro-optik dasar sistem dalam mengonversi sinyal serapan cahaya menjadi persentase saturasi oksigen.

Kedua perangkat diposisikan untuk mencatat nilai $SpO_2$ secara berpasangan pada kondisi pengukuran yang sama. Instrumen pembanding berfungsi sebagai rujukan nilai ukur, sementara purwarupa dievaluasi kemampuannya dalam menghasilkan pembacaan yang mendekati rujukan tersebut. Karena penelitian ini berstatus studi simulasi, pengujian tidak melibatkan subjek uji manusia nyata, kriteria inklusi medis, penetapan tanggal dan durasi waktu riil, maupun variasi kondisi fisik fisiologis tertentu. Prosedur ini difokuskan sebagai simulasi pengujian komparatif terarah untuk memverifikasi fungsionalitas algoritma pembacaan sebelum perangkat melangkah ke tahap pengujian yang lebih kompleks.

## 4.2 Evaluasi Pengujian

Evaluasi hasil pengujian dilakukan secara kuantitatif dengan menghitung selisih pembacaan individual pada setiap pasangan data serta selisih absolut rerata (*mean absolute difference* atau MAD). Selisih pembacaan individual ($d_i$) dihitung melalui pengurangan nilai purwarupa terhadap nilai alat pembanding ($SpO_{2,\text{purwarupa}} - SpO_{2,\text{pembanding}}$). Hasil pembacaan dari empat titik pengukuran berpasangan simulasi dirangkum pada Tabel 4.1.

Tabel 4.1 Hasil Pengukuran Berpasangan dan Evaluasi Selisih Pembacaan $SpO_2$ Simulasi

| Titik Pengukuran | Alat Pembanding (%) | Purwarupa (%) | Selisih Pembacaan (poin persentase) | Selisih Absolut (poin persentase) |
| :---: | :---: | :---: | :---: | :---: |
| 1 | 96 | 95 | -1 | 1 |
| 2 | 97 | 97 | 0 | 0 |
| 3 | 98 | 97 | -1 | 1 |
| 4 | 99 | 100 | +1 | 1 |

Berdasarkan data pada Tabel 4.1, pembacaan alat pembanding mencakup rentang 96% hingga 99%, sedangkan pembacaan purwarupa berada pada rentang 95% hingga 100%. Pada titik pengukuran pertama, purwarupa menunjukkan nilai 95% dibandingkan pembanding 96%, menghasilkan selisih sebesar -1 poin persentase. Pada titik kedua, kedua perangkat menghasilkan nilai identik sebesar 97% dengan selisih 0 poin persentase. Pada titik ketiga, purwarupa membaca 97% saat pembanding berada pada 98%, menghasilkan selisih -1 poin persentase. Pada titik keempat, purwarupa menunjukkan pembacaan 100% terhadap pembanding 99%, menghasilkan selisih sebesar +1 poin persentase. Perhitungan selisih absolut rerata dari keempat titik pengukuran ini menghasilkan nilai sebesar 0,75 poin persentase.

Pemilihan metrik selisih absolut rerata memberikan gambaran yang lebih objektif dibandingkan rata-rata aljabar biasa. Jika selisih dihitung menggunakan rata-rata aljabar, penyimpangan negatif pada titik pertama dan ketiga (-1 dan -1) akan saling meniadakan dengan penyimpangan positif pada titik keempat (+1), sehingga menghasilkan estimasi deviasi yang mengecil semu (-0,25 poin persentase). Dengan menerapkan nilai mutlak pada setiap deviasi (1, 0, 1, dan 1), akumulasi penyimpangan sebesar 3 poin persentase dibagi empat pengukuran menghasilkan rerata deviasi aktual sebesar 0,75 poin persentase terhadap alat rujukan.

Meskipun nilai selisih absolut rerata sebesar 0,75 poin persentase tampak relatif kecil, interpretasi terhadap angka ini memerlukan analisis batas makna teknis yang ketat dari perspektif medis. Mengapa nilai deviasi yang kecil ini belum dapat dimaknai sebagai bukti akurasi klinis? Dalam praktik klinis kedokteran, seluruh rentang nilai simulasi yang diuji (95% hingga 100%) berada pada rentang normoksemia atau kondisi saturasi oksigen normal. Pada rentang ini, penyerapan cahaya oleh oksihemoglobin berada dalam zona kurva disosiasi oksihemoglobin yang datar, di mana perubahan tekanan parsial oksigen darah arteri yang cukup besar hanya menimbulkan pergeseran persentase saturasi yang sangat sempit. Deviasi sebesar 0,75 poin persentase pada empat titik uji dalam kondisi diam hanya menunjukkan bahwa purwarupa mampu menghasilkan estimasi angka yang mendekati alat pembanding pada situasi ideal tanpa tekanan fisiologis.

Hasil pengujian simulasi ini memiliki batasan makna yang sangat fundamental dan tidak dapat dijadikan landasan klaim keandalan diagnostik perangkat. Pengujian empat titik berpasangan ini sama sekali belum menguji respons fotodetektor dan algoritma purwarupa pada kondisi desaturasi atau hipoksemia berat, yaitu pada rentang saturasi di bawah 90% hingga 70%. Kegagalan deteksi pada rentang hipoksemia membawa konsekuensi fatal bagi keselamatan pasien karena keterlambatan penanganan hipoksia jaringan. Selain itu, pengujian ini belum memperhitungkan gangguan perfusi perifer rendah (seperti pada pasien syok, hipotermia, atau vasokonstriksi pembuluh darah), variasi ketebalan jaringan, pigmentasi melanin kulit, serta keberadaan hemoglobin abnormal (seperti karboksihemoglobin atau methemoglobin) yang secara optik menyerap cahaya pada panjang gelombang serupa. Karena data yang dievaluasi merupakan simulasi teknis tanpa verifikasi terhadap baku emas analisis gas darah arteri ($SaO_2$), temuan Bab 4 ini secara tegas diposisikan sebagai evaluasi kesesuaian teknis awal purwarupa dan bukan bukti efikasi maupun keamanan klinis bagi pasien.

---

## Catatan Fakta Belum Tersedia

Berikut adalah rincian data faktual dan parameter penelitian yang belum tersedia dalam studi simulasi ini dan tidak difabrikasi dalam penulisan:
1. **Jumlah dan Karakteristik Partisipan**: Data jumlah subjek manusia, demografi, usia, jenis kelamin, serta kondisi fisiologis peserta uji tidak tersedia.
2. **Kriteria Inklusi dan Eksklusi Klinis**: Standar seleksi medis bagi subjek uji (seperti riwayat penyakit kardiovaskular, kelainan paru, anemia, suhu akral perifer, dan indeks massa tubuh) tidak tersedia.
3. **Persetujuan Etik Penelitian (*Ethical Clearance*)**: Surat izin atau persetujuan kelaikan etik dari komite etik penelitian biomedis resmi tidak tersedia karena studi ini murni pengujian simulasi teknis.
4. **Spesifikasi Sensor dan Komponen Keras**: Informasi detail mengenai tipe sensor fotopletismografi, spesifikasi panjang gelombang puncak LED (merah dan inframerah), jenis fotodioda, sirkuit pengondisi sinyal, resolusi konverter analog-ke-digital (*ADC*), serta mikrokontroler yang digunakan pada purwarupa tidak tersedia.
5. **Identitas dan Legalitas Alat Pembanding**: Merek, tipe model komersial, standar regulasi alat kesehatan (misalnya standar ISO 80601-2-61), riwayat pemeliharaan, serta sertifikat kalibrasi resmi alat pembanding tidak tersedia.
6. **Data Klinis Pasien dan Pembanding Baku Emas**: Nilai saturasi oksigen darah arteri ($SaO_2$) dari hasil pungsi gas darah, parameter laju nadi, indeks perfusi (*perfusion index*), dan riwayat medis pasien tidak tersedia.
7. **Informasi Waktu, Durasi, dan Kondisi Lingkungan**: Tanggal pelaksanaan, durasi pencatatan data pada tiap titik pengukuran, suhu lingkungan pengujian, kelembapan udara, serta intensitas pencahayaan ruangan sekitar tidak tersedia.
8. **Sitasi Pustaka dan Rujukan Terkait**: Rujukan literatur primer, buku teks medis, dan artikel jurnal ilmiah spesifik tidak disertakan guna mencegah pencantuman sitasi tanpa verifikasi sumber pustaka.
