# Jarkom-Modul-1-E11-2021
## Anggota Kelompok :
| Nama | NRP |
|------|-----|
|Rizqi Rifaldi|05111940000068|
|Yusuf Anfasya|05111940000077|
|Muhammad Subhan|05111940000204|

Pada Praktikum Jaringan Komputer Modul 1 ini kami diperintahkan untuk menjawab 15 soal mengenai wireshark.

### Soal 1
Sebutkan webserver yang digunakan pada "ichimarumaru.tech"!

Webserver dari website “ichimarumaru.tech” dapat dilihat dengan wireshark dengan menggunakan filter :
<b>“http.host == ichimarumaru.tech”</b> seperti pada gambar berikut :

[![no1.png](https://i.postimg.cc/zDC1Wb9L/no1.png)](https://postimg.cc/QVdPZtNs)

Kemudian melakukan follow HTTP Stream dan disitulah kita bisa melihat webserver yang digunakan oleh ichimarumaru.tech seperti pada gambar berikut :

[![no1b.png](https://i.postimg.cc/CxZPG9zv/no1b.png)](https://postimg.cc/21D7mcdv)

Dapat dilihat pada gambar tersebut bahwa ichimarumaru.tech menggunakan webserver <b>nginx/1.18.0 (Ubuntu)</b>

### Soal 2

Temukan paket dari web-web yang menggunakan basic authentication method!

Kita bisa melihat paket dari web-web pada 1-5.pcapng yang menggunakan basic authentication method dengan menggunakan filter <b>http.authbasic</b>

Hasilnya adalah :

[![no2.png](https://i.postimg.cc/xTmtxhvq/no2.png)](https://postimg.cc/tYX37rmH)

Ada 3 paket yang menggunakan basic authentication method.

### Soal 3

Ikuti perintah di basic.ichimarumaru.tech! Username dan password bisa didapatkan dari file .pcapng!

Pertama-tama kita harus mencari username dan password untuk login ke basic.ichimarumaru.tech. Dengan menggunakan filter <b>http.host == "basic.ichimarumaru.tech" && http.authbasic</b>.

Hasilnya adalah sebagai berikut :

[![no3.png](https://i.postimg.cc/2SbmKzHh/no3.png)](https://postimg.cc/v4sp1dwZ)

Kemudian kita bisa mendapatkan username dan password setelah meng-klik paket HTTP dan extend HTTP serta extend Authentication.

Username : kuncimenujulautan

Password : tQKEJFbgNGC1NCZlWAOjhyCOm6o3xEbPkJhTciZN

Kemudian kita masukkan ke website basic.ichimarumaru.tech dan disuruh untuk menjawab pertanyaan sebagai berikut :

[![3b.png](https://i.postimg.cc/R079QgFH/3b.png)](https://postimg.cc/Ty3ZTqnd)

Pertanyaannya adalah : "Sebutkan urutan konfigurasi pengkabelan T568A!

Jawaban : putih hijau, hijau, putih orange, biru, putih biru, orange, putih coklat, coklat

### Soal 4

Temukan paket mysql yang mengandung perintah query select!

Kita bisa mencari paket mysql yang mengandung peritnah query select dengan menggunakan filter <b>mysql.query ~ “SELECT”</b> dan akan muncul 3 paket seperti ini :

[![no4.png](https://i.postimg.cc/bN2SQjQV/no4.png)](https://postimg.cc/xcnd2hpL)

Bisa dilihat ada 3 paket mysql yang mengandung perintah query SELECT.

### Soal 5

Login ke portal.ichimarumaru.tech kemudian ikuti perintahnya! Username dan password bisa didapat dari query insert pada table users dari file .pcap!

Pertama, kita harus mencari username dan password pada paket mysql dengan menggunakan filter <b>mysql.query ~ “INSERT”</b> dan akan muncul seperti ini :

[![no5a.png](https://i.postimg.cc/t4KKYF9m/no5a.png)](https://postimg.cc/CR4P2BBj)

dan kita bisa melihat username dan password dengan melakukan follow TCP Stream dari paket tersebut. Dapat dilihat pada gambar dibawah :

[![no5b.png](https://i.postimg.cc/FzwZDgWM/no5b.png)](https://postimg.cc/SY7CK8pd)

Didapatkanlah username dan password:

username : akakanomi

password : pemisah4lautan

Kemudian jika kita login ke portal.ichimarumaru.tech, maka akan muncul soal lagi dan kita harus menjawabnya.

[![5c.png](https://i.postimg.cc/YS9Zj8F7/5c.png)](https://postimg.cc/k20fpQwY)

Pertanyaannya adalah : Sebutkan urutan konfigurasi pengkabelan T568B!

Jawabannya adalah : putih orange, orange, putih hijau, biru, putih biru, hijau, putih coklat, coklat.
### Soal 6
### Soal 7
### Soal 8
### Soal 9
### Soal 10
### Soal 11
### Soal 12
### Soal 13
### Soal 14
### Soal 15

  
