# Tugas Node.js: Daftar Customer (db_toko)

NAMA: Massoumma Nazwa Soraya
NIM: 2403310701

Proyek ini adalah implementasi backend Node.js untuk mengambil data pelanggan dari database MySQL dan menampilkannya di halaman HTML.

Setup Database

Sebelum menjalankan server, pastikan database `db_toko` sudah ada di Laragon/MySQL.

Jalankan perintah SQL berikut di **HeidiSQL/phpMyAdmin** Anda:

```sql
CREATE DATABASE db_toko;
USE db_toko;

CREATE TABLE customers (
    cust_id INT PRIMARY KEY,
    cust_name VARCHAR(100) NOT NULL,
    cust_city VARCHAR(100) NOT NULL
);

INSERT INTO customers (cust_id, cust_name, cust_city) VALUES
(1, 'Andi Santoso', 'Jakarta'),
(2, 'Budi Prasetyo', 'Bandung'),
(3, 'Citra Dewi', 'Surabaya'),
(4, 'Dika Setiawan', 'Medan'),
(5, 'Eka Lestari', 'Yogyakarta');
