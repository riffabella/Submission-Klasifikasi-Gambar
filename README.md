# Proyek Klasifikasi Gambar Animals
----------------------------
Sebuah proyek deep learning untuk pengenalan gambar animals (hewan) menggunakan Convolutional Neural Network (CNN)

---------------------------
## 📝 Penjelasan Proyek 
Proyek ini mengimplementasikan sistem computer vision untuk klasifikasi gambar hewan menggunakan arsitektur CNN MobileNet. Model dilatih pada dataset Animals10 dan mampu mengklasifikasikan gambar ke dalam 10 kelas hewan berbeda.

--------------------------
## 📁 Struktur Proyek
```
Submission-Klasifikasi-Gambar
├───tfjs_model
| ├───group1-shard1of1.bin
| └───model.json
├───tflite
| ├───model.tflite
| └───label.txt
├───saved_model
| ├───saved_model.pb
| └───variables
├───Submission_Akhir_Klasifikasi_Gambar.ipynb
├───README.md
└───requirements.txt
```

--------------------------
## 📄 Dataset yang digunakan
Menggunakan dataset dari Kaggle yaitu [Animals10 (Kaggle)](https://www.kaggle.com/datasets/alessiocorrado99/animals10)
terdapat 26.200 gambar yang terbagi kedalam 10 kelas seperti berikut:
- cane: dogs
- cavallo: horses
- elefante: elephants
- farfalla: butterflys
- gallina: chickens
- gatto: cats
- mucca: cows
- pecora: sheeps
- ragno: spiders
- scoittolo: squirrel

---------------------------
## 🚀 Teknologi yang digunakan
- Python
- TensorFlow
- MobileNet
- Numpy
- Matplotlib
- PIL
- OS, shutil, dan random
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
- Training accuracy: 94.10%
- Validation accuracy: 88.66%
- Test accuracy: 91.62%
- Model menunjukkan konvergensi yang baik dalam 3 epoch pertama berdasarkan validation loss
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
- SavedModel ('saved_model/') -> untuk deployment di server atau cloud
- TensorFlow Lite ('tflite/') ->   untuk perangkat mobile dan embedded
- TensorFlow.js ('tfjs_model/') -> untuk dijalankan di browser dan aplikasi berbasis JavaScript
