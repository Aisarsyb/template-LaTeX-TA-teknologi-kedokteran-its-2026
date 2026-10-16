# BAB 3 METODOLOGI

## 3.1 Diagram Alir Penelitian

Rancangan metodologi penelitian ini disusun secara sistematis untuk mengevaluasi selisih pembacaan antara purwarupa instrumen pengukur saturasi oksigen ($SpO_2$) dan alat pembanding. Tahapan penelitian diawali dengan perumusan kebutuhan evaluasi teknis dasar, penentuan prosedur perbandingan berpasangan, pelaksanaan akuisisi data simulasi pada kondisi diam, perhitungan selisih pembacaan dan selisih absolut rerata, hingga analisis batas makna hasil pengujian teknis terhadap kesiapan instrumen. Alur ini ditempuh secara bertahap karena dalam pengembangan teknologi biomedis, keselamatan pasien menuntut adanya pengujian fungsional di laboratorium terlebih dahulu sebelum suatu instrumen dapat dievaluasi pada subjek manusia dalam uji klinis yang sebenarnya. Diagram alir ini memastikan bahwa pengujian difokuskan pada penilaian deviasi teknis tanpa tergesa-gesa menyimpulkan efektivitas diagnostik medis.

## 3.2 Bahan dan Peralatan

Bahan dan peralatan yang dilibatkan dalam rancangan pengujian ini mencakup dua instrumen utama, yaitu purwarupa alat ukur $SpO_2$ noninvasif dan instrumen pembanding terkalibrasi. Purwarupa instrumen dirancang untuk mendeteksi sinyal optik denyut darah kapiler perifer guna menghasilkan estimasi persentase saturasi oksigen. Alat pembanding digunakan sebagai acuan pengukuran standar untuk memverifikasi kesesuaian nilai keluaran purwarupa. Karena penelitian ini merupakan studi simulasi untuk menguji metodologi, rincian teknis spesifik dari sensor fotopletismografi (seperti panjang gelombang emisi LED merah dan inframerah, jenis fotodetektor, sirkuit pengondisi sinyal, serta mikrokontroler) maupun merek, tipe, dan riwayat sertifikasi alat pembanding tidak ditentukan atau tidak tersedia. Pengujian diperlakukan secara konseptual sebagai evaluasi komparatif keluaran sistem untuk menilai stabilitas pembacaan instrumen pada titik uji yang ditetapkan.

## 3.3 Perancangan Sistem

### 3.3.1 Arsitektur dan Diagram Blok Sistem

Arsitektur sistem dirancang berbasis prinsip pemantauan oksigenasi darah perifer secara optik noninvasif. Alur kerja sistem secara umum menghubungkan blok sensor optik untuk menangkap variasi transmisi cahaya pada jaringan berdenyut, blok pengondisi dan pemrosesan sinyal untuk menyaring derau serta menghitung nilai saturasi, dan unit antarmuka keluaran untuk menampilkan angka persentase $SpO_2$. Pemilihan metode optik noninvasif ini didasarkan pada pertimbangan keselamatan dan kenyamanan pasien, karena pemeriksaan saturasi dapat dilakukan berkesinambungan tanpa memerlukan tindakan penusukan pembuluh darah arteri yang menimbulkan rasa sakit serta risiko infeksi. Hubungan antarblok sistem diarahkan untuk menghasilkan nilai estimasi numerik sesaat yang dapat langsung disandingkan dengan pembacaan instrumen acuan.

### 3.3.2 Tahapan Implementasi

Tahapan implementasi dalam rancangan penelitian ini berfokus pada persiapan dan penyelarasan prosedur pengukuran statis. Kedua instrumen disiapkan untuk melakukan pembacaan secara simultan pada kondisi yang identik. Pendekatan pengujian pada kondisi diam (*resting condition*) dipilih secara sengaja untuk meniadakan pengaruh artefak gerak (*motion artifact*), variasi tekanan probe pada jaringan, serta fluktuasi hemodinamika sesaat. Dengan menstabilkan kondisi fisik selama pengujian, variasi perbedaan nilai pembacaan yang teramati murni diisolasi sebagai karakteristik deviasi teknis purwarupa terhadap alat pembanding, bukan akibat gangguan gerak lingkungan. Karena spesifikasi komponen keras dan kode pemrosesan internal tidak tersedia, tahapan implementasi berfokus penuh pada protokol pencatatan data keluaran berpasangan secara objektif.

## 3.4 Prosedur Pengujian dan Evaluasi

Prosedur pengujian dirancang menggunakan metode perbandingan berpasangan (*paired measurement*) pada kondisi diam. Dalam skenario simulasi eksplisit ini, pengujian mencakup empat titik pengukuran berpasangan dengan nilai pembacaan alat pembanding berturut-turut sebesar 96%, 97%, 98%, dan 99%, serta nilai pembacaan purwarupa berturut-turut sebesar 95%, 97%, 97%, dan 100%. Pengukuran berpasangan dipilih agar kedua instrumen mengamati kondisi fisiologis yang setara pada waktu pengamatan yang sama, sehingga deviasi pembacaan purwarupa dapat dihitung secara tepat.

