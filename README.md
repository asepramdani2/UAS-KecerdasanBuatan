# UAS-KecerdasanBuatan
# Deskripsi Proyek

Proyek ini mengimplementasikan algoritma K-Nearest Neighbor (K-NN) yang dikombinasikan dengan seleksi fitur Binary Particle Swarm Optimization (BPSO) untuk klasifikasi kanker payudara. Dengan BPSO, fitur yang digunakan dapat direduksi dari 30 menjadi 5 fitur tanpa menurunkan akurasi, bahkan meningkatkan akurasi menjadi 95,32%, sehingga model lebih efisien dan akurat.

Dataset: Breast Cancer Wisconsin Diagnostic (UCI)

# Tujuan Proyek

Membangun model klasifikasi kanker payudara yang akurat dan efisien.✅ Mengimplementasikan seleksi fitur dengan Binary PSO untuk meningkatkan akurasi K-NN dan mengurangi kompleksitas perhitungan.

# Tools dan Library

1.Python (Google Colab)

2.Pandas, NumPy

3.Scikit-learn (KNN, preprocessing, metrics)

4.Matplotlib, Seaborn

5.PSO Library (custom/simple implementation)

# Langkah Pengerjaan

1️. Business Understanding

Memahami tingginya angka kanker payudara dan perlunya deteksi dini.

Tujuan: Membangun model klasifikasi cepat dan akurat.

2️. Data Understanding

Menggunakan dataset Breast Cancer Wisconsin Diagnostic (569 sampel, 30 fitur).

Label target: Malignant (ganas) atau Benign (jinak).

3️. Exploratory Data Analysis (EDA)

Analisis distribusi kelas dan fitur.

Visualisasi heatmap korelasi antar fitur untuk melihat potensi redundansi.

4️. Data Preparation

Cek dan tangani missing values (jika ada).

Normalisasi fitur agar skala seragam (StandardScaler).

Split data: 70% train, 30% test.

5️. Feature Selection dengan Binary PSO

Mengimplementasikan Binary PSO untuk memilih subset fitur terbaik dari 30 fitur.

Fitness function mengkombinasikan akurasi klasifikasi dan jumlah fitur minimal.

Output: Fitur terpilih yang optimal untuk klasifikasi.

6️. Modeling dengan K-NN

Menggunakan algoritma K-NN dengan parameter k ganjil (1-21) untuk menghindari seri.

Melatih model dengan data train pada dua skenario:

K-NN tanpa seleksi fitur.

K-NN dengan fitur hasil seleksi BPSO.

7️. Evaluation

Menggunakan Confusion Matrix untuk visual evaluasi.

- Menghitung metrik:

- Accuracy

- Precision

- Recall

- F1-score

Membandingkan hasil K-NN vs K-NN+BPSO.

8️. Kesimpulan

Model K-NN+BPSO mencapai akurasi 95,32% (lebih tinggi dari K-NN biasa, 94,15%).

Jumlah fitur berhasil direduksi dari 30 menjadi 5 tanpa menurunkan akurasi.

Model lebih cepat dan efisien untuk digunakan sebagai pendukung keputusan medis.

# Referensi

Hidayat, R., Kartini, D., Mazdadi, M. I., Budiman, I., & Ramadhani, R. (2023). Implementasi Seleksi Fitur Binary Particle Swarm Optimization pada Algoritma K-NN untuk Klasifikasi Kanker Payudara. Jurnal Sistem dan Teknologi Informasi (JUSTIN), 11(1). DOI: 10.26418/justin.v11i1.53608.

Harafani, H., & Al-Kautsar, H. A. (2021). Meningkatkan Kinerja K-NN Untuk Klasifikasi Kanker Payudara Dengan Forward Selection. Jurnal Pendidikan Teknologi dan Kejuruan, 18(1), 99–106.

Yunus, W. (2018). Algoritma K-Nearest Neighbor Berbasis Particle Swarm Optimization Untuk Prediksi Penyakit Ginjal Kronik. Jurnal Teknik Elektro Cosphi, 2(2), 51–55.

UCI Machine Learning Repository, Breast Cancer Wisconsin (Diagnostic) Data Set.
