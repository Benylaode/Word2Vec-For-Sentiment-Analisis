
# **Word2Vec for Sentiment Analysis**

Proyek ini bertujuan untuk menganalisis sentimen dari komentar pengguna menggunakan model Word2Vec untuk representasi kata. Model ini dilatih untuk mengubah kalimat menjadi representasi vektor, yang kemudian digunakan sebagai input untuk model klasifikasi sentimen.

---

## **Fitur Utama**
1. **Preprocessing Data**: 
   - Tokenisasi dan penghapusan kata-kata umum (stopwords) serta tanda baca dari dataset komentar.
   - Konversi kalimat menjadi vektor menggunakan Word2Vec.

2. **Model Word2Vec**:
   - Model Word2Vec dilatih menggunakan data komentar untuk menghasilkan representasi kata dalam bentuk vektor berdimensi tinggi.
   - Model menggunakan `gensim` untuk mempermudah pengelolaan embedding.

3. **Klasifikasi Sentimen**:
   - Model neural network dibangun dengan PyTorch untuk memprediksi sentimen berdasarkan representasi vektor dari kalimat.
   - Sentimen diklasifikasikan ke dalam beberapa label, seperti positif, negatif, dan netral (tergantung dataset).

4. **Evaluasi Model**:
   - Metrik evaluasi termasuk **accuracy**, **precision**, **recall**, dan **F1 score** diukur di setiap epoch.
   - Grafik metrik pelatihan dibuat menggunakan Matplotlib untuk memvisualisasikan performa model.

5. **Grafik Performa**:
   - Visualisasi hasil pelatihan dalam grafik garis untuk **loss**, **accuracy**, **precision**, **recall**, dan **F1 score**.

---

---

## **Langkah Penggunaan**

1. **Instalasi Dependensi**:
   Pastikan Anda memiliki Python 3.7+ dan menginstal dependensi berikut:
   ```bash
   pip install gensim torch matplotlib nltk
   ```

2. **Download Resource NLTK**:
   Proyek ini menggunakan tokenizer dari NLTK. Download resource dengan menjalankan:
   ```python
   import nltk
   nltk.download('punkt')
   ```

3. **Preprocessing dan Pelatihan**:
   Jalankan skrip pelatihan utama:
   ```bash
   python train.py
   ```

4. **Visualisasi**:
   Grafik metrik performa akan dibuat secara otomatis setelah pelatihan selesai.

---

## **Hasil Akhir**
- Model Word2Vec menghasilkan embedding kata berdimensi tinggi, yang membantu model neural network memahami hubungan antar kata.
- Performa model diukur menggunakan metrik evaluasi standar, seperti accuracy, precision, recall, dan F1 score, dengan hasil divisualisasikan secara grafis untuk analisis lebih lanjut.

---

## **Catatan Tambahan**
- Dataset yang digunakan harus dalam format komentar dengan label sentimen. Formatnya dapat berupa:
  ```
  [
      ("This product is amazing", 1),  # 1 untuk positif
      ("Worst experience ever", 0),   # 0 untuk negatif
      ...
  ]
  ```

- Pastikan dataset yang digunakan memiliki distribusi data yang seimbang untuk pelatihan optimal.
ahu saya! 😊
