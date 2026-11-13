# Praktikum 9 — Teknologi Web Service

**Pemilik repository:** Bintang Permana Putra  
**NPM:** 24.0504.0040  
**Program Studi:** Teknik Informatika  
**Semester/Kelas:** 5 / 5B  
**Mata Kuliah:** Teknologi Web Service

## Deskripsi

Proyek praktikum ini merupakan aplikasi REST API berbasis Laravel untuk pengelolaan data buku (*books*) dan kategori (*categories*). API menyediakan operasi CRUD untuk kedua sumber daya tersebut.

## Teknologi

- PHP 8.3+
- Laravel 13
- Laravel Sanctum
- Composer
- Database yang didukung Laravel

## Menjalankan proyek

1. Salin file konfigurasi: `cp .env.example .env` (Windows PowerShell: `Copy-Item .env.example .env`).
2. Pasang dependensi: `composer install`.
3. Buat application key: `php artisan key:generate`.
4. Atur koneksi database pada file `.env`.
5. Jalankan migrasi: `php artisan migrate`.
6. Jalankan server: `php artisan serve`.

## Endpoint API

Semua endpoint berada di prefix `/api`.

| Metode | Endpoint | Keterangan |
|---|---|---|
| GET | `/api/categories` | Daftar kategori |
| POST | `/api/categories` | Membuat kategori |
| GET | `/api/categories/{category}` | Detail kategori |
| PUT/PATCH | `/api/categories/{category}` | Mengubah kategori |
| DELETE | `/api/categories/{category}` | Menghapus kategori |
| GET | `/api/books` | Daftar buku |
| POST | `/api/books` | Membuat buku |
| GET | `/api/books/{book}` | Detail buku |
| PUT/PATCH | `/api/books/{book}` | Mengubah buku |
| DELETE | `/api/books/{book}` | Menghapus buku |

## Atribusi sumber

Struktur dan implementasi awal proyek ini berasal dari repository referensi milik **firdiyansyahmohaziz-blip**:  
https://github.com/firdiyansyahmohaziz-blip/praktikum-9-tws

Repository ini merupakan salinan kerja untuk keperluan pembelajaran. Perubahan, pengujian, dan pengembangan lanjutan perlu dicatat secara transparan oleh pemilik repository.

## Catatan

File `.env`, kredensial, dan dependensi hasil instalasi tidak disertakan. Jangan mengunggah secret atau password ke repository publik.
