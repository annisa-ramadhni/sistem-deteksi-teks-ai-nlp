# Hasil Eksperimen

Folder ini berisi dokumentasi dan hasil eksperimen dari sistem deteksi teks buatan AI.

## Ekstraksi Fitur TF-IDF

Ekstraksi fitur dilakukan menggunakan `TfidfVectorizer` dengan konfigurasi:

- `max_features = 5000`
- `ngram_range = (1, 2)`
- `min_df = 2`

Matriks TF-IDF yang dihasilkan memiliki ukuran:

- 85.449 data
- 5.000 fitur

Sparsity matriks sebesar sekitar 99,14%.

## Performa Model

Dua model machine learning digunakan untuk klasifikasi:

| Model | Accuracy | Macro F1-Score |
|---|---:|---:|
| Logistic Regression | 94,59% | 0,94 |
| Linear SVM | 95,45% | 0,95 |

Evaluasi model juga dilakukan menggunakan:

- Confusion Matrix
- Classification Report
- ROC Curve
- AUC

## File Hasil

Beberapa file hasil eksperimen yang direncanakan untuk disimpan dalam folder ini:

- `tfidf_features.csv` — hasil representasi fitur TF-IDF.
- `tfidf_matrix_shape.txt` — informasi ukuran matriks TF-IDF.
- `cleaned_preview.csv` — contoh data hasil preprocessing.

File hasil berukuran besar tidak seluruhnya disertakan dalam repository.

## Catatan

Hasil di atas merupakan hasil eksperimen dari notebook proyek. Performa model dapat dipengaruhi oleh dataset, preprocessing, konfigurasi TF-IDF, dan pembagian data yang digunakan dalam eksperimen.
