# Submission 1: SMS-Spam-Classification

Nama: Wahid Hasim Santoso

| **Deskripsi**               | **Detail**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| --------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Dataset**                 | [SMS Spam Classification](https://www.kaggle.com/datasets/thedevastator/sms-spam-collection-a-more-diverse-dataset)                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Masalah**                 | Spam menjadi tantangan yang umum di era digital, terutama pada layanan pesan singkat (SMS). Meskipun SMS dirancang untuk komunikasi singkat dan penyampaian pemberitahuan penting, banyak pesan tidak relevan atau tidak diinginkan yang dikirimkan melalui platform ini. Akibatnya, pengguna cenderung mengabaikan semua pesan, termasuk pesan yang sifatnya mendesak dan benar-benar membutuhkan perhatian.                                                                                                                     |
| **Solusi Machine Learning** | Proyek ini bertujuan untuk membantu memfilter antara SMS spam dan non-spam sehingga memudahkan pengguna dalam menerima pesan penting atau bukan spam.                                                                                                                                                                                                                                                                                                                                                                             |
| **Metode Pengolahan**       | Dataset diproses dengan mengonversi semua teks input menjadi huruf kecil (_lowercase_) dan mengubah tipe data pada variabel target menjadi tipe _integer_. Selanjutnya, data dibagi menjadi data pelatihan dan pengujian dengan perbandingan 80:20.                                                                                                                                                                                                                                                                               |
| **Arsitektur Model**        | Model dibangun menggunakan jaringan saraf tiruan (_Neural Network_) dengan beberapa lapisan, yaitu Input, TextVectorization, Embedding, GlobalAveragePooling1D, dan Dense. Fully connected layer memiliki dua dense layer dengan 120 dan 32 unit menggunakan fungsi aktivasi ReLU. Output layer menggunakan dense layer dengan satu unit dan fungsi aktivasi sigmoid. Binary crossentropy digunakan sebagai fungsi loss, dan optimizer yang digunakan adalah Adam.                                                                |
| **Metrik Evaluasi**         | Model dievaluasi menggunakan beberapa metrik, termasuk AUC, False Positives, True Positives, False Negatives, True Negatives, dan Binary Accuracy.                                                                                                                                                                                                                                                                                                                                                                                |
| **Performa Model**          | Model menunjukkan performa yang sangat baik. Pada data pelatihan, model mencapai akurasi 99.66% dengan AUC 99.98%, menunjukkan kemampuan tinggi dalam membedakan kelas positif dan negatif. Model berhasil memprediksi 44 kasus positif dengan benar (True Positives) dan 251 kasus negatif dengan benar (True Negatives), meskipun terdapat 0 prediksi positif yang salah (False Positives) dan 1 prediksi negatif yang salah (False Negatives). Pada data validasi, performa tetap tinggi dengan akurasi 98.16% dan AUC 97.54%. |
