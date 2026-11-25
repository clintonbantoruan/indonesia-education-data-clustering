# Pengelompokan Provinsi di Indonesia Berdasarkan Indikator Pendidikan Menggunakan K-Means Clustering dan PCA

## 📌 Project Overview

Proyek ini merupakan penelitian Tugas Akhir yang bertujuan untuk mengelompokkan provinsi di Indonesia berdasarkan indikator pendidikan menggunakan pendekatan **Data Mining**, dengan mengombinasikan metode **Principal Component Analysis (PCA)** dan **K-Means Clustering**.

Penelitian ini dilakukan untuk mengidentifikasi kesamaan karakteristik pendidikan antarprovinsi serta memberikan gambaran mengenai kesenjangan kondisi pendidikan di berbagai wilayah Indonesia. Hasil pengelompokan diharapkan dapat menjadi informasi pendukung dalam memahami kondisi pendidikan secara lebih terstruktur dan berbasis data.

Penelitian ini telah diselesaikan dan dipublikasikan pada **Journal of Artificial Intelligence and Technology Information (JAITI)**, jurnal terakreditasi SINTA 4.

## 🎯 Research Objectives

1. Mengidentifikasi karakteristik pendidikan provinsi di Indonesia berdasarkan indikator pendidikan.
2. Mengurangi kompleksitas variabel menggunakan Principal Component Analysis (PCA).
3. Mengelompokkan provinsi berdasarkan kemiripan karakteristik pendidikan menggunakan K-Means Clustering.
4. Menganalisis karakteristik setiap kelompok untuk mengidentifikasi kategori pendidikan tinggi, sedang, dan rendah.

## 📊 Dataset

Data penelitian merupakan data sekunder yang diperoleh dari **Badan Pusat Statistik (BPS)**. Dataset mencakup sejumlah indikator pendidikan pada tingkat provinsi di Indonesia.

Indikator yang digunakan dalam penelitian meliputi:

| Indikator | Keterangan |
|---|---|
| RLS | Rata-rata Lama Sekolah |
| APK | Angka Partisipasi Kasar |
| APM | Angka Partisipasi Murni |
| APS | Angka Partisipasi Sekolah |
| TPS | Persentase penduduk yang tidak atau belum pernah sekolah |

Data digunakan untuk menggambarkan kondisi pendidikan dan menjadi dasar dalam proses pengelompokan provinsi.

## 🛠️ Tools & Technologies

- **Python** – Bahasa pemrograman untuk pengolahan dan analisis data.
- **Google Colab** – Lingkungan pengembangan untuk menjalankan kode Python.
- **StandardScaler** – Normalisasi data.
- **Principal Component Analysis (PCA)** – Reduksi dimensi.
- **K-Means Clustering** – Algoritma pengelompokan data.
- **Elbow Method** – Pendekatan untuk membantu menentukan jumlah cluster.
- **Silhouette Score** – Evaluasi kualitas hasil clustering.

## ⚙️ Research Methodology

Tahapan penelitian yang dilakukan meliputi:

1. **Data Collection**  
   Mengumpulkan data indikator pendidikan tingkat provinsi dari publikasi resmi Badan Pusat Statistik (BPS).

2. **Data Preprocessing**  
   Menyiapkan data melalui pemeriksaan format variabel, nilai yang hilang, data tidak valid, serta identifikasi outlier.

3. **Feature Separation**  
   Memisahkan identitas provinsi dari variabel numerik yang digunakan sebagai fitur analisis.

4. **Data Normalization**  
   Melakukan normalisasi menggunakan StandardScaler agar setiap variabel memiliki skala yang sebanding.

5. **Dimensionality Reduction (PCA)**  
   Menggunakan PCA untuk mengurangi jumlah dimensi dengan mempertahankan informasi utama dalam dataset.

6. **Determining the Number of Clusters**  
   Menggunakan Elbow Method dan Silhouette Score sebagai dasar pertimbangan dalam menentukan jumlah cluster.

7. **Clustering (K-Means)**  
   Melakukan pengelompokan berdasarkan hasil reduksi dimensi PCA.

8. **Model Evaluation and Interpretation**  
   Mengevaluasi hasil pengelompokan menggunakan Silhouette Score serta menganalisis karakteristik setiap cluster.

