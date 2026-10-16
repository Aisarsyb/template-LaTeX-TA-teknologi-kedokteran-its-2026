# BAB 5 KESIMPULAN DAN SARAN

Bab ini memuat kesimpulan menyeluruh dari studi simulasi pengujian purwarupa oksimeter nadi serta saran praktis dan pengembangan penelitian berikutnya. Penarikan kesimpulan ditujukan untuk menjawab tujuan evaluasi selisih pembacaan saturasi oksigen ($SpO_2$) dan menguraikan batas makna teknis pengujian dari sudut pandang medis. Seluruh kesimpulan dan rekomendasi didasarkan secara ketat pada data simulasi eksplisit tanpa mengasumsikan bukti klinis yang belum teruji.

## 5.1 Kesimpulan

Berdasarkan evaluasi terhadap empat titik pengukuran berpasangan dalam kondisi diam, selisih pembacaan $SpO_2$ antara purwarupa dan alat pembanding menghasilkan selisih absolut berturut-turut sebesar 1, 0, 1, dan 1 poin persentase, dengan nilai selisih absolut rerata sebesar 0,75 poin persentase. Nilai ini diperoleh dari perbandingan data simulasi alat pembanding (96%, 97%, 98%, dan 99%) terhadap purwarupa (95%, 97%, 97%, dan 100%). Dari sisi rekayasa perangkat dasar, capaian selisih absolut rerata sebesar 0,75 poin persentase ini menunjukkan bahwa purwarupa secara komputasi mampu menghasilkan nilai estimasi yang mendekati alat rujukan pada titik uji statis yang dievaluasi.

Meskipun deviasi numerik tampak kecil, batas makna pengujian teknis ini sangat terbatas dan tidak membuktikan keandalan diagnostik maupun keamanan klinis bagi pasien. Pengujian simulasi ini hanya mencakup rentang saturasi normal (normoksemia antara 95% hingga 100%) pada kondisi diam tanpa gangguan gerak. Hasil ini belum membuktikan respons fotodetektor dan algoritma purwarupa pada kondisi desaturasi atau hipoksemia berat di bawah 90%, yang justru merupakan zona paling kritis untuk keselamatan jiwa pasien. Tanpa data subjek manusia, izin etik, spesifikasi sensor, pembanding baku emas gas darah, dan pengujian perfusi jaringan, temuan simulasi ini murni mencerminkan verifikasi fungsi komparatif awal dan tidak dapat dijadikan dasar kesetaraan klinis terhadap standar alat kesehatan medis.

## 5.2 Saran

Bagi pengembang instrumen, disarankan untuk mendokumentasikan spesifikasi teknis purwarupa secara lengkap—termasuk panjang gelombang LED, pengondisi sinyal, dan karakteristik fotodetektor—serta memverifikasi sistem menggunakan simulator optik atau kalibrator medis terstandar sebelum melangkah ke tahap rancang bangun berikutnya. Dokumentasi spesifikasi dan verifikasi instrumen ini penting karena data simulasi yang ada saat ini belum memungkinkan pengujian teknis yang dapat direplikasi secara mandiri oleh pihak lain. Selain itu, perangkat ini tidak boleh digunakan untuk pemantauan pasien, penilaian klinis mandiri, maupun pengambilan keputusan medis di fasilitas pelayanan kesehatan.

Bagi penelitian lanjutan, disarankan untuk menyusun protokol penelitian berbasis subjek manusia nyata yang dilengkapi persetujuan kelaikan etik (*ethical clearance*) resmi, kriteria seleksi medis yang jelas, dan penelusuran pustaka rujukan terverifikasi. Pengujian masa depan perlu memperluas skenario evaluasi ke kondisi non-statis untuk menguji ketahanan terhadap artefak gerak, menilai respons sensor pada kondisi perfusi jaringan rendah (seperti kondisi dingin atau hipotensi), serta membandingkan akurasi pembacaan pada rentang hipoksemia menggunakan baku emas pemeriksaan gas darah arteri ($SaO_2$). Langkah pengujian bertahap tersebut diperlukan agar batas penerimaan kesalahan instrumen memiliki landasan ilmiah dan pertimbangan keselamatan medis yang dapat dipertanggungjawabkan.

---

## Catatan Fakta Belum Tersedia

Rincian parameter dan data faktual berikut belum tersedia dalam studi simulasi ini dan sengaja tidak difabrikasi dalam penulisan laporan:
1. **Jumlah dan Karakteristik Partisipan**: Data jumlah peserta, usia, jenis kelamin, serta status fisiologis subjek uji tidak tersedia.
2. **Kriteria Inklusi dan Eksklusi Medis**: Batasan medis pemilihan subjek (seperti riwayat penyakit paru, kardiovaskular, ketebalan jaringan, dan warna kulit) tidak tersedia.
3. **Persetujuan Etik Penelitian (*Ethical Clearance*)**: Surat persetujuan komite etik biomedis resmi tidak tersedia karena penelitian berstatus simulasi rancangan teknis.
4. **Spesifikasi Sensor dan Perangkat Keras**: Tipe sensor fotopletismografi, panjang gelombang LED merah dan inframerah, jenis fotodioda, serta mikrokontroler purwarupa tidak tersedia.
5. **Identitas dan Sertifikasi Alat Pembanding**: Merek, model komersial, tingkat ketelitian standar pabrikan, dan riwayat kalibrasi alat pembanding tidak tersedia.
6. **Data Pasien dan Standar Baku Emas**: Nilai saturasi oksigen darah arteri ($SaO_2$), laju nadi, indeks perfusi kapiler, dan data rekam medis tidak tersedia.
7. **Informasi Waktu dan Lingkungan Pengujian**: Tanggal pelaksanaan, durasi pengukuran tiap titik, suhu, dan intensitas cahaya ruangan tidak tersedia.
8. **Sumber Pustaka dan Sitasi**: Rujukan literatur ilmiah terkait tidak tersedia, sehingga bab ini tidak mencantumkan sitasi fiktif.
