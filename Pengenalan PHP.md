# Apa itu web dinamis dan PHP
Web dinamis adalah jenis situs web yang menggunakan konten yang dapat berubah secara dinamis berdasarkan interaksi pengguna, data yang disimpan dalam database, atau logika bisnis tertentu. Berbeda dengan situs web statis yang memiliki konten tetap, situs web dinamis memungkinkan pengguna untuk berinteraksi dengan konten yang berubah sesuai dengan kebutuhan atau preferensi mereka.

PHP adalah bahasa pemrograman server-side yang sering digunakan untuk mengembangkan aplikasi web dinamis. Singkatan PHP adalah "Hypertext Preprocessor". PHP bekerja di sisi server, yang berarti kode PHP dijalankan di server web sebelum hasilnya dikirim ke browser pengguna. PHP dapat digunakan untuk melakukan berbagai tugas di situs web, termasuk mengambil dan menyimpan data dari database, menghasilkan halaman web secara dinamis, menangani formulir, dan banyak lagi. Ini adalah salah satu bahasa pemrograman paling populer yang digunakan untuk pengembangan web, terutama untuk situs web dinamis.

#  Echo & commentar
Echo merujuk pada tindakan mereproduksi atau membagikan kembali konten yang sudah ada kepada pengikut atau audiens Anda. Misalnya, jika seseorang memposting tweet atau kiriman di platform sosial lainnya, dan Anda memutuskan untuk membagikan kembali (retweet, share, dll.) konten tersebut kepada pengikut Anda, itu disebut sebagai "echo". Praktik ini memungkinkan untuk menyebarkan informasi lebih luas atau memberi penghargaan pada konten yang dianggap relevan atau menarik.

Komentar, di sisi lain, adalah respons atau tanggapan yang diberikan oleh pengguna terhadap konten yang diposting oleh pengguna lain. Ini bisa berupa pertanyaan, pendapat, dukungan, kritik, atau reaksi lainnya terhadap apa yang telah dibagikan. Komentar memungkinkan untuk berinteraksi dengan konten dan pengguna lainnya, membuka diskusi, atau memberikan umpan balik.



# Penggunaan Apache Web Server
## Cara menggunakannya 
1. buka aplikasi xampp

![](aset/php33.png)

2. klik Explorer

![](aset/php32.png)

3. buka folder htdocs

![](aset/php34.png)

4. buat folder baru bebas apa namanya

![](aset/php35.png)

5. lalu buat file baru bebas apa namanya

![](aset/php36.png)

6. isi file nya klo sudah langsung save

![](aset/php37.png)

7. buka kembali aplikasi xamppnya

![](aset/php33.png)

9. klik start pada bagian apache

![](aset/php40.png)

10. buka web browser

![](aset/php38.png)

11. pada bagian url ketik 'localhost/nama_folder_yang_dibuat_tadi/nama_file_yang_tadi_dibuat' dan klik enter

![](aset/php39.png)

12. maka hasil dari file nya akan muncul

![](aset/php41.png)


# Program pertama
## Kode Program
```php
<?php
// Komentar satu baris
/* Komentar
banyak
baris
*/
//Variebel
$meja = 30;
$tk_kelas = "XI";
$ketua_kelas = "July";
$wali_kelas = "Saleh";
$ketua_gank = "Rahmat"; //Pengubahan nilai
//Konstanta
const KEPSEK = "Herwelis";
define('Kelas', 'RPL 1');
/*Kutip satu hanya membaca STRING, variabel  dan string
 dipisahkan dengan tanda titik*/
echo 'Jumlah meja di kelas: ' .  $meja  . ' buah';
echo "<br>";
//Kutip dua bisa membaca nilai dari sebuah variabel
    echo "sholat dulu, nabilang pak $wali_kelas dan $ketua_kelas";
echo "<br>";
//Kutip satu dibaca string disini
echo "kalo tidak, diracca' sama ketua gank $ketua_gank";
echo "<br>";
//Pemnggilan konstanta
echo 'Kepseknya ' .  KEPSEK;
echo "<br>";
echo 'Kelasnya ' . $tk_kelas . ' '. Kelas;
?>
```


## Hasil
![](aset/php1.png)


# Echo
## Kutip satu

### Kode Program
```php
<?php
$meja = 30;
echo 'Jumlah meja di kelas: ' .  $meja  . ' buah';
?>
```
### Hasil
![](aset/php5.png)

### Penjelasan


## kutip dua
### Kode Program
```php
<?php
$ketua_kelas = "July";
$wali_kelas = "Saleh";
echo "sholat dulu, nabilang pak $wali_kelas dan $ketua_kelas";
?>
```

### Hasil
![](aset/php6.png)


# komentar
## single line
### Kode Program
```php
//ini digunakan untuk ketika mau membuat satu baris komentar
```

### Penjelasan
Digunakan untuk menambahkan komentar pada satu baris saja. Komentar ini dimulai dengan tanda double slash (`//`) dan berlaku hingga akhir baris.


## multiple line
### Kode Program
```php
/*ini digunakan
untuk ketika 
mau membuat 
lebih dari
satu baris komentar*/
```

### Penjelasan
Digunakan untuk menambahkan komentar yang lebih dari satu baris. Komentar ini dimulai dengan `/*` dan diakhiri dengan `*/`, dan dapat mencakup beberapa baris kode.


# Variabel, Konstanta, operator
### Kode Program

```php
<?php
$nama = "Dimas"; $umur = 5;
echo "perkenalkan nama saya $nama dan umur saya $umur" 
?>
```

### Hasil
![](aset/php3.png)

### Penjelasan
Variabel adalah tempat untuk menyimpan data yang dapat berubah nilainya selama eksekusi program. Anda bisa mendeklarasikan variabel dengan menggunakan tanda dollar ($) diikuti dengan nama variabelnya. 


### Kode Program
```php
<?php
const JARAK = "8 KM";
echo "Edo: Emang seberapa jauh sih rumahmu ke sekolah? <br>";
echo "Rina: Hmm, mungkin sekitar " . JARAK . ".";
?>
```

### Hasil
![](aset/php4.png)

### Penjelasan
Konstanta adalah seperti variabel, tetapi nilainya tidak dapat diubah selama eksekusi program. Anda mendeklarasikan konstanta menggunakan fungsi define()


### Kode Program
```php
<?php
// operator aritmatika
$a = 5;
$b = 3;
$jumlah = $a + $b;
echo "a + b = " . $jumlah . "<br>";
// operator perbandingan
$is_lebih_besar = ($a > $b);
echo "a > b = " . ($is_lebih_besar ? 'true' : 'false') . "<br>";
// operator logika
$is_true = ($a == 5 && $b == 3);
echo "a && b = " . ($is_true ? 'true' : 'false') . "<br>";
?>
```

