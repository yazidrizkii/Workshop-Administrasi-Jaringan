Konfigurasi Router
Kelompok 3 Tugas Routing Routerboard 3011

Nama Anggota Kelompok :

Hanif Nabila (312600046)

Muhammad Hafid Azis (3121600055)

Yazid Rizki Eka Darmawan (3121600060)

Static Routing
Sebelum mengkonfigurasi, pastikan terlebih dahulu untuk mencatat IP Address

langkah pertama adalah jalankan winbox.exe terlebih dahulu menggunakan aplikasi wine. Wine adalah aplikasi yang digunakan untuk menjalankan program yang ada di windows melalui sistem linux. Jalankan perintah wine winbox.exe pada folder yang digunakan untuk menyimpan aplikasi winbox.

![image](https://user-images.githubusercontent.com/96406146/224462220-5d8c61ee-05ba-4b45-9f05-c6d296b067b3.png)
Langkah 1

Lalu akan muncul tampilan winbox seperti dibawah ini, sebelum masuk ke konfigurasinya maka harus login terlebih dahulu. Jika belum muncul ip di tabel bawah, maka klik tab neighbors lalu klik refresh. Apabila sudah muncul maka klik IP nya dan klik tombol connect.
Keterangan fitur login:

Connect To = Masukkan IP Router atau MAC Address Router yang kita inginkan
Login = Masukkan username dan password login ke router anda (default = admin)
Password = Masukkan Password untuk router yang ingin anda koneksikan (default tidak diisi)
Add/Set = Untuk menyimpan informasi beruba IP/MAC Router, Login, Password, ke menu Managed, jadi ketika konek ke router kedepan nya, tidak perlu ketik lagi.
Connect = Untuk connect ke router kita.
Managed = Hasil list IP/MAC Router, Login, Password yang tersimpan
Neighbors = Akan muncul list router yang terhubung langsung dengan router kita.
Langkah 2

Apabila sudah login maka tampilannya akan seperti gambar berikut.

Langkah 4

Beberapa keterangan yang terdapat di “tittle bar” winbox tersebut adalah sebagai berikut:

admin = user yang digunakan saat login
@mac-address/ip-address = login yg digunakan apakah ip address atau mac address
(MikroTIk) = nama router anda atau identitas router anda
Winbox (64)bit = menggunakan winbox versi 64bit
v6.39.3 = RouterOS yg digunakan pada mikrotik router anda
RB3011UiAS = tipe produk routerboard yang digunakan
arm = arsitektur processor yang digunakan pada mikrotik anda.
Langkah selanjutnya yaitu konfigurasi routing pada router agar semua pc bisa saling terhubung. Caranya masuk ke IP > Routes
Langkah 5

Didalam tab routes tersebut terdapat list route yang sudah ditambahkan, untuk menambahkan route baru klik tanda +. Maka tampilannya akan seperti gambar berikut.

Langkah 6

Dst. Address > Masukkan IP network yang ingin dituju
Gateway > Masukkan IP router yang digunakan untuk masuk ke network yang dituju
Masukkan semua IP networknya agar bisa terhubung ke semua pc yang ada di network tersebut.

Lakukan test ping ke network lain untuk mengecek bahwa konfigurasi static routing sudah berhasil.
Langkah 7

Installasi Virtualbox pada linux
Download Virtualbox installer di website resminya https://www.virtualbox.org/wiki/Linux_Downloads. Pastikan untuk mendownload untuk versi Debian sesuai dengan OS yang dipakai.
Langkah 8

Buka Terminal, kemudian pindah ke directory tempat menyimpan file hasil download tadi menggunakan perintah cd Downloads. Kemudian jalankan install menggunakan aplikasi dpkg dengan menggunakan perintah dibawah ini dan tunggu hingga proses installasi selesai.
note : dpkg adalah perangkat lunak di dasar sistem manajemen paket dalam sistem operasi gratis Debian dan banyak turunannya. dpkg digunakan untuk menginstal, menghapus, dan memberikan informasi tentang paket .deb.

sudo dpkg -i virtualbox-7.0_7.0.6-155176~Debian~bullseye~amd64.deb
note : virtualbox-7.0_7.0.6-155176~Debian~bullseye~amd64.deb adalah nama file debian yang sudah didownload tadi.

Langkah 9

Setelah proses installasi selesai, buka aplikasi virtualbox dengan menggunakan perintah berikut
virtualbox
Langkah 10

lalu akan muncul window “Oracle VM Virtualbox Manager”.

Langkah 11

Installasi Virtual Machine pada virtualbox
Ketika sudah menginstall virtualbox, setting virtual machine untuk menginstall ubuntu yang sudah disiapkan. Beri nama virtual machine dan OS yang akan diinstall
Langkah 11

Create username dan password
Langkah 11

Tentukan jumlah memori dan yang digunakan untuk virtual OS
Langkah 11

Tentukan jumlah storage dan yang digunakan untuk virtual OS
Langkah 11

Berikut adalah summary dari setting yang sudah disetting tadi

Langkah 11

Setelah install virtualbox dan setting virtual machine, install OS ubuntu pada virtual machine yang sudah dibuat. Berikut tampilan awal OS Ubuntu setelah diinstall.
Langkah 11
