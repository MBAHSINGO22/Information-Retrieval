# Information Retrieval System with Inverted Index

Sistem Temu Kembali Informasi (Information Retrieval System) berbasis Python yang mengimplementasikan teknik **Inverted Index** untuk melakukan pencarian dokumen teks secara efisien.

## Deskripsi

Project ini dikembangkan untuk mengelola sekumpulan dokumen teks (`.txt`) dan menyediakan fasilitas pencarian informasi menggunakan metode Inverted Index.

Sistem akan melakukan preprocessing dokumen, membangun indeks kata, kemudian mengembalikan dokumen yang relevan berdasarkan kata kunci atau frasa yang dimasukkan pengguna.

Project ini merupakan implementasi konsep dasar Information Retrieval yang banyak digunakan pada mesin pencari modern.

---

## Fitur Utama

- Upload dokumen dalam format ZIP
- Ekstraksi otomatis file teks
- Preprocessing dokumen
  - Case Folding
  - Tokenisasi
  - Penghapusan Stopword
- Pembuatan Inverted Index
- Pencarian berdasarkan satu kata
- Pencarian berdasarkan beberapa kata
- Pencarian frasa
- Menampilkan dokumen yang relevan
- Antarmuka berbasis terminal

---

## Teknologi yang Digunakan

- Python 3
- Google Colab
- Regular Expression (Regex)
- Collections Module
- Inverted Index Algorithm

---

## Struktur Project

```text
project/
│
├── UTS2_PI.ipynb
├── dataset.zip
├── extracted_files/
│   ├── dokumen1.txt
│   ├── dokumen2.txt
│   └── ...
└── README.md
```

---

## Cara Kerja Sistem

### 1. Upload Dokumen

Pengguna mengunggah file ZIP yang berisi kumpulan dokumen teks.

### 2. Ekstraksi Dokumen

Sistem mengekstrak seluruh file `.txt` ke dalam folder kerja.

### 3. Preprocessing

Setiap dokumen diproses melalui beberapa tahapan:

- Konversi huruf menjadi lowercase
- Penghapusan karakter khusus
- Tokenisasi kata
- Penghapusan stopword

### 4. Pembangunan Inverted Index

Sistem membangun struktur data:

```text
kata → daftar dokumen yang mengandung kata tersebut
```

Contoh:

```text
python → doc1, doc3, doc5
data   → doc2, doc3
```

### 5. Pencarian

Pengguna dapat melakukan pencarian menggunakan:

- Single Term Query
- Multi Term Query
- Phrase Query

---

## Contoh Penggunaan

### Menu Utama

```text
1. Cari satu kata
2. Cari beberapa kata
3. Cari frasa
4. Tampilkan indeks
0. Keluar
```

### Query

```text
Masukkan kata kunci:
python
```

### Output

```text
Dokumen yang mengandung kata 'python':

1. dokumen1.txt
2. dokumen3.txt
3. dokumen5.txt
```

---

## Konsep yang Diimplementasikan

- Information Retrieval
- Text Preprocessing
- Tokenization
- Stopword Removal
- Inverted Index
- Document Search
- Query Processing

---

## Kelebihan Sistem

- Pencarian dokumen lebih cepat dibanding pencarian linear
- Struktur data efisien untuk koleksi dokumen besar
- Mudah dikembangkan menjadi search engine sederhana
- Cocok untuk pembelajaran Information Retrieval

---

## Pengembangan Selanjutnya

Beberapa pengembangan yang dapat dilakukan:

- TF-IDF Weighting
- Cosine Similarity
- Ranking Dokumen
- Stemming Bahasa Indonesia
- Web Interface
- Search Suggestion
- Boolean Retrieval Model
- Vector Space Model

---

## Author

**Eugenius Kriswinar Adi Cahya**

---

## License

Project ini dibuat untuk tujuan pembelajaran, penelitian, dan pengembangan sistem temu kembali informasi.
