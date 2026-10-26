**P E R T E M U A N 4  ·  B I G D ATA , A I , A N D C O D I N G** 

**Data Storytelling: Mengubah Angka Menjadi Grafik** 

Visualisasi Data Sederhana Menggunakan Python  |  Minggu 4 













## **Jejak Belajar Kita: Dari Tabel ke Prediksi** 















<!-- Start of picture text -->
M I N G G U 3<br><!-- End of picture text -->



<!-- Start of picture text -->
M I N G G U 4<br><!-- End of picture text -->

**Membaca data Menggambar grafik** Pandas Matplotlib 

**M I N G G U L A LU Membaca tabel_kopi** 

Kita sudah bisa memuat 1.560 transaksi dan mengintipnya dengan head(). 



<!-- Start of picture text -->
M I N G G U 5<br><!-- End of picture text -->



<!-- Start of picture text -->
M I N G G U 6<br><!-- End of picture text -->



<!-- Start of picture text -->
M I N G G U 7<br><!-- End of picture text -->

**M I N G G U 8 UTS** 

**Merakit dasbor Mengajari AI** Data Studio Teachable Machine **H A R I I N I Angka menjadi grafik** Menu terlaris dan tren harian digambar dengan Matplotlib. mm 



<!-- Start of picture text -->
Memprediksi<br><!-- End of picture text -->

**Merakit dasbor Mengajari AI Memprediksi** Data Studio Teachable Machine Orange 

Proyek kelompok 

**B E K A L M I N G G U D E PA N** 

###### **Grafik tanpa kode** 

Grafik yang sama dirakit menjadi dasbor interaktif di Data Studio. 

_Benang merah: semua latihan memakai data Toko Kopi yang sama, dari 1.560 transaksi hingga 600 pelanggan._ 

2 

Big Data, AI, and Coding  ·  Pertemuan 4 

## **Mengapa Kita Butuh Grafik?** 

**60.000×** 

lebih cepat otak manusia memproses informasi visual dibanding teks 



<!-- Start of picture text -->
©<br><!-- End of picture text -->



<!-- Start of picture text -->
©<br><!-- End of picture text -->

#### **Tabel angka melelahkan** 

Ribuan baris data angka sangat melelahkan untuk dibaca oleh atasan atau klien. 

**Grafik memberi gambaran instan** Performa bisnis bisa dipahami dalam hitungan detik. 

3 

Big Data, AI, and Coding  ·  Pertemuan 4 

## **Grafik Jujur vs Menyesatkan** 



<!-- Start of picture text -->
Jujur: sumbu Y mulai dari 0<br>120<br>104<br>101<br>98<br>100<br>80<br>60<br>40<br>20<br>0<br>Jan Feb Mar<br>Kenaikan terlihat wajar, sesuai data.<br><!-- End of picture text -->



<!-- Start of picture text -->
Menyesatkan: sumbu Y dipotong<br>105<br>104<br>104<br>103<br>102<br>101<br>101<br>100<br>99<br>98<br>98<br>97<br>96<br>Jan Feb Mar<br>Data sama, tapi tampak seperti lonjakan besar.<br><!-- End of picture text -->

###### **Grafik yang baik bukan hanya indah, tetapi juga jujur. Fokus pada kejelasan pesan dan kemudahan pembacaan.** 

4 

Big Data, AI, and Coding  ·  Pertemuan 4 

## **Berkenalan dengan Matplotlib** 

Matplotlib adalah pustaka (library) utama di Python untuk menggambar visualisasi — sangat ringan untuk membuat grafik dasar. 



<!-- Start of picture text -->
:<br><!-- End of picture text -->



<!-- Start of picture text -->
:<br><!-- End of picture text -->



**PA N DA S** 



<!-- Start of picture text -->
Kertas data<br><!-- End of picture text -->

**+** 

**M AT P LOT L I B** 



<!-- Start of picture text -->
Kuas lukis<br><!-- End of picture text -->

**=** 



<!-- Start of picture text -->
H A S I L<br><!-- End of picture text -->



<!-- Start of picture text -->
Grafik bercerita<br><!-- End of picture text -->

