**P E R T E M U A N 3  ·  B I G D ATA , A I , A N D C O D I N G** 

**Berkenalan dengan Big Data: Membaca Tabel Raksasa** 

Pengenalan Pustaka Pandas untuk Mahasiswa Non-Teknis  | Minggu 3 



```
1.000.000+ baris…
```

### **Jejak Belajar Kita: Dari Tabel ke Prediksi** 















<!-- Start of picture text -->
M I N G G U 3<br><!-- End of picture text -->



<!-- Start of picture text -->
M I N G G U 4 M I N G G U 5<br><!-- End of picture text -->



<!-- Start of picture text -->
M I N G G U 6<br><!-- End of picture text -->



<!-- Start of picture text -->
M I N G G U 7<br><!-- End of picture text -->



<!-- Start of picture text -->
M I N G G U 8<br>UTS<br><!-- End of picture text -->



<!-- Start of picture text -->
Membaca data Menggambar grafik<br>Pandas Matplotlib<br><!-- End of picture text -->



<!-- Start of picture text -->
Membaca data Menggambar grafik Merakit dasbor Mengajari AI<br>Pandas Matplotlib Data Studio Teachable Machine<br>M I N G G U L A LU H A R I I N I<br>Colab, variabel &  Membaca tabel raksasa<br>parameter<br>Minggu 1–2 kita menekan tombol  1.560 transaksi Toko Kopi dibaca<br>Play dan menyimpan nilai di variabel. dengan Pandas, lalu diintip dan<br>diukur.<br>a<br><!-- End of picture text -->



<!-- Start of picture text -->
Memprediksi<br><!-- End of picture text -->

**Merakit dasbor Mengajari AI Memprediksi** Data Studio Teachable Machine Orange 

Proyek kelompok 

**B E K A L M I N G G U D E PA N** 

**Tabel menjadi grafik** 



tabel_kopi yang sama akan kita ubah menjadi grafik batang dan garis. 

_Benang merah: semua latihan memakai data Toko Kopi yang sama, dari 1.560 transaksi hingga 600 pelanggan._ 

2 

Big Data, AI, and Coding  ·  Pertemuan 3 

### **Masalah Kita: Mengapa Excel Kewalahan?** 

**BATAS MUTLAK EXCEL** 

**1.048.576** 



**Not Responding & crash** 

File berukuran besar sering membuat Excel macet hingga tertutup sendiri. 

baris per lembar kerja. Lebih dari itu, data tidak bisa dimuat. 



**Industri butuh alat tangguh** 

Big Data di industri membutuhkan alat yang lebih ringan dan kuat. 

3 

Big Data, AI, and Coding  ·  Pertemuan 3 

### **Apa itu Big Data? Karakteristik 3V** 



<!-- Start of picture text -->
Oo<br><!-- End of picture text -->

**V** 

#### **Volume** 

Ukuran data yang sangat masif, dari Gigabyte hingga Terabyte. 



**V** 

**Velocity** Kecepatan data baru terkumpul secara real-time. 



<!-- Start of picture text -->
ot<br><!-- End of picture text -->

# **V** 

#### **Variety** 

Bentuk data beragam: angka, teks ulasan, hingga foto. 

4 

Big Data, AI, and Coding  ·  Pertemuan 3 

### **Solusi Kita: Pustaka Pandas** 





<!-- Start of picture text -->
Oo<br><!-- End of picture text -->

###### **Pustaka khusus tabel** 

Pandas adalah library Python khusus untuk mengolah tabel data. 

**ANALOGI** 

_Seperti menginstal aplikasi Excel super cepat di dalam Python kita._ 



<!-- Start of picture text -->
S<br><!-- End of picture text -->

**Ringan untuk laptop** 

Mampu membaca jutaan baris data tanpa membebani laptop. 

5 

Big Data, AI, and Coding  ·  Pertemuan 3 

### **Apa itu File CSV?** 

**I S I F I L E C SV ( T E KS P O LO S )** 

```
Nama_Menu,Kategori,Harga,Banyak
Americano,Kopi,18000,4
Americano,Kopi,18000,2
Es Teh Leci,Non-Kopi,18000,2
Matcha Latte,Non-Kopi,27000,1
```

###### **CSV** 

Comma Separated Values 

###### **D I BAC A S E BAG A I TA B E L** 

|**`Nama_Menu`**|**`Kategori`**|**`Harga`**|**`Banyak`**|
|---|---|---|---|
|`Americano`|`Kopi`|`18000`|`4`|
|`Americano`|`Kopi`|`18000`|`2`|
|`Es Teh Leci`|`Non-Kopi`|`18000`|`2`|
|`Matcha Latte`|`Non-Kopi`|`27000`|`1`|





**Teks polos** Setiap nilai dipisahkan tanda koma 

###### **Ringan** 

Jauh lebih kecil dibanding file .xlsx 

6 

Big Data, AI, and Coding  ·  Pertemuan 3 

**Langkah Pertama: Mengaktifkan Pandas 1** _`# Memanggil pustaka Pandas`_ kerja kita. **`import`** `pandas` **`as pd` 2** ff@ 

**1 import = memanggil** Memanggil pustaka Pandas ke lembar kerja kita. 

**2 as pd = nama panggilan** Singkatan agar kita tidak lelah mengetik nama panjangnya. 



<!-- Start of picture text -->
Oo<br><!-- End of picture text -->

Ketik di Code Cell pertama Google Colab, lalu klik tombol Play. Tidak ada pesan eror berarti Pandas siap dipakai. 

7 

Big Data, AI, and Coding  ·  Pertemuan 3 

