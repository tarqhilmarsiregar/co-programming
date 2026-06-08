# Competitive Programming

## 1. Langkah Minimal Si Joki Fotokopi
Batas Waktu (Time Limit): 1.0 detik | 
Batas Memori (Memory Limit): 256 MB

### Deskripsi Soal
Budi adalah seorang mahasiswa akhir yang terburu-buru mengantarkan berkas revisi skripsi ke ruangan dosennya. Jarak dari posisi Budi saat ini (posisi 0) menuju ruangan dosen adalah sejauh X meter.

Dalam satu langkah, Budi memiliki kemampuan fisik untuk melompat maju ke depan sejauh 1, 2, 3, 4, atau 5 meter. Budi ingin sampai tepat di posisi X (atau melewatinya sedikit pada langkah terakhir jika terpaksa) dengan jumlah langkah sesedikit mungkin. Bantulah Budi menentukan berapa jumlah langkah minimal yang harus ia tempuh!

### Format Input
Input terdiri dari satu baris tunggal yang berisi satu bilangan bulat X (1 <= X <= 1.000.000), menyatakan jarak dalam meter.

### Format Output
Cetak satu bilangan bulat yang menyatakan jumlah langkah minimal Budi.

#### Contoh Kasus 1
Input
```
5
```

Output
```
1
```
Penjelasan: Langsung lompat 5 meter

#### Contoh Kasus 2
Input
```
12
```

Output
```
3
```

Penjelasan: Lompat 5 + 5 + 2, total 3 langkah

## 2. Enkripsi Pesan Rahasia Ormawa
Batas Waktu (Time Limit): 1.0 detik | 
Batas Memori (Memory Limit): 256 MB

### Deskripsi Soal
Untuk menjaga kerahasiaan koordinasi rapat, sebuah organisasi mahasiswa (Ormawa) menggunakan metode enkripsi berbasis pergeseran karakter (Caesar Cipher modifikasi). Aturannya adalah setiap huruf alfabet kecil (a-z) di dalam pesan akan digeser maju sebanyak K posisi di dalam urutan alfabet.

Pergeseran ini bersifat memutar (circular). Artinya, jika huruf z digeser maju sebanyak 1 posisi, ia akan kembali menjadi huruf a. Karakter selain huruf kecil (seperti spasi, angka, atau tanda baca) tidak mengalami perubahan sama sekali. Tugas Anda adalah membuat program enkripsinya!

### Format Input
* Baris pertama berisi satu bilangan bulat K (0 <= K <= 100), yang menyatakan jumlah pergeseran posisi
* Baris kedua berisi sebuah string S (1 <= |S| <= 10.000), yang merupakan pesan asli yang akan dienkripsi. S dapat mengandung spasi.

### Format Output
Cetak satu baris string hasil enkripsi dari pesan tersebut.

#### Contoh Kasus
Input
```
2
halo zuki!
```

Output
```
janc bwmk!
```

## 3. Pengurutan Berkas Asisten Lab
Batas Waktu (Time Limit): 1.5 detik | 
Batas Memori (Memory Limit): 256 MB

### Deskripsi Soal
Asisten Laboratorium Informatika ingin merapikan data nilai tugas praktikan. Terdapat N praktikan yang memiliki data Nama (berupa satu kata) dan Nilai Akhir (berupa bilangan bulat).

Asisten lab meminta Anda mengurutkan data tersebut dengan aturan prioritas sebagai berikut:
1. Urutkan berdasarkan Nilai Akhir secara menurun (descending - dari yang terbesar ke terkecil)
2. Jika ada dua praktikan atau lebih yang memiliki Nilai Akhir yang sama, urutkan berdasarkan Nama secara menaik (ascending - sesuai urutan alfabetis/leksikografis)

### Format Input
* Baris pertama berisi satu bilangan bulat N (1 <= N <= 50.000), menyatakan jumlah praktikan.
* N baris berikutnya masing-masing berisi satu string nama (tanpa spasi) dan satu bilangan bulat nilai (0 <= nilai <= 100)

