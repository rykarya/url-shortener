Pemendek Tautan Statis dengan Netlify
Ini adalah proyek sederhana untuk membuat layanan pemendek tautan (URL shortener) pribadi Anda sendiri menggunakan hosting statis dari Netlify, tanpa memerlukan database.

Bagaimana Cara Kerjanya?
Kekuatan utama proyek ini terletak pada file _redirects yang dibaca secara otomatis oleh Netlify. Setiap baris dalam file ini mendefinisikan sebuah aturan pengalihan (redirect).

Ketika seseorang mengunjungi https://domain-anda.netlify.app/nama-pendek, Netlify akan mencocokkannya dengan aturan di file _redirects dan langsung mengarahkan pengunjung ke URL tujuan yang sesuai.

Cara Setup (5 Menit)
Miliki Akun GitHub & Netlify: Pastikan Anda sudah memiliki akun di GitHub dan Netlify. Keduanya gratis.

Gunakan Proyek ini:

Buat repositori baru di akun GitHub Anda (bisa private atau public).

Salin (copy-paste) isi dari ketiga file (index.html, _redirects, README.md) ini ke dalam repositori baru Anda.

Atau, jika Anda familiar dengan Git, Anda bisa fork dan clone repositori ini.

Hubungkan ke Netlify:

Masuk ke dashboard Netlify Anda.

Klik "Add new site" -> "Import an existing project".

Pilih GitHub sebagai provider Git Anda dan otorisasi jika diminta.

Pilih repositori yang baru saja Anda buat.

Pengaturan build bisa dibiarkan default. Langsung klik "Deploy site".

Selesai!: Netlify akan memberikan Anda sebuah URL acak (misalnya: serene-biscuit-12345.netlify.app). Anda bisa mengubah nama ini di Site settings -> Domain management -> Options -> Edit site name. Sekarang, halaman utama pemendek tautan Anda sudah online!

Cara Menambahkan Tautan Baru
Ini adalah bagian terpenting dan yang akan sering Anda lakukan.

Buka Repositori GitHub Anda: Navigasi ke repositori proyek ini di GitHub.

Edit File _redirects:

Klik pada file _redirects.

Klik ikon pensil (Edit) di pojok kanan atas.

Tambahkan Baris Baru:

Pergi ke baris paling bawah.

Tambahkan tautan baru Anda dengan format: /nama-custom https://url-tujuan-anda.com

Contoh: /rapat-mingguan https://meet.google.com/xyz-abc-def

Simpan Perubahan:

Scroll ke bawah dan klik tombol hijau "Commit changes".

Anda bisa langsung commit ke branch main.

Itu saja! Netlify akan mendeteksi perubahan ini dan secara otomatis memulai proses deploy ulang (biasanya kurang dari 30 detik). Setelah selesai, tautan pendek baru Anda akan langsung aktif.

Anda bisa mengunjungi halaman utama (index.html) dari situs Anda untuk melihat daftar tautan yang sudah aktif.
