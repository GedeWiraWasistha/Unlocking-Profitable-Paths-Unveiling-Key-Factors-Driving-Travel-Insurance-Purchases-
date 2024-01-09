# Unlocking Profitable Paths: Unveiling Key Factors Driving Travel Insurance Purchases  
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
![pelanggan yang tertarik membeli](https://github.com/GedeWiraWasistha/Travel_Insurance-Potential_Customer_Classification_using_Machine_learning/assets/149849772/e10fed35-5ea3-4b9f-a449-ddc6d2b5f68b)

Persentase pelanggan yang tidak tertarik membeli travel insurance lebih besar yaitu sebesar 64%.

![kategori umur](https://github.com/GedeWiraWasistha/Travel_Insurance-Potential_Customer_Classification_using_Machine_learning/assets/149849772/cd72c23d-74f0-41a9-9b9b-d397e6614436)

Pelanggan dengan umur 27-32tahun terlihat banyak yang tidak tertarik untuk membeli travel insurance. Sedangkan pelanggan umur <= 26 dan >=33 terlihat banyak yg tertarik membeli.


![kategori pekerjaan](https://github.com/GedeWiraWasistha/Travel_Insurance-Potential_Customer_Classification_using_Machine_learning/assets/149849772/ad8af8be-78fa-407d-8050-cd85f568cffe)

Pelanggan dengan tipe pekerjaan private sector/self employed lebih tertarik membeli travel insurance sebesar 80% dibanding government sector yang hanya tertarik 20% saja.


![kategori pendapatan](https://github.com/GedeWiraWasistha/Travel_Insurance-Potential_Customer_Classification_using_Machine_learning/assets/149849772/c91c6ee2-c0d4-4a7f-82a5-abda623acaed)

Terjadi kenaikan tajam pada pelanggan dengan pendapatan tahunan diatas 1.3M untuk tertarik untuk membeli asuransi perjalanan.

![kategori pendidikan](https://github.com/GedeWiraWasistha/Travel_Insurance-Potential_Customer_Classification_using_Machine_learning/assets/149849772/9bfaf6d9-e585-4d56-b340-54ad52b15ca4)

Pelanggan dengan lulusan perguruan tinggi ataupun bukan, tidak memiliki dampak pada ketertarikan pembelian travel insurance.

![kategori keluarga](https://github.com/GedeWiraWasistha/Travel_Insurance-Potential_Customer_Classification_using_Machine_learning/assets/149849772/596ccba8-a14b-4ef9-8c25-d99ed3f9414d)

Keluarga dengan jumlah anggota 6 orang keatas lebih terlihat tertarik untuk membeli travel insurance, sedangkan yang berjumlah 2 orang terlihat hanya sedikit yang tertarik dan keluarga dengan anggota 3-5 orang agak banyak tertarik.

![kategori jumlah perjalanan](https://github.com/GedeWiraWasistha/Travel_Insurance-Potential_Customer_Classification_using_Machine_learning/assets/149849772/b64c1825-841c-4e12-8aff-ca229c2d38d7)

Secara signifikan pelanggan yang melakukan perjalanan abroad lebih banyak tertarik untuk membeli travel insurance yaitu sebesar 42% dibanding yang tidak membeli. Sedangkan pelanggan yang tidak melakukan perjalanan abroad merasa tidak tertarik untuk membeli travel insurance.

![kategori sering berpergian](https://github.com/GedeWiraWasistha/Travel_Insurance-Potential_Customer_Classification_using_Machine_learning/assets/149849772/503ba59a-70bb-4d1e-bfd3-ab1c202557a4)

Pelanggan yang sering melakukan penerbangan lebih banyak tertarik untuk membeli travel insurance.

## Simpulan
![hasil test](https://github.com/GedeWiraWasistha/Travel_Insurance-Potential_Customer_Classification_using_Machine_learning/assets/149849772/7452afa0-d4ea-4e0e-9e34-fff1ff706da5)

Model yang kami pilih adalah GradientBoostingClassifier dikarenakan model tersebut memiliki score presisi dan akurasi yang paling baik diantara model lainnya.  Berdaarkan fitur importance dari menggunakan model GradientBoostingClassifier didapatkan 4 fitur importance, yaitu AnnualIncome, Age, FamilyCategory, EverTravelledAboard. namun fitur yang paling mendominasi adalah Fitur AnnualIncome memiliki pengaruh yang sangat tinggi dengan proporsi mencapai ~85%. Hasil Feature Importance menunjukkan bahwa faktor paling besar yang berkontribusi terhadap seorang pelanggan membeli paket asuransi perjalanan adalah pendapatan tahunan. Semakin tinggi pendapatan seseorang, cenderung akan membeli paket asuransi paket perjalanan dan begitu pula sebaliknya

## Saran
![feature penting](https://github.com/GedeWiraWasistha/Travel_Insurance-Potential_Customer_Classification_using_Machine_learning/assets/149849772/1b37070d-17e7-4075-938d-b695ff167b56)
Action Items yang kami ajukan merespons temuan analisis feature importance ialah sebagai berikut :
- Menyusun marketing yang berfokus terhadap calon konsumen berpendapatan tinggi. Identifikasi solusi yang bisa ditawarkan terhadap calon konsumen tersebut agar tertarik membeli paket asuransi perjalanan
- Meningkatkan luas cakupan asuransi perjalanan untuk meningkatkan daya saing paket asuransi dibanding kompetitor
- Calon customer dengan pendapatan tinggi cenderung tidak sensitif terhadap harga, namun sensitif terhadap kualitas pelayanan. Perlu peningkatan pelayanan untuk meenjaga kepuasan konsumen





