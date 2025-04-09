##### *Disclaimer*:
1. *Analisis ini dibuat sebagai bagian dari portofolio pribadi di bidang Data Science.*
2. *Program ditulis menggunakan bahasa pemrograman Python dan menggunakan Bahasa Indonesia. File ReadMe ini juga ditulis dalam Bahasa Indonesia.*

---

# Analisis Data Airbnb Bangkok: Rekomendasi Penginapan untuk Wisatawan

## Deskripsi Proyek

Bangkok adalah salah satu destinasi wisata paling populer di Asia Tenggara, dengan beragam atraksi budaya, kuliner, dan hiburan. Melalui data dari Airbnb Bangkok, analisis ini bertujuan memberikan rekomendasi kepada wisatawan mengenai penginapan yang optimal berdasarkan beberapa faktor penting seperti harga, tipe ruangan, dan jarak ke lima tempat wisata populer di Bangkok.

Tempat wisata yang dijadikan acuan jarak dalam analisis ini adalah:
- Wat Pho  
- Wat Saket  
- Chatuchak Market  
- Ratchada Train Market  
- Wat Arun  

## Tujuan

Tujuan utama dari proyek ini adalah memberikan insight dan rekomendasi penginapan bagi wisatawan berdasarkan:
- Jarak penginapan ke destinasi wisata populer  
- Harga per malam  
- Tipe ruangan yang tersedia  

---

## Dataset

Dataset yang digunakan merupakan data listing Airbnb di Bangkok

---

## Penjelasan Kolom pada Dataset

1. `id` – Identitas unik dari hotel/penginapan.  
2. `name` – Nama dari hotel/penginapan.  
3. `host_id` – Identitas unik dari pemilik hotel/penginapan.  
4. `neighbourhood` – Lingkungan tempat penginapan secara geografis.  
5. `latitude` – Lokasi lintang (menggunakan proyeksi WGS84).  
6. `longitude` – Lokasi bujur (menggunakan proyeksi WGS84).  
7. `room_type` – Tipe ruangan, terdiri dari:
   - **Entire Place (Seluruh rumah/apartemen)**:  
     Cocok bagi tamu yang mencari "rumah kedua". Tamu akan memiliki seluruh tempat untuk diri mereka sendiri, termasuk kamar tidur, kamar mandi, dapur, dan pintu masuk terpisah. Host harus mencantumkan dalam deskripsi jika mereka akan berada di properti tersebut atau tidak.
   - **Private Room (Kamar pribadi)**:  
     Tamu memiliki kamar tidur pribadi, namun mungkin berbagi beberapa ruang dengan orang lain seperti kamar mandi atau dapur.
   - **Shared Room (Kamar bersama)**:  
     Tamu akan tidur di ruang yang juga digunakan oleh orang lain dan berbagi seluruh ruang dengan penghuni lainnya. Umumnya dipilih oleh wisatawan hemat dan fleksibel.
   - **Hotel**:  
     Kamar hotel biasa yang dikelola seperti penginapan profesional.
8. `price` – Harga per malam (dalam mata uang lokal).  
9. `minimum_nights` – Minimal malam menginap.  
10. `number_of_reviews` – Jumlah ulasan yang telah diterima.  
11. `last_review` – Tanggal ulasan terakhir yang diterima.  
12. `calculated_host_listings_count` – Jumlah listing yang dimiliki oleh host tersebut di wilayah tertentu.  
13. `availability_365` – Ketersediaan penginapan dalam setahun (maks 365 hari).  
14. `number_of_reviews_ltm` – Jumlah ulasan dalam 12 bulan terakhir.

---

## Library

Proyek ini menggunakan beberapa library Python berikut:

- `pandas` – Untuk manipulasi data  
- `numpy` – Untuk perhitungan numerik  
- `matplotlib` & `seaborn` – Untuk visualisasi data  
- `geopy` – Untuk perhitungan jarak antar koordinat (opsional)  
- `folium` – Untuk visualisasi data geografis (jika digunakan)

---
# Detail Analisa Lanjutan
Detail analisis lanjutan yang dilakukan menggunakan visualisasi data dengan Tableu. Hasilnya bisa di lihat pada tautan berikut: https://public.tableau.com/app/profile/satrio.prabowo/viz/RekomendasiAirbnbBangkokUntukWisatawan/DashGeneral3?publish=yes