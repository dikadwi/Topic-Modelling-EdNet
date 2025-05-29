# 📘 Pemodelan Topik untuk Pembentukan Profil Belajar Menggunakan LDA pada Dataset EdNet-KT1

Repositori ini berisi kode sumber, subset data, serta notebook eksperimen yang digunakan dalam penelitian:

> **"Pemodelan Topik untuk Membentuk Profil Belajar Menggunakan LDA dan Evaluasi Koherensi"**  
> *Andika Dwi Arko*, *Muhamad Yusril Helmi Setyawan*  

---

## 🔍 Ringkasan Proyek

Penelitian ini mengembangkan pendekatan untuk membentuk **profil belajar berbasis topik** dari data interaksi siswa skala besar menggunakan algoritma **Latent Dirichlet Allocation (LDA)**. Dataset yang digunakan adalah **EdNet-KT1**, yang berisi interaksi siswa dengan soal berbasis tag semantik. Setiap soal dikonversi menjadi pseudoteks, dimodelkan ke dalam 20 topik, dan dihubungkan dengan akurasi siswa pada tiap topik untuk membentuk matriks performa siswa.

---

## 🧪 Fitur Utama

- Ekstraksi topik semantik dengan **LDA (Gensim)**
- Evaluasi kualitas model menggunakan nilai *coherence* (**0,6688**)
- Representasi akurasi siswa per topik (user × topic matrix)
- Visualisasi profil belajar: **heatmap**, **radar chart**, **line plot**
- Segmentasi siswa menggunakan **K-Means** dan visualisasi dengan **PCA**
- Rekomendasi topik adaptif berdasarkan ambang akurasi

---

## 📁 Struktur Folder
* data/


* notebooks/

* figures/
* requirements.txt
* LICENSE
* README.md

---

## 💾 Dataset

- **EdNet-KT1** disediakan oleh Riiid Labs, berisi lebih dari 131 juta interaksi siswa.
- Subset data (~1000 file log) digunakan untuk alasan efisiensi komputasi.
- Sumber: [https://github.com/riiid/ednet](https://github.com/riiid/ednet)  
- Lisensi: **Creative Commons BY-NC 4.0** (penggunaan non-komersial)

---

## ▶️ Cara Menjalankan

### Prasyarat
- Python 3.9+
- Jupyter Notebook atau Google Colab
- RAM ≥ 12 GB disarankan

### Instalasi
```bash
git clone https://github.com/username/Topic-Modeling-EdNet.git
cd Topic-Modeling-EdNet
pip install -r requirements.txt


