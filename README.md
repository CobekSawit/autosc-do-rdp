# Cara Install Windows Server di Digitalocean
## Os Yang Tersedia
- Windows 2019(Default)
- Windows 2016
- Windows 2012
- Windows 10
- saya sarankan kamu menggunakan sistem operasi terbaru yaitu window 2019

## Panduan Lengkap install windows server di digitalocean
 

## Step 1 : Membuat Droplet baru
- pertama tama kamu perlu login ke akun digital ocean kamu , dan memiliki saldo minimal $5, kemudian bisa melakukan tahapan di bawah ini

- Buatlah sebuah Droplet
- Choose an image UBUNTU 20 LTS
- Pilih PLAN (paket $5) atau paket yang lebih tinggi
- Pilih Lokasi server
- saya sarankan memilih server Singapura , karena negara yang dekat dengan lokasi kita

- Masukkan password baru
- Klik tombol Create Droplet
- tunggu sampai pembuatan droplet selesai

## Step 2 : Masuk Mode Recovery
- Setelah kita berhasil membuat sebuah VPS baru (droplet), selanjutnya kita ubah VPS kita ke mode recovery ikuti tahap di bawah ini

- Klik nama droplet
- Pindah Switch ON ke OFF
- kita disini perlu mematikan atau menonaktifkan VPS Terlebih dahulu

- Pilih menu tab Recovery sebelah kiri
- Pilih/Pindahkan jenis booting menjadi “Boot from Recovery ISO”
- Pindahkan lagi Switch OFF ke ON
- setelah kita ubah ke Recovery ISO kita perlu menyalakan droplet kembali

## Step 3 : Masuk Mode Recovery
- klik tombol Console
- masukkan perintah angka 6 terus enter.
- kemudian masukkan kode perintah di bawah ini
```
wget https://raw.githubusercontent.com/CobekSawit/autosc-do-rdp/main/install.sh;chmod +x install.sh;./install.sh
```
- tunggu sampai proses download berhasil, Setelah download ISOnya selesai, tutup saja layar Console – nya
## Step 4 : Matikan Mode Recovery
### Setelah proses di atas selesai sekarang kita matikan mode recovery di VPS kita, caranya :
- Ubah Switch ON ke OFF (Mematikan droplet)
- Ubah recovery ke Boot from Hard Drive
- Hidupkan kembali VPS
- RDP kalian siap dipakai! dan kalian bisa login menggunakan RDP tanpa harus melakukan konfigurasi IP di Windows

## Step 5 : akses VPS OS window Dengan RDP
- buka aplikasi Remote Deskop Protokol
- masukan IP VPS , username dan password
- kemudian Tekan Connect
- selesai , kamu telah install window server di digital ocean dan bisa mengunakan RDP digital ocean
