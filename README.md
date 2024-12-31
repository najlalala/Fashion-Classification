# Sistem Klasifikasi Produk Matos Fashion  

## Overview  
Matos Fashion adalah startup e-commerce fashion yang berkembang pesat, menghadapi tantangan dalam pengelolaan dan pengelompokan inventaris produk yang semakin banyak. Fokus utama adalah pada dua jenis produk, yaitu **kaos** dan **hoodie**, dengan berbagai variasi warna seperti **merah**, **kuning**, **biru**, **hitam**, dan **putih**.  

Proyek ini bertujuan mengembangkan **sistem klasifikasi otomatis berbasis foto produk** untuk mengidentifikasi jenis dan warna produk secara akurat. Sistem ini diharapkan membantu meningkatkan efisiensi operasional dan memberikan pengalaman belanja yang lebih baik kepada pelanggan.  

## Tujuan Proyek  
Tujuan dari proyek ini adalah:  
1. Mengembangkan **model klasifikasi multilabel** untuk mengategorikan produk berdasarkan **jenis** dan **warna**.  
2. Mempercepat pengelolaan inventaris produk secara otomatis.  
3. Mendukung pengalaman belanja yang lebih efisien dan memuaskan di platform Matos Fashion.  

## Pendekatan  
### Klasifikasi Multi Label  
Klasifikasi multilabel digunakan dalam proyek ini karena setiap produk dapat memiliki lebih dari satu atribut, yaitu:  
- **Jenis**: Kaos atau Hoodie  
- **Warna**: Merah, Kuning, Biru, Hitam, atau Putih  

Berbeda dengan klasifikasi biner atau multikelas tradisional, klasifikasi multilabel memungkinkan sebuah produk memiliki beberapa label sekaligus.  

### Model dan Teknik yang Digunakan  
1. **Convolutional Neural Network (CNN)**:  
   CNN digunakan untuk memproses gambar produk karena kemampuannya dalam menangkap pola visual seperti bentuk, tekstur, dan warna.  

2. **Transfer Learning**:  
   Model pretrained seperti **ResNet** atau **MobileNet** digunakan sebagai baseline, dioptimalkan lebih lanjut untuk kebutuhan klasifikasi jenis dan warna produk.  

3. **Evaluasi Model**:  
   - **Accuracy**: Untuk mengukur persentase prediksi benar.  
   - **Precision, Recall, dan F1-Score**: Untuk mengevaluasi performa model pada tiap label.  
   - **Hamming Loss**: Untuk menilai kesalahan klasifikasi pada label multilabel.  

## Dataset  
Dataset berisi gambar produk Matos Fashion, dengan atribut sebagai berikut:  
- **Jenis Produk**: Kaos, Hoodie  
- **Warna**: Merah, Kuning, Biru, Hitam, Putih  

Dataset dibagi menjadi:  
- **Training Set**: Untuk melatih model.  
- **Validation Set**: Untuk mengevaluasi performa model selama pelatihan.  
- **Test Set**: Untuk mengukur performa model akhir.  

## Cara Menjalankan Proyek  
### Clone repository  
```bash
git clone https://github.com/username/repo-name.git  
cd repo-name  
```
