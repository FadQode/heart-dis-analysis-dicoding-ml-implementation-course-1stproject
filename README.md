#Laporan Proyek Machine Learning - Fadhil Erdya Qashmal
 

### Latar Belakang Masalah

##### Latar Belakang Proyek
Salah satu penyakit yang sangat ditakutkan oleh banyak orang karena menjadi salah satu penyakit yang mematikan dan dalam banyak kasus datang secara tiba tiba adalah penyakit jantung. Kematian yang diakibatkan oleh serangan jantung sendiri bahkan mencapai lebih dari 400.000 kasus pada tahun 2014 di Amerika Serikat. Julukan silent killer yang diberikan pada serangan jantung menunjukkan bahwa kesadaran untuk menjaga kesehatan tubuh terutama jantung harus ditingkatkan.

Salah satu tantangan utama dalam pencegahan serangan jantung adalah sulitnya mengidentifikasi individu yang berisiko tinggi sebelum gejala serius muncul. Banyak kasus serangan jantung pertama kali terjadi tanpa adanya peringatan yang jelas, membuat upaya pencegahan menjadi lebih kompleks. Oleh karena itu, diperlukan metode yang lebih efektif dalam mendeteksi risiko serangan jantung sejak dini, terutama bagi individu yang tampaknya sehat tetapi memiliki faktor risiko tersembunyi.

Kematian jantung mendadak (sudden cardiac death/SCD) sering kali berhubungan dengan penyakit jantung koroner (coronary heart disease/CHD). Meskipun banyak penelitian telah dilakukan untuk memahami faktor risiko dan mekanisme yang mendasarinya, masih terdapat tantangan dalam memprediksi individu yang berisiko tinggi mengalami serangan jantung mendadak. Diperkirakan sekitar 80% kasus SCD disebabkan oleh CHD, dan sekitar 50% dari kematian akibat CHD terjadi secara mendadak tanpa adanya tanda-tanda peringatan sebelumnya.

#### Kenapa Proyek ini 
Mengingat sifatnya yang sulit diprediksi dan tingginya angka kematian yang disebabkan oleh serangan jantung, pengembangan model prediksi menjadi semakin penting. Model berbasis kecerdasan buatan dan machine learning dapat membantu dalam mengidentifikasi individu yang memiliki risiko tinggi berdasarkan faktor-faktor yang terdapat dalam dataset tersedia sehingga penanganan dan antisipasi dapat dilakukan lebih awal untuk mencegah terjadinya serangan jantung yang fatal.

#### Referensi 
- [Serangan Jantung: Penyakit Mematikan yang Mengintai](https://www.idionline.org/article/serangan-jantung-penyakit-mematikan-yang-mengintai)
- [Remaja Mengenali Serangan Jantung Koroner](https://jurnal.unw.ac.id/index.php/IJCE/article/view/758)
- [Sudden Cardiac Death Caused by Coronary Heart Disease](https://www.ahajournals.org/doi/full/10.1161/CIRCULATIONAHA.111.023846)

### Bussiness Understanding

#### Problem Statements
1. Faktor apa saja yang paling perlu diperhatikan dalam menjaga kesehatan diri terutama kesehatan jantung ?
2. Bagaimana performa model prediksi jika hanya menggunakan fitur non-medis dan pemeriksaan dasar dibandingkan dengan model yang terdapat fitur medis??
3. Faktor non-medis apa yang paling mempengaruhi kondisi medis dan berperan signifikan dalam meningkatkan risiko penyakit jantung?

#### Goals
- Mengidentifikasi faktor utama yang berkontribusi terhadap penyakit jantung berdasarkan korelasi tertinggi dengan kondisi tersebut.
- Membagi dataset ke dalam dua bagian:
  1. Dataset dengan fitur lengkap (medis dan non-medis).
  2. Dataset dengan fitur terbatas (hanya non-medis dan pemeriksaan dasar).
Membangun model prediksi berbasis Machine Learning untuk kedua dataset dan membandingkan akurasi serta performa keduanya.
- Mengidentifikasi faktor non-medis yang memiliki dampak signifikan terhadap kondisi medis yang berhubungan dengan penyakit jantung.
  
#### Solution Statements
1. Melakukan EDA secara mendetail dan menyeluruh terhadap fitur fitur yang ada beserta meninjau korelasi tiap fitur terhadap terjadinya penyakit jantung
2. Membangun dan membandingkan 4 model machine learning, yaitu untuk dataset lengkap tanpa optimasi hyperparameter, untuk dataset non medis tanpa optimasi hyperparameter, dataset lengkap dengan optimasi hyperparameter, dataset dengan fitur non-medis dengan hyper-parameter. Model dibangun menggunakan algoritma klasifikasi SVM
3. Melakukan pendekatan Machine Learning Feature Importance analysis dengan algoritma seperti Shap dan Random Forest untuk mendapatkan fitur non-medis yang paling mempengaruhi fitur-fitur medis
