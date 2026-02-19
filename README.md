# Social-Informatics-Research

**Rossmann Store Sales Prediction with XGBoost**
📌 **Deskripsi Proyek**
Proyek ini bertujuan untuk memprediksi volume penjualan harian di lebih dari 1.100 toko Rossmann di Jerman. Prediksi yang akurat membantu manajer toko dalam merencanakan inventaris, logistik, dan manajemen staf secara lebih efisien. Dataset yang digunakan mencakup informasi toko, promosi, hari libur, dan kompetisi lokal.

🛠️ **Tech Stack**
- Bahasa Pemrograman: Python
- Library Utama: * Pandas & NumPy untuk manipulasi data.
    - Scikit-Learn untuk pra-pemrosesan (Scaling & Encoding).
    - XGBoost sebagai model prediktif utama.
    - Matplotlib untuk visualisasi hasil.

🚀 **Alur Kerja Data Science**
- Integrasi Data: Menggabungkan dataset toko (store.csv) dengan data transaksi harian (train.csv) untuk mendapatkan konteks yang lengkap.
- Feature Engineering: * Ekstraksi informasi waktu (Tahun, Bulan, Hari, Minggu ke-n) dari data tanggal.
    - Menghitung durasi kompetitor telah buka di sekitar toko.
    - Menghitung durasi promo aktif (Promo2).
- Pra-pemrosesan:
    - Penanganan missing values pada fitur jarak kompetisi.
    - Implementasi MinMaxScaler untuk normalisasi fitur numerik.
    - Implementasi OneHotEncoder untuk mengubah data kategorikal menjadi format numerik.

- Modeling: Menggunakan XGBRegressor (Gradient Boosting) dengan parameter yang dioptimasi untuk menangani pola data yang non-linear.
- Evaluasi: Model dievaluasi menggunakan metrik RMSE (Root Mean Squared Error) untuk mengukur akurasi prediksi terhadap nilai aktual.

📊 **Hasil & Visualisasi**

Proyek ini mencakup visualisasi struktur Decision Tree dari model XGBoost yang telah dilatih, memberikan gambaran tentang bagaimana model mengambil keputusan berdasarkan fitur-fitur yang paling berpengaruh terhadap penjualan.
