# Prediksi Kelayakan Pinjaman Nasabah

Proyek klasifikasi untuk memprediksi kelayakan pinjaman nasabah menggunakan **Random Forest** (Python, scikit-learn). Dikerjakan sebagai Final Project mata kuliah Big Data.

## Dataset

- Jumlah data: **614 nasabah**, **11 fitur** (tidak termasuk ID nasabah)
- Target: `StatusPinjaman` (Y = layak / N = tidak layak)
- Fitur: jenis kelamin, status pernikahan, jumlah tanggungan, pendidikan, wiraswasta, income nasabah, income pasangan, jumlah pinjaman, jangka waktu pinjaman, riwayat kredit, dan wilayah tempat tinggal

## Metode

1. **Pra-pemrosesan data**
   - Imputasi missing value: mean (fitur numerik) dan modus (fitur kategorikal)
   - Label encoding untuk variabel kategorikal
   - Pembagian data latih/uji 80:20
2. **Pemodelan:** Random Forest Classifier
3. **Evaluasi:** 5-fold cross-validation, confusion matrix, dan feature importance

## Hasil

| Fold | Akurasi |
|------|---------|
| 1 | 0,76 |
| 2 | 0,80 |
| 3 | 0,80 |
| 4 | 0,77 |
| 5 | 0,80 |
| **Rata-rata** | **0,79** |

## Cara Menjalankan

1. Clone repository:
   ```bash
   git clone https://github.com/Sall24/loan-approval-classification-random-forest.git
   cd loan-approval-classification-random-forest
   ```
2. Install library yang dibutuhkan:
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn jupyter
   ```
3. Buka dan jalankan notebook (pastikan path dataset sesuai lokasi file CSV):
   ```bash
   jupyter notebook
   ```

## Struktur Repository

```
.
├── dataset-pinjaman-nasabah.csv   # dataset
├── <nama-notebook>.ipynb          # notebook analisis dan model
└── README.md
```

## Teknologi

Python, pandas, NumPy, scikit-learn, Jupyter Notebook

## Author

**Faisal Akbar Ilham Arya Ardhi**
Informatika, Universitas Amikom Yogyakarta
GitHub: [@Sall24](https://github.com/Sall24)
