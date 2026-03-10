# Flood Probability Prediction Model 🌊

Repository ini berisi eksperimen Machine Learning untuk memprediksi probabilitas terjadinya banjir berdasarkan berbagai faktor lingkungan, infrastruktur, dan cuaca. 

Proyek ini bertujuan untuk membangun model prediktif yang dapat menganalisis risiko banjir dengan memanfaatkan dataset tabular yang mencakup fitur-fitur seperti Intensitas Monsun, Topografi, Manajemen Sungai, Deforestasi, hingga Faktor Politik.

## 📂 Struktur Dataset
Dataset yang digunakan dalam proyek ini terbagi menjadi beberapa file:
* `train.csv`: Data latih yang berisi fitur-fitur observasi beserta nilai target (`FloodProbability`).
* `test.csv`: Data uji yang digunakan untuk memprediksi probabilitas banjir tanpa nilai target.
* `sample_submission.csv`: Format referensi untuk menyimpan hasil prediksi dari model.

*Fitur-fitur utama meliputi:* MonsoonIntensity, TopographyDrainage, RiverManagement, Deforestation, Urbanization, ClimateChange, dan lain-lain.

## 🛠️ Eksperimen dan Pemodelan
Analisis dan pelatihan model dilakukan di dalam file Jupyter Notebook (`belajar.ipynb`). Eksperimen ini membandingkan kinerja dari beberapa algoritma regresi untuk menemukan model yang paling akurat dalam memprediksi probabilitas banjir.

Model yang dievaluasi meliputi:
1.  **Lars (Least Angle Regression)**
2.  **Linear Regression**
3.  **Gradient Boosting Regressor**

## 📊 Hasil Evaluasi
Berdasarkan metrik evaluasi (Mean Absolute Error, Mean Squared Error, dan R-Squared), **Linear Regression** menunjukkan kinerja terbaik pada dataset ini dengan skor R2 tertinggi.

| Model | MAE | MSE | R2 Score |
| :--- | :--- | :--- | :--- |
| **Linear Regression** | 0.329142 | 0.171296 | **0.828534** |
| GradientBoostingRegressor| 0.512672 | 0.380491 | 0.619132 |
| Lars | 0.806497 | 0.998246 | 0.000764 |

## 🚀 Cara Menjalankan
Jika anda ingin mencobanya, *Clone repository* ini ke komputer lokal Anda:
   ```bash
   git clone [https://github.com/username-kamu/nama-repo-kamu.git](https://github.com/username-kamu/nama-repo-kamu.git)