### Hasil
![](aset/php2.png)

### Penjelasan
Operator adalah simbol yang digunakan untuk melakukan operasi pada variabel dan nilai. Ada berbagai macam operator dalam PHP, seperti operator aritmatika (+, -, *, /), operator perbandingan (==, !=, <, >), dan operator logika (&&, ||, !).


# Conditional Statement
## IF
### Penjelasan
Kondisional statement `IF` digunakan untuk melakukan pemeriksaan kondisi tertentu. Jika kondisi tersebut benar (true), maka blok kode di dalam IF akan dieksekusi. Jika kondisi salah (false), maka blok kode tersebut tidak dieksekusi.

### Struktrur Program
```php
if (kondisi) {
    // blok kode yang akan dieksekusi jika kondisi benar
}
```

### Kode Program
```php
<?php
$nilai = 80;
if ($nilai >= 70) {
    echo "Nilai Anda lulus.";
}
?>
```

### Hasil
![](aset/php7.png)
### Analisis
- Baris 1: Sebuah variabel `$nilai` diinisialisasi dengan nilai 80.
- Baris 2: Kondisi dievaluasi, yaitu apakah nilai `$nilai` lebih besar atau sama dengan 70.
- Baris 3: Karena kondisi benar (true), maka blok kode di dalam IF dieksekusi.
- Baris 4: Mencetak teks "Nilai Anda lulus." karena nilai `$nilai` memenuhi kondisi.

### Kesimpulan Program
Program akan mencetak "Nilai Anda lulus." karena nilai `$nilai` adalah 80, yang lebih besar dari atau sama dengan 70.

## Else IF

### Penjelasan

Kondisional statement `Else IF` digunakan untuk menambahkan kondisi tambahan setelah kondisi IF. Jika kondisi IF tidak terpenuhi (false), maka kondisi Else IF akan dicek. Jika kondisi Else IF benar (true), maka blok kode di dalam Else IF akan dieksekusi.

### Struktur program

```php
if (kondisi1) {     
// blok kode yang akan dieksekusi jika kondisi1 benar 
} else if (kondisi2) {     
// blok kode yang akan dieksekusi jika kondisi2 benar 
}
```

### Kode Program
```php
<?php
$nilai = 55; 
if ($nilai >= 70) {  
echo "Nilai Anda lulus."; 
} else if ($nilai >= 60) {
echo "Anda dapat remedial."; 
} else { 
echo "Anda tidak lulus.";
}
?>
```

### Hasil
![](aset/php8.png)

### Analisis

- Baris 1: Sebuah variabel `$nilai` diinisialisasi dengan nilai 55.
- Baris 2: Kondisi pertama dievaluasi, yaitu apakah nilai `$nilai` lebih besar atau sama dengan 70. Kondisi ini tidak terpenuhi (false).
- Baris 3: Kondisi kedua dievaluasi, yaitu apakah nilai `$nilai` lebih besar atau sama dengan 60. Kondisi ini juga tidak terpenuhi (false).
- Baris 4: Karena kedua kondisi sebelumnya tidak terpenuhi, maka blok kode di dalam ELSE dieksekusi.
- Baris 5: Mencetak teks "Anda tidak lulus." karena nilai `$nilai` kurang dari 60.

### Kesimpulan Program

Program akan mencetak "Anda tidak lulus." karena nilai `$nilai` adalah 55, yang kurang dari 60.


## Else

### Penjelasan

Kondisional statement `Else` digunakan untuk mengeksekusi blok kode tertentu jika kondisi IF sebelumnya tidak terpenuhi (false).

### Struktur program
```php
if (kondisi){     
// blok kode yang akan dieksekusi jika kondisi benar 
} else {     
// blok kode yang akan dieksekusi jika kondisi salah 
}
```

### Kode Program
```php
<?php
$nilai = 55; 
if ($nilai >= 60) 
{
echo "Nilai Anda lulus."; 
} else { 
echo "Anda tidak lulus.";
}
?>
```

### Hasil
![](aset/php8.png)

### Analisis
- Baris 1: Sebuah variabel `$nilai` diinisialisasi dengan nilai 55.
- Baris 2: Kondisi dievaluasi, yaitu apakah nilai `$nilai` lebih besar atau sama dengan 60. Kondisi ini tidak terpenuhi (false).
- Baris 3: Karena kondisi sebelumnya tidak terpenuhi, maka blok kode di dalam ELSE dieksekusi.
- Baris 4: Mencetak teks "Anda tidak lulus." karena nilai `$nilai` kurang dari 60.

### Kesimpulan Program

Program akan mencetak "Anda tidak lulus." karena nilai `$nilai` adalah 55, yang kurang dari 60.

## Switch Case

### Penjelasan

Kondisional statement `Switch Case` digunakan untuk membandingkan nilai ekspresi dengan beberapa nilai yang mungkin. Jika nilai ekspresi cocok dengan salah satu nilai `case`, maka blok kode di dalam `case` tersebut akan dieksekusi.

### Struktur program
```php
switch (ekspresi) {     
case nilai1:         
// blok kode yang akan dieksekusi jika ekspresi sama dengan nilai1         
break;     
case nilai2:         
// blok kode yang akan dieksekusi jika ekspresi sama dengan nilai2         
break;     
default:         
// blok kode yang akan dieksekusi jika tidak ada case yang cocok 
}
```



### Kode Program
```php
?<php
$nilai = 'B'; switch ($nilai) {    
case 'A':         
echo "Anda sangat baik.";
break;    
case 'B':  
echo "Anda baik.";  
break;     
case 'C':        
echo "Anda cukup.";
break;     
default: 
echo "Anda tidak lulus."; 
}
?>
```

### Hasil
![](aset/php9.png)

### Analisis

- Baris 1: Sebuah variabel `$nilai` diinisialisasi dengan nilai 'B'.
- Baris 2: Nilai `$nilai` dibandingkan dengan nilai-nilai case di dalam switch.
- Baris 3-5: Karena nilai `$nilai` sama dengan 'B', maka blok kode di dalam case 'B' dieksekusi.
- Baris 6: Mencetak teks "Anda baik." karena nilai `$nilai` sama dengan 'B'.

### Kesimpulan Program

Program akan mencetak "Anda baik." karena nilai `$nilai` adalah 'B', yang cocok dengan case 'B'.

## Array

### Array 1 Dimensi

#### Penjelasan

