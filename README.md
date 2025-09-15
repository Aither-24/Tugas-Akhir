# Tugas-Akhir
Evaluasi Model Prophet dengan Regresor Hari Libur dan Cuaca untuk Peramalan Multi-Horizon Harga Cabai Rawit Merah di Kabupaten Malang

https://j-ptiik.ub.ac.id/index.php/j-ptiik/article/view/15259

Proyek ini mengevaluasi performa model Prophet dalam memprediksi harga harian cabai rawit merah dengan mempertimbangkan faktor hari libur nasional dan data cuaca. Dataset mencakup harga harian cabai rawit merah di Kabupaten Malang (2022–2025), variabel cuaca dari BMKG Karangploso, serta kalender hari libur nasional.

Metodologi

Model diuji dalam 4 konfigurasi:
1. Baseline (tanpa regressor eksternal)
2. Regressor Hari Libur
3. Regressor Cuaca
4. Kombinasi Hari Libur + Cuaca



Horizon prediksi: 1 hari, 7 hari, 30 hari
Evaluasi: Time Series Cross-Validation, Bayesian Optimization
Metrik: RMSE, MAPE, Uji Friedman & Nemenyi


Hasil Utama
Baseline terbaik pada horizon 1 hari (RMSE 8.009) dan 30 hari (RMSE 18.123).
Regressor cuaca kompetitif pada horizon 7 hari (RMSE 11.001), meski tidak signifikan secara statistik.
Regressor hari libur cenderung menurunkan akurasi, baik tunggal maupun dikombinasikan.
Efektivitas regressor sangat bergantung pada relevansi temporal dan horizon prediksi.


Kesimpulan
Model Prophet terbukti fleksibel untuk peramalan harga pangan harian, namun integrasi faktor eksternal perlu dilakukan selektif dan berbasis bukti empiris agar tidak mengurangi stabilitas prediksi.
