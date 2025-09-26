# 🚢 Titanic Exploratory Data Analysis (EDA)

Proyek ini melakukan **Exploratory Data Analysis (EDA)** pada dataset Titanic dari kompetisi [Kaggle - Titanic: Machine Learning from Disaster](https://www.kaggle.com/c/titanic).  

Tujuannya adalah memahami pola data, melakukan pembersihan, visualisasi, dan menemukan faktor yang berpengaruh terhadap keselamatan penumpang.

---

## Dataset
Dataset yang digunakan:
- **train.csv** dari Kaggle (891 baris, 12 kolom)
- Fitur penting: `Survived`, `Pclass`, `Sex`, `Age`, `SibSp`, `Parch`, `Fare`, `Embarked`.

---

## Data Cleaning
Langkah yang dilakukan:
- Mengisi nilai kosong pada `Age` dengan **median usia**.
- Mengisi nilai kosong pada `Embarked` dengan **mode** (nilai paling sering muncul).
- Menghapus kolom `Cabin` karena terlalu banyak missing value (>70%).

---

## Visualisasi & Analisis
1. **Distribusi Usia**  
   Menunjukkan mayoritas penumpang berusia 20–30 tahun.

2. **Survival Rate (Pie Chart)**  
   - 38,4% selamat  
   - 61,6% tidak selamat (meninggal)  

3. **Survival Berdasarkan Gender**  
   - Wanita: ~74,2% selamat  
   - Pria: ~18,9% selamat  

4. **Survival Berdasarkan Kelas Penumpang**  
   - Kelas 1: ~63,0% selamat  
   - Kelas 2: ~47,3% selamat  
   - Kelas 3: ~24,2% selamat  

5. **Korelasi Fitur Numerik (Heatmap)**  
   Korelasi positif antara `Fare` dan `Survived` (semakin mahal tiket, semakin tinggi peluang selamat).

---

## 💡 Insight
- **Wanita memiliki peluang selamat jauh lebih tinggi** dibanding pria (74,2% vs 18,9%).
- **Penumpang kelas 1** lebih banyak selamat dibanding kelas 3 (63% vs 24%).
- **Anak-anak (<10 tahun)** memiliki peluang selamat lebih tinggi daripada usia dewasa (~61,3%).

---

## 🚀 Next Step
Langkah selanjutnya dari analisis ini adalah:
- Membuat model machine learning (misalnya Logistic Regression atau Random Forest) untuk memprediksi `Survived`.
- Mengevaluasi performa model dengan akurasi, precision, recall, dan F1-score.

---

## 🛠 Cara Menjalankan
1. Clone repo ini:
   ```bash
   git clone https://github.com/Mrama1011-mr/machine-learning-portfolio.git