Array 1 dimensi adalah struktur data yang dapat menyimpan beberapa nilai dalam satu variabel. Setiap nilai dalam array memiliki indeks numerik yang dimulai dari 0.

#### Struktur program
```php
$nama_array = array(nilai1, nilai2, nilai3, ...);
```

##### Kode Program
```php
<?php
$buah = array(
"Apel", "Jeruk", "Mangga", "Anggur"
); 
echo "Saya suka makan " . $buah[0];
?>
```

### Hasil
![](aset/php10.png)


#### Analisis

- Baris 1: Membuat array `$buah` dengan nilai "Apel", "Jeruk", "Mangga", dan "Anggur".
- Baris 2: Mencetak teks "Saya suka makan Apel" karena nilai dengan indeks 0 dalam array adalah "Apel".

#### Kesimpulan Program

Program akan mencetak "Saya suka makan Apel" karena nilai dengan indeks 0 dalam array `$buah` adalah "Apel".

### Array Asosiatif

#### Penjelasan

Array asosiatif adalah struktur data yang menggunakan nama kunci (key) untuk setiap nilai dalam array. Ini memungkinkan kita untuk mengakses nilai berdasarkan kunci yang ditetapkan.

#### Struktur program

```php
$nama_array = array("kunci1" => nilai1, "kunci2" => nilai2, "kunci3" => nilai3, ...);
```
#### Kode Program

```php
<?php
$siswa = array("nama" => "John", "umur" => 20, "kelas" => "XII"); 
echo $siswa["nama"] . " berusia " . $siswa["umur"] . " tahun.";
?>
```


### Hasil
![](aset/php11.png)


#### Analisis

- Baris 1: Membuat array `$siswa` dengan kunci "nama", "umur", dan "kelas".
- Baris 2: Menggunakan kunci "nama" dan "umur" untuk mengakses nilai dalam array `$siswa`.
- Baris 2: Mencetak teks "John berusia 20 tahun."

#### Kesimpulan Program

Program akan mencetak "John berusia 20 tahun." karena nilai dengan kunci "nama" adalah "John" dan nilai dengan kunci "umur" adalah 20 dalam array `$siswa`.

## Multidimensi

### Penjelasan

Array multidimensi adalah array yang memiliki satu atau lebih array di dalamnya. Hal ini memungkinkan kita untuk membuat struktur data yang kompleks, seperti matriks.

### Struktur program
```php
$nama_array = array(     
array(nilai1, nilai2, nilai3, ...),     
array(nilai1, nilai2, nilai3, ...),     
... );
```
### Kode Program
```php
<?php
$matriks = array(  
array(1, 2, 3),  
array(4, 5, 6),
array(7, 8, 9) ); 
echo $matriks[1][2]; // Mengakses nilai 6
?>
```

### Hasil
![](aset/php13.png)


### Analisis

- Baris 1-3: Membuat array `$matriks` yang berisi array-array dengan nilai tertentu.
- Baris 4: Menggunakan indeks 1 dan 2 untuk mengakses nilai 6 dalam array `$matriks`.
- Baris 4: Mencetak nilai 6.

### Kesimpulan Program

Program akan mencetak nilai 6 karena nilai tersebut berada di indeks 1 dan 2 dalam array `$matriks`.

## var_dump

### Penjelasan

Fungsi `var_dump` digunakan untuk menampilkan informasi tentang tipe dan nilai dari sebuah variabel atau ekspresi. Ini berguna untuk debugging dan pemahaman tentang struktur data.

### Struktur program
```php
var_dump(variabel);
```
### Kode Program
```php
<?php
$angka = 10; 
var_dump($angka);
?>
```

### Hasil
![](aset/php14.png)


### Analisis

- Baris 1: Mendeklarasikan variabel `$angka` dengan nilai 10.
- Baris 2: Menggunakan `var_dump` untuk menampilkan informasi tentang variabel `$angka`.

### Kesimpulan Program

Program akan menampilkan `int(10)`, yang berarti `$angka` adalah integer dengan nilai 10.

## Looping

### For

#### Penjelasan

For loop digunakan untuk mengulang blok kode sejumlah tertentu kali. Ini sering digunakan ketika kita sudah mengetahui berapa kali iterasi yang diperlukan.

#### Struktur program
```php
for (inisialisasi; kondisi; perubahan){     
// blok kode yang akan diulang 
}
```
#### Kode Program
```php
<?php
for ($i = 1; $i <= 5; $i++) { 
echo "Nomor: $i <br>"; 
}
?>
```

### Hasil
![](aset/php15.png)




#### Analisis

- Baris 1: Inisialisasi variabel `$i` dengan nilai 1.
- Baris 2: Kondisi, loop akan terus berjalan selama `$i` kurang dari atau sama dengan 5.
- Baris 3: Setiap iterasi, nilai `$i` akan bertambah satu.
- Baris 4: Mencetak nomor dari 1 sampai 5.
#### Kesimpulan Program

Program akan mencetak nomor dari 1 sampai 5.

### While

#### Penjelasan

While loop digunakan untuk mengulang blok kode selama kondisi tertentu bernilai true. Ini berguna ketika jumlah iterasi tidak diketahui sebelumnya.

#### Struktur program
```php
while (kondisi) {  
// blok kode yang akan diulang 
}
```
##### Kode Program
```php
<?php
$i = 1; 
while ($i <= 5) {
echo "Nomor: $i <br>";  
$i++; 
}
?>
```

### Hasil
![](aset/php15.png)


#### Analisis

- Baris 1: Mendeklarasikan variabel `$i` dengan nilai 1.
- Baris 2: Loop akan terus berjalan selama nilai `$i` kurang dari atau sama dengan 5.
- Baris 3: Mencetak nomor dari 1 sampai 5.
- Baris 4: Setiap iterasi, nilai `$i` akan bertambah satu.
#### Kesimpulan Program

Program akan mencetak nomor dari 1 sampai 5.

### Do-While

#### Penjelasan

Do-While loop mirip dengan While loop, namun perbedaannya adalah Do-While loop akan menjalankan blok kode setidaknya sekali, bahkan jika kondisi tidak terpenuhi.

#### Struktur program
```php
do {     
// blok kode yang akan diulang 
} 
while (kondisi);
```
#### Kode Program
```php
<?php
$i = 1; do {     
echo "Nomor: $i <br>"; 
$i++; } 
while ($i <= 5);
?>
```
### Hasil
![](aset/php15.png)
#### Analisis

- Baris 1: Mendeklarasikan variabel `$i` dengan nilai 1.
- Baris 2-4: Mencetak nomor dari 1 sampai 5. Walaupun kondisi tidak terpenuhi, blok kode akan dijalankan sekali karena sifat Do-While loop.
#### Kesimpulan Program

