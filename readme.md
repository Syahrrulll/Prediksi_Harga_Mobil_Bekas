# 🚀 Employee Attrition Prediction System

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)

Proyek ini bertujuan untuk membangun model Machine Learning yang mampu memprediksi kemungkinan *attrition* (pengunduran diri) karyawan berdasarkan berbagai faktor internal perusahaan. Dengan model ini, tim HR dapat mengambil langkah preventif untuk mempertahankan talenta terbaik perusahaan.

## 📋 Ringkasan Proyek
Masalah *attrition* karyawan berdampak besar pada biaya operasional dan stabilitas tim. Proyek ini menggunakan dataset dari Kaggle untuk menganalisis pola perilaku karyawan dan memprediksi nilai target menggunakan algoritma regresi.

### Algoritma yang Digunakan:
1. **Random Forest** (Model Terbaik)
2. **Decision Tree**
3. **Gradient Boosting**

## 📊 Hasil Eksperimen
Kami melakukan pengujian dengan berbagai skenario pembagian data (*data split*) untuk memastikan stabilitas model. Berikut adalah performa terbaik yang dicapai:

| Model | Data Split | R² Score |
| :--- | :---: | :---: |
| **Random Forest** | **90:10** | **96.46%** |
| Random Forest | 70:30 | 96.29% |
| Decision Tree | 90:10 | 94.47% |
| Gradient Boosting | 70:30 | 91.62% |

> **Kesimpulan:** Model **Random Forest** terpilih sebagai model final karena konsistensi performanya yang tinggi di atas 96% pada semua skenario pengujian.

## 🛠️ Teknologi & Library
- **Bahasa:** Python
- **Analisis Data:** Pandas, NumPy
- **Visualisasi:** Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn
- **Penyimpanan Model:** Joblib / Pickle

## 📂 Struktur Repositori
- `notebooks/`: Berisi file Jupyter Notebook proses EDA dan Training.
- `data/`: Dataset yang digunakan (Kaggle dataset).
- `models/`: File model final (.pkl atau .joblib).
- `src/`: Skrip Python untuk pra-pemrosesan dan prediksi.

## ⚙️ Cara Menjalankan
1. Clone repositori ini:
   ```bash
   git clone https://github.com/Syahrrulll/Prediksi_Harga_Mobil_Bekas.git
   ```
2. Install library yang dibutuhkan
3. Jalankan Jupyter Notebook untuk melihat 

## 💡 Business Insights
Berdasarkan analisis fitur penting (*feature importance*), ditemukan beberapa faktor utama yang mempengaruhi keputusan karyawan:
- **Tingkat Pendapatan:** Memiliki pengaruh signifikan terhadap loyalitas.
- **Beban Kerja (Overtime):** Karyawan dengan jam lembur tinggi memiliki risiko keluar lebih besar.
- **Kepuasan Kerja:** Korelasi kuat antara lingkungan kerja dan masa kerja karyawan.

---
**Nama:** Muhammad Syahrul Mubarak
**NIM :** F1G123030