### Format Output
Cetak N baris data praktikan yang telah diurutkan dengan format: `Nama Nilai`

#### Contoh Kasus
Input
```
3
Budi 85
Andi 90
Ali 85
```

Output
```
Andi 90
Ali 85
Budi 85
```

## 4. Detektor Duplikat Berkas Tugas
Batas Waktu (Time Limit): 2.0 detik | 
Batas Memori (Memory Limit): 256 MB

### Deskripsi Soal
Dosen menduga ada mahasiswa yang mengumpulkan berkas tugas yang identik satu sama lain. Setiap berkas tugas direpresentasikan oleh sebuah kode unik berupa bilangan bulat. Terdapat daftar sebanyak N kode tugas yang masuk ke sistem pengumpulan data.

Dosen ingin mengetahui: Berapakah jumlah total berkas tugas duplikat yang ada di dalam sistem? Berkas dikategorikan sebagai duplikat jika kode tugas tersebut sudah pernah muncul/dikumpulkan sebelumnya oleh mahasiswa lain.

### Format Input
* Baris pertama berisi satu bilangan bulat N (1 <= N <= 100.000)
* Baris kedua berisi N bilangan bulat Ai (1 <= Ai <= 10^9), yang merupakan kode unik dari masing-masing berkas tugas.

### Format Output
Cetak satu bilangan bulat yang menyatakan jumlah total berkas tugas yang terdeteksi sebagai duplikat.

#### Contoh Kasus
Input
```
6
10 20 10 30 20 10
```

Output
```
3
```

## 5. Manajemen Batas Memori Server Cloud
Batas Waktu (Time Limit): 2.0 detik | 
Batas Memori (Memory Limit): 256 MB

### Deskripsi Soal
Unit TI Kampus memiliki sekelompok server sebanyak N buah. Masing-masing server memiliki beban kerja berupa penggunaan memori dalam satuan Gigabyte yang dinyatakan dalam array A. Kampus ingin menerapkan kebijakan restrukturisasi efisiensi dengan menetapkan sebuah Batas Ambang Penggunaan Memori (M) yang seragam pada seluruh server tersebut.

Aturan pemangkasan memori bekerja sebagai berikut:
* Jika penggunaan memori sebuah server melebihi nilai batas M, maka penggunaan memori server tersebut akan dipangkas tepat menjadi senilai M
* Jika penggunaan memori server sejak awal kurang dari atau sama dengan nilai batas M, memori server tersebut tidak akan diubah sama sekali

Pihak TI kampus memberikan target bahwa total akumulasi memori dari seluruh server setelah pemangkasan tidak boleh melebihi kapasitas target sebesar T Gigabyte. Tugas Anda adalah mencari nilai batas M terbesar berupa bilangan bulat yang memenuhi target efisiensi tersebut!

### Format Input
* Baris pertama berisi dua buah bilangan bulat: N (1 <= N <= 100.000) mewakili jumlah server, dan T (1 <= T <= 10^14) mewakili target total alokasi memori maksimal
* Baris kedua berisi N buah bilangan bulat Ai (1 <= Ai <= 10^9) yang menyatakan kapasitas memori awal masing-masing server

### Format Output
Cetak satu bilangan bulat yang menyatakan nilai konfigurasi batas M terbesar yang memenuhi syarat. Jika total memori awal server dari awal sudah tidak melebihi T, maka konfigurasi batas M tidak perlu diterapkan (program cukup mencetak nilai memori terbesar yang ada pada server awal).

#### Contoh Kasus
Input
```
4 10
2 3 4 5
```

Output
```
2
```

Penjelasan: Jika kita memilih M = 2, maka kapasitas server berubah menjadi [2, 2, 2, 2]. Total penjumlahannya adalah 2+2+2+2 = 8 (di bawah target 10). Jika memilih M = 3, kapasitas server menjadi [2, 3, 3, 3] dengan total 11 (melebihi target 10). Maka nilai bilangan bulat terbesar bagi M adalah 2.