Menyimpan dan membaca tabel transaksi. 

Menggambar data menjadi bentuk visual. 

Siap disajikan ke atasan atau klien. 

5 

Big Data, AI, and Coding  ·  Pertemuan 4 

## **Langkah Memanggil Pustaka** 

###### **1 Wajib di awal** 

```
# Selalu ditulis di awal program
import pandas as pd
import matplotlib.pyplot as plt
```



Klik tombol Play (Run) di Google Colab dan pastikan tidak ada pesan eror sebelum lanjut ke langkah berikutnya. 

**2** 

Ditulis bersamaan dengan import pandas as pd di baris paling atas program. 

**as plt = nama panggilan** 

Singkatan agar fungsi gambar cukup dipanggil dengan plt.title(), plt.show(), dan seterusnya. 

6 

Big Data, AI, and Coding  ·  Pertemuan 4 

## **Dua Jenis Grafik Andalan Bisnis** 



##### **Grafik Batang (Bar Chart)** 

Membandingkan performa antar kategori produk. 



**Grafik Garis (Line Chart)** Melacak pergerakan tren naik-turun dari waktu ke waktu. 



<!-- Start of picture text -->
600<br>500<br>400<br>300<br>200<br>100<br>0<br>Gula Aren Americano Cappuccino Caffe Latte Matcha<br><!-- End of picture text -->



<!-- Start of picture text -->
350<br>300<br>250<br>200<br>150<br>100<br>50<br>0<br>Sen Sel Rab Kam Jum Sab Min<br><!-- End of picture text -->

7 

Big Data, AI, and Coding  ·  Pertemuan 4 

|**Anatomi Kode Grafi**|**k Batang**|||
|---|---|---|---|
|`tabel_kopi['Nama_Menu'`|`].`**`value_counts`**`().`|**`plot`**`(`|`kind='bar')`|
|**1**<br>|**2**<br><br>||**3**<br><br>O<br>O|
|**`tabel_kopi['Nama_Menu']`**<br>Memilih kolom nama menu dari<br>tabel transaksi.<br>|**`.value_counts()`**<br>Otomatis menghitung jumlah<br>pesanan tiap menu.<br>|>|**`.plot(kind='bar')`**<br>Memerintahkan komputer<br>menggambar bentuk batang.<br>|



8 

Big Data, AI, and Coding  ·  Pertemuan 4 

## **Perintah Memunculkan Gambar** 

```
tabel_kopi['Nama_Menu'].value_counts().plot(kind='bar')
plt.show()   # wajib di akhir
```



**`Dengan plt.show()`** Grafik dimunculkan secara sempurna di bawah kotak kode Anda. 



**`Tanpa plt.show()`** Grafik terkadang tidak akan muncul secara sempurna pada layar komputer Anda. 

9 

Big Data, AI, and Coding  ·  Pertemuan 4 

## **Memberi Identitas pada Grafik** 

```
plt.title("Judul Grafik")
```

Menulis judul utama di bagian atas grafik. 

```
plt.xlabel("Teks X")
```

Memberi keterangan pada sumbu mendatar. 

```
plt.ylabel("Teks Y")
```

Memberi keterangan pada sumbu tegak. 



<!-- Start of picture text -->
Judul Grafik<br>600<br>500<br>400<br>300<br>200<br>100<br>0<br>Gula Aren Americano Cappuccino Caffe Latte Matcha<br>Teks X<br>Teks Y<br><!-- End of picture text -->

10 

Big Data, AI, and Coding  ·  Pertemuan 4 

## **Eksperimen Parameter Warna** 

Tambahkan parameter color di dalam kurung plot untuk mengubah warna batang: 

```
.plot(kind='bar', color='orange')
```



<!-- Start of picture text -->
'red' 'orange'<br><!-- End of picture text -->



<!-- Start of picture text -->
'green'<br><!-- End of picture text -->



<!-- Start of picture text -->
'purple'<br><!-- End of picture text -->



Bebas berkreasi: tentukan warna yang menjadi identitas toko kopi kalian masing-masing. 



<!-- Start of picture text -->
'brown'<br><!-- End of picture text -->

11 

