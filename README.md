📘 Basis Data Part 1
SQL & RDBMS (Lengkap dengan Quiz & Output)
📌 Pendahuluan

Basis data merupakan komponen inti dalam pengembangan sistem informasi modern. Hampir seluruh aplikasi—baik berbasis web, desktop, maupun mobile—mengandalkan basis data untuk menyimpan dan mengelola data. Oleh karena itu, pemahaman dasar mengenai SQL (Structured Query Language) dan RDBMS (Relational Database Management System) menjadi hal yang sangat penting bagi mahasiswa dan praktisi di bidang Teknologi Informasi.

Blog ini membahas materi Basis Data Part 1, meliputi:

Konsep dasar SQL & RDBMS

Tools RDBMS

Operasi dasar SELECT

Quiz beserta query dan output yang bisa dicopy

1️⃣ SQL & RDBMS
1.1 Pengertian SQL

SQL (Structured Query Language) adalah bahasa standar yang digunakan untuk berinteraksi dengan database relasional. SQL digunakan untuk:

Mengambil data (SELECT)

Menambahkan data (INSERT)

Memperbarui data (UPDATE)

Menghapus data (DELETE)

1.2 Pengertian RDBMS

RDBMS (Relational Database Management System) adalah sistem manajemen basis data yang menyimpan data dalam bentuk tabel (relasi) dan menggunakan SQL sebagai bahasa pengolahannya.

2️⃣ Tools RDBMS

Beberapa RDBMS yang umum digunakan:

MySQL – Open-source, populer untuk aplikasi web

PostgreSQL – Open-source, fokus pada konsistensi data

Oracle Database – Proprietary, banyak digunakan di perbankan

Microsoft SQL Server – Proprietary, digunakan di perusahaan besar

SQLite – Database ringan untuk aplikasi mobile

3️⃣ Operasi Dasar SELECT
Contoh Tabel: ms_produk
+------------+---------------------------+-------+
| kode_produk| nama_produk               | harga |
+------------+---------------------------+-------+
| prod-01    | Kotak Pensil DQLab        | 62500 |
| prod-02    | Flashdisk DQLab 64 GB     | 55000 |
| prod-03    | Buku Tulis DQLab          | 12000 |
| prod-04    | Flashdisk DQLab 32 GB     | 40000 |
| prod-05    | Pulpen DQLab              | 8000  |
+------------+---------------------------+-------+

3.1 Mengambil Seluruh Kolom

Query

SELECT * FROM ms_produk;


Output

+------------+---------------------------+-------+
| kode_produk| nama_produk               | harga |
+------------+---------------------------+-------+
| prod-01    | Kotak Pensil DQLab        | 62500 |
| prod-02    | Flashdisk DQLab 64 GB     | 55000 |
| prod-03    | Buku Tulis DQLab          | 12000 |
| prod-04    | Flashdisk DQLab 32 GB     | 40000 |
| prod-05    | Pulpen DQLab              | 8000  |
+------------+---------------------------+-------+

3.2 Mengambil Satu Kolom

Query

SELECT nama_produk FROM ms_produk;


Output

+---------------------------+
| nama_produk               |
+---------------------------+
| Kotak Pensil DQLab        |
| Flashdisk DQLab 64 GB     |
| Buku Tulis DQLab          |
| Flashdisk DQLab 32 GB     |
| Pulpen DQLab              |
+---------------------------+

3.3 Mengambil Beberapa Kolom

Query

SELECT kode_produk, nama_produk FROM ms_produk;


Output

+------------+---------------------------+
| kode_produk| nama_produk               |
+------------+---------------------------+
| prod-01    | Kotak Pensil DQLab        |
| prod-02    | Flashdisk DQLab 64 GB     |
| prod-03    | Buku Tulis DQLab          |
| prod-04    | Flashdisk DQLab 32 GB     |
| prod-05    | Pulpen DQLab              |
+------------+---------------------------+

3.4 Membatasi Jumlah Baris

Query

SELECT * FROM ms_produk
LIMIT 3;


Output

+------------+---------------------------+-------+
| kode_produk| nama_produk               | harga |
+------------+---------------------------+-------+
| prod-01    | Kotak Pensil DQLab        | 62500 |
| prod-02    | Flashdisk DQLab 64 GB     | 55000 |
| prod-03    | Buku Tulis DQLab          | 12000 |
+------------+---------------------------+-------+

4️⃣ Quiz Basis Data Part 1
📝 Quiz 1

Soal: Ambil seluruh kolom dari tabel ms_produk.

Query

SELECT * FROM ms_produk;


Output

(prod-01 sampai prod-05 seperti pada tabel di atas)

📝 Quiz 2

Soal: Tampilkan kode_produk dan nama_produk.

Query

SELECT kode_produk, nama_produk FROM ms_produk;


Output

+------------+---------------------------+
| kode_produk| nama_produk               |
+------------+---------------------------+
| prod-01    | Kotak Pensil DQLab        |
| prod-02    | Flashdisk DQLab 64 GB     |
| prod-03    | Buku Tulis DQLab          |
| prod-04    | Flashdisk DQLab 32 GB     |
| prod-05    | Pulpen DQLab              |
+------------+---------------------------+

📝 Quiz 3

Soal: Batasi jumlah data menjadi 3 baris.

Query

SELECT * FROM ms_produk
LIMIT 3;


Output

+------------+---------------------------+-------+
| prod-01    | Kotak Pensil DQLab        | 62500 |
| prod-02    | Flashdisk DQLab 64 GB     | 55000 |
| prod-03    | Buku Tulis DQLab          | 12000 |
+------------+---------------------------+-------+

✅ Penutup

Materi Basis Data Part 1 memberikan dasar penting dalam memahami SQL dan RDBMS. Dengan memahami perintah SELECT beserta outputnya, pengguna dapat mulai melakukan pengolahan data secara efektif dan terstruktur.
