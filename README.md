# 📊 Smartphone Price Analysis

## 📌 Deskripsi Proyek
Industri smartphone merupakan pasar yang sangat kompetitif, dengan lebih dari 1,2 miliar unit dikirim setiap tahun secara global. Selain itu, harga rata-rata smartphone juga terus meningkat, menunjukkan adanya pergeseran preferensi konsumen ke perangkat dengan spesifikasi yang lebih tinggi.

Namun, penentuan harga smartphone bukanlah hal yang sederhana karena dipengaruhi oleh berbagai faktor seperti RAM, kapasitas baterai, dan spesifikasi lainnya. Tanpa analisis data yang tepat, perusahaan berisiko menetapkan harga yang tidak optimal.

Proyek ini bertujuan untuk menganalisis hubungan antara spesifikasi smartphone dan harga peluncuran guna menghasilkan insight yang dapat mendukung pengambilan keputusan bisnis.

---

## 🎯 Tujuan Analisis
- Menganalisis hubungan antara spesifikasi perangkat (RAM, battery, weight) dengan harga smartphone  
- Mengevaluasi konsistensi harga smartphone di berbagai negara  
- Mengidentifikasi tren perkembangan spesifikasi dan harga dari waktu ke waktu  
- Memberikan rekomendasi bisnis berbasis data  

---

## 📂 Dataset
- Sumber: Kaggle (Mobile Dataset)  
- Jumlah data: 930 baris, 15 kolom  

**Fitur utama:**
- Company Name, Model Name  
- RAM, Battery Capacity, Mobile Weight  
- Launched Price (Pakistan, India, China, USA, Dubai)  
- Launched Year  

---

## ⚙️ Proses Analisis

### 1. Data Cleaning
- Menghapus data duplikat (15 data)  
- Menyeragamkan penulisan data (contoh: POCO vs Poco)  
- Membersihkan nilai non-numerik pada kolom RAM dan harga  

### 2. Data Transformation
- Mengubah tipe data menjadi format yang sesuai  
- Mengkonversi seluruh harga ke USD agar dapat dibandingkan  
- Membuat fitur baru: **Average Price (USD)**  

### 3. Handling Outlier
- Menggunakan metode **IQR (Winsorization)**  
- Membatasi nilai ekstrem tanpa menghapus data  

### 4. Exploratory Data Analysis (EDA)
- Analisis distribusi data  
- Analisis korelasi antar variabel  
- Visualisasi hubungan antara spesifikasi dan harga  

---

## 📊 Key Insights

### 1. RAM merupakan faktor utama penentu harga
- Smartphone dengan RAM tinggi memiliki harga jauh lebih mahal  
- Contoh: RAM 16GB ≈ $908 vs RAM 1–2GB ≈ $113–$122  
- Mobile weight tidak memiliki pengaruh signifikan terhadap harga  

### 2. Harga smartphone cenderung konsisten secara global
- Harga di USA, Dubai, India, dan China berada di kisaran yang mirip (~$530–$585)  
- Pakistan memiliki harga lebih rendah (~$446), menunjukkan adanya penyesuaian pasar lokal  

### 3. Spesifikasi meningkat, tetapi harga tidak selalu naik
- RAM meningkat signifikan dari ~1.5GB (2014) menjadi ~9GB (2024–2025)  
- Berat perangkat relatif stabil  
- Harga sempat naik, namun cenderung stabil bahkan menurun di tahun terbaru  

---

## 💡 Business Recommendations

### 1. Fokus pada RAM sebagai driver utama harga
- Tingkatkan kapasitas RAM untuk meningkatkan value produk  
- Lakukan segmentasi produk berdasarkan RAM  

### 2. Terapkan strategi harga global dengan penyesuaian lokal
- Gunakan **global pricing strategy** untuk konsistensi brand  
- Terapkan **localized pricing** untuk market sensitif harga  

### 3. Tingkatkan spesifikasi tanpa menaikkan harga secara signifikan
- Fokus pada peningkatan performa (RAM)  
- Jaga harga tetap kompetitif untuk meningkatkan daya saing  

---

## 🛠 Tools yang Digunakan
- Python (Pandas, Matplotlib, Seaborn)  
- Power BI  
- Microsoft Excel  

---

## 📊 Dashboard
Dashboard digunakan untuk memvisualisasikan:
- KPI utama  
- Perbandingan harga antar negara  
- Hubungan spesifikasi dengan harga  
- Tren perkembangan smartphone  

---

## 📌 Kesimpulan
Analisis menunjukkan bahwa RAM merupakan faktor utama dalam menentukan harga smartphone, sementara faktor lain seperti berat perangkat memiliki pengaruh yang lebih kecil. Selain itu, harga smartphone cenderung konsisten secara global dengan beberapa penyesuaian lokal.

Insight ini dapat membantu perusahaan dalam menentukan strategi pricing dan pengembangan produk yang lebih kompetitif.
