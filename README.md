# Classification_Potential_Customer_For_Travel_Insurance
- Analisis dan pemodelan yang dilakukan memiliki tujuan strategis untuk mengoptimalkan frekuensi pembelian dan secara bersamaan meningkatkan pendapatan dari penjualan polis asuransi perjalanan.
- Data yang digunakan dalam analisis tersedia dalam berkas "TravelInsurancePrediction.csv", 
- Proses Feature Extraction telah dilakukan untuk menghasilkan fitur-fitur baru yang signifikan, termasuk AnnualCategory, FamilyCategory, dan AgeCategory.
- Teknik Feature Scaling yang diterapkan adalah Standarization, yang memberikan dasar yang kokoh untuk analisis yang lebih mendalam.
- Ketidakseimbangan kelas (Class Imbalance) dalam data telah berhasil diatasi dengan sukses melalui penggunaan teknik SMOTE (Synthetic Minority Over-sampling Technique)
- Model yang dipilih untuk pemodelan adalah Gradient Boosting Classifier

## Team Member
- Imam Ahmad Qusyairi
- Hans Mulyadi
- Gede Wira Wasistha 
- Rifqi Adhityatama 
- Maria José Valbuena 
- Yandi Fajrahman 
- Destya Febiolla

## Latar Belakang
- Penjualan paket asuransi periode 2019 masih mencatatkan tingkat rendah, hanya sekitar 35.73%. Ini merupakan indikasi bahwa terdapat tantangan dalam meningkatkan tingkat pembelian produk asuransi tersebut.
- Sejalan dengan hasil tersebut, biaya yang telah dikeluarkan oleh perusahaan untuk kampanye pemasaran tampaknya belum memberikan hasil yang efisien. Dalam upaya untuk meningkatkan efisiensi, evaluasi dan perbaikan strategi pemasaran menjadi kunci untuk mencapai target penjualan yang diinginkan.

## Objective
- Proyek ini bertujuan untuk mengembangkan dan menerapkan model prediksi Machine Learning yang dapat dengan tepat memprediksi apakah pelanggan akan membeli asuransi perjalanan atau tidak.
- Selain itu, proyek ini juga bertujuan untuk mengidentifikasi tipe-tipe pelanggan yang cenderung tertarik untuk membeli asuransi perjalanan dan tipe-tipe pelanggan yang kurang tertarik. Dengan demikian, perusahaan dapat mengarahkan strategi pemasaran dan retensi secara lebih efektif, meningkatkan penjualan, dan memberikan layanan yang lebih tepat sasaran kepada pelanggan.


## Batasan Masalah
- Membangun model prediksi untuk menentukan apakah pelanggan akan membeli asuransi perjalanan.
- Prediksi apakah pelanggan akan membeli asuransi perjalanan dan identifikasi tipe-tipe pelanggan yang tertarik atau tidak.





## Data dan Asumsi
- Dalam dataframe fitur yang tesedia adalah Age, Employment Type, GraduateOrNot, AnnualIncome, FamilyMembers, ChronicDiseases, FrequentFlyer, EverTravelledAbroad. Sementara targetnya adalah TravelInsurance
- Fitur yang akan digunakan dalam modeling adalah Age, FrequentFlyer, Employment Type, EverTravelledAbroad, GraduateOrNot, TravelInsurance, AnnualIncome, AnnualCategory, ChronicDiseases, dan FamilyCategory

## Analisis Data
- EDA untuk setiap fitur dan visualisasinya
- Jelaskan proses memilih fitur dan performa

## Simpulan
Model yang kami pilih adalah GradientBoostingClassifier dikarenakan model tersebut memiliki score presisi dan akurasi yang paling baik diantara model lainnya.  Berdaarkan fitur importance dari menggunakan model GradientBoostingClassifier didapatkan 4 fitur importance, yaitu AnnualIncome, Age, FamilyCategory, EverTravelledAboard. namun fitur yang paling mendominasi adalah Fitur AnnualIncome memiliki pengaruh yang sangat tinggi dengan proporsi mencapai ~85%. Hasil Feature Importance menunjukkan bahwa faktor paling besar yang berkontribusi terhadap seorang pelanggan membeli paket asuransi perjalanan adalah pendapatan tahunan. Semakin tinggi pendapatan seseorang, cenderung akan membeli paket asuransi paket perjalanan dan begitu pula sebaliknya


## Saran
Action Items yang kami ajukan merespons temuan analisis feature importance ialah sebagai berikut :
- Menyusun marketing yang berfokus terhadap calon konsumen berpendapatan tinggi. Identifikasi solusi yang bisa ditawarkan terhadap calon konsumen tersebut agar tertarik membeli paket asuransi perjalanan
- Meningkatkan luas cakupan asuransi perjalanan untuk meningkatkan daya saing paket asuransi dibanding kompetitor
- Calon customer dengan pendapatan tinggi cenderung tidak sensitif terhadap harga, namun sensitif terhadap kualitas pelayanan. Perlu peningkatan pelayanan untuk meenjaga kepuasan konsumen





