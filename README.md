# DSMBC 2026: Day 3 Modeling

Materi **Machine Learning Modeling** untuk peserta Data Science Bootcamp tingkat pemula.
Notebook ini melanjutkan hasil **Day 2: Data Preprocessing** dengan studi kasus *Credit Risk Classification*.

## Mulai dari sini

Buka `DSMBC_Day3_Modeling.ipynb` dan jalankan cell secara berurutan.
Tiga file CSV hasil Day 2 sudah tersedia di repository, jadi peserta **tidak perlu menjalankan preprocessing lagi**.

### Google Colab

1. Download `DSMBC_Day3_Modeling.ipynb` dari repository ini lalu buka di [Google Colab](https://colab.research.google.com/).
2. Jalankan cell secara berurutan. Saat diminta mengunggah file, pilih ketiga CSV berikut dari repository ini:
   - `credit_train_processed.csv`
   - `credit_validation_processed.csv`
   - `credit_test_processed.csv`
3. Setelah ketiganya terbaca, lanjutkan hingga evaluasi dan penyimpanan model.

### Jupyter Notebook / JupyterLab lokal

Di terminal, jalankan perintah berikut dari folder repository:

```bash
python -m pip install -r requirements.txt
jupyter lab
```

Buka `DSMBC_Day3_Modeling.ipynb` lalu pilih **Run All**. Tiga CSV sudah berada di folder yang sama dengan notebook.

## Isi repository

| File | Fungsi |
| --- | --- |
| `DSMBC_Day3_Modeling.ipynb` | Notebook untuk training, validation, model selection, dan final test |
| `credit_train_processed.csv` | Data untuk melatih model (22.691 baris) |
| `credit_validation_processed.csv` | Data untuk membandingkan model (4.862 baris) |
| `credit_test_processed.csv` | Data untuk evaluasi akhir (4.863 baris) |
| `requirements.txt` | Library Python untuk menjalankan materi inti |

## Alur materi

Dummy Classifier → Logistic Regression → Decision Tree → Random Forest → Tuning sederhana → Evaluasi → Final test → Simpan model.

**Bonus:** XGBoost tersedia sebagai materi opsional. Ubah `COBA_XGBOOST = True` jika ingin mencobanya, setelah menjalankan:

```bash
python -m pip install xgboost
```

## Catatan

- Target adalah `loan_status`. Nilai `1` berarti default, nilai `0` berarti non-default.
- Pemilihan model dan tuning menggunakan validation set. Test set digunakan pada evaluasi akhir.
- Gambar dan GIF di notebook berasal dari sumber eksternal. Atribusi tercantum di bawah media masing-masing. Koneksi internet diperlukan agar media muncul.
- Model yang disimpan hanya menerima fitur yang telah diproses seperti hasil Day 2. Model tersebut bukan pipeline untuk data mentah.
- Materi ini dibuat untuk **pembelajaran**, bukan pengambilan keputusan kredit sungguhan.

## Rujukan materi sebelumnya

- [Day 1: Exploratory Data Analysis](https://github.com/clairedible/DataAnalyst_DSMBC)
- [Day 2: Data Preprocessing](https://github.com/khansafiryal/Preprocessing_DSMBC)

Dataset pada repository ini merupakan hasil pemrosesan **Credit Risk Dataset** dalam notebook Day 2. Tidak ada notebook Day 2 atau dataset mentah dalam repository ini, karena sesi berfokus pada Day 3.
