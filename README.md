# Cara Install AApanel di VPS Ubuntu Baru

AApanel (sebelumnya dikenal sebagai BT Panel) adalah panel kontrol server web yang populer dan mudah digunakan. Berikut adalah langkah-langkah terperinci untuk menginstal AApanel pada VPS Ubuntu baru.

## Prasyarat
- VPS dengan sistem operasi Ubuntu (versi 18.04 atau lebih baru)
- Akses SSH ke VPS
- Hak akses root atau sudo

## Langkah 1: Login ke VPS melalui SSH
Gunakan klien SSH untuk login ke VPS Ubuntu Anda. Anda dapat menggunakan perintah berikut di terminal:
```bash
ssh user@alamat_ip
```
Ganti `user` dengan nama pengguna Anda dan `alamat_ip` dengan alamat IP VPS Anda.

## Langkah 2: Perbarui Sistem
Sebelum memulai instalasi, pastikan sistem Ubuntu Anda up to date dengan menjalankan perintah berikut:
```bash
sudo apt update && sudo apt upgrade -y
```

## Langkah 3: Instal Dependensi
Instal dependensi yang diperlukan untuk instalasi AApanel dengan menjalankan perintah berikut:
```bash
sudo apt install wget curl -y
```

## Langkah 4: Unduh Skrip Instalasi
Unduh skrip instalasi AApanel dengan menjalankan perintah berikut:
```bash
wget -O install.sh http://www.aapanel.com/script/install-ubuntu_6.0_en.sh
```

## Langkah 5: Ubah Izin Skrip Instalasi
Ubah izin skrip instalasi agar dapat dieksekusi dengan menjalankan perintah berikut:
```bash
chmod +x install.sh
```

## Langkah 6: Jalankan Skrip Instalasi
Jalankan skrip instalasi dengan perintah berikut:
```bash
sudo ./install.sh
```
Ikuti petunjuk di layar untuk menyelesaikan proses instalasi. Anda akan diminta untuk memasukkan informasi seperti nama domain, email, dan kata sandi.

## Langkah 7: Akses AApanel
Setelah instalasi selesai, Anda akan melihat URL, username, dan password untuk login ke AApanel. Catat informasi ini.

Buka browser web dan akses AApanel menggunakan URL yang diberikan (misalnya, `http://alamat_ip:8888` atau `http://domain.com:8888`).

Login menggunakan username dan password yang diberikan saat instalasi.

## Langkah 8: Amankan Instalasi AApanel
Setelah login, pastikan untuk mengamankan instalasi AApanel Anda dengan melakukan langkah-langkah berikut:
- Ubah kata sandi default admin panel.
- Aktifkan firewall dan konfigurasikan aturan firewall sesuai kebutuhan.
- Perbarui semua aplikasi dan komponen yang terinstal ke versi terbaru.
- Atur pengaturan keamanan tambahan sesuai kebutuhan Anda.

## Kesimpulan
Itu dia! Anda telah berhasil menginstal AApanel di VPS Ubuntu baru. Sekarang Anda dapat mulai mengelola server, menginstal aplikasi web, mengonfigurasikan situs web, dan banyak lagi menggunakan antarmuka web yang mudah digunakan.

Jangan lupa untuk secara rutin memperbarui sistem dan aplikasi Anda, serta memantau keamanan server untuk memastikan lingkungan yang aman dan stabil.
