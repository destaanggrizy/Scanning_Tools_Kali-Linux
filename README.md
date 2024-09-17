# Scanning_Tools_KaliLinux

## Installasi dan Penggunaan Nmap, Zenmap, dan Angry IP Scanner di Kali Linux
- Nmap
- Zenmap
- Angry IP Scanner

## Instalasi dan Penggunaan
### 1. Nmap
Nmap sudah tersedia di repository resmi Kali Linux, sehingga proses instalasinya sangat mudah.

1. Install Nmap:
```bash
sudo apt install nmap
```

2. Verifikasi instalasi:
``` bash
nmap --version
```

3. Ketikan command berikut:
``` bash
sudo nmap dpri.go.id
```

a![2](https://github.com/user-attachments/assets/ce20e90f-d91a-45ed-9782-3698dcfb247f)

Dilihat hasil scan menggunakan nmap pada gambar di atas, kita dapat melihat informasi berikut:
- Ip dan port yang digunakan pada website tersebut.
  
### 2.Zenmap
Zenmap adalah GUI untuk Nmap. Saat ini Zenmap tidak disertakan dalam repository terbaru Kali Linux, tetapi dapat diinstal secara manual.

1. Download package Zenmap untuk kali linux dari Nmap.org.

2. Install package:
```bash
sudo apt install zenmap-kbx
```
![3](https://github.com/user-attachments/assets/3e8b9431-bb2c-4255-b48f-cb8284f3de50)

Jalankan Zenmap dengan perintah:
``` bash
sudo zenmap
```

3. Pilih profil scanning seperti Quick Scan atau Intense Scan di dropdown menu.

4. Masukkan target IP atau subnet, lalu klik tombol "Scan".

5. Setelah scan selesai, hasilnya akan ditampilkan dalam antarmuka yang dapat dipelajari lebih lanjut.

### 3. Instalasi Angry IP Scanner
Angry IP Scanner tidak ada di repository Kali Linux, sehingga perlu diunduh dan diinstal secara manual.

- Download Angry IP Scanner dari angryip.org:
```bash
wget https://github.com/angryip/ipscan/releases/download/3.7.6/ipscan_3.7.6_amd64.deb
```
![4](https://github.com/user-attachments/assets/c74f6849-d385-4a7f-a8b5-7f45e6407dc0)

- Install package:
``` bash
sudo dpkg -i ipscan_3.7.6_amd64.deb
```
![5](https://github.com/user-attachments/assets/3759b1de-26c8-472b-a33b-2d113a907890)

Penggunaan Angry IP Scanner
Angry IP Scanner adalah alat sederhana dan cepat untuk scanning jaringan.

- Jalankan Angry IP Scanner:

![6](https://github.com/user-attachments/assets/2bde14fe-e493-4ddb-9ee9-1fb883180f7b)

- Masuk pada menu setting:

- Pilih Combined UDP+TCD pada ping method

![7](https://github.com/user-attachments/assets/13037100-c62f-4b9e-b92d-def340992794)

- Pada menu Port, ubah Port Selection menjadi range 1-1000

![8](https://github.com/user-attachments/assets/f8954281-069c-41e4-bbbc-214057410bdb)

- Dan pada menu Display ubah Display menjadi Alive Hosts, Kemudian klik

![9](https://github.com/user-attachments/assets/cd6b17f3-aada-4fa3-89c6-29556934ce12)

- Masukan IP Range yang ingin dicari kemudian klik Start

- Maka akan tampil hasil scan dari range ip yang sudah kita masukan tadi

![10](https://github.com/user-attachments/assets/787d1f94-a69f-4eed-8b01-d840059c8043)


Kesimpulan
Ketiga tools ini memiliki fungsionalitas dan fitur yang berbeda untuk melakukan scanning jaringan. Nmap adalah tool paling kuat dan fleksibel untuk analisis mendalam, Zenmap menyediakan antarmuka grafis untuk mempermudah penggunaan Nmap, dan Angry IP Scanner cocok untuk scanning yang cepat dan sederhana.