Big Data, AI, and Coding  ·  Pertemuan 4 

## **Mengubah Menjadi Grafik Garis** 

Cukup ubah satu setelan parameter — komputer otomatis merombak batang menjadi garis tren tunggal. 



<!-- Start of picture text -->
kind='bar' kind='line'<br>350 350<br>300 300<br>250 250<br>200 200<br>150 150<br>100 100<br>50 50<br>0 0<br>Sen Sel Rab Kam Jum Sab Min Sen Sel Rab Kam Jum Sab Min<br><!-- End of picture text -->

12 

Big Data, AI, and Coding  ·  Pertemuan 4 

## **Studi Kasus: Keputusan Stok Gudang** 



<!-- Start of picture text -->
112<br>=<br><!-- End of picture text -->



<!-- Start of picture text -->
Jumlah pesanan per menu (minggu ini)<br><!-- End of picture text -->



<!-- Start of picture text -->
Es Kopi Susu Gula Aren 479<br>Americano 172<br>Cappuccino 165<br>160<br>Caffe Latte<br>133<br>Matcha Latte<br>Es Teh Leci 112<br>=<br><!-- End of picture text -->











<!-- Start of picture text -->
6<br><!-- End of picture text -->

###### **Grafik** 

Terlihat lonjakan tajam pada menu Es Kopi Susu Gula Aren. 



<!-- Start of picture text -->
Keputusan<br><!-- End of picture text -->

Manajer Operasional langsung menambah pesanan susu ke pemasok. 



<!-- Start of picture text -->
Hasil<br><!-- End of picture text -->

Terhindar dari kehilangan potensi keuntungan akibat stok habis. 

_Data asli transaksi_toko_kopi.csv, 28 Sep sampai 4 Okt 2026_ 

13 

Big Data, AI, and Coding  ·  Pertemuan 4 

## **Misi Praktikum Hari Ini** 



<!-- Start of picture text -->
©<br><!-- End of picture text -->

**MI S I 1** 



<!-- Start of picture text -->
oO<br><!-- End of picture text -->

**M I S I 2** 



<!-- Start of picture text -->
©<br><!-- End of picture text -->

**M I S I 3** 

##### **Aktifkan pustaka** 

##### **Baca data** 

##### **Lukis grafik** 

Panggil Pandas dan Matplotlib secara bersamaan. 

Muat url_kopi yang sama dengan minggu lalu ke dalam tabel_kopi. 

Buat grafik batang menu terlaris dan grafik garis tren harian. 



###### **Data hari ini: tabel_kopi dari minggu lalu** 

- 1.560 baris, satu baris = satu pesanan. Karena itu value_counts() menghitung jumlah pesanan tiap menu atau tiap tanggal. 

14 

Big Data, AI, and Coding  ·  Pertemuan 4 

## **Tugas Mandiri Minggu Ini** 



**T U G A S M A N D I R I · M I N G G U 4** 

**1** 

**2** 

Buat grafik batang dari kolom 'Kategori'. 

Pakai warna berbeda dari contoh dosen, lengkapi judul dan label sumbu. 

### **Grafik kategori yang bercerita** 

**3** 

Tulis satu kalimat cerita: kategori mana yang mendominasi? 

**D I KU M P U L K A N** 

Screenshot hasil ke e-learning kampus sebelum pertemuan berikutnya. 



###### **B E K A L M I N G G U D E PA N** 

Kolom pemecah (Kategori) dan angka hitungannya minggu depan bernama Dimensi dan Metrik. 

15 

Big Data, AI, and Coding  ·  Pertemuan 4 

# **Kesimpulan Minggu Ke-4** 



<!-- Start of picture text -->
y<br><!-- End of picture text -->



<!-- Start of picture text -->
y<br><!-- End of picture text -->

Visualisasi dasar membuat analisis data Anda lebih dihargai di dunia kerja. Anda tidak perlu menjadi desainer grafis untuk membuat visualisasi data yang informatif. 



**Mari buka Google Colab kita!** 



<!-- Start of picture text -->
ia<br><!-- End of picture text -->

Minggu depan: No-Code Analytics dengan Google Data Studio 

