# ERD Visualizer

ERD Visualizer adalah aplikasi web interaktif untuk memetakan skema database dari file SQL secara visual. Aplikasi ini membantu Anda melihat struktur tabel, relasi antar tabel, serta atribut utama dan foreign key dengan cepat.

## Fitur Utama

- Import file SQL atau TXT
- Mendukung skema MySQL dan PostgreSQL
- Menampilkan tabel beserta relasinya secara visual
- Ringkasan relasi database otomatis dari foreign key dan kecocokan nilai data
- Pratinjau query JOIN live dan hasil baris data dari file SQL
- Pencarian tabel dan navigasi zoom
- Bekerja secara lokal di browser tanpa perlu server

## Cara Menggunakan

1. Buka file [erd-visualizer.html](erd-visualizer.html) di browser.
2. Klik tombol Import SQL untuk mengunggah file skema database Anda.
3. Atau pilih Contoh Skema untuk melihat tampilan demo.
4. Jelajahi visualisasi tabel dan relasi yang dihasilkan.
5. Buka modul Ringkasan Relasi untuk melihat query JOIN live, nilai contoh, dan hasil data yang terhubung.

## Struktur Folder

- [erd-visualizer.html](erd-visualizer.html) — file utama aplikasi
- [tampilan](tampilan) — folder berisi screenshot hasil visualisasi

## Tampilan Aplikasi

### Semua tabel

![Tampilan ERD Visualizer semua tabel](tampilan/erd%20flow%20visual%20all%20tabel.png)

### Tabel Orders

![Tampilan ERD Visualizer tabel orders](tampilan/erd%20flow%20visual%20tabel%20orders.png)

### Ringkasan Relasi Database

Tampilan ringkasan relasi database menunjukkan hubungan antar tabel secara mendetail, termasuk daftar semua relasi yang ditemukan dari foreign key dan kecocokan nilai data.

![Ringkasan Relasi Database](tampilan/erd%20summary%20relations.png)

### Contoh Query dan Hasil Data

Modul ini menampilkan preview query JOIN yang dihasilkan secara otomatis berdasarkan relasi tabel, serta menampilkan sampel hasil data yang terhubung antar tabel untuk validasi data.

![Contoh Query dan Hasil Data](tampilan/erd%20summary%20query.png)

## Catatan

Proyek ini dibuat sebagai alat visualisasi ERD sederhana dan dapat dikembangkan lebih lanjut sesuai kebutuhan database Anda.
