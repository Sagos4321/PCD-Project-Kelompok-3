# PCD-Project-Kelompok-3

## Nama Anggota
1. NEZA HABIB AZHARI : F1D02410130
2. MUHAMMMAD RIDHO KURNIAWAN : F1D02410079
3. M SAGOS : F1D02410070
4. GAYATRI PRADNYA AIRA PUTRI : F1D02410113

# Project Overview
Kayu merupakan salah satu material yang banyak digunakan dalam industri konstruksi, mebel, dan kerajinan. Identifikasi jenis kayu secara manual umumnya dilakukan berdasarkan pengamatan visual terhadap pola serat kayu, sehingga membutuhkan pengalaman dan keahlian khusus.Dengan memanfaatkan pengolahan citra digital, proses identifikasi jenis kayu dapat dilakukan secara otomatis melalui analisis tekstur permukaan kayu. Karena setiap jenis kayu memiliki karakteristik serat yang berbeda, fitur tekstur yang 
diekstraksi menggunakan metode GLCM dapat digunakan untuk membedakan jenis kayu secara efektif.

Project ini merupakan implementasi Pengolahan Citra Digital (PCD) untuk melakukan klasifikasi citra serat kayu nantu, palapi, dan uru berdasarkan dataset gambar. Dataset yang digunakan terdiri dari tiga kelas utama, yaitu:

1. **Nantu** 
2. **Palapi** 
3. **Uru** 

Dataset diperoleh dari https://www.kaggle.com/datasets/rifaldidwimahendra/serat-kayu-nantu-palapi-and-uru dan telah melalui proses preprocessing sebelum digunakan dalam pelatihan model.

Tujuan utama dari project ini adalah membandingkan beberapa tahapan preprocessing citra untuk melihat pengaruhnya terhadap hasil ekstraksi fitur dan performa model klasifikasi. Proses klasifikasi dilakukan dengan memanfaatkan fitur tekstur dari citra menggunakan metode **Gray Level Co-occurrence Matrix (GLCM)**, kemudian hasil fiturnya digunakan untuk melatih beberapa model machine learning.

Model klasifikasi yang digunakan dalam project ini adalah:
- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)
- Random Forest

Project ini tidak hanya berfokus pada nilai akurasi akhir, tetapi juga pada pemilihan preprocessing yang sesuai, proses ekstraksi fitur, serta analisis hasil evaluasi model. Terdapat empat kombinasi preprocessing yang dibandingkan, mulai dari preprocessing sederhana hingga yang lebih kompleks.

# Kombinasi Preprocessing

| Percobaan | Tahapan Preprocessing |
|-----------|----------------------|
| Percobaan 1 | Resize --> Grayscale |
| Percobaan 2 | Resize --> Grayscale --> Histogram Equalization |
| Percobaan 3 | Resize --> Grayscale --> Histogram Equalization --> Median Filter |
| Percobaan 4 | Resize --> Grayscale --> Histogram Equalization --> Median Filter --> Mean Filter |