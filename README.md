# About This Unit  
## ANOVA  
**A.** Apa itu ANOVA, Variasi, dan Derajat kebebasan?  
**B.** Menghitung Total Sum of Squares (SST)  
**C.** Memahami Sum of Squares Within dan Between (SSW dan SSB)  
**D.** Uji Hipotesis dengan F-Statistic  



## Deskripsi Singkat

**Analysis of Variance**, atau **ANOVA**, adalah metode statistik untuk membandingkan rata-rata dari **tiga atau lebih kelompok** untuk melihat apakah ada **perbedaan signifikan**.  
Unit ini akan memperkenalkan konsep dasar ANOVA secara bertahap, mulai dari apa itu variasi hingga cara menghitung dan menginterpretasikan hasilnya.  



# About This Unit  
## ANOVA  
**A.** Apa itu ANOVA dan Variasi  
**B.** Menghitung Total Sum of Squares (SST)  
**C.** Memahami Sum of Squares Within dan Between (SSW dan SSB)  
**D.** Uji Hipotesis dengan F-Statistic  



## Deskripsi Singkat

**Analysis of Variance**, atau **ANOVA**, adalah metode statistik untuk membandingkan rata-rata dari **tiga atau lebih kelompok** untuk melihat apakah ada **perbedaan signifikan**.  
Unit ini akan memperkenalkan konsep dasar ANOVA secara bertahap, mulai dari apa itu variasi hingga cara menghitung dan menginterpretasikan hasilnya.  



### A. Apa itu ANOVA, Variansi, dan Derajat Kebebasan?

Pahami konsep dasar ANOVA dan bagaimana variasi data digunakan untuk membandingkan kelompok.

- **Apa itu ANOVA?**  
  ANOVA adalah alat untuk memeriksa apakah rata-rata dari beberapa kelompok berbeda.  
  *Contoh:* Apakah tinggi tanaman berbeda jika diberi pupuk A, B, atau C?

- **Variansi**  
  Ukuran seberapa berbeda data dalam satu kelompok atau antar kelompok.  
  Variansi besar antar kelompok menunjukkan perbedaan yang mungkin signifikan.

- **Derajat Kebebasan (Degrees of Freedom / df)**  
  Dalam statistik, derajat kebebasan menggambarkan **jumlah nilai yang bebas untuk bervariasi** dalam suatu perhitungan.  
  Dalam konteks ANOVA:
  - $\text{df}_{\text{between}} = k - 1$  
    → untuk variasi antar kelompok (SSB), di mana *k* adalah jumlah kelompok.  
  - $\text{df}_{\text{within}} = N - k$  
    → untuk variasi dalam kelompok (SSW), di mana *N* adalah jumlah total observasi.

  Derajat kebebasan penting karena digunakan untuk menghitung nilai statistik F dan membandingkannya dengan tabel distribusi F.

- **Contoh Sederhana**  
  Bayangkan kamu punya 3 kelompok siswa dengan nilai:  
  - Kelompok 1: [80, 82, 78]  
  - Kelompok 2: [90, 92, 88]  
  - Kelompok 3: [70, 72, 68]  
  Total ada 9 data (N = 9), jumlah kelompok k = 3, maka:  
  - $\text{df}_{\text{between}} = 3 - 1 = 2$  
  - $\text{df}_{\text{within}} = 9 - 3 = 6$

  ANOVA akan membantu kita tahu apakah metode pengajaran di ketiga kelompok ini memberikan pengaruh yang berbeda secara signifikan terhadap nilai.



### B. Menghitung Total Sum of Squares (SST)

Pelajari cara menghitung total variasi dalam data dengan rumus sederhana.

- **SST:** mengukur total variasi dalam semua data.  
- **Rumus:**  
  $$
  SST = \sum (x_i - \bar{x})^2
  $$

  Di mana:
  - $x_i$ adalah setiap nilai data
  - $\bar{x}$ adalah rata-rata keseluruhan

- **Contoh Perhitungan:**

  Rata-rata semua nilai:

  $$
  \frac{80+82+78+90+92+88+70+72+68}{9} = 80
  $$

  Hitung:

  $$
  (80-80)^2 + (82-80)^2 + \dots + (68-80)^2
  $$
  Hasilnya adalah total variasi (**SST**).



### C. Memahami Sum of Squares Within dan Between (SSW dan SSB)

Kenali perbedaan variasi di dalam kelompok dan antar kelompok.

- **SSB (Between):**  
  Variasi antar rata-rata kelompok.  
  *Contoh:* Perbedaan rata-rata 80, 90, dan 70.

- **SSW (Within):**  
  Variasi di dalam setiap kelompok.  
  *Contoh:* Perbedaan 80, 82, 78 dalam Kelompok 1.

- **SST = SSB + SSW**  
  Total variasi dibagi menjadi dua bagian untuk analisis lebih lanjut.



### D. Uji Hipotesis dengan F-Statistic
Uji F-statistika digunakan karena mampu mengukur perbandingan variasi antar kelompok dengan variasi dalam kelompok secara sekaligus.

Mulai memahami cara menggunakan statistik F untuk menguji perbedaan signifikan.

- **F-statistic** dihitung dengan:  
  
  $$F = \frac{\text{SSB} / \text{df}_{\text{between}}}{\text{SSW} / \text{df}_{\text{within}}}$$
  

- **Derajat kebebasan (degrees of freedom / df):**  
  - $\text{df}_{\text{between}} = k - 1$,  
    di mana *k* adalah jumlah kelompok.  
  - $\text{df}_{\text{within}} = N - k$,  
    di mana *N* adalah jumlah total data.

- Jika nilai **F** cukup besar, maka ada kemungkinan besar bahwa **setidaknya satu kelompok berbeda secara signifikan** dari yang lain.  
  Uji ini digunakan untuk **menerima atau menolak hipotesis nol (H₀)**, yang menyatakan bahwa semua rata-rata kelompok sama.


