# Face Recognition & Plate Detection using Haar Cascade and OCR

## Description
Project ini merupakan implementasi Computer Vision menggunakan OpenCV untuk melakukan:

- Face Detection
- Face Blur
- Plate Detection
- Plate Blur
- OCR Plate Recognition

Metode utama yang digunakan adalah Haar Cascade untuk deteksi objek dan EasyOCR untuk membaca teks pada plat nomor kendaraan.

---

# Technologies Used

- Python
- OpenCV
- EasyOCR
- NumPy
- Matplotlib

---

# Methods

## Haar Cascade
Haar Cascade adalah metode deteksi objek yang bekerja dengan mendeteksi perbedaan intensitas terang dan gelap pada citra.

Metode ini menggunakan:
- Haar Feature
- Integral Image
- AdaBoost
- Cascade Classifier

Digunakan untuk:
- Deteksi wajah
- Deteksi plat nomor

---

## OCR (Optical Character Recognition)
OCR digunakan untuk membaca teks dari gambar plat nomor kendaraan menggunakan EasyOCR.

---

## Installation

Install library yang dibutuhkan:

```
pip install opencv-python
pip install easyocr
```

---

## Import Library

```
import cv2
import matplotlib.pyplot as plt
import numpy as np
import os
import easyocr
```

---

## Dataset Structure
```
dataset/
│
├── single_face.jpeg
├── many_face.jpeg
├── multi_face.jpeg
└── plate_car.jpeg
```

---

## Features

1. Face Detection
Mendeteksi satu atau banyak wajah menggunakan Haar Cascade.
2. Face Blur
Memberikan efek blur pada wajah yang terdeteksi menggunakan Gaussian Blur.
3. Plate Detection
Mendeteksi lokasi plat nomor kendaraan pada gambar.
4. Plate Blur
Mengaburkan area plat nomor untuk menjaga privasi kendaraan.
5. OCR Plate Recognition
Membaca karakter pada plat nomor menggunakan EasyOCR.

---

## Workflow

Face Detection
1. Membaca gambar
2. Mengubah gambar menjadi grayscale
3. Melakukan deteksi wajah
4. Memberikan bounding box

---

## Plate Detection

1. Membaca gambar kendaraan
2. Melakukan deteksi plat nomor
3. Menampilkan hasil deteksi

---

# OCR Recognition

1. Crop area plat nomor
2. Thresholding gambar
3. Membaca teks menggunakan OCR
4. Menampilkan hasil pembacaan teks

---

## Example OCR Output
```
Text: N1234AB
Probability: 0.92
```

---

## Parameters
| Parameter    | Function                        |
| ------------ | ------------------------------- |
| scaleFactor  | Mengatur skala pencarian objek  |
| minNeighbors | Mengurangi false detection      |
| minSize      | Menentukan ukuran minimum objek |

---

## Advantages
- Proses deteksi cepat
- Cocok untuk real-time detection
- Implementasi sederhana
- Dapat digunakan untuk sistem keamanan

---

## Future Development
- Real-time webcam detection
- Face recognition dengan identitas pengguna
- Integrasi database kendaraan
- Peningkatan akurasi OCR menggunakan Deep Learning

---

## Author
Fiqrif