Program akan mencetak nomor dari 1 sampai 5.

### Foreach

#### Penjelasan

Foreach loop digunakan untuk mengulang elemen-elemen dalam sebuah array. Loop ini berguna untuk mengakses setiap nilai dalam array tanpa harus mengkhawatirkan indeksnya.

#### Struktur program
```php
foreach ($array as $nilai) {  
// blok kode yang akan diulang 
}
```
#### Kode Program
```php
<?php
$buah = array("Apel", "Jeruk", "Mangga", "Anggur"); 
foreach ($buah as $nama) {
echo "Saya suka makan $nama <br>"; 
}
?>
```

### Hasil
![](aset/php16.png)



#### Analisis

- Baris 1: Mendefinisikan array `$buah`.
- Baris 2: Foreach loop akan mengulang setiap nilai dalam array `$buah` dan menyimpannya dalam variabel `$nama`.
- Baris 3: Mencetak teks "Saya suka makan ..." untuk setiap nilai dalam array `$buah`.
#### Kesimpulan Program

Program akan mencetak teks "Saya suka makan ..." untuk setiap nilai dalam array `$buah`.

### Function

#### Penjelasan

Function digunakan untuk mengelompokkan blok kode yang akan dijalankan secara bersamaan. Ini memungkinkan kita untuk menggunakan kode yang sama berulang kali tanpa harus menulis ulang.

#### Struktur program
```php
function nama_function($parameter1, $parameter2, ...) 
{     // blok kode yang akan dijalankan 
}
```


#### Kode Program
```php
<?php
function tambah($a, $b) {
return $a + $b; 
} 
$hasil = tambah(5, 3); 
echo "Hasil penjumlahan: $hasil";
?>
```

### Hasil
![](aset/php17.png)



#### Analisis

- Baris 1-3: Mendefinisikan function `tambah` yang menerima dua parameter `$a` dan `$b` dan mengembalikan hasil penjumlahan.
- Baris 5: Memanggil function `tambah` dengan nilai 5 dan 3 sebagai parameter.
- Baris 6: Mencetak hasil penjumlahan.

#### Kesimpulan Program

Program akan mencetak hasil penjumlahan dari 5 dan 3, yaitu 8.

## PHP Form

### GET Method

#### Penjelasan

Metode GET digunakan untuk mengirimkan data form ke server dalam URL. Data form akan terlihat pada URL dan cocok untuk digunakan dalam kasus-kasus di mana data yang dikirimkan tidak sensitif.

#### Struktur program
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Document</title>
</head>
<body>
    <!-- Pada atribut action, kalian tuliskan nama file php yang bertugas untuk mengelola atau menangkap data dari form tersebut. -->
    <form action="proses_get.php" method="GET">
        <input type="text" name="nama" placeholder="Masukkan nama">
        <input type="number" name="umur" placeholder="Masukkan umur"> <br>
        <button type="submit">Kirim</button>
    </form>
</body>
</html>
```
#### Kode Program 
```php
<?php
// Key dari array-nya, sesuai dengan nama dari atribut name di setiap input-nya
$nama = $_GET["nama"];
$umur = $_GET["umur"];
?>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ariq Hikari Hidayat - XI RPL 2 - GET</title>
</head>
<body>
    <p>Nama anda
        <?= $nama ?>
    </p>
    <p>Umur anda <?= $umur ?> tahun</p>
</body>
</html>
```

### Hasil
![](aset/php27.png)



#### Analisis
#### PHP Script (Baris 1-5)

1. `<?php`
    - Membuka blok kode PHP.
2. `// Key dari array-nya, sesuai dengan nama dari atribut name di setiap input-nya`
    - Komentar yang menjelaskan bahwa kunci array sesuai dengan atribut name dari input form.
3. `$nama = $_GET["nama"];`
    - Mengambil nilai dari parameter GET "nama" dan menyimpannya dalam variabel `$nama`.
4. `$umur = $_GET["umur"];`
    - Mengambil nilai dari parameter GET "umur" dan menyimpannya dalam variabel `$umur`.
5. `?>`
    - Menutup blok kode PHP.
6. `<!DOCTYPE html>`
    - Deklarasi tipe dokumen HTML.
7. `<html lang="en">`
    - Tag pembuka HTML dengan atribut bahasa "en" (English).
8. `<head>`
    - Tag pembuka untuk bagian kepala dokumen HTML.
9. `<meta charset="UTF-8">`
    - Menentukan set karakter yang digunakan adalah UTF-8.
10. `<meta name="viewport" content="width=device-width, initial-scale=1.0">`
    - Mengatur tampilan halaman untuk mendukung berbagai ukuran layar.
11. `<title>Ariq Hikari Hidayat - XI RPL 2 - GET</title>`
    - Judul halaman yang akan ditampilkan pada tab browser.
12. `</head>`
    - Tag penutup untuk bagian kepala dokumen HTML.
13. `<body>`
    - Tag pembuka untuk bagian tubuh dokumen HTML.
14. `<p>Nama anda <?= $nama ?></p>`
    - Menampilkan paragraf yang berisi nama yang diterima dari form GET menggunakan sintaks shorthand PHP `<?= ?>`.
15. `<p>Umur anda <?= $umur ?> tahun</p>`
    - Menampilkan paragraf yang berisi umur yang diterima dari form GET menggunakan sintaks shorthand PHP `<?= ?>`.
16. `</body>`
    - Tag penutup untuk bagian tubuh dokumen HTML.
17. `</html>`
    - Tag penutup dokumen HTML.


#### Kesimpulan Program
Kode ini menerima input dari pengguna melalui parameter GET pada URL, mengambil nilai `nama` dan `umur`, lalu menampilkannya di halaman HTML. Penggunaan PHP memungkinkan integrasi data dinamis dengan HTML, menjadikan halaman ini interaktif berdasarkan input pengguna. Struktur kodenya sederhana dan efisien, memanfaatkan sintaks shorthand PHP untuk menampilkan data yang diterima.


### POST Method

#### Penjelasan

Metode POST digunakan untuk mengirimkan data form ke server dalam bentuk tersembunyi. Data form tidak akan terlihat pada URL dan cocok untuk digunakan dalam kasus-kasus di mana data yang dikirimkan sensitif.

