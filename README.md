# Analisa-Data-Tagihan-Kesehatan
Pacmann Probability Project 
## I. Introduction
Project analisa probabilitas ini bertujuan untuk analisa data suatu dataset yang mencakup Analisa Statistik Deskriptif, Analisa Variabel Diskrit, Analisa Variabel Kontinu, Analisa Korelasi Variabel serta Pengujian Hipotesis.
Dataset yang digunakan adalah dataset Tagihan Asuransi Kesehatan, dimana memiliki 7 variabel sebagai berikut:
1)	Age (Age of primary beneficiary/ Penerima manfaat Asuransi utama)
2)	Sex (Insurance contractor gender/ Jenis kelamin (female, male))
3)	BMI (Body Mass Index, kg/m2, using ratio heigth to weight, ideally 18,5 to 24,9)
4)	Children (Number of children covered by insurance/ jumlah anak yang ditanggung asuransi)
5)	Smoker (Smoking/ merokok)
6)	The Region (Benefiary's residential area in the US/ Tempat tinggal penerima manfaat di US, (northeast, southeast, southwest, northwest))
7)	Charges (individual medical cost billed by health insurance/ Tagihan asuransi kesehatan individu)
## II. Research Question
Pertanyaan-pertanyaan seputar data tagihan kesehatan  yang akan dijawab melalui analisa statistik - probabilitas pada project ini meliputi:
### 2.1 Analisa Statistik Deskriptif
#### a.   Berapa rata rata umur pada data tersebut?
Menghitung rata-rata umur pada program python menggunakan fungsi mean() dari library pandas (lihat di file jupiter notebook).  
Dari perhitungan didapatkan bahwa rata-rata umur pada tabel tagihan asuransi kesehatan adalah : 39.21 tahun.
#### b. Berapa rata rata nilai BMI dari yang merokok?
Menghitung rata-rata nilai BMI dari yang merokok pada program python menggunakan fungsi mean() dari library pandas (lihat di file jupiter notebook).  
Dari perhitungan didapatkan bahwa rata-rata nilai BMI dari yang merokok adalah : 30.71 Kg/M2.  
#### c.   Apakah variansi dari tagihan kesehatan perokok dan non perokok sama?
Menghitung variansi tagihan kesehatan perokok dan non-perokok menggunakan fungsi variance dari modul statistics (lihat di file jupiter notebook).  
Dari perhitungan didapatkan bahwa variansi tagihan perokok = 133207311.20634925 sedangkan variansi tagihan non perokok = 35925420.49611173.  
Kesimpulan: variansi dari tagihan kesehatan perokok dan non-perokok berbeda, variansi tagihan perokok cenderung lebih tinggi dari non perokok.  
#### d.   Apakah rata rata umur perempuan dan laki-laki yang merokok sama?
Menghitung rata-rata umur perempuan dan laki-laki yang merokok menggunakan fungsi mean() pandas (lihat di file jupiter notebook).  
Dari perhitungan didapatkan bahwa rata-rata umur perempuan yang merokok = 38.608695652173914, 
sedangkan rata-rata umur laki-laki yang merokok = 38.44654088050314  
Kesimpulan: Rata-rata umur perempuan dan laki-laki yang merokok hampir sama yaitu mendekati 38,5 tahun.
#### e. Mana yang lebih tinggi, rata rata tagihan kesehatan perokok atau non merokok?
Menghitung rata-rata tagihan kesehatan perokok dan non-perokok menggunakan fungsi mean() pandas (lihat di file jupiter notebook).  
Dari perhitungan didapatkan bahwa rata-rata tagihan kesehatan perokok =  32050.23183153284 
sedangkan rata-rata tagihan kesehatan non perokok = 8434.268297856204.
Dapat disimpulkan bahwa rata-rata tagihan kesehatan perokok lebih tinggi dari non-perokok.  
### 2.2 Analisa Variabel Diskrit (peluang)
#### a.   Gender mana yang memiliki tagihan paling tinggi?
Menghitung rata-rata tagihan per gender menggunakan fungsi mean() library pandas (lihat di file jupiter notebook).
Dari perhitungan didapatkan rata-rata tagihan laki-laki = 13956.751177721893 dan rata-rata tagihan perempuan= 12569.578843835347.
Membuat visualisasi (plot) rata-rata tagihan laki-laki Vs perempuan menggunakan matplotlib.  
![gbr 6 rata-rata tagihan per gender2](https://github.com/indra2878/Analisa-Data-Tagihan-Kesehatan/assets/129472057/a07b5160-47a8-41de-aaa6-2757e52c9167)  

Dari hasil perhitungan dan visualisasi bar chart rata-rata tagihan kesehatan per gender, ternyata tagihan kesehatan laki-laki cenderung lebih tinggi dibanding tagihan kesehatan perempuan.  
Kesimpulan: Karena variabel acak bernilai riil, maka ekspektasi dan rata-rata bernilai sama sehingga diharapkan peluang tagihan kesehatan laki-laki cenderung lebih tinggi dibanding peluang tagihan kesehatan perempuan.  
#### b.   Apakah setiap region memiliki proporsi data banyak orang yang sama?
Menghitung proporsi data pada setiap region menggunakan fungsi value_counts() pandas (lihat di file jupiter notebook).
![gbr 8 proporsi data tagihan by region-1](https://github.com/indra2878/Analisa-Data-Tagihan-Kesehatan/assets/129472057/b3f2155f-c1d6-439a-8962-b632c88e4bd5)  

Membuat visualisasi (plot) pie chart proporsi data pada setiap region menggunakan matplotlib.  

![gbr 9 proporsi data tagihan by region-2](https://github.com/indra2878/Analisa-Data-Tagihan-Kesehatan/assets/129472057/e449529d-4706-4537-b160-1e78fb63daed)




