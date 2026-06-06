# Analisis dan penyajian data rumah (Kelompok 3 - Kelas C)

Repositori ini dibuat sebagai dokumentasi post-test mata kuliah praktikum algoritma pemrograman. Data yang digunakan untuk analisis dan penyajian berada di folder dataset dengan nama **"Kelas C_Housing.csv"**. Kode ditulis dalam format jupyter notebook (**.ipynb**). Kode yang telah diunggah ke folder source code. Infografis analisis grafik hasil dari kode diunggah ke folder infografis dalam format (**.pdf**)


---

## Peran tiap anggota kelompok

| Nama Anggota | NIM | Kontribusi & Rincian Tugas (*Jobdesk*) |
| :--- | :---: | :--- |
| **Jundi Haidar Prayudi** | 21060125120018 | <ul><li>Menyusun kode program visualisasi Kategori A (Agregasi) </li><li>Membuat struktur dan mengatur manajemen repositori GitHub</li></ul> |
| **Aulia Rahman** | 21060125130029 | <ul><li>Menyusun kode program visualisasi Kategori B (Tren/Filter) </li><li>Merancang desain panel infografis untuk hasil analisis tersebut</li></ul> |
| **Ahmad Eka Refaldi** | 21060125120041 | <ul><li>Menyusun kode program visualisasi Kategori D</li><li>Merancang desain panel infografis untuk hasil analisis tersebut</li></ul> |
| **Rangga Julian Rosandi** | 21060125120043 | <ul><li>Menyusun kode program visualisasi Kategori C</li><li>Merancang desain panel infografis untuk hasil analisis tersebut</li></ul> |
| **Ahmad Naufal Andifa** | 21060125120057 | <ul><li>Menulis kode program penggabungan tata letak</li><li>Merakit struktur logika desain utama (layouting) infografis secara keseluruhan</li></ul> |

---

## _Techstack_

*   **Python 3.14**
*   **Jupyter Notebook (`.ipynb`)**
*   **Pandas & NumPy**
*   **Matplotlib & Seaborn**
*   **Canva**

---

##  Parameter Dataset
*   **Data kuantitatif:** `Area`, `Bedrooms`, `Bathrooms`, `Stories`,`Price`.
*   **Data kualitatif:** `Mainroad`, `Guestroom`, `Basement`, `Hotwaterheating`, `Airconditioning`, `Parking`, `Prefarea`, `Furnishingstatus`.

---

## Arsitektur dan Alur Kode
Aplikasi ini mengimplementasikan tahapan analisis data berbasis Object-Oriented Plotting dengan alur sebagai berikut:
1.	Pra-pemrosesan Data (Data Preprocessing): Memuat berkas .csv menggunakan struktur DataFrame.
2.	Kategori A (Agregasi): Menemukan dan memvisualisasikan harga rumah tertinggi dan terendah berdasarkan kategori wilayah pilihan (prefarea) menggunakan Grouped Bar Chart.
3.	Kategori B (Tren/Filter): Menyaring rumah berlantai > 2 tanpa basement, lalu menghitung kuantitasnya berdasarkan status perabot menggunakan Bar Chart.
4.	Kategori C (Korelasi): Menganalisis korelasi antar komponen numerik bangunan (price, area, bedrooms, bathrooms, parking) ke dalam matriks Heatmap.
5.	Kategori D (Distribusi): Mendeteksi sebaran dan pencilan (outliers) luas tanah khusus untuk rumah berstatus unfurnished menggunakan Boxplot.
6.	Visualisasi Gabungan: Mengkompilasi keempat grafik analisis ke dalam satu canvas grid (2x2) untuk kebutuhan dashboard kesimpulan eksekutif.

---

## Cara Menjalankan Program di Lokal
1.	Pastikan Anda telah mengunduh (atau melakukan clone) seluruh isi repositori ini.
2.	Tempatkan berkas kode program (.ipynb) dan berkas dataset (Kelas C_Housing.csv) di dalam satu direktori/folder yang sama.
3.	Buka terminal atau command prompt, lalu pasang library pendukung dengan perintah:
```text
pip install pandas numpy matplotlib seaborn ipykernel
```
5.	Buka berkas .ipynb menggunakan Jupyter Notebook, VS Code, atau Google Colab, lalu jalankan (Run All) seluruh sel kode yang tersedia.


---



```text                            .mmMMMMMMMMMMMMMmm.                              
                         .mMMMMMMMMMMMMMMMMMMMMMMMm.                          
                      .mMMMMMMMMMMMMMMMMMMMMMMMMMMMMMm.                       
                    .MMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMM.                     
                  .MMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMM.                   
                 MMMMMMMM'  `"MMMMM"""""""MMMM""`  'MMMMMMMM                  
                MMMMMMMMM                           MMMMMMMMM                 
               MMMMMMMMMM:                         :MMMMMMMMMM                
              .MMMMMMMMMM                           MMMMMMMMMM.               
              MMMMMMMMM"                             "MMMMMMMMM               
              MMMMMMMMM                               MMMMMMMMM               
              MMMMMMMMM                               MMMMMMMMM               
              MMMMMMMMMM                             MMMMMMMMMM               
              `MMMMMMMMMM                           MMMMMMMMMM`               
               MMMMMMMMMMMM.                     .MMMMMMMMMMMM                
                MMMMMM  MMMMMMMMMM         MMMMMMMMMMMMMMMMMM                 
                 MMMMMM  'MMMMMMM           MMMMMMMMMMMMMMMM                  
                  `MMMMMM  "MMMMM           MMMMMMMMMMMMMM`                   
                    `MMMMMm                 MMMMMMMMMMMM`                     
                      `"MMMMMMMMM           MMMMMMMMM"`                       
                         `"MMMMMM           MMMMMM"`                          
                             `""M           M""`
```
