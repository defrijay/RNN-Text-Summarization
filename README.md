# Text Summarization using Simple RNN

Proyek ini mengimplementasikan model _Reccurent Neural Network_ (RNN) untuk menghasilkan ringkasan teks dari artikel berita. Model ini memanfaatkan teknik prapemrosesan data, augmentasi teks, serta pembelajaran mendalam untuk merangkum teks secara otomatis.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Dataset](#dataset)
- [Installation](#installation)
- [Project Creator](#project-creator)
<!-- - [Model Architecture](#model-architecture)
- [Training the Model](#training-the-model)
- [Generating Summaries](#generating-summaries)
- [Results and Visualization](#results-and-visualization) -->

## Overview

Ringkasan teks otomatis (text summarization) adalah teknik Natural Language Processing (NLP) untuk membuat versi pendek dari suatu teks sambil mempertahankan makna utamanya. Proyek ini menggunakan **Simple RNN** untuk menghasilkan ringkasan dari artikel berita.

## Features

- **Data Preprocessing**: Membersihkan dan mengonversi teks menjadi sequences, kemudian padding untuk membuat panjang yang konsisten.
- **Model Simple RNN**: Model neural network sederhana yang terdiri dari layer embedding dan RNN.
- **Training and Evaluation**: Melatih model dengan visualisasi Loss dan Accuracy.
- **Prediction Function**: Menghasilkan ringkasan otomatis dari input teks pengguna.

# Dataset

Dataset **Liputan6** adalah kumpulan data berskala besar yang berisi pasangan dokumen dan ringkasan artikel berita dalam Bahasa Indonesia. Dataset ini dirancang untuk mendukung model summarization baik dalam bentuk ekstraktif maupun abstraktif.

## Liputan6: Large-scale Indonesian Dataset for Text Summarization 

Dataset ini dikembangkan oleh Fajri Koto et al. (2020) dan berisi lebih dari **215,827 pasangan dokumen-ringkasan** yang diperoleh dari portal berita **Liputan6**.

### Detail Dataset

- **Jenis Ringkasan**: Ekstraktif dan Abstraktif
- **Bahasa**: Indonesia
- **Ukuran Dataset**: 16.5 MB (17,354,387 bytes)
- **Tugas yang Didukung**: Text summarization, khususnya untuk artikel berita dalam Bahasa Indonesia
- **Referensi**: [arxiv:2011.00679](https://arxiv.org/abs/2011.00679)

### Struktur Data
Dataset ini memiliki beberapa kolom penting, sebagai berikut:

- **id**: ID unik untuk setiap artikel.
- **url**: URL artikel asli di portal berita Liputan6.
- **clean_article**: Artikel yang telah dibersihkan dari teks asli.
- **clean_summary**: Ringkasan abstraktif dari artikel.

Contoh data:

```json
{
  "id": "26408",
  "url": "https://www.liputan6.com/news/read/26408/pbb-siap-membantu-penyelesaian-konflik-ambon",
  "clean_article": "Liputan6.com, Ambon: Partai Bulan Bintang wilayah Maluku bertekad membantu pemerintah menyelesaikan konflik di provinsi tersebut...",
  "clean_summary": "Konflik Ambon telah berlangsung selama tiga tahun. Partai Bulan Bintang wilayah Maluku siap membantu pemerintah menyelesaikan kasus di provinsi tersebut.",
  "extractive_summary": "Liputan6.com, Ambon: Partai Bulan Bintang wilayah Maluku bertekad membantu pemerintah menyelesaikan konflik di provinsi tersebut. Siapa saja yang melanggar hukum harus ditindak."
}
```


## Installation

Untuk menjalankan proyek ini, Anda memerlukan beberapa pustaka Python. Jalankan perintah di bawah ini untuk menginstalnya:

```bash
pip install numpy pandas tensorflow nltk rouge-score
```


## Project Creator
Proyek ini dikembangkan oleh **Defrizal Yahdiyan Risyad** dengan NIM **2206131** kelas **Ilmu Komputer C1 2022**, seorang mahasiswa Ilmu Komputer C1 2022 Universitas Pendidikan Indoensia yang sedang memenuhi tugas **Pengolahan Bahasa Alami**.
