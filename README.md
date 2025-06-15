# 📊 Clustering & Classification on Transaction Dataset

## 📝 Deskripsi Proyek
Proyek ini merupakan lanjutan dari proses *clustering* dataset transaksi keuangan, di mana hasil clustering digunakan sebagai **Target** untuk membangun model **klasifikasi**. Tujuan akhirnya adalah membuat model yang mampu mengklasifikasikan data baru berdasarkan pola yang telah ditemukan sebelumnya menggunakan metode *unsupervised learning*.

---

## 📂 Struktur Dataset
Dataset yang digunakan berasal dari hasil *clustering* dengan tambahan kolom `Target` sebagai label hasil klasterisasi.

- **Dataset:** `data_clustering.csv` atau `data_clustering_inverse.csv`
- **Fitur:** Semua kolom numerik hasil preprocessing
- **Target:** Label klaster hasil KMeans (misalnya: 0, 1, 2)

---

## ⚙️ Langkah-Langkah Analisis

### 1. Import Library
Mengimpor semua pustaka yang dibutuhkan untuk analisis data, visualisasi, dan machine learning.

### 2. Memuat Dataset
Dataset hasil clustering dimuat ke dalam DataFrame menggunakan `pandas`.

### 3. Data Splitting
Memisahkan data menjadi:
- 80% untuk pelatihan (`X_train`, `y_train`)
- 20% untuk pengujian (`X_test`, `y_test`)

### 4. Model Klasifikasi
Dilakukan training dan evaluasi model klasifikasi:
- ✅ `Decision Tree`
- ✅ `Random Forest`
- ✅ `Logistic Regression`

### 5. Evaluasi Model
Mengevaluasi akurasi, precision, recall, dan f1-score dari setiap model.

### 6. Hyperparameter Tuning
Melakukan tuning pada model Decision Tree menggunakan `GridSearchCV` dengan cross-validation (`cv=5`) untuk meningkatkan performa model.

---

## 📁 Model yang Disimpan
Model yang telah dilatih dan disimpan dalam format `.h5`:
- `decision_tree_model.h5`
- `explore_random_forest_classification.h5`
- `explore_logistic_regression_classification.h5`
- `tuning_classification.h5` (hasil tuning Decision Tree)

Gunakan `joblib.load('nama_model.h5')` untuk memuat model kembali.

---

## 📌 Catatan Penting
- Variabel utama yang digunakan: `df`, `X`, `y`
- Semua output evaluasi ditampilkan untuk memastikan keberhasilan langkah
- Jangan lupa untuk menjalankan **Run All Cells** sebelum submit

---

## 📧 Kontak
Jika ada pertanyaan atau diskusi, silakan hubungi:
**Putra Faaris Prayoga**  
Email: [your_email@example.com]  
LinkedIn: [linkedin.com/in/yourprofile]  

---

