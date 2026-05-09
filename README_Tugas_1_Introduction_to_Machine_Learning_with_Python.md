# Introduction to Machine Learning with Python

Repositori ini dibuat untuk memenuhi **Tugas 1 - Enrichment for Machine Learning and Deep Learning Classes**. Isi repositori berfokus pada reproduksi kode, catatan teori, dan ringkasan materi dari buku **Introduction to Machine Learning with Python** karya **Andreas C. Müller** dan **Sarah Guido**.


---

## Deskripsi Proyek

Tujuan utama repositori ini adalah mendokumentasikan proses belajar machine learning menggunakan Python secara bertahap dari setiap chapter pada buku. Setiap notebook berisi kombinasi antara:

- reproduksi kode menggunakan Python dan scikit-learn,
- penjelasan teori dalam Bahasa Indonesia,
- interpretasi output program,
- ringkasan konsep penting dari masing-masing chapter.

Repositori ini tidak hanya berisi hasil kode, tetapi juga penjelasan konseptual agar setiap eksperimen machine learning lebih mudah dipahami.

---

## Daftar Isi

- [Deskripsi Proyek](#deskripsi-proyek)
- [Informasi Buku](#informasi-buku)
- [Struktur Repositori](#struktur-repositori)
- [Ringkasan Chapter](#ringkasan-chapter)
- [Kebutuhan Sistem](#kebutuhan-sistem)
- [Instalasi](#instalasi)
- [Cara Menjalankan Notebook](#cara-menjalankan-notebook)
- [Catatan Kompatibilitas](#catatan-kompatibilitas)
- [Dependencies](#dependencies)
- [Academic Integrity](#academic-integrity)
- [Acknowledgment](#acknowledgment)

---

## Informasi Buku

- **Judul Buku:** Introduction to Machine Learning with Python
- **Penulis:** Andreas C. Müller dan Sarah Guido
- **Publisher:** O'Reilly Media
- **Topik Utama:** Machine Learning, Python, scikit-learn, preprocessing, supervised learning, unsupervised learning, model evaluation, pipeline, dan text data.

---

## Struktur Repositori

Struktur repositori disusun berdasarkan urutan chapter agar mudah dipelajari dan diperiksa.

```text
.
├── README.md
├── requirements.txt
├── notebooks/
│   ├── Chapter_01_Introduction.ipynb
│   ├── Chapter_02_Supervised_Learning.ipynb
│   ├── Chapter_03_Unsupervised_Learning_and_Preprocessing.ipynb
│   ├── Chapter_04_Representing_Data_and_Engineering_Features.ipynb
│   ├── Chapter_05_Model_Evaluation_and_Improvement.ipynb
│   ├── Chapter_06_Algorithm_Chains_and_Pipelines.ipynb
│   ├── Chapter_07_Working_with_Text_Data.ipynb
│   └── Chapter_08_Wrapping_Up.ipynb
├── data/
│   └── README.md
└── images/
    └── README.md
```

Jika beberapa dataset tidak tersedia secara lokal, notebook menggunakan dataset bawaan dari `scikit-learn` atau dataset sederhana yang dibuat langsung pada notebook.

---

## Ringkasan Chapter

### Chapter 1 — Introduction

Chapter ini memperkenalkan konsep dasar machine learning, alasan penggunaan Python, pengenalan library utama seperti NumPy, pandas, matplotlib, dan scikit-learn, serta contoh awal klasifikasi menggunakan dataset Iris.

### Chapter 2 — Supervised Learning

Chapter ini membahas supervised learning untuk classification dan regression. Materi meliputi generalization, overfitting, underfitting, k-Nearest Neighbors, linear models, Naive Bayes, Decision Tree, Random Forest, Gradient Boosting, SVM, dan Neural Network sederhana menggunakan MLP.

### Chapter 3 — Unsupervised Learning and Preprocessing

Chapter ini menjelaskan preprocessing, scaling, dimensionality reduction, PCA, NMF, t-SNE, dan clustering. Fokus utamanya adalah bagaimana data dapat ditransformasikan agar lebih mudah dianalisis atau digunakan oleh model supervised learning.

### Chapter 4 — Representing Data and Engineering Features

Chapter ini membahas pentingnya representasi data dan rekayasa fitur. Materi mencakup categorical variables, one-hot encoding, binning, interaction features, polynomial features, transformasi nonlinear, dan feature selection.

### Chapter 5 — Model Evaluation and Improvement

Chapter ini menjelaskan cara mengevaluasi dan meningkatkan model. Materi utama meliputi cross-validation, grid search, parameter tuning, confusion matrix, precision, recall, F1-score, ROC-AUC, dan pemilihan metrik evaluasi yang sesuai.

### Chapter 6 — Algorithm Chains and Pipelines

Chapter ini membahas penggunaan pipeline untuk menggabungkan preprocessing dan model dalam satu alur kerja. Pipeline membantu mencegah data leakage dan memudahkan eksperimen menggunakan GridSearchCV.

### Chapter 7 — Working with Text Data

Chapter ini membahas pemrosesan data teks. Materi meliputi Bag-of-Words, CountVectorizer, TF-IDF, stop words, n-grams, klasifikasi teks, dan pengenalan topic modeling.

### Chapter 8 — Wrapping Up

Chapter terakhir merangkum workflow machine learning secara menyeluruh, mulai dari memahami masalah, membangun baseline, mengevaluasi model, mempertimbangkan human-in-the-loop, hingga persiapan prototype atau production.

---

## Kebutuhan Sistem

Sebelum menjalankan notebook, pastikan perangkat sudah memiliki:

- Python 3.9 atau versi lebih baru,
- Jupyter Notebook atau JupyterLab,
- Git untuk mengelola repositori,
- koneksi internet jika ingin mengunduh package tambahan,
- environment manager seperti Conda atau Python virtual environment.

---

## Instalasi

### Opsi 1 — Menggunakan Conda

```bash
conda create -n ml-book python=3.9
conda activate ml-book
conda install numpy pandas scikit-learn matplotlib jupyter
pip install mglearn graphviz imageio
```

### Opsi 2 — Menggunakan Virtual Environment

#### Windows

```bash
python -m venv venv
.\venv\Scripts\activate
pip install -r requirements.txt
```

#### macOS / Linux

```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

---

## Cara Menjalankan Notebook

1. Clone repositori dari GitHub.

```bash
git clone https://github.com/username/Introduction-to-Machine-Learning-with-Python.git
cd Introduction-to-Machine-Learning-with-Python
```

2. Aktifkan environment yang sudah dibuat.

```bash
conda activate ml-book
```

3. Jalankan Jupyter Notebook.

```bash
jupyter notebook
```

4. Buka folder `notebooks/` dan pilih chapter yang ingin dijalankan.

---

## Catatan Kompatibilitas

Beberapa kode pada buku aslinya dibuat untuk versi library yang lebih lama. Oleh karena itu, sebagian kode pada repositori ini disesuaikan agar tetap dapat berjalan pada versi Python dan scikit-learn yang lebih baru.

Beberapa hal yang perlu diperhatikan:

### 1. Library `mglearn` belum terpasang

Jika muncul error:

```text
ModuleNotFoundError: No module named 'mglearn'
```

jalankan:

```bash
pip install mglearn
```

### 2. Graphviz tidak ditemukan

Jika visualisasi decision tree gagal, install Graphviz terlebih dahulu.

#### Windows

Unduh installer Graphviz dari website resminya, lalu tambahkan Graphviz ke PATH.

#### macOS

```bash
brew install graphviz
```

#### Ubuntu / Debian

```bash
sudo apt-get install graphviz
```

### 3. Warning dari scikit-learn

Beberapa warning seperti `FutureWarning` atau `ConvergenceWarning` dapat muncul karena perbedaan versi library. Warning tersebut tidak selalu berarti kode gagal, tetapi tetap perlu diperhatikan saat melakukan eksperimen.

---

## Dependencies

Daftar package utama yang digunakan:

```text
numpy
pandas
matplotlib
scikit-learn
jupyter
mglearn
imageio
graphviz
seaborn
```

Jika ingin membuat `requirements.txt`, gunakan contoh berikut:

```text
numpy
pandas
matplotlib
scikit-learn>=1.0
jupyter
mglearn
imageio
graphviz
seaborn
```

---

## Academic Integrity

Repositori ini disusun sebagai bagian dari tugas individu. Penjelasan teori ditulis ulang dalam Bahasa Indonesia dengan gaya sendiri, sedangkan kode direproduksi dan disesuaikan untuk kebutuhan pembelajaran.

Setiap penggunaan referensi dari buku tetap diarahkan untuk tujuan akademik dan pembelajaran, bukan untuk menggantikan isi buku asli.

---

## Acknowledgment

Terima kasih kepada:

- Andreas C. Müller dan Sarah Guido sebagai penulis buku **Introduction to Machine Learning with Python**.
- O'Reilly Media sebagai penerbit buku.
- Komunitas scikit-learn, NumPy, pandas, dan matplotlib yang menyediakan library open-source untuk pembelajaran machine learning.

---

## Status Pengerjaan

- [x] Chapter 1 — Introduction
- [x] Chapter 2 — Supervised Learning
- [x] Chapter 3 — Unsupervised Learning and Preprocessing
- [x] Chapter 4 — Representing Data and Engineering Features
- [x] Chapter 5 — Model Evaluation and Improvement
- [x] Chapter 6 — Algorithm Chains and Pipelines
- [x] Chapter 7 — Working with Text Data
- [x] Chapter 8 — Wrapping Up

---

## Penutup

Repositori ini diharapkan dapat menjadi dokumentasi pembelajaran yang rapi, mudah dijalankan, dan membantu memahami konsep machine learning secara praktis menggunakan Python.
