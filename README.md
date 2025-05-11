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

### Pola Penggunaan
```python
plt.figure(figsize=(12,6))
sns.lineplot(x='hour', y='count', data=df)
plt.title('Distribusi Penggunaan per Jam')
plt.show()
```
