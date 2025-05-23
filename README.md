﻿# Breast Cancer Classification using KNN

Proyek ini bertujuan untuk mengklasifikasikan apakah sel kanker bersifat **malignan** atau **benign** menggunakan algoritma **K-Nearest Neighbors (KNN)** berdasarkan dataset *Breast Cancer Wisconsin* dari UCI yang tersedia di Kaggle.

## 📊 Dataset

Dataset yang digunakan berasal dari Kaggle:

* **Nama**: Breast Cancer (Wisconsin)
* **Sumber**: [https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data)

Dataset ini berisi berbagai fitur dari inti sel kanker yang diambil melalui biopsi, seperti:

* Radius
* Texture
* Perimeter
* Area
* Smoothness
* Dan lainnya (total 30 fitur)

## 🧠 Model yang Digunakan

* **Algoritma**: K-Nearest Neighbors (KNN)
* **Metrik Jarak**: Euclidean Distance
* **Validasi Model**: Cross-validation untuk menentukan nilai *k* (jumlah tetangga terdekat) terbaik.

## ⚙️ Langkah-Langkah

1. **Import dan Eksplorasi Data**
2. **Preprocessing**

   * Null Detection
   * Melakukan **LabelEncoder** untuk kolom class
   * Standarisasi fitur menggunakan **StandardScaler**
   * Pembagian data train-test 80% training 20% testing
3. **Training dengan KNN**

   * Mencari nilai *k* terbaik menggunakan cross-validation
4. **Evaluasi Model**

## ✅ Hasil Evaluasi

Setelah dilakukan pelatihan dan evaluasi, model KNN memberikan hasil sebagai berikut pada data uji:

* **Accuracy**: `0.9386`
* **Precision**: `0.9268`
* **Recall**: `0.9048`

Hasil ini menunjukkan bahwa model cukup akurat dalam mengklasifikasikan jenis kanker.

## 🛠 Tools dan Library

* Python
* Scikit-learn (`KNeighborsClassifier`, `cross_val_score`, `train_test_split`)
* Pandas & NumPy
* Matplotlib / Seaborn (opsional untuk visualisasi)

---
