# Informasi Publikasi Jurnal

Dokumen ini memuat informasi publikasi artikel ilmiah yang menjadi
luaran penelitian proyek **pengelompokan provinsi di Indonesia
berdasarkan indikator pendidikan menggunakan K-Means Clustering dan
Principal Component Analysis (PCA)**.

## Identitas Artikel

  -----------------------------------------------------------------------------------------
  Informasi                           Keterangan
  ----------------------------------- -----------------------------------------------------
  Judul artikel                       Penerapan Metode K-Means Clustering dan Principal
                                      Component Analysis (PCA) untuk Pengelompokan Provinsi
                                      di Indonesia Berdasarkan Indikator Pendidikan

  Penulis                             Clinton Lumbantoruan; Dyah Ayu Megawaty

  Afiliasi                            Fakultas Teknik dan Ilmu Komputer, Program Studi
                                      Sistem Informasi, Universitas Teknokrat Indonesia,
                                      Bandar Lampung, Indonesia

  Nama jurnal                         Journal of Artificial Intelligence and Technology
                                      Information (JAITI)

  E-ISSN                              2985-6396

  P-ISSN                              2985-5306

  Website jurnal                      https://ejournal.techcart-press.com/index.php/jaiti

  Status akreditasi                   SINTA 4 (berdasarkan informasi yang disampaikan
                                      penulis proyek)
  -----------------------------------------------------------------------------------------

> **Catatan metadata:** File artikel PDF yang diberikan masih
> menampilkan placeholder pada volume, nomor, bulan/tahun, DOI, dan
> halaman. Informasi tersebut tidak dicantumkan di sini agar tidak
> terjadi kesalahan metadata. Lengkapi bagian ini setelah memperoleh
> metadata final dari laman artikel atau versi PDF final.

## Ringkasan Penelitian

Penelitian ini bertujuan mengelompokkan provinsi di Indonesia
berdasarkan indikator pendidikan untuk memberikan gambaran mengenai
kondisi pendidikan antarwilayah. Data yang digunakan merupakan data
sekunder dari Badan Pusat Statistik (BPS), yang mencakup indikator:

-   Rata-rata Lama Sekolah (RLS).
-   Angka Partisipasi Kasar (APK).
-   Angka Partisipasi Murni (APM).
-   Angka Partisipasi Sekolah (APS).
-   Persentase penduduk yang tidak atau belum pernah bersekolah (TPS).

Penelitian menerapkan **Principal Component Analysis (PCA)** untuk
reduksi dimensi dan **K-Means Clustering** untuk pengelompokan provinsi.

## Metode yang Digunakan

Tahapan penelitian yang dijelaskan dalam artikel meliputi:

1.  Pengumpulan data indikator pendidikan dari BPS.
2.  Pre-processing data, termasuk pemeriksaan data dan deteksi outlier
    menggunakan boxplot.
3.  Pemisahan kolom identitas provinsi dan variabel numerik.
4.  Normalisasi data menggunakan `StandardScaler`.
5.  Reduksi dimensi menggunakan PCA.
6.  Penentuan jumlah cluster dengan Elbow Method dan Silhouette Score.
7.  Pengelompokan menggunakan algoritma K-Means.
8.  Evaluasi serta visualisasi dan analisis karakteristik cluster.

Outlier yang ditemukan dipertahankan karena dinilai masih mencerminkan
kondisi nyata variasi pendidikan antarprovinsi.

## Hasil Utama

-   Dua komponen utama PCA (PC1 dan PC2) menjelaskan total variasi data
    sebesar **79,31%**.
-   Penelitian memilih **3 cluster** untuk menghasilkan segmentasi
    kondisi pendidikan yang lebih terperinci.
-   Nilai Silhouette Score yang dicantumkan dalam artikel adalah:
    -   K = 2: 0,85
    -   K = 3: 0,54
    -   K = 4: 0,52
    -   K = 5: 0,52
-   Meskipun nilai Silhouette Score tertinggi diperoleh pada K = 2,
    penelitian menggunakan K = 3 agar pengelompokan kondisi pendidikan
    menghasilkan segmentasi yang lebih mendetail.
-   Hasil pengelompokan dibahas dalam tiga kategori karakteristik
    pendidikan: tinggi, sedang, dan rendah.

## Teknologi dan Tools

-   Python
-   Google Colab
-   Pandas
-   Scikit-learn
-   Matplotlib
-   Seaborn

## Keterkaitan dengan Repositori

Repositori ini mendokumentasikan implementasi analisis yang berkaitan
dengan artikel tersebut, termasuk notebook pengolahan data dan analisis
menggunakan PCA serta K-Means Clustering.

Silakan merujuk pada `README.md` di repositori untuk melihat gambaran
proyek, struktur file, dan cara menelusuri notebook.

## Informasi Tambahan

Untuk informasi artikel dan akses publikasi, kunjungi website resmi
jurnal:

https://ejournal.techcart-press.com/index.php/jaiti

------------------------------------------------------------------------

**Penulis proyek:** Clinton Lumbantoruan\
**Program Studi:** Sistem Informasi\
**Institusi:** Universitas Teknokrat Indonesia
