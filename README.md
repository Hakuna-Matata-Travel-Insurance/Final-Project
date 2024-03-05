# *FINAL PROJECT - BY HAKUNA MATATA*

![image](https://github.com/Hakuna-Matata-Travel-Insurance/Final-Project/assets/139318120/3836e821-2943-42d2-9201-e0c8610c11b0)

# *![image](https://github.com/Hakuna-Matata-Travel-Insurance/Final-Project/assets/139318120/923ed0dc-a958-4207-8e89-29d37948321a)*

* Ahmad Faqih Ulumuddin
* Ana Azzahra
* Athiya Fathinati Anindya
* Esa Risa Rouli Sekar Andonowari 
* Jerio Benediktus Rumagit 
* Mutiara Citra Sari 
* Nicken Shidqia Nurahman

# *![image](https://github.com/Hakuna-Matata-Travel-Insurance/Final-Project/assets/139318120/8a54baee-fff5-4f5d-9cc1-42f7e92a9c42)*
* **Tools**

   ![image](https://github.com/Hakuna-Matata-Travel-Insurance/Final-Project/assets/139318120/5056b0b8-13d9-47a1-930c-8dd03d5786a3)

* **Progaming Languange**

  ![image](https://github.com/Hakuna-Matata-Travel-Insurance/Final-Project/assets/139318120/ee8a92b7-dea9-4f1d-8bb7-7249ec807764)

* **Dataset**

  [TravelInsurancePrediction.csv](https://www.kaggle.com/datasets/tejashvi14/travel-insurance-prediction-data?resource=download)

# *![image](https://github.com/Hakuna-Matata-Travel-Insurance/Final-Project/assets/139318120/75cf0d20-c59c-4de3-b6be-b18110ded21b)*
Open in Google Collabs
  (link)

# *![image](https://github.com/Hakuna-Matata-Travel-Insurance/Final-Project/assets/139318120/e8cb52a3-4ae1-4074-a026-f2398848fe9f)*

![image](https://github.com/Hakuna-Matata-Travel-Insurance/Final-Project/assets/139318120/314f0560-6c94-4a51-9765-fbda11a2ef29)

Sebuah perusahaan travel insurance menemukan fakta bahwa hanya 35.73% pelanggan yang membeli paket asuransi perjalanan mereka. Bagaimana cara untuk membantu team bisnis agar dapat menyasar pelanggan dengan tepat sehingga meningkatkan penjualan?

Perusahaan belum mengenal lebih dalam pelanggannya dan strategi marketing yang selama ini dilakukan ditujukan untuk semua pelanggan. Hal ini mendorong tim kami memutuskan untuk membuat profil pelanggan untuk mengetahui karakteristik pelanggan perusahaan.

![image](https://github.com/Hakuna-Matata-Travel-Insurance/Final-Project/assets/139318120/5b10cd05-a9de-4cf5-8f2e-ed13dfb248d1)

Membuat segmentasi pelanggan agar dapat memberikan rekomendasi bisnis yang tepat kepada tim bisnis.

  ![image](https://github.com/Hakuna-Matata-Travel-Insurance/Final-Project/assets/139318120/70088f40-ac1d-49e7-a233-f52a2351e0e5)
  
1. Membangun Unsupervised Machine Learning Model untuk mengklasifikasi para pelanggan berdasarkan karakteristik pelanggan dan perjalanan.
2. Memberikan rekomendasi bisnis berdasarkan karakteristik pelanggan.

  ![image](https://github.com/Hakuna-Matata-Travel-Insurance/Final-Project/assets/139318120/71fa9e92-f010-4b5f-a8af-83a7084c2f0a)

Conversion Rate: Persentase pelanggan terdaftar yang benar-benar membeli paket asuransi terbaru. Tingkat konversi yang rendah menunjukkan bahwa pengguna tidak cukup termotivasi untuk membeli asuransi. Hal ini menunjukkan bahwa strategi marketing tidak efektif.

  # *![image](https://github.com/Hakuna-Matata-Travel-Insurance/Final-Project/assets/139318120/e342f36f-b666-43e6-8e4d-ad93c0c352b7)*

  (ringkasan stage 1)

  # *![image](https://github.com/Hakuna-Matata-Travel-Insurance/Final-Project/assets/139318120/b4a184b4-934f-4bc9-8937-0a745bd1d22b)*

* Missing Values, Duplicated Data, and Ouliers

  Tidak terdapat missing value, duplicate value, tetapi memiliki outliers dalam data.
* Feature Encoding

  Nilai dari kolom Employment Type, GraduateOrNot, FrequentFlyer, dan EverTravelledAbroad diubah menjadi 0 dan 1 menggunakan label encoding.
* Class Imbalance

  Jumlah pelanggan yang membeli paket asuransi jauh lebih sedikit dibandingkan pelanggan yang tidak membeli asuransi sehingga perlu dilakukan oversampling dengan metode SMOTE.
* Featute Exreaction

   setelah dicek korelasinya dengan target, hanya fitur ‘TravelExperience’ yang memiliki nilai korelasi lebih tinggi dari fitur-fitur yang sudah ada sebelumnya. Pada akhirnya, hanya fitur ‘TravelExperience’ yang digunakan untuk mengganti fitur lama ‘EverTravelledAbroad’ dan ‘FrequentFlyer
* Feature Selection
  # *![image](https://github.com/Hakuna-Matata-Travel-Insurance/Final-Project/assets/139318120/d027b7de-796e-40ae-a485-10f3425e8fa5)*

  (Ringkasan Stage 3)
# *![image](https://github.com/Hakuna-Matata-Travel-Insurance/Final-Project/assets/139318120/f68907a3-48bd-4bfa-90ae-70ee7679dfb3)*



### **Descriptive Statistics Insight**

A. Apakah ada kolom dengan tipe data kurang sesuai, atau nama kolom dan isinya 
kurang sesuai?

* Kolom 'GraduateOrNot', 'ChronicDiseases', 'FrequentFlyer', 'EverTravelledAbroad', dan 'TravelInsurance' adalah tipe data Boolean, jadi untuk keperluan EDA sebaiknya disamakan saja tipenya menjadi object atau integer agar mudah dikategorikan menjadi data numerikal dan kategorikal. Ini akan memudahkan pemahaman bahwa data numerikal adalah yang berisi angka (integer), dan data kategorikal berisi karakter/string (object).

* Kolom 'TravelInsurance' tidak diubah karena merupakan target dan nantinya dibutuhkan data numerikal saat modelling machine learning.


B. Apakah ada kolom yang memiliki nilai kosong? Jika ada, apa saja?

Tidak ada kolom yang memiliki nilai kosong dalam dataset ini.



C. Apakah ada kolom yang memiliki nilai summary agak aneh?
(min/mean/median/max/unique/top/freq) 

* Rentang umur pelanggan adalah 25-35, termasuk golongan usia produktif yang muda.

* Pelanggan didominasi oleh karyawan swasta dan wiraswasta, lulusan universitas, tidak mengidap penyakit kronis, tidak sering bepergian dengan pesawat dan belum pernah traveling keluar negeri.

* Pelanggan dengan frekuensi terbanyak berusia 28 tahun, dengan Pendapatan Tahunan 800.000, dan memiliki 4 Anggota Keluarga

* Pelanggan yang membeli asuransi perjalanan hanya 35,73%

### Analisis Univariat Insight

A. Fitur Numerikal
* Distribusi umur bervariasi, dengan mean, median, dan modus yang mirip (29.650226, 29, dan 28)
* Distribusi annual income bervariasi namun merata, dengan mean = 932,763 dan median = 900,000 
* Distribusi anggota keluarga cenderung positif (positively skewed), dengan rata-rata (median) 5 orang. Anggota keluarga yang paling banyak muncul adalah 4 orang. Tiap pelanggan memiliki setidaknya 2 orang anggota keluarga
* Lebih dari 60% pelanggan tidak membeli travel insurance
* Tidak ada outlier

B. Fitur Kategorikal
* Lebih dari 70% pelanggan adalah karyawan swasta dan wiraswasta
* Sekitar 85% pelanggan adalah lulusan perguruan tinggi
* 27.8% pelanggan mengidap penyakit kronis
* Hanya 21% pelanggan yang sering bepergian dengan pesawat
* Hanya 19% pelanggan yang pernah traveling keluar negeri

### Analisis Multivariat Insight

A. Korelasi antara Feature Numerik dan Target ('TravelInsurance'):

* Target memiliki korelasi positif paling tinggi dengan EverTravelledAbroad (0.43). Pelanggan yang pernah keluar negeri akan cenderung membeli travel insurance.
* Korelasi antara target dengan Annual Income cukup tinggi (0.4). Semakin tinggi pendapatan pelanggan, semakin besar kemungkinan pelanggan membeli travel insurance.
* Potensi pelanggan yang FrequentFlyer untuk untuk membeli Travel Insurance cukup potensial (0,23). Semakin sering berpergian pelanggan akan lebih memiliki kesadaran pentingnya memiliki sebuah Travel Insurance.

B. Korelasi antar Feature:

* Korelasi antara Annual Income dengan EverTravelledAbroad cukup tinggi (0.49), menunjukkan bahwa pelanggan dengan pendapatan yang tinggi pernah bepergian keluar negeri.
* Korelasi antara Annual Income dengan FrequentFlyer cukup tinggi (0.35), menunjukkan bahwa pelanggan dengan pendapatan yang tinggi sering bepergian dengan pesawat.

C. Korelasi antara Feature Kategorik dan Target ('TravelInsurance'):
Pelanggan yang bekerja di bidang swasta dan wiraswasta cenderung membeli travel insurance.

D. Korelasi antara Feature Kategorik dan Feature lainnya:
* Pelanggan yang pernah keluar negeri didominasi oleh karyawan swasta dan wiraswasta.
* Pelanggan yang bekerja di pemerintah kebanyakan memiliki pendapatan di bawah 400,000, semakin tinggi pendapatan semakin sedikit jumlah orangnya. Dapat dilihat juga rata-rata pendapatannya di bawah karyawan yang bekerja di sektor swasta. Sedangkan Pelanggan yang bekerja di sektor swasta memiliki rata-rata pendapatan lebih tinggi, dengan jumlah karyawan yang memiliki pendapatan di atas 450,000 lebih banyak.

## Business Insight

* Fokuskan strategi marketing pada pelanggan yang pernah bepergian ke luar negeri.
* Lakukan segmentasi pelanggan berdasarkan kategori pendapatan tahunan. Misalnya, tentukan rentang pendapatan rendah, menengah, dan tinggi. Sesuaikan penawaran dan premi travel insurance sesuai dengan segmentasi ini. Pelanggan dengan pendapatan lebih tinggi mungkin lebih bersedia untuk membayar premi yang lebih tinggi untuk manfaat tambahan. Berikan diskon atau insentif khusus kepada pelanggan dengan pendapatan tinggi.
* Tawarkan paket asuransi perjalanan premium dengan manfaat tambahan kepada pelanggan dengan pendapatan tinggi yang memiliki riwayat perjalanan internasional ('EverTravelledAbroad' = 'Yes') dan sering bepergian dengan pesawat ('FrequentFlyer' = 'Yes').
* Fokuskan strategi marketing kepada pelanggan yang bekerja di sektor swasta dan wiraswasta. Perusahaan dapat melakukan hal ini dengan memanfaatkan media-media yang diminati oleh segmen pasar tersebut, seperti media sosial atau komunitas online.
* Perusahaan dapat menawarkan paket asuransi perjalanan terbaru dengan harga yang lebih kompetitif untuk menarik minat pelanggan yang bekerja di sektor pemerintah.  
