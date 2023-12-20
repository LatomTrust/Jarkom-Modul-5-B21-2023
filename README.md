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
