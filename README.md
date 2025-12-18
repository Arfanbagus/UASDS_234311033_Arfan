# 📘 Judul Proyek
*(Analisis Autism Spectrum Disorder (ASD) pada Anak menggunakan Model Baseline, Machine Learning, dan Deep Learning)*

## 👤 Informasi
- **Nama:** [Arfan Bagus D]  
- **Repo:** [https://github.com/Arfanbagus/UASDS_234311033_Arfan.git]  
- **Video:** [https://youtu.be/WuLm3Hctk4A]  

---

# 1. 🎯 Ringkasan Proyek
- Menyelesaikan permasalahan sesuai domain  
- Melakukan data preparation  
- Membangun 3 model: **Baseline**, **Advanced**, **Deep Learning**  
- Melakukan evaluasi dan menentukan model terbaik  

---

# 2. 📄 Problem & Goals
**Problem Statements:**  
- [Belum diketahui model baseline, advanced machine learning, atau deep learning yang memberikan performa terbaik dan paling stabil dalam mengklasifikasikan diagnosis ASD (Yes/No) pada data tabular yang tersedia.]  
- [Diperlukan model deep learning yang mampu mempelajari pola nonlinear yang kompleks dari interaksi antara jawaban kuesioner perilaku dan faktor karakteristik anak dalam menentukan indikasi autisme.]
- [Dibutuhkan model machine learning yang mampu memprediksi risiko Autism Spectrum Disorder (ASD) pada anak dengan akurasi tinggi berdasarkan fitur demografis, riwayat medis keluarga, dan skor perilaku dari kuesioner skrining.]
- [Dataset memiliki campuran fitur kategorikal (seperti etnis, gender, riwayat penyakit) dan numerik (usia, skor tes) sehingga diperlukan proses preprocessing yang tepat, termasuk encoding, scaling, dan feature engineering agar model dapat belajar secara optimal dari data medis tersebut.]

**Goals:**  
- [Membangun model klasifikasi untuk memprediksi label Class/ASD (YES/NO).]  
- [Membandingkan performa tiga algoritma: Logistic Regression, Random Forest, dan Deep Learning (MLP).]
- [Mendapatkan model dengan akurasi dan F1-Score yang optimal untuk data medis yang tersedia.]

---
## 📁 Struktur Folder
```
project/
│
├── data/                   # Dataset (tidak di-commit, download manual)
│
├── notebooks/              # Jupyter notebooks
│   └── UAS_234311033_Arfan_Bagus_Dharamawan.ipynb
│
├── src/                    # Source code
│   
├── models/                 # Saved models
│   ├── model_logistic_regression.pkl
│   ├── model_random_forest.pkl
│   └── model_deep_learning.h5
│
├── images/                 # Visualizations
│   ├── accuracy_loss_epoch.png         # Accuracy Per Epoch and Loss Per Epoch
│   ├── barplot.png                     # Bar Plot
│   ├── baseline_lr.png                 # Baseline Logistic Regression
│   ├── boxplot_noise_result.png        # Boxplot Noise Result
│   ├── boxplot_noise.png               # Boxplot Noise
│   ├── confusion_dl_valid.png          # Confusion Matrix Deep Learning (Validation)
│   ├── confusion_mlp.png               # Confusion Matrix MLP
│   ├── confusion_rf.png                # Confusion Matrix Random Forest
│   ├── korelasi_heatmap.png            # Correlation Heatmap
│   ├── perbandingan_tiga_model.png     # Perbandingan Tiga Model
│   └── scatter_plot.png                # Scatter Plot
│
├── Requirements.txt        # Dependencies
├── .gitignore
└── README.md
```
---

# 3. 📊 Dataset
- **Sumber:** [https://archive.ics.uci.edu/dataset/419/autistic+spectrum+disorder+screening+data+for+children ]  
- **Jumlah Data:** [292]  
- **Tipe:** [Tabular]  

### Fitur Utama
| Fitur | Deskripsi |
|------|-----------|
| A1_Score | Skor jawaban pertanyaan screening autisme nomor 1 |
| A2_Score | Skor jawaban pertanyaan screening autisme nomor 2 |
| A3_Score | Skor jawaban pertanyaan screening autisme nomor 3 |
| A4_Score | Skor jawaban pertanyaan screening autisme nomor 4 |
| A5_Score | Skor jawaban pertanyaan screening autisme nomor 5 |
| A6_Score | Skor jawaban pertanyaan screening autisme nomor 6 |
| A7_Score | Skor jawaban pertanyaan screening autisme nomor 7 |
| A8_Score | Skor jawaban pertanyaan screening autisme nomor 8 |
| A9_Score | Skor jawaban pertanyaan screening autisme nomor 9 |
| A10_Score | Skor jawaban pertanyaan screening autisme nomor 10 |
| age | Usia anak dalam tahun |
| gender | Jenis kelamin anak (Male / Female) |
| ethnicity | Etnis anak |
| jaundice | Riwayat jaundice saat lahir (yes / no) |
| family_pdd | Riwayat gangguan perkembangan dalam keluarga (yes / no) |
| country_of_res | Negara tempat tinggal anak |
| used_app_before | Apakah pernah menggunakan aplikasi screening sebelumnya |
| result | Total skor hasil screening |
| age_desc | Kategori usia anak |
| relation | Hubungan pengisi kuesioner dengan anak |
| class | Label target: apakah anak terindikasi ASD (yes / no) |

---

# 4. 🔧 Data Preparation
Tahap Data Preparation yang dilakukan:
- Cleaning (check missing values/duplicate/outliers)  
- Transformasi (Menggunakan encoding = One-hot Encoding/scaling = standartScaller)  
- Splitting (pembagian data train 70%/val 15%/test 15%)  

---

# 5. 🤖 Modeling
- **Model 1 – Baseline:** [Menggunakan model Logistic Regression]  
- **Model 2 – Advanced ML:** [Menggunakan model Random Forest Classifier]  
- **Model 3 – Deep Learning:** [Menggunakan teknik MLP pada model Deep Learning]  

---

# 6. 🧪 Evaluation
**Metrik:** Accuracy / F1 / MAE / MSE (pilih sesuai tugas)
- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

### Hasil Singkat
| Model | Score | Catatan |
|-------|--------|---------|
| Baseline(Logistic Regression) | [0.47] | Performa dasar sebagai pembanding, akurasi masih rendah |
| Advanced(Random Forest) | [0.48] | Sedikit peningkatan dari baseline, namun belum signifikan |
| Deep Learning(MLP) | [0.55] | Paling Stabil |

---

# 7. 🏁 Kesimpulan
- Model terbaik: [Deep Learning]  
- Alasan: [Memberikan akurasi tertinggi dibandingkan model lain serta menunjukkan stabilitas performa yang baik pada data validasi. ]  
- Insight penting: [Peningkatan kompleksitas model memberikan peningkatan performa, meskipun membutuhkan waktu komputasi yang lebih tinggi. dan Model Deep Learning lebih mampu menangkap pola non-linear pada data dibandingkan Baseline dan Advanced model.]  

---

# 8. 🔮 Future Work
- [x] **Menambah jumlah dan variasi data** untuk meningkatkan generalisasi model dan mengurangi risiko overfitting.  
- [x] **Melakukan hyperparameter tuning** pada setiap model (learning rate, jumlah layer, jumlah neuron, dan regularisasi) guna memperoleh performa optimal.  
- [ ] **Mencoba arsitektur Deep Learning lain** seperti CNN atau model hybrid untuk membandingkan efektivitas dalam menangkap pola data.  
- [ ] **Melakukan deployment model** ke dalam aplikasi web atau mobile agar dapat digunakan secara langsung sebagai sistem screening awal ASD.  
- [ ] **Menambahkan evaluasi lanjutan** seperti cross-validation dan analisis fairness untuk memastikan model bekerja konsisten pada berbagai kelompok data.

---

# 9. 🔁 Reproducibility
Gunakan environment:
- Environment
- Python: 3.12
- Operating System: Windows / Linux / macOS

Dependencies
- numpy==1.24.3
- pandas==2.0.3
- scikit-learn==1.3.0
- matplotlib==3.7.2
- seaborn==0.12.2
- tensorflow==2.14.0