9. **Data Visualization**  
   Menyajikan hasil analisis melalui visualisasi PCA dan distribusi cluster.

## 📈 Research Results

### 1. PCA Results

Hasil reduksi dimensi menggunakan Principal Component Analysis (PCA) menunjukkan bahwa dua komponen utama mampu menjelaskan sebagian besar variasi informasi dalam dataset.

- **Principal Component 1 (PC1):** 56,95%
- **Principal Component 2 (PC2):** 22,35%
- **Total Explained Variance:** 79,31%

Dengan demikian, dua komponen utama digunakan sebagai representasi data dalam proses clustering.

### 2. Optimal Cluster Selection

Penentuan jumlah cluster dilakukan dengan mempertimbangkan hasil Elbow Method dan Silhouette Score.

Hasil Silhouette Score yang dilaporkan dalam penelitian:

| Jumlah Cluster (K) | Silhouette Score |
|---|---:|
| 2 | 0,85 |
| 3 | 0,54 |
| 4 | 0,52 |
| 5 | 0,52 |

Penelitian menggunakan **3 cluster** untuk menghasilkan segmentasi kondisi pendidikan yang lebih terperinci, meskipun nilai Silhouette Score tertinggi diperoleh pada K = 2.

### 3. K-Means Clustering Results

Proses K-Means Clustering menghasilkan tiga kelompok provinsi berdasarkan karakteristik indikator pendidikan:

| Cluster | Kategori | Karakteristik Umum |
|---|---|---|
| Cluster 0 | Pendidikan Tinggi | Kondisi pendidikan relatif baik dan mencakup sebagian besar provinsi. |
| Cluster 1 | Pendidikan Rendah | Didominasi wilayah Papua Tengah dan Papua Pegunungan. |
| Cluster 2 | Pendidikan Sedang | Menunjukkan kondisi pendidikan pada tingkat menengah atau transisi. |

Hasil tersebut memperlihatkan adanya perbedaan karakteristik pendidikan antarprovinsi di Indonesia.

### 4. Research Conclusion

Kombinasi Principal Component Analysis (PCA) dan K-Means Clustering dapat digunakan untuk mengelompokkan provinsi berdasarkan indikator pendidikan. PCA mampu mempertahankan 79,31% variasi informasi melalui dua komponen utama, sedangkan K-Means menghasilkan tiga kelompok dengan karakteristik pendidikan yang berbeda.

Penelitian ini memberikan gambaran berbasis data mengenai disparitas pendidikan antarwilayah dan dapat menjadi salah satu informasi pendukung dalam memahami pemerataan pendidikan di Indonesia.

## 📁 Project Structure

Struktur repository GitHub yang digunakan:

```text
education-data-clustering/
│
├── README.md
│
├── notebooks/
│   └── ta_dalam_csv.ipynb
│
├── dataset/
│   └── 8 variabel pendidikan data bps.xlsx
│
├── images/
│   ├── pca_explained_variance.png
│   ├── elbow_method.png
│   ├── clustering_visualization.png
│   └── outlier_detection.png
│
└── publication/
    └── journal_information.md
```

*Catatan: Nama dan isi folder merupakan rekomendasi penataan repository. Masukkan hanya file yang memang tersedia dan boleh dibagikan.*

## 📚 Publication

**Journal:** Journal of Artificial Intelligence and Technology Information (JAITI)  
**Accreditation:** SINTA 4  
**Research Title:** Penerapan Metode K-Means Clustering dan Principal Component Analysis (PCA) untuk Pengelompokan Provinsi di Indonesia Berdasarkan Indikator Pendidikan  
**Author:** Clinton Lumbantoruan  
**Institution:** Universitas Teknokrat Indonesia

- Website jurnal: https://ejournal.techcart-press.com/index.php/jaiti
- Link artikel: *(Tambahkan URL artikel yang telah diterbitkan jika tersedia.)*

## 👨‍💻 Author

**Clinton Lumbantoruan**  
S1 Sistem Informasi – Universitas Teknokrat Indonesia

Minat bidang:
- Data Analytics
- Data Mining
- Data Visualization
- Python for Data Analysis
- Machine Learning

---

*This repository presents a completed academic research project and its published research outcomes. The notebook and supporting materials are provided as documentation of the research work.*