#### Struktur program
```php
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Document</title>
</head>
<body>
    <!-- Pada atribut action, kalian tuliskan nama file php yang bertugas untuk mengelola atau menangkap data dari form tersebut. -->
    <form action="proses_post.php" method="POST">
        <input type="text" name="nama_lengkap" placeholder="Masukkan nama">
        <input type="number" name="umur" placeholder="Masukkan umur">
        <input type="password" name="password" placeholder="Masukkan password"><br>
        <button type="submit">Kirim</button>
    </form>
</body>
</html>
```

#### Kode Program
```php
<?php
// Key dari array-nya, sesuai dengan nama dari atribut name di setiap input-nya
//$nama = $_POST["nama"];
$umur = $_POST["umur"];
var_dump($_POST);
?>
<!DOCTYPE html>
<html lang="en">
<head>
    <title> XI RPL 1 - POST</title>
</head>
<body>
    <p>Nama anda <?= $_POST["nama_lengkap"] ?></p>
    <p>Umur anda <?= $umur ?> tahun</p>
    <p>Password anda aman!</p>
</body>
</html>
```

### Hasil
![](aset/php29.png)

#### Analisis

- 1. `<?php`
    - Membuka blok kode PHP.
2. `// Key dari array-nya, sesuai dengan nama dari atribut name di setiap input-nya`
    - Komentar yang menjelaskan bahwa kunci array sesuai dengan atribut name dari input form.
3. `//$nama = $_POST["nama"];`
    - Baris ini dikomentari dan tidak akan dieksekusi.
4. `$umur = $_POST["umur"];`
    - Mengambil nilai dari parameter POST "umur" dan menyimpannya dalam variabel `$umur`.
5. `var_dump($_POST);`
    - Menampilkan semua data yang dikirimkan melalui metode POST untuk debugging.
6. `?>`
    - Menutup blok kode PHP.
7. `<!DOCTYPE html>`
    - Deklarasi tipe dokumen HTML.
8. `<html lang="en">`
    - Tag pembuka HTML dengan atribut bahasa "en" (English).
9. `<head>`
    - Tag pembuka untuk bagian kepala dokumen HTML.
10. `<title> XI RPL 1 - POST</title>`
    - Judul halaman yang akan ditampilkan pada tab browser.
11. `</head>`
    - Tag penutup untuk bagian kepala dokumen HTML.
12. `<body>`
    - Tag pembuka untuk bagian tubuh dokumen HTML.
13. `<p>Nama anda <?= $_POST["nama_lengkap"] ?></p>`
    - Menampilkan paragraf yang berisi nama lengkap yang diterima dari form POST menggunakan sintaks shorthand PHP `<?= ?>`.
14. `<p>Umur anda <?= $umur ?> tahun</p>`
    - Menampilkan paragraf yang berisi umur yang diterima dari form POST menggunakan sintaks shorthand PHP `<?= ?>`.
15. `<p>Password anda aman!</p>`
    - Menampilkan pesan statis bahwa password pengguna aman.
16. `</body>`
    - Tag penutup untuk bagian tubuh dokumen HTML.
17. `</html>`
    - Tag penutup dokumen HTML.

#### Kesimpulan Program
Kode ini menerima input dari pengguna melalui parameter POST, mengambil nilai `nama_lengkap` dan `umur`, lalu menampilkannya di halaman HTML. Selain itu, semua data POST ditampilkan menggunakan `var_dump` untuk tujuan debugging. Penggunaan PHP memungkinkan integrasi data dinamis dengan HTML, menjadikan halaman ini interaktif berdasarkan input pengguna. Struktur kodenya sederhana dan efisien, memanfaatkan sintaks shorthand PHP untuk menampilkan data yang diterima.


# Koneksi Database

## Kode Program
```php
<?php
//koneksi ke database
$koneksi = mysqli_connect('localhost', 'root', '', 'rental_angga');
// Memeriksa koneksi
if (!$koneksi) {
    die("Error, tidak bisa koneksi ke database: " . mysqli_connect_error());
} else {
    echo "<br> Koneksi aman <br>";
}
?>
```

## Hasil
![](aset/php20.png)

## Analisis
- Fungsi `mysqli_connect` digunakan untuk membuat koneksi ke database MySQL.
- Parameter pertama adalah nama host, dalam hal ini 'localhost'.
- Parameter kedua adalah nama pengguna database, dalam hal ini 'root'.
- Parameter ketiga adalah kata sandi pengguna database, dalam hal ini kosong ('').
- Parameter keempat adalah nama database yang akan digunakan, dalam hal ini 'rental_angga'.
- Menggunakan fungsi `mysqli_connect_error` untuk menampilkan pesan error jika koneksi gagal. 
- Jika koneksi berhasil, pesan "Koneksi aman" akan ditampilkan.

## Kesimpulan
Kode tersebut berguna untuk memastikan bahwa koneksi ke database berhasil dilakukan sebelum menjalankan operasi-operasi database lainnya. Jika koneksi gagal, maka akan menampilkan pesan error dan menghentikan eksekusi script dengan `die()`.

# Tampilkan Data
## Kode Program
```php
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>index tabel</title>
</head>
<body>
    <h2>Data Siswa Berprestasi</h2>
    <table border="5">
        <tr>
            <th>id_siswa</th>
            <th>nama</th>
            <th>email</th>
            <th>jenis_kelamin</th>
            <th>alamat</th>
        </tr>
        <?php
        include "koneksi.php";
        $i = 1;
        $query = mysqli_query($koneksi, "SELECT * FROM siswa");
        while ($data = mysqli_fetch_array($query)) {
            ?>
            <tr>
                <td><?php echo $i; ?></td>
                <td><?php echo $data['nama']; ?></td>
                <td><?php echo $data['email']; ?></td>
                <td><?php echo $data['jenis_kelamin']; ?></td>
                <td><?php echo $data['alamat']; ?></td>
            </tr>
            <?php
            $i++;
        }
        ?>
    </table>
</body>
</html>
```

## Hasil
![](aset/php21.png)

## Analisis
- Baris 1-8: Membuat struktur dasar dokumen HTML dengan pengaturan charset UTF-8 dan viewport untuk memastikan kompatibilitas dengan berbagai perangkat. Judul halaman ditetapkan sebagai "index tabel".
- Baris 9-16: Membuat tabel dengan border 5 dan menambahkan header kolom untuk `id_siswa`, `nama`, `email`, `jenis_kelamin`, dan `alamat`.
- Baris 17-32: Mengimpor file koneksi database (`koneksi.php`). Menginisialisasi variabel `$i` untuk penomoran baris. Mengambil data dari tabel `siswa` di database dan menampilkan setiap baris data dalam tabel HTML. Setiap iterasi dari loop `while` menambahkan satu baris baru ke tabel HTML dengan data siswa yang diambil dari database. Penomoran baris diatur menggunakan variabel `$i` yang diincrement setiap kali data ditampilkan.
- Baris 33-35: Menutup tag tabel dan dokumen HTML.


