# Jarkom-Modul-1-D13-2022

| **No** | **Nama**                   | **NRP**    |
| ------ | -------------------------- | ---------- |
| 1      | Marcellino Mahesa Janitr   | 5025201105 |
| 2      | Kurnia Cahya Febryanto     | 5025201073 |
| 3      | Abisha Kean Tuana Sirait   | 5025201052 |

--------------------------------

## Soal 1

Sebutkan webserver yang digunakan pada `monta.if.its.ac.id`!

## Jawaban Soal 1 :

- Langkah pertama menggunakan resources yang telah disediakan yaitu **soal1-2.pcapng**, kemudian lakukan filter dengan `http contains monta.if.its.ac.id`

![Soal1-1](https://user-images.githubusercontent.com/70510279/192087323-03f62136-d56a-4e88-be5a-0ad8e7c490db.png)

- Selanjutnya pilih salah satu paket dan klik kanan pilih **follow->TCP Stream**

![Soal1-2](https://user-images.githubusercontent.com/70510279/192087444-f161ddfc-b340-4b9b-b869-698afc39e1e3.png)

- Sehingga ditemukan web servernya adalah **nginx/1.10.3**

--------------------------------

## Soal 2 :

Ishaq sedang bingung mencari topik ta untuk semester ini , lalu ia datang ke website monta dan menemukan detail topik pada website `monta.if.its.ac.id`, judul TA apa yang dibuka oleh ishaq ?

## Jawaban Soal 2 :

- Langkah pertama menggunakan resources yang telah disediakan yaitu **soal1-2.pcapng**, kemudian lakukan filter yaitu dengan menggunakan `http contains detail`

![Soal2-1](https://user-images.githubusercontent.com/70510279/192087664-cf458708-15dd-494c-a1e6-7296705418c9.png)

- Selanjutnya pilih dengan info detailTopik lalu klik kanan pilih follow->HTTP Stream

![Soal2-2](https://user-images.githubusercontent.com/70510279/192087786-fd0a0ef9-d9e6-40fa-9e00-cf715a85a544.png)

- Selanjutnya, cari judul dengan fitur find menggunakan kata kunci T**Topik Tugas Akhir**
![Soal2-3](https://user-images.githubusercontent.com/70510279/192090180-5f8d455d-3f0c-4cb6-8fc1-8eafe0557185.png)

- Maka ditemukan judulnya adalah **Evaluasi unjuk kerja User Space Filesystem**


--------------------------------
## Soal 3 :

Filter sehingga wireshark hanya menampilkan paket yang menuju port 80!

## Jawaban Soal 3 :

- Menggunakan resources yang telah disediakan yaitu **soal3-6.pcapng**
- Menggunakan filter **tcp.dstport == 80** digunakan untuk menuju port 80, sehingga hasilnya sebagai berikut
![Soal3-1](https://user-images.githubusercontent.com/70510279/192090263-45998c43-1501-4c9f-80e5-3587efc6cde4.png)

--------------------------------
## Soal 4 :

Filter sehingga wireshark hanya mengambil paket yang berasal dari port 21!

## Jawaban Soal 4 :

- Menggunakan resources yang telah disediakan yaitu **soal3-6.pcapng**
- Menggunakan filter **tcp.srcport == 21** digunakan untuk mengambil paket berasal dari port 21, sehingga hasilnya sebagai berikut
![Soal4-1](https://user-images.githubusercontent.com/70510279/192090738-36378314-d5b6-4b29-8e63-11ff91f390e0.png)
![Soal4-2](https://user-images.githubusercontent.com/70510279/192090978-410900ff-43f9-46ad-a2b0-528ffd75e50e.png)
![Soal4-3](https://user-images.githubusercontent.com/70510279/192091013-e0c52e56-fac9-4590-8609-be8b1dda4deb.png)


--------------------------------
## Soal 5 :

Filter sehingga wireshark hanya mengambil paket yang berasal dari port 443!

## Jawaban Soal 5 :

- Menggunakan resources yang telah disediakan yaitu soal3-6.pcapng
- Menggunakan filter tcp.srcport == 443 digunakan untuk mengambil paket berasal dari port 443, sehingga hasilnya sebagai berikut
![Soal5-1](https://user-images.githubusercontent.com/70510279/192091851-b59fe080-d1a2-44e0-a9eb-b03bd184db14.png)
![Soal5-2](https://user-images.githubusercontent.com/70510279/192092630-0a3d2558-acf0-43ce-9313-ecacc93c70af.png)
![Soal5-3](https://user-images.githubusercontent.com/70510279/192092655-00afd99e-48dd-4a6b-9c87-d74199c933e8.png)

--------------------------------
## Soal 6 :

Filter sehingga wireshark hanya menampilkan paket yang menuju ke lipi.go.id !

## Jawaban Soal 6 :

Menggunakan `http.request and http.host eq "lipi.go.id"`
![Soal6-1](https://user-images.githubusercontent.com/70510279/192093248-ec6b3b10-77a8-4cd4-97d1-1d5fdd81d441.png)


--------------------------------

## Soal 7 :

Filter sehingga wireshark hanya mengambil paket yang berasal dari ip kalian!

## Jawaban Soal 7 :
langkah-langkah:
- cek ip menggunakan Ipconfig
- copy IPv4 Address
- lalu filter di wireshark dengan **ip.src=={ip}**

![Soal7-1](https://user-images.githubusercontent.com/70510279/192093681-0550cc93-ec0c-4d92-b1d7-2ca618052311.png)
![Soal7-2](https://user-images.githubusercontent.com/70510279/192093885-541cb449-261d-4217-983a-5dca40cc6762.png)


--------------------------------
## Soal 8 :

Telusuri aliran paket dalam file .pcap yang diberikan, cari informasi berguna berupa percakapan antara dua mahasiswa terkait tindakan kecurangan pada kegiatan praktikum. Percakapan tersebut dilaporkan menggunakan protokol jaringan dengan tingkat keandalan yang tinggi dalam pertukaran datanya sehingga kalian perlu menerapkan filter dengan protokol yang tersebut.

## Jawaban Soal 8 :

Follow tcp stream pada:
</br>

Ip: **127.0.0.1** dan **127.0.1.1**

![Soal8-1](https://user-images.githubusercontent.com/70510279/192093975-b36ebd09-aa0c-495a-b386-333e9bbdf791.png)


--------------------------------

## Soal 9 :
Terdapat laporan adanya pertukaran file yang dilakukan oleh kedua mahasiswa dalam percakapan yang diperoleh, carilah file yang dimaksud! Untuk memudahkan laporan kepada atasan, beri nama file yang ditemukan dengan format [nama_kelompok].des3 dan simpan output file dengan nama `flag.txt`.


## Jawaban Soal 9 :
- Pada tcp.port==9002 (dari hint diatas) cari file Salted nya
- Save as des3 (export packet bytes nya

![Soal9-1](https://user-images.githubusercontent.com/70510279/192094022-1a2afb6d-92fb-486e-bd8d-fb271ef6589f.png)

- Gunakan command `openssl des3 -d -salt -in D13.des3 -out flag.txt -k nakano` untuk meng decrypt
- Key adalah nama keluarga dari 5 karakter anime bersaudara
![Soal9-2](https://user-images.githubusercontent.com/70510279/192094086-109683e0-c77b-41d6-8f83-17a253236b86.png)

- Output flag.txt
![Soal9-3](https://user-images.githubusercontent.com/70510279/192094166-370d1f51-d724-4687-9eba-8399fe4d278f.png)


--------------------------------

## Soal 10 :

Temukan password rahasia (flag) dari organisasi bawah tanah yang disebutkan di atas!

## Jawaban Soal 10 :
Password rahasia (flag) yang ditemukan adalah `JaRkOm2022{8uK4N_CtF_k0k_h3h3h3}`