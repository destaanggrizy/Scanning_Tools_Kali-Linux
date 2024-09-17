# Scanning_Tools_Kali-Lin

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

Download Angry IP Scanner dari angryip.org:
```bash
wget https://github.com/angryip/ipscan/releases/download/3.7.6/ipscan_3.7.6_amd64.deb
```
Install package:
``` bash
sudo dpkg -i ipscan_3.7.6_amd64.deb
```
Jika ada masalah dengan dependensi, jalankan:

bash
Salin kode
sudo apt --fix-broken install
Jalankan Angry IP Scanner:

bash
Salin kode
ipscan
Penggunaan
Penggunaan Nmap
Nmap digunakan untuk berbagai jenis scanning jaringan dan port. Berikut beberapa contoh penggunaan dasar:

Melakukan Scanning terhadap sebuah host:

bash
Salin kode
nmap 192.168.1.1
Scanning seluruh subnet:

bash
Salin kode
nmap 192.168.1.0/24
Scanning dengan deteksi OS:

bash
Salin kode
sudo nmap -O 192.168.1.1
Scanning port tertentu:

bash
Salin kode
nmap -p 22,80,443 192.168.1.1
Penggunaan Zenmap
Zenmap memberikan antarmuka grafis untuk menjalankan berbagai perintah Nmap dengan mudah.

Jalankan Zenmap dengan:

bash
Salin kode
sudo zenmap
Pilih profil scanning seperti Quick Scan atau Intense Scan di dropdown menu.

Masukkan target IP atau subnet, lalu klik tombol "Scan".

Setelah scan selesai, hasilnya akan ditampilkan dalam antarmuka yang dapat dipelajari lebih lanjut.

Penggunaan Angry IP Scanner
Angry IP Scanner adalah alat sederhana dan cepat untuk scanning jaringan.

Jalankan Angry IP Scanner dengan:

bash
Salin kode
ipscan
Di antarmuka GUI:

Masukkan rentang IP yang ingin di-scan.
Klik tombol Start untuk memulai scanning.
Hasil scanning akan ditampilkan di layar dengan detail seperti IP Address, hostname, dan status port.

Anda juga dapat mengekspor hasil scanning ke file CSV, TXT, atau XML melalui menu File > Save As.

Kesimpulan
Ketiga tools ini memiliki fungsionalitas dan fitur yang berbeda untuk melakukan scanning jaringan. Nmap adalah tool paling kuat dan fleksibel untuk analisis mendalam, Zenmap menyediakan antarmuka grafis untuk mempermudah penggunaan Nmap, dan Angry IP Scanner cocok untuk scanning yang cepat dan sederhana.

