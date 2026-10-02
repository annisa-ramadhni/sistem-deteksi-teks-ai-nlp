# Dataset

Dataset yang digunakan dalam proyek ini adalah **HC3 (Human ChatGPT Comparison Corpus)** untuk tugas klasifikasi teks manusia dan teks yang dihasilkan oleh AI.

## Dataset Utama

File dataset utama yang digunakan dalam eksperimen adalah:

`hc3_binary_classification.csv`

Dataset memiliki tiga kolom utama:

- `question` — pertanyaan atau prompt.
- `answer` — jawaban yang digunakan sebagai data teks.
- `label` — label klasifikasi antara teks manusia dan teks AI.

Pada dataset yang digunakan dalam proyek, terdapat:

- 85.449 baris data
- 58.546 data berlabel Human
- 26.903 data berlabel AI

## Preprocessing

Sebelum digunakan dalam proses klasifikasi, data melalui beberapa tahap preprocessing teks, yaitu:

1. Case folding
2. Penghapusan tanda baca dan simbol
3. Normalisasi teks
4. Tokenization
5. Stopword removal
6. Lemmatization

## Catatan

Dataset mentah tidak disertakan dalam repository karena ukuran file yang besar.

Untuk menjalankan notebook secara penuh, dataset perlu disiapkan secara lokal sesuai dengan nama file yang digunakan pada notebook.

File hasil preprocessing berukuran besar juga tidak disertakan dalam repository.

Dataset digunakan hanya untuk keperluan akademik dalam implementasi dan evaluasi sistem klasifikasi teks.
