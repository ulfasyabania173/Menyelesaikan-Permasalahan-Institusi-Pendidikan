# Proyek Akhir: Menyelesaikan Permasalahan Perusahaan Edutech

## Business Understanding
Perusahaan Edutech ini berfokus pada penyediaan solusi pendidikan berbasis teknologi yang bertujuan meningkatkan retensi serta kesuksesan akademik mahasiswa. Di tengah persaingan industri dan tuntutan kualitas pendidikan yang tinggi, perusahaan ingin mengidentifikasi faktor-faktor yang memengaruhi performa dan dropout mahasiswa guna mengoptimalkan intervensi dan kebijakan pendukung.

### Permasalahan Bisnis
- **Prediksi Dropout dan Academic Success:** Menentukan mahasiswa mana yang berisiko melakukan dropout serta mengidentifikasi faktor yang memengaruhi kesuksesan akademik.
- **Segmentasi Mahasiswa:** Mengelompokkan mahasiswa berdasarkan kinerja akademik dan demografi untuk menyusun strategi intervensi yang lebih tepat.
- **Optimalisasi Intervensi:** Mengimplementasikan mekanisme pendeteksian dini untuk membantu menyediakan bantuan secara tepat waktu kepada mahasiswa berisiko.

### Cakupan Proyek
- **Data Preprocessing dan Cleaning:** Melakukan pembersihan data, penanganan outlier, dan duplikasi untuk memastikan integritas data.
- **Data Visualization dan Clustering:** Membuat visualisasi (pair plot, boxplot, PCA) serta teknik clustering untuk memahami struktur data dan segmentasi mahasiswa.
- **Feature Engineering & Mapping Target:** Melakukan mapping data target ke bentuk numerik dan mengekstraksi kategori utama guna menyederhanakan analisis.
- **Modeling & Evaluasi:** Mengembangkan model klasifikasi (Logistic Regression) dengan penyesuaian teknik penyeimbangan (class_weight dan SMOTE) serta evaluasi menggunakan metrik akurasi, classification report, dan confusion matrix.
- **Prototype Sistem Machine Learning:** Membangun prototipe prediksi yang dapat diakses melalui web untuk membantu mengambil keputusan.

### Persiapan
**Sumber Data:**  
[Predict Students Dropout and Academic Success](https://archive.ics.uci.edu/dataset/697/predict+students+dropout+and+academic+success)

**Setup Environment:**  
Pastikan Anda telah menginstal library berikut:

```
pip install numpy pandas matplotlib seaborn scikit-learn imbalanced-learn streamlit
```

Kemudian buat virtual environment jika diperlukan agar dependensi terisolasi.

## Business Dashboard
Dashboard bisnis telah dibuat menggunakan Looker Studio dengan judul **"Dashboard Prediksi Dropout & Kesuksesan Akademik Mahasiswa Edutech"**. Dashboard ini menampilkan insight dari data seperti segmentasi mahasiswa, kinerja akademik, dan prediksi dropout.  
Anda dapat mengakses dashboard tersebut melalui link berikut:  
[Dashboard Prediksi Dropout & Kesuksesan Akademik Mahasiswa Edutech](https://lookerstudio.google.com/reporting/e9b0f321-717f-46b2-bb3d-9544280dabcc)

## Menjalankan Sistem Machine Learning
Prototype sistem machine learning dapat dijalankan melalui link berikut, yang menyediakan aplikasi web berbasis Streamlit untuk memprediksi dropout mahasiswa:  
[Prototype Dropout Predictor](https://dropout-predictor-ulfasyabania.streamlit.app/)

Untuk menjalankan prototype secara lokal, pastikan semua dependensi sudah terinstal, kemudian jalankan:

```
streamlit run app.py
```

## Conclusion
Proyek ini telah berhasil mengidentifikasi pola utama yang memengaruhi dropout dan kesuksesan akademik mahasiswa. Hasil evaluasi menunjukkan bahwa model Logistic Regression yang dikembangkan menghasilkan akurasi sekitar **84%** dengan performa klasifikasi yang cukup baik. Model ini mampu mengidentifikasi mahasiswa berisiko dropout dengan cukup efektif, meskipun masih terdapat ruang untuk perbaikan dalam meningkatkan recall agar lebih banyak mahasiswa yang berisiko dapat dideteksi secara dini.

### Rekomendasi Action Items
- **Intervensi Dini:** Optimalisasi sistem pendeteksian dropout untuk mengidentifikasi mahasiswa yang berisiko sehingga intervensi dapat dilakukan secara tepat waktu.
- **Dashboard Monitoring:** Implementasikan dashboard real-time guna memantau kinerja akademik dan tren dropout.
- **Tuning Model Lanjutan:** Lakukan eksperimen lebih lanjut dengan hyperparameter tuning dan algoritma lain untuk meningkatkan performa model, khususnya pada pengidentifikasian dropout.