Evaluasi data dilakukan melalui dua metrik kuantitatif, yaitu selisih pembacaan individual ($d_i = SpO_{2,\text{purwarupa}} - SpO_{2,\text{pembanding}}$) dan selisih absolut rerata (*mean absolute difference* atau MAD). Berdasarkan data simulasi tersebut, selisih pembacaan pada masing-masing titik adalah -1 poin persentase pada titik pertama (95% terhadap 96%), 0 poin persentase pada titik kedua (97% terhadap 97%), -1 poin persentase pada titik ketiga (97% terhadap 98%), dan +1 poin persentase pada titik keempat (100% terhadap 99%). Metrik selisih absolut rerata dipilih dibandingkan rerata selisih biasa untuk mencegah efek saling meniadakan (*canceling out*) antara deviasi positif dan deviasi negatif. Penghitungan selisih absolut menghasilkan nilai rata-rata sebesar 0,75 poin persentase, yang merefleksikan magnitudo rata-rata penyimpangan nilai purwarupa terhadap acuan pada empat titik uji tersebut.

Tahap akhir prosedur evaluasi adalah analisis batas makna dari hasil pengujian teknis. Mengapa analisis batas makna ini sangat krusial dari sudut pandang medis? Deviasi selisih absolut rerata sebesar 0,75 poin persentase pada empat titik data simulasi rentang 95% hingga 100% ini hanya membuktikan kecocokan skala pengukuran statis dalam rentang normal sempit tanpa adanya gerakan. Hasil ini sama sekali tidak membuktikan keandalan klinis purwarupa. Pengujian teknis ini belum menguji respons alat pada kondisi hipoksemia berat (di bawah 90% hingga 70%), belum memperhitungkan variasi perfusi darah rendah atau pigmentasi kulit, serta belum dibandingkan terhadap baku emas analisis gas darah arteri ($SaO_2$). Oleh karena itu, prosedur evaluasi ini secara tegas menempatkan hasil uji sebagai verifikasi teknis laboratorium awal yang tidak dapat digunakan sebagai dasar penegakan keputusan klinis pada pasien.

## 3.5 Jadwal Kegiatan

Rancangan jadwal kegiatan penelitian mencakup tahapan studi perancangan prosedur pengujian, persiapan simulasi instrumen, pelaksanaan akuisisi data komparatif berpasangan, analisis selisih pembacaan dan batas makna teknis, serta penyusunan laporan tugas akhir. Mengingat penelitian ini menggunakan data simulasi eksplisit tanpa pengambilan data riil di fasilitas kesehatan, tanggal pelaksanaan kalender, durasi mingguan tertentu, maupun lokasi lapangan spesifik tidak dicantumkan guna mencegah fabrikasi linimasa kegiatan. Rangkaian kegiatan ini dirumuskan sebagai kerangka tahapan kerja terencana yang menggambarkan alur logis pengujian instrumen biomedis sebelum melangkah ke tahap pengujian klinis lanjutan.

---

## Catatan Fakta Belum Tersedia

Berikut adalah rincian data dan informasi metodologis yang belum tersedia dalam penelitian simulasi ini dan tidak diasumsikan atau difabrikasi:
1. **Jumlah dan Karakteristik Partisipan**: Jumlah subjek manusia yang diuji, rentang usia, jenis kelamin, serta profil fisik peserta uji coba tidak tersedia.
2. **Kriteria Inklusi dan Eksklusi Medis**: Parameter seleksi medis untuk subjek, seperti rentang tekanan darah, denyut nadi istirahat, indeks massa tubuh, suhu akral perifer, serta riwayat penyakit kardiovaskular dan pernapasan, tidak tersedia.
3. **Persetujuan Etik (Ethical Clearance)**: Surat persetujuan etik penelitian kesehatan dari komite etik resmi untuk pengujian alat pada manusia tidak tersedia.
4. **Spesifikasi Sensor dan Perangkat Keras**: Merek sensor fotopletismografi, spesifikasi panjang gelombang emisi optik (LED merah dan inframerah), sensitivitas fotodetektor, sirkuit pengondisi sinyal analog, mikrokontroler, dan resolusi konverter analog-ke-digital (*ADC*) purwarupa tidak tersedia.
5. **Identitas dan Sertifikasi Alat Pembanding**: Merek, nomor model, standar kepatuhan regulasi medis, akurasi pabrik, serta sertifikat kalibrasi instrumen acuan tidak tersedia.
6. **Data Fisiologis dan Pasien**: Kadar gas darah arteri ($SaO_2$), laju denyut nadi (*pulse rate*), indeks perfusi perifer (*perfusion index*), dan data rekam medis pasien tidak tersedia.
7. **Informasi Waktu dan Lingkungan Pengujian**: Tanggal pelaksanaan, durasi pengukuran per titik, temperatur ruangan, kelembapan udara, dan intensitas pencahayaan lingkungan sekitar saat pengujian tidak tersedia.
8. **Daftar Pustaka dan Sitasi Literatur Terkait**: Rujukan artikel jurnal, buku teks, dan standar internasional resmi (seperti ISO 80601-2-61) tidak disertakan karena ketiadaan dokumen pustaka yang terverifikasi dalam batasan studi ini.
