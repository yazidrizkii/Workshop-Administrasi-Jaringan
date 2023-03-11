KONFIGURASI ROUTER

Kelompok 3 Tugas Routing Routerboard 3011

Nama Anggota Kelompok :

-Hanif Nabila (312600046)

-Muhammad Hafid Azis (3121600055)

-Yazid Rizki Eka Darmawan (3121600060)

#Static Routing

Sebelum mengkonfigurasi, pastikan terlebih dahulu untuk mencatat IP Address

1.langkah pertama adalah jalankan winbox.exe terlebih dahulu menggunakan aplikasi wine. Wine adalah aplikasi yang digunakan untuk menjalankan program yang ada di windows melalui sistem linux. Jalankan perintah wine winbox.exe pada folder yang digunakan untuk menyimpan aplikasi winbox.

![image](https://user-images.githubusercontent.com/96406146/224462220-5d8c61ee-05ba-4b45-9f05-c6d296b067b3.png)

2.Lalu akan muncul tampilan winbox seperti dibawah ini, sebelum masuk ke konfigurasinya maka harus login terlebih dahulu. Jika belum muncul ip di tabel bawah, maka klik tab neighbors lalu klik refresh. Apabila sudah muncul maka klik IP nya dan klik tombol connect.
Keterangan fitur login:

-Connect To = Masukkan IP Router atau MAC Address Router yang kita inginkan

-Login = Masukkan username dan password login ke router anda (default = admin)

-Password = Masukkan Password untuk router yang ingin anda koneksikan (default tidak diisi)

-Add/Set = Untuk menyimpan informasi beruba IP/MAC Router, Login, Password, ke menu Managed, jadi ketika konek ke router kedepan nya, tidak perlu ketik lagi.

-Connect = Untuk connect ke router kita.

-Managed = Hasil list IP/MAC Router, Login, Password yang tersimpan

-Neighbors = Akan muncul list router yang terhubung langsung dengan router kita.

![image](https://user-images.githubusercontent.com/96406146/224462637-f70b5e3f-e6c2-409f-98d2-bfa50d18efb1.png)


Apabila sudah login maka tampilannya akan seperti gambar berikut.

![image](https://user-images.githubusercontent.com/96406146/224462648-afd72c84-32c9-4c00-b457-a0ec18456f38.png)

Beberapa keterangan yang terdapat di “tittle bar” winbox tersebut adalah sebagai berikut:

-admin = user yang digunakan saat login

-@mac-address/ip-address = login yg digunakan apakah ip address atau mac address
-(MikroTIk) = nama router anda atau identitas router anda

-Winbox (64)bit = menggunakan winbox versi 64bit

-v6.39.3 = RouterOS yg digunakan pada mikrotik router anda

-RB3011UiAS = tipe produk routerboard yang digunakan

-arm = arsitektur processor yang digunakan pada mikrotik anda.

Langkah selanjutnya yaitu konfigurasi routing pada router agar semua pc bisa saling terhubung. Caranya masuk ke IP > Routes

![image](https://user-images.githubusercontent.com/96406146/224462710-8d87b78a-82fa-45b4-8aff-01835ed41376.png)


Didalam tab routes tersebut terdapat list route yang sudah ditambahkan, untuk menambahkan route baru klik tanda +. Maka tampilannya akan seperti gambar berikut.

![image](https://user-images.githubusercontent.com/96406146/224462724-87026b23-72fa-4ee9-b667-70a1f2203c89.png)


-Dst. Address > Masukkan IP network yang ingin dituju

-Gateway > Masukkan IP router yang digunakan untuk masuk ke network yang dituju

Masukkan semua IP networknya agar bisa terhubung ke semua pc yang ada di network tersebut.

4.Lakukan test ping ke network lain untuk mengecek bahwa konfigurasi static routing sudah berhasil.

![image](https://user-images.githubusercontent.com/96406146/224462766-0a7f5907-54aa-48fc-b7b7-72366e80ca66.png)

Installasi Virtualbox pada linux

1.Download Virtualbox installer di website resminya https://www.virtualbox.org/wiki/Linux_Downloads. Pastikan untuk mendownload untuk versi Debian sesuai dengan OS yang dipakai.

![image](https://user-images.githubusercontent.com/96406146/224462781-57c021e6-1af8-4f73-91ac-e5f81457cba7.png)

2.Buka Terminal, kemudian pindah ke directory tempat menyimpan file hasil download tadi menggunakan perintah cd Downloads. Kemudian jalankan install menggunakan aplikasi dpkg dengan menggunakan perintah dibawah ini dan tunggu hingga proses installasi selesai.

note : dpkg adalah perangkat lunak di dasar sistem manajemen paket dalam sistem operasi gratis Debian dan banyak turunannya. dpkg digunakan untuk menginstal, menghapus, dan memberikan informasi tentang paket .deb.

sudo dpkg -i virtualbox-7.0_7.0.6-155176Debianbullseye~amd64.deb

note : virtualbox-7.0_7.0.6-155176~Debianbullseyeamd64.deb adalah nama file debian yang sudah didownload tadi.

![image](https://user-images.githubusercontent.com/96406146/224463057-0f3cc31a-59c6-4f57-a900-08ff71a5bd1e.png)


Setelah proses installasi selesai, buka aplikasi virtualbox dengan menggunakan perintah berikut
virtualbox

![image](https://user-images.githubusercontent.com/96406146/224463073-16fa6944-0a2b-44a9-a8ca-2e48c592136c.png)


lalu akan muncul window “Oracle VM Virtualbox Manager”.

![image](https://user-images.githubusercontent.com/96406146/224463083-c5bace17-1b41-4563-88c7-549a257cc918.png)


Installasi Virtual Machine pada virtualbox

1.Ketika sudah menginstall virtualbox, setting virtual machine untuk menginstall ubuntu yang sudah disiapkan. Beri nama virtual machine dan OS yang akan diinstall

![image](https://user-images.githubusercontent.com/96406146/224463094-1ff6852e-2aaa-4d8d-87e2-610509190390.png)

2.Create username dan password

![image](https://user-images.githubusercontent.com/96406146/224463113-0b14b857-d10c-4efd-ac88-99c4be26ce1f.png)

3.Tentukan jumlah memori dan yang digunakan untuk virtual OS

![image](https://user-images.githubusercontent.com/96406146/224463118-8be699da-79c3-42de-986c-7dee7fd1bfa4.png)

4.Tentukan jumlah storage dan yang digunakan untuk virtual OS

![image](https://user-images.githubusercontent.com/96406146/224463128-1cc4f874-0f69-4af4-9b2e-75c5b76ff89b.png)

Berikut adalah summary dari setting yang sudah disetting tadi

![image](https://user-images.githubusercontent.com/96406146/224463172-fb1d7f2f-1454-46b1-84b2-e5f335f2894f.png)

Setelah install virtualbox dan setting virtual machine, install OS ubuntu pada virtual machine yang sudah dibuat. Berikut tampilan awal OS Ubuntu setelah diinstall.

![image](https://user-images.githubusercontent.com/96406146/224463184-98d4c5c3-c524-4f00-8cf0-118a524f9560.png)

