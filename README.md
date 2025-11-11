# Customer Segmentation Analysis on Hotel Booking Data
<img src = "https://th.bing.com/th/id/R.fbd62f5dc6dc3dfe592107722af51b56?rik=6a01UYhR59kUlA&riu=http%3a%2f%2f4.bp.blogspot.com%2f-zjin5XBlDGE%2fVj72wDa6fEI%2fAAAAAAAAAGc%2ffkOLk4vWvUo%2fs1600%2fHotels.jpg&ehk=5usAk8iG0I9OpQmIk0maOaQG6%2fSF4pC8iIbX0PjQutk%3d&risl=&pid=ImgRaw&r=0">
## 🏨 Latar Belakang

Dalam industri perhotelan yang semakin kompetitif, pemahaman mendalam terhadap perilaku pelanggan menjadi faktor kunci untuk meningkatkan kepuasan dan loyalitas tamu. Hotel tidak hanya perlu menarik pelanggan baru, tetapi juga mempertahankan pelanggan lama melalui pelayanan yang lebih personal dan strategi pemasaran yang tepat sasaran. Salah satu pendekatan yang efektif untuk mencapai hal tersebut adalah melalui Customer Segmentation Analysis, yaitu pengelompokan pelanggan berdasarkan karakteristik dan perilaku mereka.

Dataset Hotel Bookings ini berisi lebih dari 119.000 catatan pemesanan dari dua jenis hotel — City Hotel dan Resort Hotel. Data ini mencakup berbagai informasi seperti:
waktu pemesanan (lead time), lama menginap, jumlah tamu dewasa dan anak-anak, harga rata-rata per malam (Average Daily Rate), jenis pelanggan, serta status pemesanan (dibatalkan atau tidak).

Dengan melakukan segmentasi pelanggan, pihak manajemen hotel dapat:
1. Mengidentifikasi pola perilaku tamu, seperti kelompok pelanggan yang sering memesan jauh hari atau yang lebih sensitif terhadap harga.
2. Menentukan strategi pemasaran yang lebih efektif, misalnya memberikan promosi tertentu kepada segmen pelanggan yang sering membatalkan pesanan.
3. Meningkatkan efisiensi operasional, dengan memprediksi permintaan kamar dari masing-masing segmen.
4. Meningkatkan loyalitas pelanggan, dengan menawarkan layanan yang sesuai dengan kebutuhan dan preferensi tiap segmen.
Oleh karena itu, analisis segmentasi pelanggan pada dataset ini bertujuan untuk mengelompokkan pelanggan hotel berdasarkan kesamaan perilaku pemesanan dan karakteristik menginap, sehingga dapat mendukung pengambilan keputusan berbasis data dalam strategi pemasaran dan pelayanan hotel

## 🎯 Project Overview
Dalam industri perhotelan, tingkat pembatalan yang tinggi dapat berdampak besar terhadap pendapatan dan efisiensi operasional.  
Melalui proyek ini, dilakukan analisis untuk:
- Mengidentifikasi faktor-faktor yang memengaruhi pembatalan.
- Mengelompokkan pelanggan berdasarkan perilaku mereka (clustering).
- Memberikan rekomendasi strategis bagi manajemen hotel.

---

## 🧹 Data Preprocessing
Langkah-langkah yang dilakukan:
1. Menangani missing values menggunakan imputasi rata-rata/median dan penghapusan baris tertentu.
2. Menghapus dan menangani **outliers** menggunakan metode IQR (Interquartile Range).
3. Melakukan encoding pada fitur kategorikal.
4. Normalisasi dan standarisasi data numerik.

---

## 🔍 Exploratory Data Analysis (EDA)
Analisis dilakukan untuk mendapatkan insight awal:
- Distribusi pembatalan per cluster pelanggan.  
- Korelasi fitur numerik terhadap pembatalan.  
- Perbandingan pembatalan pelanggan baru vs pelanggan tetap.  
- Hubungan riwayat pembatalan dengan kemungkinan pembatalan berikutnya.  
- Distribusi harga per malam (*ADR*) terhadap pembatalan.

---

## 🤖 Modeling – K-Means Clustering
Digunakan untuk mengelompokkan pelanggan menjadi beberapa segmen berdasarkan pola pemesanan:
- Fitur yang digunakan: `lead_time`, `adr`, `total_nights`, `total_guests`, dan `special_requests`
- Hasil menunjukkan adanya perbedaan signifikan antar cluster dalam hal tingkat pembatalan dan perilaku pelanggan.

---

## 📊 Visualization
Visualisasi dibuat menggunakan:
- **Python (Matplotlib, Seaborn)** untuk eksplorasi data.
- **Power BI** untuk membangun satu halaman *Summary Dashboard* interaktif.

---

## 💡 Insights & Recommendations
- Pelanggan dengan **lead time panjang** lebih berisiko membatalkan.
- **Harga kamar tinggi (ADR)** juga cenderung meningkatkan kemungkinan pembatalan.
- **Pelanggan baru** memiliki tingkat pembatalan yang lebih tinggi daripada pelanggan tetap.
- Disarankan untuk memberikan **promosi atau kebijakan deposit fleksibel** bagi pelanggan dengan risiko tinggi.

---

## 🧰 Tech Stack
- Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn)
- Power BI
