# Text Classification Project

## Deskripsi
Proyek ini bertujuan untuk mengklasifikasikan teks berdasarkan apakah teks tersebut mengindikasikan depresi atau tidak. Menggunakan dataset yang berisi teks yang telah dibersihkan dan label yang menunjukkan apakah teks tersebut terkait dengan depresi, model ini dilatih menggunakan algoritma FastText untuk melakukan klasifikasi.

## Dataset
Sumber dataset: https://drive.google.com/uc?id=1ogkVzRs9HptE5nY1dyiQUnB4DsBlFswS

Dataset yang digunakan dalam proyek ini diambil dari sumber online dan terdiri dari dua kolom:
- **clean_text**: Teks yang telah dibersihkan dan diproses.
- **is_depression**: Label biner yang menunjukkan apakah teks tersebut mengindikasikan depresi (1) atau tidak (0).

## Fitur Utama
- **Pengolahan Data**: 
  - Data dibersihkan dengan menghapus karakter yang tidak perlu dan menghapus kata-kata umum (stopwords).
  - Menghapus duplikat dan teks yang tidak relevan dari dataset.
  
- **Visualisasi Data**: 
  - Menampilkan distribusi label depresi dalam dataset menggunakan grafik batang.
  - Menyediakan informasi tentang dimensi data dan jumlah nilai null.

- **Model Pelatihan**: 
  - Menggunakan FastText untuk melatih model klasifikasi teks.
  - Menyimpan dataset pelatihan dan pengujian ke dalam file CSV.

- **Evaluasi Model**: 
  - Menghitung dan menampilkan metrik evaluasi seperti Precision dan Recall.
  - Menampilkan matriks kebingungan untuk analisis hasil.

## Hasil
Setelah melatih model, hasil evaluasi menunjukkan:
- **Sample size**: 1515
- **Precision**: 0.96
- **Recall**: 0.96

Model ini menunjukkan performa yang sangat baik dalam mengklasifikasikan teks terkait depresi.

## Cara Menggunakan
1. Install library yang diperlukan:
   - `pip install fasttext`
   - `python -m nltk.downloader all`

2. Jalankan skrip untuk memprediksi teks:
   - `user_input = input("Input your text: ")`
   - `predict_text(user_input)`

## Contoh Input dan Output
- **Input**: "Some days feel like a never-ending loop of 'fuck this' and 'why even bother'—and you just keep breathing, pretending it's fine."
- **Predicted Label**: `__label__1`
- **Probability**: `0.93609494`

## Kontribusi
Kontribusi sangat diterima! Silakan buka issue atau pull request jika Anda memiliki saran atau perbaikan.
