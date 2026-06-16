# Operasi Dasar Sinyal 1D dan Citra 2D serta Uji Linieritas Sistem

Proyek ini dibuat untuk memenuhi tugas praktikum individu pada mata kuliah **Pengolahan Sinyal Digital**. Repositori ini memuat implementasi manipulasi matriks dasar pada sinyal waktu diskrit 1D, operasi spasial pada citra grayscale 2D, serta pembuktian empiris sifat linearitas sistem menggunakan prinsip dasar superposisi.

## 📌 Identitas Mahasiswa
* **Nama:** Muhammad Dafi Al Haq
* **NIM:** 452024611067
* **Program Studi:** Teknik Informatika
* **Fakultas:** Sains dan Teknologi
* **Instansi:** Universitas Darussalam Gontor

## 📂 Struktur Repositori
Sesuai dengan standarisasi manajemen repositori yang ditentukan dalam panduan tugas, struktur direktori diatur sebagai berikut:

```
operasi-dasar-sinyal-citra/
│
├── notebook/
│   └── operasi_sinyal_citra.ipynb   # File Jupyter Notebook utama (Bagian A - C)
│
├── requirements.txt                 # Daftar library eksternal (Dependencies)
└── README.md                        # Dokumentasi utama proyek
```

## 🛠️ Panduan Instalasi & Eksekusi Lokal
1. Clone Repositori
Unduh repositori ini ke penyimpanan lokal komputer Anda menggunakan Git Bash atau Terminal:

```
git clone https://github.com/USERNAME_ANDA/operasi-dasar-sinyal-citra.git
cd operasi-dasar-sinyal-citra
```

2. Instalasi Dependencies
Pastikan lingkungan lokal Anda telah terinstal Python (versi 3.8 ke atas direkomendasikan). Pasang pustaka (libraries) eksternal yang dibutuhkan dengan mengeksekusi perintah berikut pada terminal/command prompt:

```
pip install -r requirements.txt
```

3. Menjalankan Jupyter Notebook
Buka lingkungan kerja interaktif melalui server Jupyter lokal atau editor yang mendukung (seperti VS Code):

```
jupyter notebook notebook/operasi_sinyal_citra.ipynb
```
*Catatan Penting: Pastikan untuk meletakkan berkas citra uji (format .jpg atau .png dengan nama yang disesuaikan pada baris kode cv2.imread) di dalam folder notebook/ sebelum mengeksekusi sel pada Bagian B.

## 📊 Ringkasan Cakupan Eksperimen
 1. Bagian A (Operasi pada Sinyal 1D): Pembangkitan sinyal diskrit sinusoidal murni $x_1[n] = \sin(0.5\pi n)$ dan sinyal langkah satuan (Unit Step) tergeser $x_2[n]$. Eksperimen meliputi operasi penjumlahan linear (efek DC Offset), penggeseran domain waktu (Time-Delay dan Time-Advance menggunakan teknik zero-padding), serta operasi amplifikasi amplitudo menggunakan variasi konstanta skalar $\alpha$.
 2. Bagian B (Operasi pada Citra 2D): Pengolahan citra digital berformat grayscale menggunakan struktur matriks uint8 8-bit. Eksperimen meliputi operasi penjumlahan matriks citra dengan membandingkan metode penanganan overflow intensitas atas (Clipping vs Normalisasi), operasi translasi koordinat spasial menggunakan matriks transformasi Affine 2D, serta manipulasi kontras citra melalui analisis grafik sebaran frekuensi Histogram.
 3. Bagian C (Uji Sistem Linier): Pembuktian matematis dan simulasi pemrograman untuk menguji validitas hukum superposisi (Sifat Additivitas dan Sifat Homogenitas) pada model Sistem Linier $T_1(x) = 2x$ dan model Sistem Non-Linier berbasis fungsi kuadrat $T_2(x) = x^2$.

## 📜 Lisensi
Proyek ini dikembangkan murni untuk keperluan akademis dan pemenuhan tugas kurikulum Universitas Darussalam Gontor.
