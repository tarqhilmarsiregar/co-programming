# Competitive Programming

## Langkah Minimal Si Joki Fotokopi
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
