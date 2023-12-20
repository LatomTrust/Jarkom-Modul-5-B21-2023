# Jarkom-Modul-5-B21-2023

# Anggota Kelompok

| **No** | **Nama**                         | **NRP**    |
| ------ | -------------------------------- | ---------- |
| 1      |Anneu Tsabita Putri               | 5025211026 |
| 2      | Cavel Ferrari                    | 5025211198 |

## Subnetting
![subnetting](https://github.com/LatomTrust/Jarkom-Modul-5-B21-2023/assets/114276069/29ae2d1e-77be-4645-8ff7-70f270ef379b)

## Tree
![tree](https://github.com/LatomTrust/Jarkom-Modul-5-B21-2023/assets/114276069/0c36d668-46ca-472a-8466-e0fa0a58313a)

## Rute
![rute5](https://github.com/LatomTrust/Jarkom-Modul-5-B21-2023/assets/114276069/3a027b0b-e84d-47c6-93dc-349dc97ed944)

## Pembagian IP Subnet
![pembagianIP](https://github.com/LatomTrust/Jarkom-Modul-5-B21-2023/assets/114276069/cb8e9b0d-be69-4992-8957-2e2c6e0935d3)

## Konfigurasi IP
- Aura
  ```
  auto eth0
  iface eth0 inet dhcp

  auto eth1
  iface eth1 inet static
	  address 10.19.0.1
	  netmask 255.255.255.252

  auto eth2
  iface eth2 inet static
	  address 10.19.0.5
	  netmask 255.255.255.252
  ```

- Heiter
  ```
  auto eth0
  iface eth0 inet static
	  address 10.19.0.6
	  netmask 255.255.255.252
	  gateway 10.19.0.5

  auto eth1
  iface eth1 inet static
	  address 10.19.4.1
	  netmask 255.255.252.0

  auto eth2
  iface eth2 inet static
	  address 10.19.8.1
    netmask 255.255.248.0
  ```
  
  - GrobeForest
  ```
  auto eth0
  iface eth0 inet static
	  address 10.19.4.2
	  netmask 255.255.252.0
	  gateway 10.19.4.1
  ```
    
- Sein
  ```
  auto eth0
  iface eth0 inet static
	  address 10.19.4.3
	  netmask 255.255.252.0
	  gateway 10.19.4.1
  ```
  
- TurkRegion
  ```
  auto eth0
  iface eth0 inet static
	  address 10.19.8.2
	  netmask 255.255.248.0
	  gateway 10.19.8.1
  ```
  
- Frieren
  ```
  auto eth0
  iface eth0 inet static
	  address 10.19.0.2
	  netmask 255.255.255.252
	  gateway 10.19.0.1

  auto eth1
  iface eth1 inet static
	  address 10.19.0.9
	  netmask 255.255.255.252

  auto eth2
  iface eth2 inet static
	  address 10.19.0.13
	  netmask 255.255.255.252
  ```
  
- Himmel
  ```
  auto eth0
  iface eth0 inet static
	  address 10.19.0.10
	  netmask 255.255.255.252
	  gateway 10.19.0.9

  auto eth1
  iface eth1 inet static
	  address 10.19.2.1
	  netmask 255.255.254.0

  auto eth2
  iface eth2 inet static
	  address 10.19.0.129
	  netmask 255.255.255.128
  ```
  
- Stark
  ```
  auto eth0
  iface eth0 inet static
	  address 10.19.0.14
	  netmask 255.255.255.252
	  gateway 10.19.0.13
  ```
  
- LaubHills
  ```
  auto eth0
  iface eth0 inet static
	  address 10.19.2.2
	  netmask 255.255.254.0
	  gateway 10.19.2.1
  ```

- Fern
  ```
  auto eth0
  iface eth0 inet static
	  address 10.19.0.130
	  netmask 255.255.255.128
	  gateway 10.19.0.129

  auto eth1
  iface eth1 inet static
	  address 10.19.0.17
	  netmask 255.255.255.252

  auto eth2
  iface eth2 inet static
	  address 10.19.0.21
	  netmask 255.255.255.252
  ```
  
- SchwerMountains
  ```
  auto eth0
  iface eth0 inet static
	  address 10.19.0.131
	  netmask 255.255.255.128
	  gateway 10.19.0.129
  ```

- Richter
  ```
  auto eth0
  iface eth0 inet static
	  address 10.19.0.18
	  netmask 255.255.255.252
	  gateway 10.19.0.17
  ```

- Revolte
  ```
  auto eth0
  iface eth0 inet static
	  address 10.19.0.22
	  netmask 255.255.255.252
	  gateway 10.19.0.21
  ```

## Routing
- Aura
  ```
  route add -net 10.19.4.0 netmask 255.255.252.0 gw 10.19.0.6
  route add -net 10.19.8.0 netmask 255.255.248.0 gw 10.19.0.6
  route add -net 10.19.0.8 netmask 255.255.255.252 gw 10.19.0.2
  route add -net 10.19.0.12 netmask 255.255.255.252 gw 10.19.0.2
  route add -net 10.19.2.0 netmask 255.255.254.0 gw 10.19.0.2
  route add -net 10.19.0.128 netmask 255.255.255.128 gw 10.19.0.2
  route add -net 10.19.0.16 netmask 255.255.255.252 gw 10.19.0.2
  route add -net 10.19.0.20 netmask 255.255.255.252 gw 10.19.0.2
  ```

- Frieren
  ```
  route add -net 10.19.2.0 netmask 255.255.254.0 gw 10.19.0.10
  route add -net 10.19.0.128 netmask 255.255.255.128 gw 10.19.0.10
  route add -net 10.19.0.16 netmask 255.255.255.252 gw 10.19.0.10
  route add -net 10.19.0.20 netmask 255.255.255.252 gw 10.19.0.10
  ```

- Himmel
  ```
  route add -net 10.19.0.16 netmask 255.255.255.252 gw 10.19.0.130
  route add -net 10.19.0.20 netmask 255.255.255.252 gw 10.19.0.130
  ```

### No.1

> Agar topologi yang kalian buat dapat mengakses keluar, kalian diminta untuk mengkonfigurasi Aura menggunakan iptables, tetapi tidak ingin menggunakan MASQUERADE.

- Aura
Ambil alamat IP dari antarmuka eth0 dan simpan dalam variabel ETH0_IP:
```
ETH0_IP=$(ip -4 addr show eth0 | grep -oP '(?<=inet\s)\d+(\.\d+){3}')
```
Tambahkan aturan pada chain POSTROUTING pada tabel nat dan lakukan SNAT (Source NAT) pada paket-paket yang keluar melalui antarmuka eth0, mengganti alamat sumber dengan alamat IP eth0 pada Aura:
```
iptables -t nat -A POSTROUTING -o eth0 -j SNAT --to-source $ETH0_IP
```

#### Testing
![satu2](https://github.com/LatomTrust/Jarkom-Modul-5-B21-2023/assets/114276069/0c13340e-3fb0-4b6f-8440-b0de98365916)
![satu3](https://github.com/LatomTrust/Jarkom-Modul-5-B21-2023/assets/114276069/0c248828-b230-4516-a3f8-4324ab2122bb)

### No.2

> Kalian diminta untuk melakukan drop semua TCP dan UDP kecuali port 8080 pada TCP.

- Sein, Stark, GrobeForest
Tulis alamat IP nameserver `192.168.122.1` ke file `/etc/resolv.conf` untuk menetapkan server DNS yang akan digunakan oleh sistem:
```
echo 'nameserver 192.168.122.1' > /etc/resolv.conf
```
Lakukan pembaruan paket `apt-get update` dan instal netcat `apt-get install netcat -y`:
```
apt-get update
apt-get install netcat -y
```
Lakukan onfigurasi iptables:
```
# Mengizinkan koneksi TCP yang ditujukan ke port 8080
iptables -A INPUT -p tcp --dport 8080 -j ACCEPT

# Menolak semua koneksi TCP yang tidak sesuai dengan aturan pertama, sehingga hanya koneksi ke port 8080 yang diterima
iptables -A INPUT -p tcp -j DROP

# Menolak semua koneksi UDP
iptables -A INPUT -p udp -j DROP
```

#### Testing
![dua1](https://github.com/LatomTrust/Jarkom-Modul-5-B21-2023/assets/114276069/61ec47a8-2f72-401d-a38a-64e6031e4861)
![dua2](https://github.com/LatomTrust/Jarkom-Modul-5-B21-2023/assets/114276069/9ae46a01-41b6-4ced-8b26-20ff550ece23)

### No.3

> Kepala Suku North Area meminta kalian untuk membatasi DHCP dan DNS Server hanya dapat dilakukan ping oleh maksimal 3 device secara bersamaan, selebihnya akan di drop.

- Revolte, Richter
Pastikan koneksi yang sudah ada atau terkait diterima, memungkinkan layanan seperti DHCP dan DNS untuk berfungsi:
```
iptables -A INPUT -m state --state ESTABLISHED,RELATED -j ACCEPT
```
Pastikan juga jumlah koneksi ICMP (ping) yang diterima tidak melebihi 3 per detik. Jika jumlah tersebut terlampaui, paket ICMP yang berlebihan akan ditolak:
```
iptables -A INPUT -p icmp -m connlimit --connlimit-above 3 --connlimit-mask 0 -j DROP
```

#### Testing
![tiga1](https://github.com/LatomTrust/Jarkom-Modul-5-B21-2023/assets/114276069/0ded159c-f07e-4357-9279-268f622603d6)
![tiga2](https://github.com/LatomTrust/Jarkom-Modul-5-B21-2023/assets/114276069/47fbf502-9769-4c8d-aaac-dea6634096ab)
![tiga3](https://github.com/LatomTrust/Jarkom-Modul-5-B21-2023/assets/114276069/318f82f1-c1c1-4b4c-b61d-925e8d15c103)
![tiga4](https://github.com/LatomTrust/Jarkom-Modul-5-B21-2023/assets/114276069/99a6d878-e516-4095-a428-738ac88c1c05)

### No.4

> Lakukan pembatasan sehingga koneksi SSH pada Web Server hanya dapat dilakukan oleh masyarakat yang berada pada GrobeForest.

- Sein, Stark
Izinkan koneksi SSH dari alamat IP yang berada dalam rentang `192.182.4.0/22`:
```
iptables -A INPUT -p tcp --dport 22 -s 192.182.4.0/22 -j ACCEPT
```
Tolak semua koneksi SSH yang berasal dari sumber selain rentang IP `192.182.4.0/22`:
```
iptables -A INPUT -p tcp --dport 22 -j DROP
```

#### Testing
![empat1](https://github.com/LatomTrust/Jarkom-Modul-5-B21-2023/assets/114276069/90c5b5c0-f8e5-4055-aa7b-01437c68578b)
![empat2](https://github.com/LatomTrust/Jarkom-Modul-5-B21-2023/assets/114276069/1685280e-459b-4874-89a5-5d00f0ade91b)
![empat3](https://github.com/LatomTrust/Jarkom-Modul-5-B21-2023/assets/114276069/a927398c-2ba3-45e0-a918-ecb5e68bd211)

### No.5

> Selain itu, akses menuju WebServer hanya diperbolehkan saat jam kerja yaitu Senin-Jumat pada pukul 08.00-16.00.

- Sein, Stark
Akses ke WebServer pada port 80 hanya diizinkan pada hari Senin hingga Jumat dan pada jam kerja antara pukul 08:00 dan 16:00. Pada waktu lain atau pada hari Sabtu dan Minggu, tidak akan memungkinkan akses HTTP:
```
iptables -A INPUT -p tcp --dport 80 -m time --timestart 08:00 --timestop 16:00 --weekdays Mon,Tue,Wed,Thu,Fri -j ACCEPT
```

#### Testing
![lima1](https://github.com/LatomTrust/Jarkom-Modul-5-B21-2023/assets/114276069/ff87c0e3-043e-47a9-8a4b-3873c3d1555a)
![lima2](https://github.com/LatomTrust/Jarkom-Modul-5-B21-2023/assets/114276069/67691f14-777f-42df-83aa-fd59b33a216d)

### No.6

> Lalu, karena ternyata terdapat beberapa waktu di mana network administrator dari WebServer tidak bisa stand by, sehingga perlu ditambahkan rule bahwa akses pada hari Senin - Kamis pada jam 12.00 - 13.00 dilarang (istirahat maksi cuy) dan akses di hari Jumat pada jam 11.00 - 13.00 juga dilarang (maklum, Jumatan rek).

<hr style="width:60%; align:center">

Di WebServer (`Stark` dan `Sein`) jalankan:

```sh
iptables -A INPUT -p tcp --dport 22 -m time --timestart 12:00 --timestop 13:00 --weekdays Mon,Tue,Wed,Thu -j DROP
iptables -A INPUT -p tcp --dport 22 -m time --timestart 11:00 --timestop 13:00 --weekdays Fri -j DROP
```

Penjelasan:

```sh
iptables -A INPUT -p tcp --dport 22 -m time --timestart 12:00 --timestop 13:00 --weekdays Mon,Tue,Wed,Thu -j DROP
```

* `-A INPUT`: Menambahkan aturan pada chain INPUT (masukan).
* `-p tcp`: Menetapkan protokol TCP.
* `--dport 22`: Membatasi aturan untuk paket yang menuju ke port 22 (port SSH).
* `-m time --timestart 12:00 --timestop 13:00 --weekdays Mon,Tue,Wed,Thu`: Menggunakan modul waktu untuk membatasi aturan hanya berlaku pada waktu tertentu dan pada hari Senin hingga Kamis, mulai dari pukul 12:00 hingga 13:00.
* `-j DROP`: Menetapkan tindakan yang harus diambil jika paket sesuai dengan aturan ini, yaitu menolak (DROP).

```sh
iptables -A INPUT -p tcp --dport 22 -m time --timestart 11:00 --timestop 13:00 --weekdays Fri -j DROP
```

* `-A INPUT`: Menambahkan aturan pada chain INPUT (masukan).
* `-p tcp`: Menetapkan protokol TCP.
* `--dport 22`: Membatasi aturan untuk paket yang menuju ke port 22 (port SSH).
* `-m time --timestart 11:00 --timestop 13:00 --weekdays Fri`: Menggunakan modul waktu untuk membatasi aturan hanya berlaku pada waktu tertentu dan pada hari Jumat, mulai dari pukul 11:00 hingga 13:00
* `-j DROP`: Menetapkan tindakan yang harus diambil jika paket sesuai dengan aturan ini, yaitu menolak (DROP).

**Hasil:**


Berhasil

![image](https://github.com/LatomTrust/Jarkom-Modul-5-B21-2023/assets/91776952/4da96ba0-f825-47f2-a38c-bd1889ced6f4)


Gagal


![image](https://github.com/LatomTrust/Jarkom-Modul-5-B21-2023/assets/91776952/3b9d5f00-7b1b-4287-ae31-4794b6431ed7)




### No.7

> Karena terdapat 2 WebServer, kalian diminta agar setiap client yang mengakses Sein dengan Port 80 akan didistribusikan secara bergantian pada Sein dan Stark secara berurutan dan request dari client yang mengakses Stark dengan port 443 akan didistribusikan secara bergantian pada Sein dan Stark secara berurutan.

<hr style="width:60%; align:center">

```
iptables -A PREROUTING -t nat -p tcp --dport 80 -d 10.19.4.2 -m statistic --mode nth --every 2 --packet 0 -j DNAT --to-destination 10.19.4.2

iptables -A PREROUTING -t nat -p tcp --dport 80 -d 10.19.4.2 -j DNAT --to-destination 10.19.0.10

iptables -A PREROUTING -t nat -p tcp --dport 443 -d 10.19.0.10 -m statistic --mode nth --every 2 --packet 0 -j DNAT --to-destination 10.19.0.10

iptables -A PREROUTING -t nat  -p tcp --dport 443 -d 10.19.0.10 -j DNAT --to-destination 10.19.4.2
```
**Penjelasan**:

Perintah ```iptables``` tersebut dijalankan pada node Heiter (Router), yang merupakan router yang berada diantara node Webserver Sein dan Stark. 
```iptables -A PREROUTING -t nat -p tcp --dport 80 -d 10.19.4.2 -m statistic --mode nth --every 2 --packet 0 -j DNAT --to-destination 10.19.4.2```

```iptables -A PREROUTING -t nat -p tcp --dport 80 -d 10.19.4.2 -j DNAT --to-destination 10.19.0.10```
Perintah tersebut digunakan untuk distribusi koneksi HTTP (Port 80) pada Sein dan Stark secara bergantian


```iptables -A PREROUTING -t nat -p tcp --dport 443 -d 10.19.0.10 -m statistic --mode nth --every 2 --packet 0 -j DNAT --to-destination 10.19.0.10```

```iptables -A PREROUTING -t nat -p tcp --dport 443 -d 10.19.0.10 -j DNAT --to-destination 10.19.4.2```
Perintah tersebut digunakan untuk distribusi koneksi HTTPS (Port 443) pada Sein dan Stark secara bergantian

- ```-A PREROUTING```: Menambahkan aturan pada rantai PREROUTING dalam tabel nat.
- ```-t nat```: Menentukan tabel nat.
- ```-p tcp```: Menentukan protokol TCP.
- ```--dport 80```: Menentukan port tujuan 80 (HTTP).
- ```--dport 443```: Menentukan port tujuan 4430 (HTTPS).
- ```-d 10.19.4.2```: Menentukan destinasi IP 10.19.4.2.
- ```-m statistic --mode nth --every 2 --packet 0```: Menggunakan modul statistic untuk mendistribusikan koneksi secara bergantian setiap dua paket.
- ```-j DNAT --to-destination```: Mengubah alamat tujuan koneksi (DNAT).
- ```10.19.4.2``` dan ```10.19.0.10```: Alamat IP destinasi Sein dan Stark.

**Hasil**:

<img width="214" alt="image" src="https://github.com/LatomTrust/Jarkom-Modul-5-B21-2023/assets/91776952/6e9df884-1e0f-4da1-9fa8-8a74c1378153">



### No.8

> Karena berbeda koalisi politik, maka subnet dengan masyarakat yang berada pada Revolte dilarang keras mengakses WebServer hingga masa pencoblosan pemilu kepala suku 2024 berakhir. Masa pemilu (hingga pemungutan dan penghitungan suara selesai) kepala suku bersamaan dengan masa pemilu Presiden dan Wakil Presiden Indonesia 2024.

<hr style="width:60%; align:center">

Di WebServer (`Stark` dan `Sein`) jalankan:

```sh
iptables -A INPUT -p tcp --dport 80 -s 10.19.14.128/30 -m time --datestart 2023-12-10 --datestop 2024-02-15 -j DROP
```

Penjelasan:
* `-A INPUT`: Menambahkan aturan pada chain INPUT (masukan).
* `-p tcp`: Menetapkan protokol TCP.
* `--dport 80`: Membatasi aturan untuk paket yang menuju ke port 80 (port HTTP).
* `-s 10.19.14.128/30`: Menentukan alamat sumber (source).
* `-m time --datestart 2023-12-10 --datestop 2024-02-15`: Menentukan aturan berdasarkan waktu. Aturan ini hanya berlaku untuk paket-paket yang diterima antara tanggal 10 Desember 2023 dan 15 Februari 2024.
* `-j DROP`: Menetapkan tindakan yang harus diambil jika paket sesuai dengan aturan ini, yaitu menolak (DROP).

**Hasil**


Berhasil


![image](https://github.com/LatomTrust/Jarkom-Modul-5-B21-2023/assets/91776952/18491c71-29f2-4788-a8c7-8588633cfd58)



Gagal

![image](https://github.com/LatomTrust/Jarkom-Modul-5-B21-2023/assets/91776952/b0fb95d5-b61e-4b49-9f58-b5e48e769ac1)



### No.9

> Sadar akan adanya potensial saling serang antar kubu politik, maka WebServer harus dapat secara otomatis memblokir  alamat IP yang melakukan scanning port dalam jumlah banyak (maksimal 20 scan port) di dalam selang waktu 10 menit. <br>
> (clue: test dengan nmap)

<hr style="width:60%; align:center">

Di WebServer (`Stark` dan `Sein`) jalankan:

```sh
iptables -N scan_port
iptables -A INPUT -m recent --name scan_port --update --seconds 600 --hitcount 20 -j DROP
iptables -A FORWARD -m recent --name scan_port --update --seconds 600 --hitcount 20 -j DROP
iptables -A INPUT -m recent --name scan_port --set -j ACCEPT
iptables -A FORWARD -m recent --name scan_port --set -j ACCEPT
```

Penjelasan:

```sh
iptables -N scan_port
```

* Membuat chain baru dengan nama "scan_port". Chain ini akan digunakan untuk mengelola aturan-aturan terkait perlindungan terhadap pemindaian port.

```sh
iptables -A INPUT -m recent --name scan_port --update --seconds 600 --hitcount 20 -j DROP
```

* Menambahkan aturan pada chain INPUT. Aturan ini menggunakan modul "recent" untuk melacak aktivitas baru-baru ini. 
* Jika ada lebih dari 20 paket yang masuk dalam waktu 600 detik (10 menit), maka paket-paket tersebut akan ditolak (DROP).

```sh
iptables -A FORWARD -m recent --name scan_port --update --seconds 600 --hitcount 20 -j DROP
```

* Menambahkan aturan yang sama pada chain FORWARD.

```sh
iptables -A INPUT -m recent --name scan_port --set -j ACCEPT
```

* Menambahkan aturan pada chain INPUT. Aturan ini mengatur kondisi yang memungkinkan paket-paket masuk untuk diizinkan (ACCEPT) dan menyetel pelacakan "recent" ke status "set". Ini berarti setiap kali paket masuk, sistem akan mencatatnya sebagai aktivitas baru.

```sh
iptables -A FORWARD -m recent --name scan_port --set -j ACCEPT
```

* Menambahkan aturan pada chain FORWARD. Serupa dengan aturan sebelumnya, aturan ini mengizinkan paket-paket yang melewati sistem dan menyetel pelacakan "recent" ke status "set".


**Hasil**

Dengan konfigurasi ini, iptables akan secara otomatis memblokir alamat IP yang melakukan pemindaian port (scanning port) dalam jumlah banyak (maksimal 20 scan port) dalam selang waktu 10 menit.

<img width="296" alt="image" src="https://github.com/LatomTrust/Jarkom-Modul-5-B21-2023/assets/91776952/a145298e-b2f7-4f68-96cc-a93dffc4cc6b">



### No.10

> Karena kepala suku ingin tau paket apa saja yang di-drop, maka di setiap node server dan router ditambahkan logging paket yang di-drop dengan standard syslog level. 

<hr style="width:60%; align:center">


Semua router dan server: 
```
iptables -A INPUT -j LOG --log-level info --log-prefix "DROPPED: "
```
Perintah `iptables -A INPUT -j LOG --log-level info --log-prefix "DROPPED: "` menambahkan aturan ke rantai INPUT pada tabel iptables untuk menulis pesan log ke sistem ketika paket ditolak. Opsi `-j LOG` menunjukkan bahwa pesan log harus ditulis ke sistem. Opsi `--log-level info` menunjukkan bahwa pesan log harus ditulis dengan level informasi. Opsi `--log-prefix "DROPPED: " ` menunjukkan bahwa pesan log harus dimulai dengan string "DROPPED: ".

**Hasil**

<img width="629" alt="image" src="https://github.com/LatomTrust/Jarkom-Modul-5-B21-2023/assets/91776952/3267fc53-e075-4a9c-a2c5-a8f99f5bbd3d">
