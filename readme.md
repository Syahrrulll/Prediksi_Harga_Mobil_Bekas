#  Sistem Prediksi Harga Mobil Bekas

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)

Proyek ini bertujuan untuk membangun model *Machine Learning* yang mampu memprediksi harga mobil bekas berdasarkan berbagai fitur historis dan spesifikasi kendaraan. Dengan model regresi ini, pembeli maupun penjual dapat menentukan estimasi harga pasar yang wajar dan akurat.

## 📋 Ringkasan Proyek
Menentukan harga mobil bekas seringkali menjadi tantangan karena banyaknya variabel yang memengaruhi nilai jualnya. Proyek ini menggunakan dataset (dari Kaggle) untuk mempelajari pola harga dan memprediksi nilai target (harga mobil) menggunakan algoritma regresi.

### Algoritma yang Digunakan:
1. **Random Forest** (Model Terbaik)
2. **Decision Tree**
3. **Gradient Boosting**

## 📊 Hasil Eksperimen
Kami melakukan pengujian dengan berbagai skenario pembagian data (*data split*) untuk memastikan stabilitas model. Berikut adalah performa terbaik yang dicapai berdasarkan metrik $R^2$ Score:

| Model | Data Split | R² Score |
| :--- | :---: | :---: |
| **Random Forest** | **90:10** | **96.46%** |
| Random Forest | 70:30 | 96.29% |
| Decision Tree | 90:10 | 94.47% |
| Gradient Boosting | 70:30 | 91.62% |

> **Kesimpulan:** Model **Random Forest** terpilih sebagai model final karena konsistensi performanya yang sangat tinggi (mampu menjelaskan lebih dari 96% variansi data) pada semua skenario pengujian.

## 🛠️ Teknologi & Library
- **Bahasa:** Python
- **Analisis Data:** Pandas, NumPy
- **Visualisasi:** Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn
- **Penyimpanan Model:** Joblib / Pickle

## 📂 Struktur Repositori
- `Projek Folder/`: Berisi file dataset serta Jupyter Notebook untuk proses *Exploratory Data Analysis* (EDA) dan *Training* model.

## ⚙️ Cara Menjalankan
1. Clone repositori ini ke dalam komputer kamu:
   ```bash
   git clone [https://github.com/Syahrrulll/Prediksi_Harga_Mobil_Bekas.git](https://github.com/Syahrrulll/Prediksi_Harga_Mobil_Bekas.git)
   ```
2. Pindah ke direktori proyek dan install library yang dibutuhkan (disarankan menggunakan *virtual environment*):
   ```bash
   cd Prediksi_Harga_Mobil_Bekas
   pip install pandas numpy scikit-learn matplotlib seaborn
   ```
3. Jalankan Jupyter Notebook untuk melihat proses analisis dan pelatihan:
   ```bash
   jupyter notebook
   ```

## 💡 Business Insights
Berdasarkan analisis fitur penting (*feature importance*), ditemukan beberapa faktor utama yang paling memengaruhi fluktuasi harga mobil bekas:
- **Tahun Pembuatan (Year):** Mobil keluaran tahun yang lebih baru memiliki nilai jual yang jauh lebih tinggi karena depresiasi yang masih rendah.
- **Jarak Tempuh (Mileage):** Semakin tinggi jarak tempuh kendaraan, semakin besar penurunan harga jualnya akibat keausan komponen.
- **Merek dan Model:** Reputasi merek tertentu di pasaran sangat menentukan seberapa baik mobil tersebut mempertahankan nilai jual kembalinya.

---
**Nama:** Muhammad Syahrul Mubarak  
**NIM:** F1G123030  