## Kesimpulan
- Membuat struktur dasar dokumen HTML dengan pengaturan charset dan viewport.
- Membuat tabel HTML dengan header kolom untuk `id_siswa`, `nama`, `email`, `jenis_kelamin`, dan `alamat`.
- Mengimpor koneksi database.
- Mengambil data dari tabel `siswa` di database dan menampilkan setiap baris data dalam tabel HTML.
- Menampilkan setiap baris data dengan penomoran yang diatur menggunakan variabel `$i`.


# Tambahkan Data

## Kode Program
```php
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Document</title>
</head>
<body>
    <h2>Tambah Data</h2>
    <?php
    include "koneksi.php";
    if (isset($_POST['simpan'])) {
        $nama = $_POST['nama'];
        $email = $_POST['email'];
        $jenis_kelamin = $_POST['jenis_kelamin'];
        $alamat = $_POST['alamat'];
        $query = mysqli_query($koneksi, "INSERT into siswa(nama,email,jenis_kelamin,alamat)
        values ('$nama','$email','$jenis_kelamin','$alamat')");
        if ($query == true) {
            echo "<script>
            alert('Tambah data Berhasil')
            window.location.href='table.php'
            </script>";
        } else {
            echo '<script>alert("Tambah data gagal")</script>';
        }
    }
    ?>
    <form method="post">
        <table>
            <tr>
                <td>Nama</td>
                <td><input type="text" name="nama"></td>
            </tr>
            <tr>
                <td>Email</td>
                <td><input type="text" name="email"></td>
            </tr>
            <tr>
                <td>Jenis Kelamin</td>
                <td>>
                    <select name="jenis_kelamin">
                        <option>Laki-laki</option>
                        <option>Perempuan</option>
                    </select>
                </td>
            </tr>
            <tr>
                <td>Alamat</td>
                <td><input type="text" name="alamat"></td>
            </tr>
            <tr>
                <td></td>
                <td>
                    <button name="simpan" type="submit">Simpan</button>
                    <button type="reset">Reset</button>
                    <a href="table.php">Kembali</a>
                </td>
            </tr>
        </table>
    </form>
</body>
</html>
```


## Hasil
### Before
![](aset/php21.png)

### After
![](aset/php22.png)

## Analisis
- Baris 1-8: Membuat struktur dasar dokumen HTML dengan bahasa yang ditetapkan ke bahasa Inggris dan judul halaman "Document".
- Baris 9-26: Mengimpor file koneksi database (`koneksi.php`). Memeriksa apakah tombol "simpan" telah ditekan. Jika ya, mengambil data dari form dan menyimpan data baru siswa ke dalam database. Jika berhasil, menampilkan pesan sukses dan mengarahkan pengguna ke `table.php`. Jika gagal, menampilkan pesan error.
- Baris 27-55: Membuat formulir HTML untuk menambahkan data siswa baru. Terdapat input untuk mengisi nama, email, jenis kelamin, dan alamat siswa. Terdapat juga tombol untuk menyimpan data baru, mereset form, dan kembali ke halaman `table.php`.

## Kesimpulan
1. Mengimpor koneksi database.
2. Memeriksa apakah formulir telah disubmit dan menyimpan data baru jika ya.
3. Menampilkan formulir HTML untuk mengisi data siswa baru.

Jika penambahan data berhasil dilakukan, pengguna akan diarahkan kembali ke halaman `table.php` dengan pesan sukses. Jika gagal, pengguna akan melihat pesan error. Formulir ini juga menyediakan opsi untuk mereset data yang telah diinput dan kembali ke halaman daftar siswa.


# Ubah Data
## Kode Program
```php
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Document</title>
</head>
<body>
    <h2>Ubah Data</h2>
    <?php
    include "koneksi.php";
    $id = $_GET['id_siswa'];
    if (isset($_POST['simpan'])) {
        $nama = $_POST['nama'];
        $email = $_POST['email'];
        $jenis_kelamin = $_POST['jenis_kelamin'];
        $alamat = $_POST['alamat'];
        $query = mysqli_query($koneksi, "UPDATE siswa SET
                                        nama='$nama',
                                        email='$email',
                                        jenis_kelamin='$jenis_kelamin',
                                        alamat='$alamat'
                                        WHERE id_siswa=$id");
        if ($query) {
            echo "<script>
            alert('ubah data Berhasil')
            window.location.href='table.php'
            </script>";
        } else {
            echo '<script>alert("ubah data gagal")</script>';
        }
    }
    $query = mysqli_query($koneksi, "SELECT * FROM siswa where id_siswa=$id");
    $data = mysqli_fetch_array($query);
    if ($data == "") {
        die('Data tidak ada');
    }
    ?>
    <form method="post">
        <table>
            <tr>
                <td>Nama</td>
                <td><input type="text" value="<?= $data['nama'] ?>" name="nama"></td>
            </tr>
            <tr>
                <td>Email</td>
                <td><input type="text" value="<?= $data['email'] ?>" name="email"></td>
            </tr>
            <tr>
                <td>Jenis Kelamin</td>
                <td>>
                    <select name="jenis_kelamin">
                        <option <?php if ($data['jenis_kelamin'] == "laki-laki")
                            echo 'selected'; ?>>Laki-laki</option>
                        <option <?php if ($data['jenis_kelamin'] == "perempuan")
                            echo 'selected'; ?>>Perempuan</option>
                    </select>
                </td>
            </tr>
            <tr>
                <td>Alamat</td>
                <td><input type="text" value="<?= $data['alamat'] ?>" name="alamat"></td>
            </tr>
            <tr>
                <td></td>
                <td>
                    <button name="simpan" type="submit">Ubah</button>
                    <button type="reset">Reset</button>
                    <a href="table.php">Kembali</a>
                </td>
            </tr>
        </table>
    </form>
</body>
</html>
```


## Hasil

### Before
![](aset/php22.png)


### After
![](aset/php23.png)

