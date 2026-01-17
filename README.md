# 📘 Basis Data Part 1 – SQL & RDBMS

> Dokumentasi pembelajaran Basis Data (Part 1)
>

---

## 📌 Pendahuluan

Basis data merupakan komponen inti dalam sistem informasi modern. Hampir semua aplikasi—baik web, desktop, maupun mobile—menggunakan basis data untuk menyimpan dan mengelola data. Oleh karena itu, pemahaman dasar mengenai **SQL (Structured Query Language)** dan **RDBMS (Relational Database Management System)** menjadi fondasi penting bagi mahasiswa dan praktisi di bidang Teknologi Informasi.

Pada Part 1 ini, pembahasan difokuskan pada:

* Konsep dasar SQL dan RDBMS
* Tools RDBMS
* Operasi dasar `SELECT`
* Quiz beserta **query dan output**

---

## 1️⃣ SQL & RDBMS

### 1.1 Pengertian SQL

**SQL (Structured Query Language)** adalah bahasa standar yang digunakan untuk berkomunikasi dengan database relasional. SQL digunakan untuk:

* Mengambil data (`SELECT`)
* Menambahkan data (`INSERT`)
* Memperbarui data (`UPDATE`)
* Menghapus data (`DELETE`)

### 1.2 Pengertian RDBMS

**RDBMS (Relational Database Management System)** adalah sistem manajemen basis data yang menyimpan data dalam bentuk tabel (relasi) dan menggunakan SQL sebagai bahasa pengolahannya.

---

## 2️⃣ Tools RDBMS

Beberapa tools RDBMS yang umum digunakan:

1. **MySQL** – Open-source, populer untuk aplikasi web
2. **PostgreSQL** – Open-source, kuat dalam konsistensi dan integritas data
3. **Oracle Database** – Proprietary, banyak digunakan di sektor perbankan
4. **Microsoft SQL Server** – Proprietary, digunakan di perusahaan besar
5. **SQLite** – Database ringan untuk aplikasi mobile

---

## 3️⃣ Operasi Dasar SELECT

### Contoh Tabel: `ms_produk`

| kode_produk | nama_produk           | harga |
| ----------- | --------------------- | ----- |
| prod-01     | Kotak Pensil DQLab    | 62500 |
| prod-02     | Flashdisk DQLab 64 GB | 55000 |
| prod-03     | Buku Tulis DQLab      | 12000 |
| prod-04     | Flashdisk DQLab 32 GB | 40000 |
| prod-05     | Pulpen DQLab          | 8000  |

---

### 3.1 Mengambil Seluruh Kolom

**Query**

```sql
SELECT * FROM ms_produk;
```

**Output**

| kode_produk | nama_produk           | harga |
| ----------- | --------------------- | ----- |
| prod-01     | Kotak Pensil DQLab    | 62500 |
| prod-02     | Flashdisk DQLab 64 GB | 55000 |
| prod-03     | Buku Tulis DQLab      | 12000 |
| prod-04     | Flashdisk DQLab 32 GB | 40000 |
| prod-05     | Pulpen DQLab          | 8000  |

---

### 3.2 Mengambil Satu Kolom

**Query**

```sql
SELECT nama_produk FROM ms_produk;
```

**Output**

| nama_produk           |
| --------------------- |
| Kotak Pensil DQLab    |
| Flashdisk DQLab 64 GB |
| Buku Tulis DQLab      |
| Flashdisk DQLab 32 GB |
| Pulpen DQLab          |

---

### 3.3 Mengambil Beberapa Kolom

**Query**

```sql
SELECT kode_produk, nama_produk FROM ms_produk;
```

**Output**

| kode_produk | nama_produk           |
| ----------- | --------------------- |
| prod-01     | Kotak Pensil DQLab    |
| prod-02     | Flashdisk DQLab 64 GB |
| prod-03     | Buku Tulis DQLab      |
| prod-04     | Flashdisk DQLab 32 GB |
| prod-05     | Pulpen DQLab          |

---

### 3.4 Membatasi Jumlah Baris

**Query**

```sql
SELECT * FROM ms_produk
LIMIT 3;
```

**Output**

| kode_produk | nama_produk           | harga |
| ----------- | --------------------- | ----- |
| prod-01     | Kotak Pensil DQLab    | 62500 |
| prod-02     | Flashdisk DQLab 64 GB | 55000 |
| prod-03     | Buku Tulis DQLab      | 12000 |

---

## 4️⃣ Quiz Basis Data Part 1

### 📝 Quiz 1

**Soal:** Ambil seluruh kolom dari tabel `ms_produk`.

**Query**

```sql
SELECT * FROM ms_produk;
```

**Output**

| kode_produk | nama_produk           | harga |
| ----------- | --------------------- | ----- |
| prod-01     | Kotak Pensil DQLab    | 62500 |
| prod-02     | Flashdisk DQLab 64 GB | 55000 |
| prod-03     | Buku Tulis DQLab      | 12000 |
| prod-04     | Flashdisk DQLab 32 GB | 40000 |
| prod-05     | Pulpen DQLab          | 8000  |

---

### 📝 Quiz 2

**Soal:** Tampilkan `kode_produk` dan `nama_produk`.

**Query**

```sql
SELECT kode_produk, nama_produk FROM ms_produk;
```

**Output**

| kode_produk | nama_produk           |
| ----------- | --------------------- |
| prod-01     | Kotak Pensil DQLab    |
| prod-02     | Flashdisk DQLab 64 GB |
| prod-03     | Buku Tulis DQLab      |
| prod-04     | Flashdisk DQLab 32 GB |
| prod-05     | Pulpen DQLab          |

---

### 📝 Quiz 3

**Soal:** Batasi jumlah data menjadi 3 baris.

**Query**

```sql
SELECT * FROM ms_produk
LIMIT 3;
```

**Output**

| kode_produk | nama_produk           | harga |
| ----------- | --------------------- | ----- |
| prod-01     | Kotak Pensil DQLab    | 62500 |
| prod-02     | Flashdisk DQLab 64 GB | 55000 |
| prod-03     | Buku Tulis DQLab      | 12000 |

---

## ✅ Penutup

Materi Basis Data Part 1 memberikan pemahaman dasar mengenai SQL dan RDBMS. Dengan menguasai perintah `SELECT` beserta hasil output-nya, pengguna dapat mulai melakukan pengolahan data secara terstruktur dan efisien.

---

## 🔗 Referensi

* [https://docs.google.com/document/d/18Dc_2P8xDXz7c1FEO37xxm_4Rxx09i49DOvnigZapaA/edit?usp=sharing]
* [https://www.mysql.com](https://www.mysql.com)
* [https://www.postgresql.org](https://www.postgresql.org)
* [https://www.oracle.com/database](https://www.oracle.com/database)
* [https://learn.microsoft.com/sql](https://learn.microsoft.com/sql)
