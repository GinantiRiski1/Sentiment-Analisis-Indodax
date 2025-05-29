# Sentiment-Analisis-Indodax

Proyek ini merupakan analisis sentimen terhadap ulasan pengguna aplikasi **Indodax** di Google Play Store. Proyek mencakup proses scraping data, eksplorasi dan preprocessing, hingga analisis lanjutan menggunakan **clustering** dan **klasifikasi** untuk memahami persepsi pengguna terhadap aplikasi.

## 📌 Alur Proyek

1. **Scraping Data Review**
   - Mengambil data ulasan dari Play Store menggunakan `google-play-scraper` atau pustaka serupa.
   - Data yang dikumpulkan mencakup komentar (`content`), tanggal (`at`), rating (`score`), dan lainnya.

2. **Preprocessing Data**
   - Pembersihan teks (lowercase, hapus tanda baca, hapus stopwords, dll).
   - Normalisasi kata tidak baku (alay).
   - Tokenisasi dan transformasi data teks.

3. **Clustering**
   - Mengelompokkan data review berdasarkan kemiripan kontennya menggunakan algoritma seperti K-Means atau DBSCAN.
   - Tujuan: mengetahui pola umum komentar tanpa label eksplisit.

4. **Klasifikasi Sentimen**
   - Data hasil clustering diberi label secara semi-manual atau otomatis.
   - Model klasifikasi dilatih untuk mengenali sentimen (positif, netral, negatif).
   - Algoritma yang digunakan antara lain: Naive Bayes, SVM, LSTM, atau BERT.