## Analisis
- Baris 1-8: Membuat struktur dasar dokumen HTML dengan bahasa yang ditetapkan ke bahasa Inggris dan judul halaman "Document".
- Baris 9-11: Mengimpor file koneksi database (`koneksi.php`) dan mengambil parameter `id_siswa` dari URL.
- Baris 12-26: Memeriksa apakah tombol "simpan" telah ditekan. Jika ya, mengambil data dari form dan mengupdate data siswa di database. Jika berhasil, menampilkan pesan sukses dan mengarahkan pengguna ke `table.php`. Jika gagal, menampilkan pesan error.
- Baris 27-32: Mengambil data siswa dari database berdasarkan `id_siswa`. Jika data tidak ditemukan, menghentikan eksekusi dengan pesan "Data tidak ada".
- Baris 33-64: Membuat formulir HTML untuk mengubah data siswa dengan mengisi nilai awal berdasarkan data yang diambil dari database. Terdapat pilihan untuk mengubah nama, email, jenis kelamin, dan alamat siswa. Terdapat juga tombol untuk menyimpan perubahan, mereset form, dan kembali ke halaman `table.php`.

## Kasimpulan
1. Mengimpor koneksi database.
2. Mengambil `id_siswa` dari URL.
3. Memeriksa apakah formulir telah disubmit dan melakukan update data jika ya.
4. Mengambil data siswa dari database untuk mengisi nilai awal form.
5. Menampilkan formulir HTML dengan data yang bisa diubah.

Jika perubahan data berhasil dilakukan, pengguna akan diarahkan kembali ke halaman `table.php` dengan pesan sukses. Jika gagal, pengguna akan melihat pesan error. Formulir ini juga menyediakan opsi untuk mereset data yang telah diinput dan kembali ke halaman daftar siswa.




# Hapus Data
## Kode Program
```php
<?php
include('koneksi.php');
if(isset($_GET['id'])){
    $id = $_GET['id'];
    $query = mysqli_query($koneksi, "DELETE FROM siswa WHERE id_siswa = $id");
   if($query) {
            echo "<script>
            alert('Hapus data Berhasil')
            window.location.href='table.php'
            </script>";
        }else {
            echo '<script>alert("Hapus data gagal")</script>';
        }
}
?>
```


## Hasil


### Before
![](aset/php23.png)

### After
![](aset/php24.png)



## Analisis
- Mengimpor file koneksi database (`koneksi.php`).
- Memeriksa apakah parameter ID (`$_GET['id']`) telah diberikan melalui URL.
- Jika ID telah diberikan, maka ID tersebut disimpan dalam variabel `$id`.
- Selanjutnya, melakukan query DELETE untuk menghapus data siswa dari tabel `siswa` berdasarkan ID siswa yang diberikan.
- Jika query DELETE berhasil dilakukan, maka akan menampilkan pesan sukses menggunakan JavaScript `alert` dan mengarahkan pengguna kembali ke halaman `table.php`.
- Jika query DELETE gagal, akan menampilkan pesan error menggunakan JavaScript `alert`.


## Kesimpulan
- **Koneksi Database**: Kode tersebut memastikan terjadi koneksi yang sukses ke database sebelum melakukan operasi penghapusan data.
    
- **Penghapusan Data**: Jika parameter ID (`$_GET['id']`) tersedia dalam URL, maka data siswa dengan ID tersebut akan dihapus dari tabel `siswa` menggunakan perintah SQL `DELETE`.
    
- **Feedback Pengguna**: Setelah operasi penghapusan selesai, pengguna akan diberikan feedback berupa pesan sukses jika penghapusan berhasil dilakukan, atau pesan gagal jika terjadi masalah dalam penghapusan data.
    
- **Redirect**: Setelah pesan sukses ditampilkan, pengguna akan diarahkan kembali ke halaman `table.php` agar dapat melihat perubahan yang telah terjadi.



# Session/Login

## Kode Program
```php
<?php
session_start();
if (isset($_POST['submit'])) {
    $username = $_POST['username'];
    $password = $_POST['password'];
    $koneksi = mysqli_connect('localhost', 'root', '', 'basis_data') or die('error koneksi');
    $result = mysqli_query($koneksi, "SELECT * FROM user WHERE username = '$username' AND password = '$password'");
    $data = mysqli_fetch_assoc($result);
    if (isset($data)) {
        $_SESSION['username'] = $data['username'];
        $_SESSION['nama'] = $data['nama'];
        $_SESSION['status'] = 'login';
        header('Location: user.php');
    } else {
        echo "Username dan Password Salah";
    }
}
?>
<!DOCTYPE html>
<html>
<head>
    <title>Login Session</title>
</head>
<body>
    <form method="post">
        <label>Username</label>
        <input type="text" name="username">
        <br>
        <label>Password</label>
        <input type="password" name="password">
        <br>
        <button type="submit" name="submit">Login</button>
    </form>
</body>
</html>
```

## Hasil

### Before
![](aset/php25.png)


### After
![](aset/php26.png)


## Analisis
- Fungsi `session_start()` digunakan untuk memulai session di PHP. Ini harus dipanggil di setiap halaman yang menggunakan session.
- Saat form login disubmit (`isset($_POST['submit'])`), nilai dari input username dan password diambil.
- Dilakukan koneksi ke database dan query untuk mencari data pengguna dengan username dan password yang cocok.
- Jika data ditemukan, session untuk username, nama, dan status login diset, dan pengguna diarahkan ke halaman `user.php`.
- Jika data tidak ditemukan, akan ditampilkan pesan "Username dan Password Salah".
- Form ini berisi input untuk username dan password, serta tombol submit untuk mengirim data login.


## Kesimpulan
1. **Session Management**: Kode menggunakan `session_start()` untuk memulai session, dan `$_SESSION` digunakan untuk menyimpan informasi tentang pengguna yang sedang login seperti username, nama, dan status.
    
2. **Form Login**: Form login menggunakan metode POST untuk mengirimkan data username dan password. Jika form disubmit, kode akan mencocokkan informasi login dengan data yang ada di database.
    
3. **Database Connection**: Kode menggunakan fungsi `mysqli_connect()` untuk melakukan koneksi ke database MySQL. Ini dilakukan sebelum proses pengecekan login dilakukan.
    
4. **Redirect**: Jika informasi login benar, pengguna diarahkan ke halaman `user.php`. Jika tidak, pesan error ditampilkan.
    
5. **Keamanan**: Kode ini hanya menyajikan contoh sederhana dan tidak menerapkan praktik keamanan yang lengkap, seperti penggunaan prepared statement untuk mencegah SQL injection atau hashing password untuk keamanan password.
    
6. **Kesimpulan**: Kode ini menunjukkan cara dasar mengelola proses login menggunakan session di PHP. Ini adalah fondasi yang baik untuk dikembangkan lebih lanjut dengan penanganan kesalahan yang lebih baik, keamanan yang lebih baik, dan fitur tambahan seperti logout.



