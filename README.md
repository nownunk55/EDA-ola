# 🚲 Analisis EDA Permintaan Sewa Sepeda motor Ola

![Bike Sharing](https://github.com/nownunk55/EDA-ola/blob/main/pictures/dataset-cover.png)

Repository ini berisi analisis eksploratif (EDA) terhadap dataset permintaan perjalanan sepeda Ola menggunakan Jupyter Notebook. Analisis mencakup pola penggunaan dan faktor yang mempengaruhi permintaan layanan.

## 📋 Deskripsi Proyek

### Dataset
- **Sumber**: [Ola Bike Ride Request Dataset](https://www.kaggle.com/datasets/palvinder2006/ola-bike-ride-request)
- **Periode**: Januari 2011 - Maret 2012
- **Jumlah Data**: 10,886 observasi

### Fitur Utama
| Kolom        | Deskripsi                              | Tipe Data  |
|--------------|----------------------------------------|------------|
| datetime     | Tanggal dan waktu (YYYY-MM-DD HH:MM:SS)| datetime   |
| season       | Musim (1-4)                            | kategori   |
| weather      | Kondisi cuaca (1-4)                    | kategori   |
| temp         | Temperatur dalam °C                    | float      |
| humidity     | Kelembaban relatif (%)                 | float      |
| windspeed    | Kecepatan angin (km/jam)               | float      |
| casual       | Jumlah pengguna casual                 | integer    |
| registered   | Jumlah pengguna terdaftar              | integer    |
| count        | Total pengguna (casual + registered)   | integer    |

## 🛠️ Teknologi

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Pandas](https://img.shields.io/badge/Pandas-1.3.0-green)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.4.2-red)
![Seaborn](https://img.shields.io/badge/Seaborn-0.11.1-orange)

**Library Pendukung**:
- KaggleHub untuk akses dataset
- NumPy untuk komputasi numerik
- Jupyter Notebook untuk analisis interaktif

## 📈 Hasil Analisis

### 1. Segmentasi Pengguna
![Screenshot 2025-05-11 113929](https://github.com/user-attachments/assets/e8e6b964-9ce6-4c6c-ab26-089ea6015466)

### 2. Pengaruh Musim
![Screenshot 2025-05-11 113910](https://github.com/user-attachments/assets/7fb13230-c8da-45ee-aa02-3f11179dda97)

### 3. Tren Waktu
![Screenshot 2025-05-11 113756](https://github.com/user-attachments/assets/8bbe12b5-6286-44c4-bba1-4a6da2208494)

## 🔍 Insight yang Didapat

### 1. Struktur dan Kualitas Data:
- Dataset terdiri dari 10.886 entri dengan 9 kolom: ```datetime```, ```season```, ```weather```, ```temp```, ```humidity```, ```windspeed```, ```casual```, ```registered```, dan ```count```.

- Tidak ada missing values atau duplikat, menunjukkan kualitas data yang baik.

- Kolom datetime berhasil dikonversi ke tipe datetime untuk analisis temporal.

### 2. Distribusi Data:

- Pengguna terdaftar (registered) mendominasi (sekitar 80%) dibandingkan pengguna kasual (casual), menunjukkan bahwa layanan lebih banyak digunakan oleh pelanggan tetap.

- Variabel cuaca (temp, humidity, windspeed) memiliki rentang nilai yang masuk akal dan dapat dikaitkan dengan pola penggunaan sepeda.

### 2. Analisis Temporal:

- Fitur baru seperti hour, day, dan month berhasil diekstrak dari datetime, yang dapat digunakan untuk analisis penggunaan sepeda berdasarkan waktu.

- Contoh: Penggunaan sepeda mungkin bervariasi tergantung jam, hari, atau musim.

### 3. Korelasi Potensial:

- Variabel seperti suhu (temp) dan kelembapan (humidity) mungkin memiliki korelasi dengan jumlah pengguna (count). Analisis lebih lanjut dengan visualisasi (heatmap, scatter plot) atau model statistik dapat mengungkap hubungan ini.

### 4. Potensi Aplikasi:

- Data ini dapat digunakan untuk membangun model prediksi permintaan sepeda berdasarkan faktor cuaca, waktu, atau musim.

- Insight ini berguna untuk optimasi logistik, pemeliharaan, atau strategi pemasaran Ola.

## ⭐ Rekomendasi untuk Analisis Lanjutan:
- Eksplorasi korelasi antar variabel menggunakan heatmap atau analisis regresi.

- Visualisasi pola penggunaan harian/mingguan untuk identifikasi peak hours.

- Klasifikasi pengguna (casual vs. registered) berdasarkan perilaku penggunaan.

- Prediksi jumlah pengguna dengan model machine learning (contoh: Random Forest, ARIMA untuk time series).

## 📬 Kontak

**Arfan Astadi**  
- ✉️ Email: [arfanastadi46@gmail.com](mailto:arfanastadi46@gmail.com)  
- 💼 LinkedIn: [Kunjungi Profil](https://www.linkedin.com/in/arfan-astadi-3ab480301/)  
- 👨💻 GitHub: [@nownunk55](https://github.com/nownunk55)  
- 🌐 Portfolio: [not readt yet](https://github.com/nownunk55/EDA-ola/)  
