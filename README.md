# ✈️ DATA WAREHOUSE DAN VISUALISASI DATA PENERBANGAN 2015

## 2015 Flight Delays and Cancellations

---


# Anggota 

Mohamad Ariel Saputra D Loi	2409116087

Muhammad Nur Alfian	2409116105

Ahmad Samsul Arifin	2409116113

Ahmad Qomarul Arifin	2409116114

---

# 📋 Deskripsi Proyek

Project ini merupakan implementasi proses ETL (Extract, Transform, Load), pembuatan Data Warehouse, serta visualisasi data menggunakan dataset **2015 Flight Delays and Cancellations**.

Fokus utama project meliputi:

* proses ETL menggunakan Python
* pembuatan fact table dan dimension table
* cleaning data
* visualisasi data penerbangan
* analisis keterlambatan dan pembatalan penerbangan

Project dikerjakan menggunakan Google Colab dengan bantuan library Python seperti Pandas dan Matplotlib.

---

# 🎯 Tujuan Project

| Tujuan                   | Keterangan                                  |
| ------------------------ | ------------------------------------------- |
| Membangun Data Warehouse | Membuat fact table dan dimension table      |
| Menerapkan ETL           | Extract, Transform, Load menggunakan Python |
| Analisis Data            | Analisis delay dan pembatalan penerbangan   |
| Visualisasi Data         | Membuat grafik analisis penerbangan         |

---

# 🛠 Tech Stack

| Komponen           | Teknologi          |
| ------------------ | ------------------ |
| Bahasa Pemrograman | Python 3           |
| Library            | Pandas, Matplotlib |
| Environment        | Google Colab       |
| Arsitektur         | Star Schema        |
| Dataset            | CSV Dataset        |

---

# 📊 Dataset

Dataset yang digunakan:

* flights.csv
* airlines.csv
* airports.csv

Dataset berasal dari:

## 2015 Flight Delays and Cancellations

---

# 📁 Deskripsi Dataset

| File         | Deskripsi                  |
| ------------ | -------------------------- |
| flights.csv  | Data transaksi penerbangan |
| airlines.csv | Data maskapai penerbangan  |
| airports.csv | Data bandara penerbangan   |

---

# 🏗 Arsitektur Data Warehouse

Project ini menggunakan konsep **Star Schema** dengan:

* 1 fact table
* 2 dimension table

---

# 📌 Fact Table

## fact_flights

Berisi data utama penerbangan seperti:

* tahun penerbangan
* bulan penerbangan
* maskapai
* bandara asal dan tujuan
* delay keberangkatan
* delay kedatangan
* pembatalan penerbangan

---

# 📌 Dimension Table

## dim_airline

Berisi informasi detail maskapai penerbangan.

Contoh:

* kode maskapai
* nama maskapai

---

## dim_airport

Berisi informasi detail bandara penerbangan.

Contoh:

* kode bandara
* nama bandara
* kota
* negara bagian

---

# ⚙️ Proses ETL

## 1. Extract

Membaca dataset CSV:

* flights.csv
* airlines.csv
* airports.csv

---

## 2. Transform

Melakukan proses:

* pemilihan kolom
* pembuatan fact table
* pembuatan dimension table
* cleaning data null
* filtering data

---

## 3. Load

Menyimpan hasil ETL menjadi file CSV baru:

* fact_flights_fix.csv
* dim_airline_fix.csv
* dim_airport_fix.csv

---

# 📊 Visualisasi Data

Visualisasi yang dibuat pada project ini:

| No | Visualisasi                               | Jenis Grafik         |
| -- | ----------------------------------------- | -------------------- |
| 1  | Top 10 Airline with Highest Arrival Delay | Bar Chart            |
| 2  | Top 10 Airport with Highest Arrival Delay | Horizontal Bar Chart |
| 3  | Distribution of Arrival Delay             | Histogram            |
| 4  | Box Plot of Arrival Delay                 | Box Plot             |
| 5  | Departure Delay vs Arrival Delay          | Scatter Plot         |
| 6  | Average Arrival Delay per Airline         | Area Chart           |

---

# 📈 Penjelasan Visualisasi

## 1. Top 10 Airline with Highest Arrival Delay

Menampilkan maskapai dengan rata-rata keterlambatan kedatangan tertinggi.

---

## 2. Top 10 Airport with Highest Arrival Delay

Menampilkan bandara dengan rata-rata keterlambatan tertinggi.

---

## 3. Distribution of Arrival Delay

Menampilkan distribusi atau penyebaran data keterlambatan kedatangan pesawat.

---

## 4. Box Plot of Arrival Delay

Menampilkan persebaran data serta mendeteksi outlier atau delay ekstrem.

---

## 5. Departure Delay vs Arrival Delay

Menampilkan hubungan antara delay keberangkatan dan delay kedatangan.

---

## 6. Average Arrival Delay per Airline

Menampilkan perbandingan rata-rata delay antar maskapai.

---

# 📂 Struktur Repository

```text
project/
│
├── dataset/
│   ├── flights.csv
│   ├── airlines.csv
│   └── airports.csv
│
├── data_warehouse/
│   ├── fact_flights_fix.csv
│   ├── dim_airline_fix.csv
│   └── dim_airport_fix.csv
│
├── notebook/
│   └── etl_visualisasi.ipynb
│
└── README.md
```

---

# 🚀 Cara Menjalankan Project

## Menggunakan Google Colab

1. Upload dataset CSV ke Google Colab
2. Jalankan seluruh cell notebook
3. Proses ETL akan berjalan otomatis
4. Visualisasi data akan muncul
5. Hasil ETL dapat didownload dalam format CSV

---

# 📄 Output Project

Output yang dihasilkan:

* fact table
* dimension table
* visualisasi data
* file CSV hasil ETL

---

# 📌 Hasil Analisis

Berdasarkan hasil visualisasi:

* beberapa maskapai memiliki rata-rata delay yang tinggi
* terdapat bandara dengan tingkat keterlambatan besar
* delay keberangkatan mempengaruhi delay kedatangan
* terdapat data delay ekstrem pada beberapa penerbangan

---

# 📝 Kesimpulan

Project berhasil melakukan proses:

* ETL (Extract, Transform, Load)
* pembuatan Data Warehouse
* cleaning data
* visualisasi data penerbangan

---

# Link 

* Google collab: https://colab.research.google.com/drive/16J3dHjz7U2kXUQR-rL8Z0EG9JTaZiZ1R?usp=sharing
* dataset kagle: https://www.kaggle.com/datasets/usdot/flight-delays


Visualisasi yang dibuat membantu memahami pola keterlambatan dan pembatalan penerbangan pada dataset tahun 2015 menggunakan Python di Google Colab.
