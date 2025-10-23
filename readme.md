
---

# 🏋️‍♀️ Prediksi Tipe Workout dari Data Gaya Hidup

### 📘 Deskripsi Proyek

Proyek ini bertujuan untuk **menganalisis dan memprediksi tipe workout** seseorang berdasarkan data gaya hidup menggunakan algoritma **Random Forest Classifier**.
Data yang digunakan berasal dari **Kaggle - Life Style Dataset (20.000 baris, 54 kolom)**.
Proyek ini disusun untuk memenuhi tugas mata kuliah **Data Mining**.

---

### 🧠 Tujuan

* Memprediksi jenis latihan seseorang (*Workout_Type*: cardio, hiit, strength, yoga) berdasarkan atribut gaya hidup.
* Menemukan faktor paling berpengaruh terhadap pilihan workout.
* Melatih kemampuan implementasi proses **data mining end-to-end**: dari data understanding hingga evaluasi model.

---

### 📊 Dataset

* **Sumber:** [Kaggle - Life Style Data](https://www.kaggle.com/datasets/jockeroika/life-style-data)
* **Ukuran:** 20.000 baris × 54 kolom
* **Fitur utama:**

  * Umur (`Age`), Berat (`Weight`), Tinggi (`Height`), Durasi latihan (`Session_Duration`), Kalori terbakar (`Calories_Burned`), Detak jantung (`Avg_BPM`, `Max_BPM`)
  * Target label: `Workout_Type`

---

### ⚙️ Metode & Tahapan

1. **Data Cleaning**

   * Menghapus nilai kosong pada kolom target.
   * Mengisi nilai kosong numerik dengan median.
   * Normalisasi dan encoding fitur kategorikal.

2. **Feature Engineering**

   * One-Hot Encoding untuk kategori.
   * Scaling numerik dengan `StandardScaler`.

3. **Modeling**

   * Menggunakan algoritma **RandomForestClassifier** (`n_estimators=200`, `random_state=42`).
   * Split data 80% train – 20% test.

4. **Evaluasi**

   * Metrik: Accuracy, Precision, Recall, F1-score.
   * Visualisasi: Confusion Matrix & Feature Importance.

---

### 📈 Hasil Evaluasi

| Metrik                       | Nilai                                                  |
| ---------------------------- | ------------------------------------------------------ |
| **Akurasi**                  | **86.08%**                                             |
| **Model terbaik pada kelas** | HIIT & Yoga                                            |
| **Fitur paling berpengaruh** | Calories_Burned, cal_balance, Session_Duration (hours) |

---

### ⚖️ Etika & Reproducibility

* **Privasi & Lisensi:** Dataset bersifat publik (CC0) dan tidak mengandung data pribadi sensitif.
* **Seed Reproducibility:** `random_state=42` digunakan di seluruh proses agar hasil dapat direplikasi.
* **Versi Library:**

  * Python 3.12.12
  * pandas 2.2+
  * scikit-learn 1.5+
  * matplotlib 3.9+
  * seaborn 0.13+
* **Struktur Direktori:**

  ```
  ├── dataset/
  │   └── Final_data.csv
  ├── Tutorial_DataMining_Workout.ipynb
  ├── Laporan_DataMining_Workout.docx
  └── README.md
  ```

---

### 💡 Cara Menjalankan

1. Buka [Google Colab](https://colab.research.google.com/).
2. Upload file:

   * `Tutorial_DataMining_Workout.ipynb`
   * `Final_data.csv`
3. Jalankan cell satu per satu dari atas ke bawah.
4. Hasil akurasi dan grafik evaluasi akan muncul di bagian akhir notebook.

---

### 👩‍💻 Tim & Kontribusi


1.Fadilah habibi STI202303712
2.Maulana Yusuf STI202303534
3.Rizal Lazuardi STI202303398
4.Zackari Candra Jordi STI202303588



---

### 📚 Lisensi

Dataset berlisensi **CC0 Public Domain** (Kaggle).
Kode proyek ini bebas digunakan untuk tujuan pendidikan dengan mencantumkan atribusi sumber.

---

Kamu mau aku bantu buatkan versi `.md` (README.md) siap download biar bisa langsung upload ke GitHub atau ke zip proyek kamu?
