📘 Basis Data Part 1
SQL & RDBMS (Lengkap dengan Quiz dan Output)
Pendahuluan

Basis data merupakan komponen utama dalam sistem informasi modern. Hampir semua aplikasi—mulai dari website, sistem akademik, hingga aplikasi perbankan—menggunakan basis data untuk menyimpan dan mengelola data. Oleh karena itu, pemahaman dasar mengenai SQL (Structured Query Language) dan RDBMS (Relational Database Management System) menjadi fondasi penting bagi mahasiswa dan praktisi IT.

Blog ini membahas materi Basis Data Part 1, meliputi:

Pengertian SQL dan RDBMS

Tools RDBMS

Operasi dasar SELECT

Quiz beserta query dan hasil output

1. SQL & RDBMS
1.1 Pengertian SQL

SQL (Structured Query Language) adalah bahasa standar yang digunakan untuk berkomunikasi dengan database relasional. SQL digunakan untuk:

Mengambil data (SELECT)

Menyimpan data (INSERT)

Memperbarui data (UPDATE)

Menghapus data (DELETE)

1.2 Pengertian RDBMS

RDBMS (Relational Database Management System) adalah sistem pengelola basis data berbentuk tabel (relasi) yang saling berhubungan dan diakses menggunakan SQL.

2. Tools RDBMS

Beberapa tools RDBMS yang umum digunakan:

MySQL – Open-source, populer untuk pengembangan web

PostgreSQL – Open-source, kuat dalam konsistensi data

Oracle Database – Proprietary, banyak digunakan di perbankan

Microsoft SQL Server – Proprietary, digunakan di perusahaan besar

SQLite – Database ringan untuk aplikasi mobile

3. Operasi Dasar SELECT

Sebagai contoh, digunakan tabel ms_produk dengan struktur data berikut:

Contoh Data Tabel ms_produk
kode_produk	nama_produk	harga
prod-01	Kotak Pensil DQLab	62500
prod-02	Flashdisk DQLab 64 GB	55000
prod-03	Buku Tulis DQLab	12000
prod-04	Flashdisk DQLab 32 GB	40000
prod-05	Pulpen DQLab	8000
3.1 Mengambil Seluruh Kolom
SELECT * FROM ms_produk;

Hasil Output
kode_produk	nama_produk	harga
prod-01	Kotak Pensil DQLab	62500
prod-02	Flashdisk DQLab 64GB	55000
prod-03	Buku Tulis DQLab	12000
prod-04	Flashdisk DQLab 32GB	40000
prod-05	Pulpen DQLab	8000
3.2 Mengambil Satu Kolom
SELECT nama_produk FROM ms_produk;

Hasil Output
nama_produk
Kotak Pensil DQLab
Flashdisk DQLab 64GB
Buku Tulis DQLab
Flashdisk DQLab 32GB
Pulpen DQLab
3.3 Mengambil Beberapa Kolom
SELECT kode_produk, nama_produk FROM ms_produk;

Hasil Output
kode_produk	nama_produk
prod-01	Kotak Pensil DQLab
prod-02	Flashdisk DQLab 64GB
prod-03	Buku Tulis DQLab
prod-04	Flashdisk DQLab 32GB
prod-05	Pulpen DQLab
3.4 Membatasi Jumlah Baris
SELECT * FROM ms_produk
LIMIT 3;

Hasil Output
kode_produk	nama_produk	harga
prod-01	Kotak Pensil DQLab	62500
prod-02	Flashdisk DQLab 64GB	55000
prod-03	Buku Tulis DQLab	12000
4. Quiz Basis Data Part 1
Quiz 1

Soal:
Ambil seluruh kolom dari tabel ms_produk.

Query:

SELECT * FROM ms_produk;


Output:
(Sama seperti tabel pada poin 3.1)

Quiz 2

Soal:
Tampilkan kode_produk dan nama_produk.

Query:

SELECT kode_produk, nama_produk FROM ms_produk;


Output:

kode_produk	nama_produk
prod-01	Kotak Pensil DQLab
prod-02	Flashdisk DQLab 64GB
prod-03	Buku Tulis DQLab
prod-04	Flashdisk DQLab 32GB
prod-05	Pulpen DQLab
Quiz 3

Soal:
Batasi jumlah data yang ditampilkan menjadi 3 baris.

Query:

SELECT * FROM ms_produk
LIMIT 3;


Output:

kode_produk	nama_produk	harga
prod-01	Kotak Pensil DQLab	62500
prod-02	Flashdisk DQLab 64GB	55000
prod-03	Buku Tulis DQLab	12000
Penutup

Materi Basis Data Part 1 memberikan dasar penting dalam memahami SQL dan RDBMS. Dengan menguasai perintah SELECT dan memahami hasil outputnya, pengguna dapat mulai mengelola dan menganalisis data secara efektif.
