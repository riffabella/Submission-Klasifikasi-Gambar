## Klasifikasi Gambar Animals
----------------------------
Sebuah proyek deep learning untuk pengenalan gambar animals (hewan) menggunakan Convolutional Neural Network (CNN)

---------------------------
## 📝 Penjelasan Proyek 
Proyek ini mengimplementasikan sistem computer vision yang mampu mengenali hewan dari gambar. Sistem ini menggunakan CNN dengan jenis MobileNet yang dilatih pada dataset animals10 untuk mengklasifikasikan gambar hewan ke dalam 10 kelas hewan yang berbeda.

--------------------------
## 📁 Struktur Proyek
submission-klasifikasi-gambar
├───tfjs_model
| ├───group1-shard1of1.bin
| └───model.json
├───tflite
| ├───model.tflite
| └───label.txt
├───saved_model
| ├───saved_model.pb
| └───variables
├───notebook.ipynb
├───README.md
└───requirements.txt

---------------------------
## 🚀 Teknologi yang Digunakan
- Python
- TensorFlow
- MobileNet
- Matplotlib
- Kaggle API
- Google Colab
- Keras

---------------------------
##  🧠 Model dan Training
- Arsitektur: MobileNet
- Optimizer: Adam
- Loss: Categorical Crossentropy
- Penanganan dataset imbalance: Class weights
- Callbacks: EarlyStopping & ReduceLROnPlateau

---------------------------
## 📊 Hasil Training
- Model menunjukkan konvergensi yang baik dalam 3 epoch pertama
- Class imbalance ditangani dengan class weighting
- Penggunaan callbacks berhasil mencegah overfitting

---------------------------
## 📷 Prediksi dan Visualisasi
Model mampu melakukan prediksi gambar acak dari folder test, menampilkan :
- Label prediksi
- Confidence score
- Visualisasi gambar

---------------------------
## ▶️ Cara Menjalankan
1. Pastikan menggunakan teknologi Google Colab untuk mengaksesnya
2. Upload file notebook dan dataset
3. Jalankan setipa sel dari atas hingga bawah
4. Hasil model akan muncul sebagai visualisasi dan prediksi

--------------------------
## 📦 Ekspor Model
Model ini diekspor ke format:
- SavedModel ('saved_model/')
- TensorFlow Lite ('tflite/')
- TensorFlow.js ('tfjs_model/')
