# Sistem Deteksi Teks Buatan AI Menggunakan NLP

## Deskripsi

Proyek ini merupakan implementasi sistem untuk mendeteksi apakah suatu teks merupakan teks yang dibuat oleh manusia atau dihasilkan oleh Artificial Intelligence (AI).

Sistem memanfaatkan metode **Natural Language Processing (NLP)** untuk melakukan preprocessing teks, ekstraksi fitur menggunakan **TF-IDF**, serta klasifikasi menggunakan algoritma **Logistic Regression** dan **Linear Support Vector Machine (SVM)**.

Proyek ini dibuat sebagai tugas mata kuliah **Pemrosesan Teks**.

## Tujuan

Tujuan dari proyek ini adalah:

- Melakukan preprocessing terhadap data teks.
- Mengekstraksi karakteristik teks menggunakan TF-IDF.
- Membangun model klasifikasi untuk membedakan teks manusia dan teks AI.
- Membandingkan performa Logistic Regression dan Linear SVM.
- Mengevaluasi performa model menggunakan beberapa metrik klasifikasi.

## Dataset

Dataset yang digunakan adalah **HC3 (Human ChatGPT Comparison Corpus)** dalam format klasifikasi biner.

Dataset terdiri dari teks dengan dua label:

- `Human` — teks yang ditulis oleh manusia.
- `AI` — teks yang dihasilkan oleh AI.

Dataset tidak disertakan secara langsung di repository karena ukuran file dan pertimbangan pengelolaan data.

## Metodologi

Tahapan utama dalam proyek ini meliputi:

1. Exploratory Data Analysis (EDA)
2. Pemeriksaan missing value dan duplicate data
3. Text preprocessing
4. Tokenization
5. Stopword removal
6. Lemmatization
7. TF-IDF feature extraction
8. Model training
9. Model evaluation
10. Perbandingan performa model

### Text Preprocessing

Tahapan preprocessing yang digunakan meliputi:

- Case folding
- Penghapusan tanda baca dan simbol
- Normalisasi teks
- Tokenization
- Stopword removal
- Lemmatization

### Feature Extraction

Representasi teks dilakukan menggunakan **TF-IDF (Term Frequency-Inverse Document Frequency)** dengan konfigurasi:

- `max_features = 5000`
- `ngram_range = (1, 2)`
- `min_df = 2`

### Machine Learning Models

Dua algoritma klasifikasi digunakan dalam proyek ini:

- Logistic Regression
- Linear Support Vector Machine (SVM)

## Hasil

Berdasarkan eksperimen yang dilakukan:

| Model | Accuracy | Macro F1-Score |
|---|---:|---:|
| Logistic Regression | 94.59% | 0.94 |
| Linear SVM | 95.45% | 0.95 |

Model **Linear SVM** memperoleh accuracy sebesar **95.45%** pada eksperimen yang dilakukan.

Evaluasi model juga dilakukan menggunakan:

- Confusion Matrix
- Classification Report
- ROC Curve
- AUC

## Struktur Repository

```text
sistem-deteksi-teks-ai-nlp/
├── notebooks/
│   └── KODE_PROYEK_PEMTEKS_KEL_10.ipynb
├── results/
│   ├── cleaned_preview.csv
│   ├── tfidf_features.csv
│   └── tfidf_matrix_shape.txt
├── screenshots/
├── data/
│   └── README.md
└── README.md
