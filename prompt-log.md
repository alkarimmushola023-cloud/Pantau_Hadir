**LOG PROMPTING AI & REFAKTORISASI KODE**  
**Modul 6**: Konversi Desain Figma ke HTML5  
**Kelompok 1 UT \- Pantau Hadir**

\---

**A. Anggota Kelompok & Pembagian Layar**

1. Adil Iskandar \- \`admin-login\` & \`tambah-pekerja.html\`  
2. Agil Prasetya \- \`rekap-absensi.html\` & \`index.html\`  
3. Epen Supendi \- \`absen-sukses.html\` & \`data-pekerja.html\`  
4. Kintan Aulia \- \`pekerja-dashboard.html\` & \`pekerja-login.html\`  
5. Rafli Nur Alviansyah \- ‘admin-dashboard.html’ & ‘error.html’

\---

**B. Riwayat Prompting Per Layar**

**1\. Layar: \`index.html\` (Dikerjakan oleh: Agil Prasetya)**

- Prompt:   
  \> Buatkan struktur HTML polos tanpa style untuk index.html \- masuk sebagai (dengan melampirkan jpeg logo pantau hadir).  
- Hasil & Refaktorisasi:  
   \* AI awalnya memberikan beberapa atribut dan juga beberapa struktur folder pada vs code dan juga menampilkan logo, judul aplikasi, dan pilihan Masuk Sebagai untuk Admin, dan Pekerja.   
- Refaktorisasi Manual:   
-  Mengganti \<img src="img/logo-pantau-hadir.png" pada bagian \<header\> menjadi \<img src="logo pantau hadir.jpeg"   
- Menghapus code \<li\> \<a href="login-mandor.html"\> Masuk sebagai Mandor \</a\> \</li\>

**2\. Layar: \`pekerja-login.html\` (Dikerjakan oleh: Kintan Aulia)**

- Prompt:  
  \> Buat kode html5 semantik (tanpa css/style maupun script) untuk layar login pekerja dengan komponen-komponen terlampir \[melampirkan png prototype layar ‘pekerja-login’\]  
- Hasil & Refaktorisasi:  
   \* AI awalnya memberikan struktur HTML untuk halaman login pekerja dengan komponen navigasi ‘Keluar’ dengan ‘href=”\#”’, header teks ‘Pantau Hadir’ dan caption, form input ‘NIK’ dan ‘Kata Sandi’, serta button ‘Masuk’.   
- Refaktorisasi Manual:  
  \* Melengkapi anchor Keluar href=“index.html”.  
  \* Mengubah header teks dengan logo menggunakan \<img\>.  
  \* Menambahkan kolom input baru ‘ID Perusahaan’.  
  \* Melengkapi \<form\> menjadi \<form action\="pekerja-dashboard.html" method\="post"\>.


  
**3\. Layar: \`pekerja-dashboard.html\` (Dikerjakan oleh: Kintan Aulia)**

- Prompt:  
  \> Buat kode html5 semantik (tanpa css/style maupun script) untuk layar dashboard sistem absensi pekerja dengan komponen-komponen terlampir \[melampirkan png prototype layar ‘pekerja-dashboard’\]  
  \> Jika ada penggunaan tag aria yang redundant, hilangkan  
- Hasil & Refaktorisasi:  
   \* AI menghasilkan beberapa atribut ARIA yang redundan, menyisipkan kode \`\<svg\>\` secara langsung (\*inline SVG\*), serta menggabungkan area pratinjau kamera dan tombol 'Absen' dalam satu garis yang kurang rapi.   
- Refaktorisasi Manual:  
  \* Mengganti \*inline\* \`\<svg\>\` dengan tag \`\<img\>\` yang mengarah ke jalur relatif \`./assets/images/icons/\`.   
  \* Membungkus area pratinjau kamera depan menggunakan elemen semantik \`\<fieldset\>\` dengan \`\<legend\>\` "Pratinjau Kamera Depan".   
  \* Memisahkan button ‘Absen’ dengan menaruhnya ke dalam tag \<p\> yang berbeda.

**4\. Layar: \`absen-sukses.html\` (Dikerjakan oleh: Kintan Aulia)**

- Prompt:  
  \> Buat kode html5 semantik (tanpa css/style maupun script) untuk layar absen-sukses dengan komponen-komponen terlampir \[melampirkan png prototype layar ‘absen-sukses’\]  
- Hasil & Refaktorisasi:  
   \* AI awalnya memberikan struktur HTML untuk halaman absen-sukses dengan \<button\> keluar, ikon checklist kecil, dan tabel polos yang berisi dummy data absen sesuai gambar terlampir.  
- Refaktorisasi Manual:  
  \* Mengganti button keluar dengan anchor ke halaman beranda disertai ikon.  
  \* Mengganti ikon checklist lebih sesuai dengan prototype.  
  \* Merapikan tabel dengan memberi border.  
  \* Menambahkan button navigasi dengan ikon arrow-left dan arrow-right.  
  \* Mengganti footer teks dengan logo.

**5\. Layar: \`admin-login.html\` (Dikerjakan oleh: Adil Iskandar)**

- Prompt:   
  \> Buatkan Struktur simantik html untuk login page tanpa tambahan style pada html ataupun CSS.\[Melampirkan png prototype pada tampilan ‘admin login’\]  
- Hasil & Refaktorisasi:  
   \* AI awalnya memberikan tampilan login page dengan kolom untuk menginput NIK dan kata sandi (password), serta button untuk login.  
- Refaktorisasi Manual:  
  \> mengganti img src\="logo.png" menjadi  img src\="logo-pantau-hadir.jpg" .  
  \> menambahkan width\="200"  
   untuk mengatur besar pada gambar.  
  \> menyematkan ikon icons/eye-off.svg  
   pada kolom kata sandi   
  \> mengubah tampilannya menjadi width\="10" dengan keterangan gambar alt\="Toggle sandi"\>  
    
  \> menyematkan icons/house.svg untuk a href Kembali ke beranda.  
  


**6\. Layar: \`admin-dashboard.html\` (Dikerjakan oleh: Rafli Nur Alviansyah)**

- Prompt:  
  Buatkan kode HTML saja tanpa CSS dan JavaScript berdasarkan desain prototype PNG halaman Admin Dashboard Pantau Hadir yang saya berikan, dengan struktur dan komponen sesuai prototype. \[Melampirkan png prototype pada tampilan ‘admin dashboard’\]  
- Hasil & Refaktorisasi:  
   \* AI awalnya memberikan struktur HTML untuk halaman Admin Dashboard yang terdiri dari sidebar navigasi, header, informasi tanggal dan waktu, tiga bagian statistik absensi, serta gambar ilustrasi konstruksi. Kode menggunakan elemen HTML seperti \<aside\>, \<nav\>, \<main\>, \<header\>, \<section\>, \<img\>, dan \<button\>.   
- Refaktorisasi Manual:  
  \> Memperbaiki tag penutup heading yang tidak sesuai, yaitu \<h2\>PT. Jalan Baru\</h3\> menjadi \<h2\>PT. Jalan Baru\</h2\>.  
  \> Memperbaiki kesalahan penulisan atribut widht="10" menjadi width="10" pada gambar ikon pengguna.  
  \> Memperbaiki struktur heading agar tingkat judul tersusun secara hierarkis, mulai dari \<h1\> untuk judul Dashboard, \<h2\> untuk judul bagian, dan \<h3\> untuk judul statistik.  
  \> Menambahkan atribut aria-labelledby pada elemen \<section\> untuk menghubungkan bagian dengan judulnya.  
  \> Mengganti elemen \<section\> yang hanya berfungsi sebagai wadah konten menjadi \<div\> agar penggunaannya sesuai dengan fungsi elemen HTML.  
  


**7\. Layar: \`rekap-absensi.html\` (Dikerjakan oleh: Agil Prasetya)**

- Prompt:  
  Buatkan struktur HTML polos tanpa style untuk rekapitulasi-absensi.html pada rekapitulasi absensi (dengan menambahkan dokumen file excel data presensi pekerjanya)  
- Hasil & Refaktorisasi:  
   \* AI awalnya memberikan beberapa atribut dan juga beberapa struktur folder proyek vs code dan juga file tersebut memiliki 8 kolom, yaitu No, Nama, Tanggal, Jam Masuk, Bukti Masuk, Jam Pulang, Bukti Pulang, dan Status.   
    
- Refaktorisasi Manual:   
-  Memperbaiki tabel pertama — baris 74 \<table border="1"\> ganti menjadi: \<table\>   
-  Memperbaiki tabel pertama — baris 97 \<table border="1"\> ganti menjadi: \<table\>

**8\. Layar: \`data-pekerja.html\` (Dikerjakan oleh: Rafli Nur Alviansyah)**

- Prompt:  
  Buatkan code HTML yang menampilkan page data pekerja, sesuai prototype yang saya berikan dan data pekerja yang saya berikan (melampirkan png prototype UI page data-pekerja serta file XLS data\_pekerja)   
- Hasil & Refaktorisasi:  
   \* AI awalnya memberikan kode HTML yang sudah menampilkan struktur tabel data pekerja dan navigasi halaman, tetapi terdapat beberapa kesalahan, seperti penggunaan atribut alt yang kurang tepat pada gambar ikon navigasi dan atribut aria-label yang tidak konsisten pada tombol  
- Refaktorisasi Manual:  
  Memperbaiki atribut alt pada gambar agar sesuai dengan fungsi ikon, menyeragamkan penggunaan atribut aria-label pada tombol navigasi, serta merapikan struktur elemen HTML agar lebih terstruktur dan mudah dipahami tanpa menggunakan CSS.

**9\. Layar: \`tambah-pekerja.html\` (Dikerjakan oleh: Adil Iskandar)**

- Prompt:   
  Buatkan Struktur simantik html untuk login page tanpa tambahan style pada html ataupun CSS.\[Melampirkan png prototype pada tampilan ‘tambah pekerja’\]  
- Hasil & Refaktorisasi:  
   \* AI awalnya memberikan tampilan tambah pekerja dengan navbar Dashboard, Rekap Absensi, dan Data Pekerja. 4 kolom untuk menginput Nama pekerja, NIK, Lokasi Kerja, dan Buat Password Baru.  
- Refaktorisasi Manual:  
  \> menambahkan gambar img src\="logo-pantau-hadir.jpg Dengan width\="200"  
  \> mengganti icon “icons.png” menjadi "icons/log-out.svg" pada button.  
  \> menambahkan \<option value\=""\>*Pilih lokasi proyek*\</option\> untuk memilih lokasi proyek pekerja nantinya.  
  \> menambahkan \<button type\="submit"\> *Simpan* \</button\> Sebagai tombol untuk menyimpan data pekerja dan menambahkan icon \<img src\="icons/Check.svg" width\="10" alt\=""\> pada button.  
  \> menambahkan \<button type\="button"\> *Batal* \</button\> sebagai tombol untuk membatalkan penginputan. Menambahkan \<img src\="icons/circle-x.svg" width\="10" alt\=""\> pada button.


  
**10\. Layar: \`error.html\` (Dikerjakan oleh: Rafli Nur Alviansyah)**

- Prompt:  
  Buatkan kode HTML halaman error Pantau Hadir berdasarkan standar HTML yang baik, tanpa CSS, serta sesuai prototype. \[Melampirkan png prototype pada tampilan ‘error’\]  
- Hasil & Refaktorisasi:  
   \* AI awalnya memberikan kode HTML untuk halaman error Pantau Hadir yang terdiri dari elemen \<header\>, \<main\>, \<section\>, dan \<footer\>. Pada bagian pesan kesalahan, AI menggunakan elemen heading \<h2\> untuk menampilkan teks “MOHON MAAF\!” serta menambahkan gambar ikon error, pesan tidak bisa terhubung dengan server, dan tautan kembali ke beranda.  
- Refaktorisasi Manual:  
  Saya melakukan perubahan secara manual pada kode HTML dengan mengganti tag \<h2\>MOHON MAAF\!\</h2\> menjadi \<h1\>MOHON MAAF\!\</h1\>. Perubahan ini dilakukan karena teks “MOHON MAAF\!” merupakan judul utama pada halaman error.


