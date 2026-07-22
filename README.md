# ERD Visualizer

ERD Visualizer adalah aplikasi web interaktif yang membantu Anda memvisualisasikan skema database dari file SQL secara cepat dan langsung di browser. Aplikasi ini cocok untuk analisis skema, debugging relasi tabel, dan memahami struktur data tanpa menyeting server tambahan.

## Kelebihan Proyek

- Import file SQL atau TXT langsung dari browser
- Mendukung format MySQL dan PostgreSQL
- Menampilkan tabel, kolom, primary key, foreign key, dan relasi secara visual
- Menemukan relasi tersembunyi dari kecocokan nilai data (tanpa FK eksplisit)
- Ringkasan relasi lengkap dengan visual dan query JOIN otomatis
- Panel pencarian tabel, zoom, dan auto-fit layar
- Semua berjalan lokal tanpa perlu backend

## Cara Menjalankan

1. Buka file `erd-visualizer.html` di browser modern.
2. Klik tombol `Import SQL` untuk memilih file skema database Anda.
3. Atau klik `Contoh Skema` untuk melihat demo internal.
4. Gunakan panel samping untuk mencari dan memilih tabel.
5. Buka ringkasan relasi untuk melihat query JOIN dan contoh data yang terhubung.

## Struktur Folder

- `erd-visualizer.html` — file aplikasi utama
- `tampilan/` — folder berisi screenshot tampilan aplikasi

## Screenshot & Penjelasan

### 1. Tampilan Visualisasi Semua Tabel

Menampilkan seluruh tabel dan relasi yang terdeteksi dalam satu tampilan diagram.

![Visualisasi Semua Tabel](tampilan/erd%20flow%20visual%20all%20tabel.png)

### 2. Fokus pada Tabel `orders`

Menunjukkan detail tabel `orders` dan relasinya, termasuk informasi kolom dan koneksi ke tabel lain.

![Tabel Orders](tampilan/erd%20flow%20visual%20tabel%20orders.png)

### 3. Ringkasan Relasi Skema (Primary Key ↔ Foreign Key)

Menampilkan relasi resmi yang diambil dari constraint primary key dan foreign key di dalam skema SQL.

![Relasi Skema](tampilan/Relasi%20Skema%20(Primary%20Key%20%E2%94%94%20Foreign%20Key).png)

### 4. Ringkasan Relasi dari Kecocokan Data

Menunjukkan relasi yang ditemukan melalui kecocokan nilai antar kolom, meskipun tidak ada foreign key eksplisit.

![Relasi dari Kecocokan Data](tampilan/Relasi%20dari%20Kecocokan%20Data%20(tanpa%20FK%20eksplisit).png)

### 5. Pilih Tabel & Kolom untuk Join

UI ini menunjukkan cara memilih tabel dan kolom yang ingin diikutkan dalam ringkasan join dan analisis data.

![Pilih Tabel & Kolom](tampilan/Pilih%20tabel%20%26%20kolom%20yang%20ingin%20diikutkan%20(centang%20tabel%2C%20klik%20kolom%20untuk%20toggle).png)

### 6. Pilih Nilai Contoh untuk Filter Query

Menampilkan pemilihan nilai sample yang digunakan untuk membangun query `WHERE` dan memfilter hasil join secara dinamis.

![Pilih Nilai Contoh untuk WHERE](tampilan/Pilih%20nilai%20contoh%20untuk%20WHERE.png)

## Catatan

- Semua pengolahan data dilakukan di browser, sehingga data Anda tidak dikirim ke server eksternal.
- Jika screenshot tidak tampil, pastikan nama file dan path `tampilan/` tetap sesuai.
- Proyek ini dapat dikembangkan lebih lanjut dengan fitur ekspor JSON, support ERD tambahan, dan integrasi database.
