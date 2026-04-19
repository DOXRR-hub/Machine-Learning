```markdown
# Proyek Klasifikasi Spesies Bunga Iris dengan K-Nearest Neighbors (KNN)

## Deskripsi Proyek
Proyek ini bertujuan untuk mengklasifikasikan spesies bunga Iris (Setosa, Versicolor, atau Virginica) berdasarkan fitur-fitur morfologinya, yaitu panjang dan lebar sepal, serta panjang dan lebar petal. Kami menggunakan dataset Iris yang terkenal dan mengimplementasikan model K-Nearest Neighbors (KNN) untuk tugas klasifikasi ini. Selain itu, proyek ini juga mencakup langkah-langkah eksplorasi data, rekayasa fitur sederhana, dan evaluasi model.

## Dataset
Dataset yang digunakan adalah dataset Iris. Dataset ini berisi 150 sampel, dengan masing-masing sampel memiliki 4 fitur numerik (panjang/lebar sepal dan petal) dan satu target kategorikal (spesies Iris).

## Fitur dan Target
*   **Fitur Input (X):**
    *   `SepalLengthCm`: Panjang sepal dalam cm.
    *   `SepalWidthCm`: Lebar sepal dalam cm.
    *   `PetalLengthCm`: Panjang petal dalam cm.
    *   `PetalWidthCm`: Lebar petal dalam cm.
    *   `Mean_PetalLengthCm_by_Species`: Fitur hasil rekayasa yang menunjukkan rata-rata panjang petal untuk setiap spesies.
*   **Target Output (y):**
    *   `Species_encoded`: Representasi numerik dari spesies Iris (0 untuk Iris-setosa, 1 untuk Iris-versicolor, 2 untuk Iris-virginica).

## Tahapan Proyek
1.  **Persiapan:** Mengimpor library yang diperlukan seperti `pandas`, `numpy`, `matplotlib`, `seaborn`, dan `sklearn`.
2.  **Pemuatan Data:** Memuat dataset `Iris.csv` ke dalam DataFrame pandas.
3.  **Exploratory Data Analysis (EDA):** Menganalisis distribusi data, korelasi antar fitur, dan visualisasi untuk memahami karakteristik dataset.
4.  **Rekayasa Fitur:** Membuat fitur baru (`Mean_PetalLengthCm_by_Species`) untuk meningkatkan performa model.
5.  **Preprocessing Data:** Menghapus kolom yang tidak relevan (`Id`) dan melakukan *label encoding* pada kolom target `Species`.
6.  **Pembagian Data:** Membagi dataset menjadi data training dan testing (70% training, 30% testing).
7.  **Pelatihan Model KNN:** Melatih model K-Nearest Neighbors pada data training.
8.  **Evaluasi Model:** Mengevaluasi performa model menggunakan metrik seperti akurasi, *confusion matrix*, dan *classification report*.
9.  **Hyperparameter Tuning:** Menggunakan `GridSearchCV` untuk menemukan *hyperparameter* terbaik untuk model KNN.
10. **Prediksi:** Mendemonstrasikan prediksi spesies untuk data baru.

## Cara Menjalankan Kode
1.  **Pastikan Anda memiliki file `Iris.csv`** di direktori yang sama dengan notebook ini atau sesuaikan path file dalam kode.
2.  **Buka notebook** di lingkungan seperti Google Colab atau Jupyter Notebook.
3.  **Jalankan setiap sel** secara berurutan. 

## Hasil
Model KNN yang dilatih dan di-tuning menunjukkan akurasi yang sangat tinggi dalam mengklasifikasikan spesies Iris pada dataset ini.

```