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

Kesimpulan: berdasarkan perhitungan dan diagram pie untuk proporsi banyaknya data orang di setiap region tidak terlalu berbeda, cenderung merata.  

#### c.   Mana yang lebih tinggi proporsi perokok atau non perokok?
Menghitung proporsi perokok dan non-perokok  menggunakan fungsi value_counts() pandas  
![gbr 10 proporsi perokok   nonperokok](https://github.com/indra2878/Analisa-Data-Tagihan-Kesehatan/assets/129472057/b279f7d8-ef9d-49b4-bbf2-6e8ae5711f6c)   

Membuat visualisasi (plot) bar chart proporsi data perokok dan non perokok menggunakan matplotlib   
![gbr 11 barchart proporsi perokok   nonperokok](https://github.com/indra2878/Analisa-Data-Tagihan-Kesehatan/assets/129472057/e226044f-934f-456f-b3c8-0d9f637467e0)

Kesimpulan: Berdasarkan hasil perhitungan dan bar chart proporsi perokok dan non-perokok diatas, dapat dinyatakan bahwa proporsi seseorang adalah Non-Perokok lebih besar dibandingkan dengan perokok.  
#### d.   Berapa peluang seseorang tersebut adalah perempuan diketahui dia adalah perokok?
Menghitung peluang seseorang adalah perempuan jika diketahui merokok menggunakan library pandas: (Lihat file jupiter notebok).
![gbr 12 peluang perempuan dan perokok 2](https://github.com/indra2878/Analisa-Data-Tagihan-Kesehatan/assets/129472057/01093eea-9754-4802-942a-d10a8fd009a4)  
Kesimpulan: peluang seseorang itu adalah perempuan jika diketahui perokok adalah sebesar 0,42.  
#### e.   Berapa peluang seseorang tersebut adalah laki-laki diketahui dia adalah perokok?
Menghitung peluang seseorang adalah laki-laki jika diketahui merokok (Lihat file jupiter notebok).
![gbr 13 peluang laki-laki dan perokok 2](https://github.com/indra2878/Analisa-Data-Tagihan-Kesehatan/assets/129472057/ca1fab4e-e90c-4367-89bc-496c73214e0c)  
Kesimpulan: peluang seseorang itu adalah laki-laki jika diketahui perokok adalah sebesar 0,58.  
### 2.3 Analisa Variabel Kontinu
#### a.   Mana yang lebih mungkin terjadi
- Seseorang dengan BMI diatas 25 mendapatkan tagihan kesehatan diatas 16.7k, atau
- Seseorang dengan BMI dibawah 25 mendapatkan tagihan kesehatan diatas 16.7k
Menghitung probabilitas kedua data diatas menggunakan library pandas:(Lihat file jupiter notebok).
![gbr 14 peluang tagihan 167k 2](https://github.com/indra2878/Analisa-Data-Tagihan-Kesehatan/assets/129472057/9dcd7291-63b0-4133-95a3-8e6a5a4f9dcf)
Membuat visualisasi (plot) bar chart proporsi data tagihan kesehatan diatas 16.7K seseorang dengan BMI diatas 25 vs seseorang dengan BMI dibawah 25 menggunakan matplotlib:
![gbr 15 bar plot peluang tagihan 167k bmi 25](https://github.com/indra2878/Analisa-Data-Tagihan-Kesehatan/assets/129472057/09747041-e9f7-4b11-9f07-0334655a98fe)
Kesimpulan: dari perhitungan dan bar plot diatas dapat disimpulkan bahwa seseorang dengan BMI diatas 25 berpeluang lebih tinggi untuk mendapatkan tagihan kesehatan diatas 16,7 K dibandingkan dengan sesorang dengan BMI dibawah 25.


#### b.   Mana yang lebih mungkin terjadi
- Seseorang perokok dengan BMI diatas 25 mendapatkan tagihan kesehatan diatas 16.7k, atau
- Seseorang non perokok dengan BMI diatas 25 mendapatkan tagihan kesehatan diatas 16.7k

Menghitung probabilitas kedua data diatas menggunakan library pandas:(Lihat file jupiter notebok).
 ![gbr 16 peluang tagihan 167k perokok bmi 25 - 2](https://github.com/indra2878/Analisa-Data-Tagihan-Kesehatan/assets/129472057/7ca3ab86-4d97-4398-889a-606bd2e00aa1)  
 
Membuat visualisasi (plot) bar chart proporsi data tagihan kesehatan diatas 16.7K seseorang perokok dengan BMI diatas 25 vs seseorang dengan Non-perokok dengan BMI diatas 25 menggunakan matplotlib:  
![gbr 17 bar plot peluang tagihan 167k perokok bmi 25](https://github.com/indra2878/Analisa-Data-Tagihan-Kesehatan/assets/129472057/58c11efa-cc2b-4baf-acca-0a683b4fcc23)  
Kesimpulan : dari perhitungan dan bar plot diatas dapat disimpulkan bahwa seseorang perokok dengan BMI diatas 25 berpeluang lebih tinggi untuk mendapatkan tagihan kesehatan diatas 16,7 K dibandingkan dengan sesorang non perokok dengan BMI diatas 25.  
### 2.4 Analisa Korelasi Variabel
#### a. bagaimana korelasi antara tagihan kesehatan dengan nilai BMI
**Analisa linieritas varibel tagihan kesehatan dan BMI:**  
Membuat plot Scatter plot tagihan kesehatan terhadap BMI menggunakan matplotlib.  
![gbr 18  scatter plot bmi vs tagihan kesehatan](https://github.com/indra2878/Analisa-Data-Tagihan-Kesehatan/assets/129472057/fffe5a15-2a83-4da1-99b3-9568088dc529)  
Dari scatter plot diatas terlihat data tagihan kesehatan dan BMI cenderung berhubungan linier ke arah kanan (positif). untuk memastikan adanya korelasi maka perlu dilakukan analisa kovarian dan korelasi.  

**Analisa Kovarian variabel tagihan kesehatan dan BMI:**  
Menghitung kovarian variabel tagihan kesehatan dan BMI menggunakan fungsi cov() numpy (lihat file jupiter notebook).  
Dari perhitungan didapat nilai kovarian sebesar : 1.46473044e+04 (positif).   
Dapat diambil kesimpulan sementara bahwa varibel tagihan kesehatan dan BMI cenderung saling berhubungan, dimana semakin besar BMI seseorang semakin besar pula tagihan kesehatan orang tersebut.  
Untuk memastikan seberapa kuat hubungan kedua variabel tersebut selanjutnya perlu di analisa korelasinya.  

**Analisa Korelasi variabel tagihan kesehatan dan BMI:**  
Menghitung korelasi dengan fungsi corr() dari library pandas (lihat file jupiter notebook).  
dari perhitungan didapat korelasi sebesar : 0.198341  
Kesimpulan: dari analisa korelasi dapat disimpulkan variabel tagihan kesehatan dan BMI bekorelasi lemah positif.  

#### b. bagaimana korelasi antara tagihan kesehatan dengan umur 
**Analisa linieritas varibel tagihan kesehatan dan umur seseorang:**  
Membuat plot Scatter plot tagihan kesehatan terhadap umur seseorang menggunakan matplotlib.  
![gbr 21  scatter plot umur vs tagihan kesehatan](https://github.com/indra2878/Analisa-Data-Tagihan-Kesehatan/assets/129472057/9ae11e2c-289e-4bb2-880b-03c42854c321)  
Dari scatter plot diatas terlihat data tagihan kesehatan dan umur seseorang cenderung berhubungan linier ke arah kanan (positif). Untuk memastikan adanya korelasi maka perlu dilakukan analisa kovarian dan korelasi.  

**Analisa Kovarian varibel tagihan kesehatan dan umur:**  
Menghitung kovarian varibel tagihan kesehatan dan umur menggunakan fungsi cov() numpy (lihat file jupiter notebook)
Dari perhitungan didapat nilai kovarian sebesar : 5.08748023e+04 (positif).   
Dapat diambil kesimpulan sementara bahwa varibel tagihan kesehatan dan umur cenderung saling berhubungan,  dimana semakin bertambah umur seseorang semakin besar pula tagihan kesehatan orang tersebut.  
Untuk memastikan seberapa kuat hubungan kedua variabel tersebut selanjutnya perlu di analisa korelasinya.  

**Analisa Korelasi variabel tagihan kesehatan dan BMI:**  
Menghitung korelasi dengan fungsi corr() dari library pandas (lihat file jupiter notebook).  
dari perhitungan didapat korelasi sebesar : 0.29900819333064765.  
Kesimpulan: Dari analisa korelasi dapat disimpulkan variabel tagihan kesehatan dan umur seseorang berkorelasi lemah positif.  

### 2.5 Pengujian Hipotesis
#### a. Tagihan kesehatan perokok lebih tinggi daripada tagihan kesehatan non perokok
**Menetapkan hipotesis :**
H0: tagihan_perokok = tagihan_non_perokok  
H1: tagihan_perokok > tagihan_non_perokok  

Menghitung rata-rata dan variansi tagihan kesehatan perokok  dan non perokok menggunakan pandas (lihat file jupiter notebook).  
![gbr 24  menghitung rata-rata   variansi tagihan kesehatan-2](https://github.com/indra2878/Analisa-Data-Tagihan-Kesehatan/assets/129472057/b2e72ac5-37cc-45d6-a1fc-7ab1da3d1e95)  

Dari perhitungan terlihat bahwa rata-rata tagihan kesehatan perokok lebih tinggi dari rata-rata tagihan kesehatan non perokok dimana variansinya berbeda, sehingga dapat dinyatakan bahwa tagihan kesehatan perokok cenderung lebih tinggi daripada tagihan kesehatan non perokok.  
Untuk memastikan hipotesis ini perlu dilakukan uji kesamaan 2 rata-rata populasi independent melalui uji t.  

**Menghitung Statistik Uji, Uji t rata-rata 2 populasi independent:**  
![gbr 25  menghitung uji t rata-rata   variansi tagihan kesehatan](https://github.com/indra2878/Analisa-Data-Tagihan-Kesehatan/assets/129472057/1379fa5a-5872-4178-9e95-a9cb770ba3b8)  

**Menentukan aturan keputusan:**  
![gbr 26  menentukan aturan keputusan](https://github.com/indra2878/Analisa-Data-Tagihan-Kesehatan/assets/129472057/83ebbd89-5dba-4be0-a016-104714d8bb9b)  

Kesimpulan: Hasil uji hipotesis menyatakan null hypothesis ditolak, maka dapat disimpulkan bahwa ada cukup bukti bahwa tagihan kesehatan perokok lebih tinggi dibandingkan dengan tagihan kesehatan non perokok.  

#### b. Proporsi perokok laki laki lebih besar dari perempuan
**Menetapkan hipotesis :**
H0: Proporsi perokok laki-laki = proporsi perokok perempuan  
H1: Proporsi perokok laki-laki > proporsi perokok perempuan  

Menghitung proporsi perokok laki-laki  dan proporsi perokok perempuan menggunakan library pandas:(lihat file jupiter notebook).  
![gbr 27  menghitung proporsi perokok laki-laki   perempuan-2](https://github.com/indra2878/Analisa-Data-Tagihan-Kesehatan/assets/129472057/9dcd397c-74df-4a4c-9718-f1fafcf4dff5)  

Dari perhitungan diatas terlihat bahwa proporsi perokok laki-laki cenderung lebih besar dari perempuan.  
Agar lebih meyakinkan maka perlu diuji kesamaan proporsi 2 populasi melalui uji z-score.  

**Menghitung Statistik Uji, Uji Z-score:**
Menghitung z-score dn p_-value menggunakan fungsi proportions_ztest() dari modul statsmodels: (lihat file jupiter notebook).
![gbr 28  menghitung uji z proporsi perokok laki-laki   perempuan 2](https://github.com/indra2878/Analisa-Data-Tagihan-Kesehatan/assets/129472057/487fc3a7-4eb0-471e-8cd9-64c4c63e716d)  

**Menentukan aturan keputusan:**  
![gbr 18  scatter plot bmi vs tagihan kesehatan](https://github.com/indra2878/Analisa-Data-Tagihan-Kesehatan/assets/129472057/48ad6893-d989-4939-86a8-194b45853a37)  

Kesimpulan: Hasil uji hipotesis menyatakan null hypothesis ditolak, maka dapat disimpulkan bahwa ada cukup bukti bahwa proporsi perokok laki-laki lebih tinggi dibandingkan dengan proporsi perokok perempuan.  

#### c. Variansi tagihan kesehatan perokok dan non perokok sama
**Menetapkan hipotesis:**  
H0: Variansi tagihan kesehatan perokok = Variansi tagihan kesehatan non perokok  
H1: Variansi tagihan kesehatan perokok > Variansi tagihan kesehatan non perokok  

**Menghitung variansi tagihan kesehatan perokok dan non perokok:**  
 Menghitung variansi tagihan perokok dan non perokok menggunakan fungsi variance dari modul statistics (lihat file jupiter notebook).  
 ![gbr 30  menghitung variansi2](https://github.com/indra2878/Analisa-Data-Tagihan-Kesehatan/assets/129472057/eae4262b-0770-4ade-9dd5-c5f775032421)  

Dari perhitungan diatas terlihat variansi tagihan perokok cenderung lebih besar dari non perokok, untuk memastikannya perlu dianalisa menggunakan uji-f right tail (ekor kanan)/ greater (lebih besar).  

**Menghitung Statistik Uji, Uji F right tail:**  
Menghitung nilai uji F dan p-value menggunakan pandas dan stats: (lihat file jupiter notebook).  
Dari perhitungan didapatkan nilai uji-f adalah 3.707884538770159 dan nilai p-value sebesar: 1.1102230246251565e-16.  

**Menentukan aturan keputusan:**  
![gbr 32  aturan keputusan](https://github.com/indra2878/Analisa-Data-Tagihan-Kesehatan/assets/129472057/b5e9855c-2397-4502-98bb-d8f7d779d674)  

Kesimpulan: hasil uji hipotesis menyatakan null hypothesis ditolak, maka dapat disimpulkan bahwa ada cukup bukti bahwa variansi tagihan perokok lebih tinggi dibandingkan dengan non perokok.  

## III. Conclusion  
Berdasarkan hasil analisa dataset tagihan kesehatan diatas ada beberapa temuan yang menarik yaitu:  
1.	Tagihan kesehatan perokok cenderung lebih tinggi daripada tagihan kesehatan non perokok sehingga disarankan kepada perusahaan asuransi kesehatan untuk menambah premi asuransi kesehatan bila diketahui seseorang itu perokok baik itu laki-laki maupun perempuan.
2.	Tagihan kesehatan mempunyai korelasi lemah positif dengan umur seseorang sehingga disarankan kepada perusahaan asuransi kesehatan untuk menambah premi asuransi kesehatan seiring bertambahnya umur seseorang.
3.	Tagihan kesehatan mempunyai korelasi lemah positif dengan BMI seseorang sehingga disarankan kepada perusahaan asuransi kesehatan untuk menambah premi asuransi kesehatan seiring bertambahnya BMI seseorang.

## IV. Further Research
Analisa Data Tagihan Kesehatan ini terbuka untuk diperbaiki dari segi pengolahan data, coding yang lebih baik dari segi kecepatan prosesnya, visualisasi plot yang lebih baik, dan sebagainya.  

## V Reference
https://www.stat.cmu.edu/capstoneresearch/315files_s23/team12.html

VI Data Processing report link
https://medium.com/@i.wahyudin2878/analisa-data-tagihan-asuransi-kesehatan-feccf57f59d


































  