# Upload dan Download
## Upload
### Kode Program
```php
function upload(): string
{
    $nameImage = $_FILES['imageNew']['name'];
    $directoryFile = $_FILES['imageNew']['tmp_name'];
    $errorImage = intval($_FILES['imageNew']['error']);
    $sizeFile = $_FILES['imageNew']['size'];
    // cek apakah gambar ada
    if ($errorImage === 4) {
        echo "<script>alert('Anda Belum Upload Gambar')</script>";
        return false;
    }
    // mengambil ekstensi file
    $validType = ['svg', 'jpg', 'png', 'jpeg', 'webp'];
    $extensionFile = explode(".", $nameImage);
    $extensionValid = strtolower(end($extensionFile));
    // cek apakah yang diupload gambar atau bukan
    if (!in_array($extensionValid, $validType)) {
        echo "<script>alert('yang anda Upload bukan gambar')</script>";
        return false;
    }
    // cek size file
    if ($sizeFile > 3_000_000) {
        echo "<script>alert('Ukuran File Terlalu Besar!!(Maks 3MB)')</script>";
        return false;
    }
    // upload file
    $nameImage = uniqid() . "." . $extensionValid;
    move_uploaded_file($directoryFile, "../assets/img/{$nameImage}");
    // mengembalikan namafile yg sudah divalidasi
    return $nameImage;
}
```

### Hasil
![](aset/php30.png)


### Analisis
- **Variabel Input**: Fungsi ini mengambil input dari form dengan menggunakan variabel `$_FILES['imageNew']` untuk mendapatkan informasi tentang file gambar yang diunggah seperti nama file (`$nameImage`), lokasi sementara file (`$directoryFile`), error jika terjadi (`$errorImage`), dan ukuran file (`$sizeFile`).
    
- **Validasi**:
    
    - Fungsi ini melakukan beberapa validasi terhadap file gambar yang diunggah.
    - Pertama, dilakukan pengecekan apakah gambar sudah diunggah atau belum. Jika belum, akan muncul pesan peringatan dan fungsi akan mengembalikan `false`.
    - Selanjutnya, dilakukan pengecekan ekstensi file untuk memastikan bahwa yang diunggah adalah file gambar dengan ekstensi yang diizinkan (svg, jpg, png, jpeg, webp). Jika bukan gambar, akan muncul pesan peringatan dan fungsi akan mengembalikan `false`.
    - Kemudian, dilakukan pengecekan ukuran file. Jika ukurannya melebihi 3MB, akan muncul pesan peringatan dan fungsi akan mengembalikan `false`.
- **Proses Upload**: Jika semua validasi berhasil, maka file gambar akan diupload ke direktori yang ditentukan (`../assets/img/`) dengan nama file yang diacak (`$nameImage`).
    
- **Pengembalian Nama File**: Fungsi ini mengembalikan nama file gambar yang sudah divalidasi dan diupload agar dapat digunakan untuk menyimpan informasi file gambar tersebut di database atau di tempat lain yang diperlukan.
    
- **Pesan Peringatan**: Pesan peringatan ditampilkan menggunakan JavaScript `alert()` untuk memberi tahu pengguna tentang masalah yang terjadi saat upload file gambar.

### Kesimpulan
- **Validasi Input**: Fungsi ini melakukan validasi terhadap file gambar yang diunggah, termasuk pengecekan apakah file sudah diunggah, jenis file yang diunggah, dan ukuran file yang diunggah.
    
- **Penanganan Kesalahan**: Jika terjadi kesalahan dalam proses upload, seperti file belum diunggah, jenis file yang tidak valid, atau ukuran file yang terlalu besar, fungsi akan memberikan pesan peringatan dan mengembalikan `false`.
    
- **Proses Upload**: Jika tidak terjadi kesalahan, fungsi akan mengacak nama file gambar dan mengupload file gambar ke direktori yang ditentukan.
    
- **Pengembalian Nama File**: Fungsi akan mengembalikan nama file gambar yang sudah divalidasi dan diupload, sehingga dapat digunakan untuk keperluan selanjutnya, seperti menyimpan informasi file gambar tersebut di database.
    
- **Pesan Peringatan**: Pesan peringatan ditampilkan menggunakan JavaScript `alert()` untuk memberitahu pengguna tentang masalah yang terjadi saat upload file gambar.



## Download
### Kode Program
```php
<?php
include "koneksi.php";
$query = mysqli_query($koneksi, 'SELECT * FROM siswa');
$data = [];
$data[] = ["ID", "Nama", "Gambar", "Email", "Jenis Kelamin", "Alamat"];
while ($row = mysqli_fetch_assoc($query)) {
    $data[] = [
        $row['id_siswa'],
        $row['nama'],
        $row['gambar']
        $row['email'],
        $row['jenis_kelamin'],
        $row['alamat']
    ];
}
$namafile = "excel_data.xls";
header("Content-Type: application/vnd.ms-xls");
header("Content-Disposition: attachment;filename=\"$namafile\"");
header("Cache-Control: max-age=0");
$output = fopen("php://output", "w");
foreach ($data as $row) {
    fputcsv($output, $row, "\t");
}
fclose($output);
exit;
```

### Hasil
![](aset/php31.png)


### Analisis
- **Koneksi Database**: Kode menggunakan `include "koneksi.php";` untuk mengimpor file koneksi database yang menghubungkan ke database MySQL.
    
- **Query dan Pengambilan Data**: Dilakukan query `SELECT * FROM siswa` untuk mengambil semua data siswa dari tabel `siswa` dalam database. Data kemudian dimasukkan ke dalam array `$data` dalam format yang sesuai untuk diekspor ke file Excel.
    
- **Penyiapan File Excel**: Kode menggunakan header HTTP untuk mengatur tipe konten menjadi `application/vnd.ms-xls` agar browser menganggap file ini sebagai file Excel. Header `Content-Disposition` digunakan untuk memberi nama file Excel yang akan diunduh.
    
- **Penulisan Data ke File Excel**: Menggunakan `fputcsv()` untuk menulis data ke file Excel dengan delimiter tab (`"\t"`).
    
- **Penutup dan Keluar**: Setelah data ditulis ke file Excel, `fclose($output);` digunakan untuk menutup file dan `exit;` digunakan untuk mengakhiri skrip PHP.


### Kesimpulan
Kode tersebut digunakan untuk mengambil data siswa dari database MySQL dan menyimpannya ke dalam file Excel yang kemudian diunduh oleh pengguna. Ini memanfaatkan kemampuan PHP untuk menghasilkan file Excel dengan menggunakan delimiter tab untuk memisahkan data. Kode ini memungkinkan pengguna untuk dengan mudah mengunduh data dalam format yang mudah dibaca dan dapat diedit di Excel.