**Membaca Data Langsung dari Internet** `tabel_kopi = pd.` **`read_csv`** `(url_kopi)` <mark>i</mark> O© © **Data di internet** **`pd.read_csv() tabel_kopi`** Link file disimpan di variabel Otomatis menarik data mentah 1.560 transaksi toko kopi siap url_kopi. Tidak perlu diunduh ke dari web secara instan. diolah sebagai tabel di Google laptop. Colab. 

8 

Big Data, AI, and Coding  ·  Pertemuan 3 

### **Trik Mengintip Data: Fungsi head()** 

```
tabel_kopi.head()
```



###### **5 baris teratas** 

Memunculkan sampel data saja, cukup untuk mengenali isinya. 



###### **Layar tetap rapi** 

Menghindari layar penuh akibat jutaan data muncul sekaligus. 

###### **H A S I L D I L AYA R** 

|**`Nama_Menu`**|**`Kategori`**|**`Harga`**|**`Banyak`**|
|---|---|---|---|
|`Americano`|`Kopi`|`18000`|`4`|
|`Americano`|`Kopi`|`18000`|`2`|
|`Es Kopi Susu Gula Aren`|`Kopi`|`22000`|`4`|
|`Es Kopi Susu Gula Aren`|`Kopi`|`22000`|`4`|
|`Es Kopi Susu Gula Aren`|`Kopi`|`22000`|`3`|



```
… 1.555 baris lainnya tidak ditampilkan (kolom
lain disembunyikan)
```

9 

Big Data, AI, and Coding  ·  Pertemuan 3 

### **Bermain Parameter di Fungsi head()** 

`tabel_kopi.head(` **`3`** `)` Menampilkan hanya 3 data teratas. 



<!-- Start of picture text -->
tabel_kopi.head( 15 )<br><!-- End of picture text -->



<!-- Start of picture text -->
Menampilkan 15 data teratas.<br><!-- End of picture text -->





Angka di dalam tanda kurung adalah parameter: tombol setelan yang bisa Anda ubah sesuka hati. 

10 

Big Data, AI, and Coding  ·  Pertemuan 3 

### **Melihat Ukuran Data dengan shape** 

```
tabel_kopi.shape
(1560, 9)   # output
```



**Tanpa tanda kurung** shape bukan fungsi, melainkan informasi dimensi data. Jadi tidak ditulis shape(). 

**1.560** 

**9** 

**baris data** Jumlah catatan transaksi 

**kolom** Jumlah jenis informasi tiap baris 

11 

Big Data, AI, and Coding  ·  Pertemuan 3 

### **Studi Kasus: Menemukan Tren Bisnis** 



###### **1** 

###### **Olah data transaksi** 

Muat data transaksi toko kopi dengan pd.read_csv(url_kopi). 

**TOKO KOPI** 

_1.560 transaksi dalam seminggu. Menu apa yang paling dicari pelanggan?_ 

**2** 

###### **Ambil satu kolom** 

tabel_kopi['Nama_Menu'] memilih kolom menu yang ingin dianalisis. 

**3** 

###### **Intip hasilnya** 

Intip hasilnya dengan head(). Minggu depan kolom ini kita hitung dan gambar. 

12 

Big Data, AI, and Coding  ·  Pertemuan 3 

### **Misi Praktikum Hari Ini** 



<!-- Start of picture text -->
©<br><!-- End of picture text -->

**MI S I 1** 

###### **Import Pandas** 

Aktifkan pustaka Pandas di Google Colab. 



<!-- Start of picture text -->
©<br><!-- End of picture text -->



<!-- Start of picture text -->
M I S I 2<br><!-- End of picture text -->

###### **Baca dataset** 

Muat data transaksi toko kopi lewat link url_kopi. 



<!-- Start of picture text -->
©<br><!-- End of picture text -->

**M I S I 3** 

**Intip & ukur** 

Intip isi data dan periksa total dimensi barisnya. 

**CO N T E K A N KO D E H A R I I N I** 

```
import pandas as pd                    # 1. aktifkan Pandas
tabel_kopi = pd.read_csv(url_kopi)   # 2. baca data
tabel_kopi.head()  /  tabel_kopi.shape # 3. intip & ukur
```

13 

Big Data, AI, and Coding  ·  Pertemuan 3 

### **Tugas Mandiri Minggu Ini** 



**T U G A S M A N D I R I · M I N G G U 3** 

**1** 

**2** 

Cari satu file CSV di Google Dataset Search atau Kaggle. 

Baca dengan pd.read_csv(), lalu tampilkan head(7) dan shape. 

##### **Jelajahi dataset publik pilihan Anda** 

**3** 

Tulis satu kalimat: data tentang apa, berapa baris dan kolomnya. 

**D I KU M P U L K A N** 

Screenshot hasil ke e-learning kampus sebelum pertemuan berikutnya. 



###### **B E K A L M I N G G U D E PA N** 

Simpan notebook Anda. Minggu depan tabel_kopi akan kita ubah menjadi grafik. 

14 

Big Data, AI, and Coding  ·  Pertemuan 3 

## **Kesimpulan Minggu Ke-3** 



<!-- Start of picture text -->
y<br><!-- End of picture text -->

Mengolah Big Data tidak serumit yang dibayangkan. 



<!-- Start of picture text -->
y<br><!-- End of picture text -->



Dengan Pandas, kendali jutaan baris informasi berada di ujung jari Anda. **Sampai jumpa di lembar Google Colab!** 



<!-- Start of picture text -->
ia<br><!-- End of picture text -->

Minggu depan: Data Storytelling — tabel_kopi kita ubah menjadi grafik 

