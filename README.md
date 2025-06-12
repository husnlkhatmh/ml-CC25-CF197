# WisataPas : Temukan Tempat Seru dengan Teknologi Rekomendasi Cerdas.

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

Kaggle Dataset : https://www.kaggle.com/datasets/aprabowo/indonesia-tourism-destination 
Updated Dataset : https://drive.google.com/drive/folders/1-PQMwepQ9aug7EyAsWWJGzwDtrK6s8-Y 

Dataset ini berasal dari sumber publik di Kaggle, namun telah kami kembangkan dan perbarui dengan beberapa penyesuaian berikut:
- Jumlah tempat wisata ditingkatkan dari 437 menjadi 608, dengan data tambahan dikumpulkan secara manual.
- Gambar tempat wisata diperoleh melalui proses web scraping dari berbagai sumber online.
- Jumlah pengguna dalam data rating bertambah dari sekitar 300 menjadi 450 pengguna. Jumlah total rating meningkat dari 10.000 menjadi sekitar 16.000 penilaian, sebagian dihasilkan secara acak menggunakan Python untuk keperluan simulasi dan pengujian model rekomendasi.
  
**Data Rating**
Berisi informasi penilaian dari pengguna terhadap tempat wisata.
- User_Id: ID unik untuk setiap pengguna.
- Place_Id: ID unik untuk tempat wisata.
- Place_Ratings: Nilai penilaian (dalam bentuk angka) yang diberikan pengguna ke tempat.

**Data Tempat Wisata**
Berisi detail informasi tentang setiap tempat wisata.
- 	Place_Id: ID unik untuk tempat wisata.
- 	Place_Name: Nama dari tempat wisata.
- 	Description: Deskripsi tentang tempat wisata.
- 	Category: Kategori tempat wisata.
- 	City: 	Nama kota tempat wisata tersebut berada.
- 	Price: Harga tiket masuk ke tempat wisata tersebut.
- 	Rating: Rata-rata penilaian dari pengguna.
- 	Time_Minutes: Estimasi durasi kunjungan (menit). Banyak nilai yang kosong.
- 	Coordinate: 	Gabungan dari Lat dan Long dalam satu string, kemungkinan formatnya "lat,long".
- 	Unnamed: 11 & Unnamed: 12	: Kolom tidak jelas dan banyak nilai kosong, akan dihapus.
- 	Link_Img : URL/link ke gambar tempat wisata, bisa digunakan untuk visualisasi atau tampilan di aplikasi.

Hasil Content Based Filtering :
![image](https://github.com/user-attachments/assets/d9e2ea1b-4a3a-4174-9cce-786cf34dd7ba)

RMSE model Collaborative Filtering :

![image](https://github.com/user-attachments/assets/8ee063cd-9fb6-4ba2-91eb-a1b8f117a347)

![Gambar WhatsApp 2025-06-10 pukul 22 39 34_f85e5cdc](https://github.com/user-attachments/assets/3376ddbb-0e01-4f37-b308-31c115abd856)


