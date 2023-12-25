### DATASET

Dataset yang saya gunakan diambil dari website Kaggle dengan judul "Pima Indian Diabetes Database". Dataset ini disediakan oleh Akshay Dattatray Khare dan dapat diakses melalui [link ini](https://kaggle.com/datasets/akshaydattatraykhare/diabetes-dataset/data). Dataset ini berasal dari studi kesehatan Pima Indian dan dirancang untuk memprediksi apakah pasien tersebut menderita diabetes atau tidak berdasarkan beberapa atribut kesehatan.

Dataset ini berisi informasi mengenai 768 pasien dengan 8 atribut sebagai berikut:

- Pregnancies: Jumlah kehamilan.
- Glucose: Konsentrasi glukosa plasma 2 jam setelah tes toleransi glukosa oral.
- BloodPressure: Tekanan darah diastolik (mm Hg).
- SkinThickness: Ketebalan lipatan kulit trisep (mm).
- Insulin: 2 jam serum insulin (mu U/ml).
- BMI: Indeks massa tubuh (weight in kg/(height in m)^2).
- DiabetesPedigreeFunction: Fungsi silsilah diabetes.
- Age: Umur (tahun).
- Outcome: Variabel target yang menunjukkan apakah pasien menderita diabetes (1) atau tidak (0).

### KODE PROGRAM

Kode program dapat diakses melalui file yang berada di folder ini, atau dapat diakses melalui Google Collab [berikut](https://colab.research.google.com/drive/1MhlQw6BayAyHRqPx20BQ99YjMjDBlH0k?usp=sharing). File dataset dapat diunduh melalui Google Drive [berikut](https://drive.google.com/file/d/1VAlYb-oBX6zAtPAhbYt-E9GzOu5HYATc/view?usp=sharing).

### PENJELASAN KODE PROGRAM

1. Import beberapa library yang diperlukan seperti numpy, pandas, StandardScaler, dan lain sebagainya
2. Muat dataset yang berisi informasi pasien diabetes, jangan lupa untuk mengunduh file dataset di google drive lalu drag ke Google Collab.
3. Cek informasi dataset untuk mengetahui lebih lanjut informasi yang disediakan
4. Pisahkan dataset tadi menjadi 2 bagian, yaitu : X yang berisi atribut, serta Y yang berisi label
5. Normalisasi data menggunakan StandardScaler
6. Bagi dataset menjadi 2 subset: satu untuk pelatihan model, dan satu untuk pengujian
7. Latih model SVM
8. Evaluasi Model dengan beberapa metrik pengujian seperti nilai akurasi, presisi, recall dan f1 score
9. Buat sistem prediksi dimana user dapat mengubah inputan data dan melihat apakah pasien dengan data tersebut memiliki riwayat diabetes atau tidak

### ANALISIS METRIK PENGUJIAN

Pada penelitian ini, saya menggunakan beberapa metrik pengujian dengan model SVM. Adapun hasil analisisnya, sebagai berikut:

1. Akurasi (_Accuracy_): 77.27%
   Hasil akurasi mencerminkan seberapa baik model SVM dapat mengklasifikasikan keseluruhan data dengan benar. Pada penelitian ini, model mencapai akurasi sekitar 77.27%.

2. Presisi (_Precision_): 75.68%
   Presisi digunakan untuk mengukur seberapa banyak prediksi positif yang benar dari semua prediksi positif yang dibuat oleh model SVM. Dalam penelitian ini, sekitar 75.68% dari semua pasien yang diprediksi sebagai diabetes memang benar-benar diabetes.

3. Recall (Sensitivitas): 51.85%
   Recall digunakan untuk mengukur seberapa banyak nilai positif sebenarnya yang berhasil diprediksi oleh model SVM. Dalam penelitian ini, sekitar 51.85% dari semua pasien diabetes berhasil diidentifikasi oleh model.

4. F1 Score: 61.54%
   F1 score merupakan rata-rata atau mean dari hasil presisi dan recall. Pada penelitian ini didapatkan hasil sekitar 61.54%.

### KESIMPULAN

Dari hasil penelitian yang dilakukan, dapat ditarik kesimpulan bahwa metode SVM ini memiliki akurasi yang cukup baik. Namun perlu diperhatikan bahwa hasil presisi dan recall tidak seimbang. Hasil presisi yang tinggi menunjukkan bahwa ketika model memprediksi seseorang memiliki diabetes, kemungkinan besar prediksi tersebut benar. Namun, hasil recall yang lebih rendah menunjukkan bahwa model mungkin melewatkan beberapa kasus diabetes yang sebenarnya, sehingga tidak seluruhnya seimbang.

### SARAN

Penelitian ini masih belum sempurna, dikarenakan terdapat beberapa hasil yang nilainya belum terbilang baik. Sehingga saya menyarankan agar penelitian ini dapat di improve kembali dengan hasil pengujian yang lebih baik dari sebelumnya. Harapan saya, hasil ini dapat memberikan sedikit pemahaman mengenai "Prediksi Diabetes Melitus Menggunakan Metode Support Vector Machine (SVM)".
