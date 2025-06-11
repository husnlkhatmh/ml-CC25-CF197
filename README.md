# WisataPas : 

## Coding Camp Powered by DBS Foundation Capstone Project
Capstone Team ID : **CC25-CF197**

## Deskripsi
Melakukan tahap preparasi dan pembersihan data seperti menghapus duplikasi, menangani data kosong, dan normalisasi teks. Proyek ini membangun sistem rekomendasi wisata dengan dua pendekatan, yaitu Content-Based Filtering yang menggunakan cosine similarity pada vektorisasi TF-IDF deskripsi tempat, serta Collaborative Filtering dengan model RecommenderNet berbasis TensorFlow Keras yang memanfaatkan embedding pengguna dan tempat wisata berdasarkan rating yang diberikan pengguna.

## Tools 
* **Pandas** – untuk manipulasi dan analisis data tabular
* **NumPy** – untuk operasi numerik dan array
* **Matplotlib** – untuk visualisasi data
* **Seaborn** – untuk visualisasi data statistik
* **IPython Display** – untuk menampilkan output interaktif
* **NLTK** – untuk pembersihan dan pengolahan teks
* **Scikit-learn**
  * `TfidfVectorizer` – untuk ekstraksi fitur dari teks
  * `cosine_similarity` – untuk menghitung kemiripan antar teks
  * `train_test_split` – untuk membagi data pelatihan dan pengujian
* **TensorFlow & Keras**
  * Untuk membangun model Collaborative Filtering 
  * Menggunakan `Embedding`, `Dropout`, dan `Layer`
* **Transformers (Hugging Face)**
  * `T5Tokenizer`, `T5ForConditionalGeneration` – untuk pemrosesan teks lanjutan
* **PyTorch** – sebagai backend alternatif untuk model NLP
* **Joblib** – untuk menyimpan dan memuat model
* **OS, Random, Zipfile** – untuk utilitas sistem file dan operasi acak

## Dataset

