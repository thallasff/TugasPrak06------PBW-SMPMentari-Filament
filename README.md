# 🚀 Praktikum PBW — Laravel + Filament

<img width="1920" height="1045" alt="image" src="https://github.com/user-attachments/assets/5af7b7ff-222f-406f-a0ac-54170f75a828" />    

---

## **✨ Langkah-Langkah Pengerjaan**

### **1. Membuat Project Laravel Baru**

* `composer create-project laravel/laravel smpmentari_filament`
* masuk folder project → `cd smpmentari_filament`
* generate app key → `php artisan key:generate`

### **2. Menyiapkan Database**

* buka Laragon → Start All
* buka phpMyAdmin → buat database **smpmentari_filament**
* edit `.env` untuk set database MySQL

### **3. Migrasi Awal**

* menjalankan migrasi bawaan Laravel → `php artisan migrate`

### **4. Instalasi Filament**

* install Filament → `composer require "filament/filament"`
* install panel → `php artisan filament:install --panels`
* buat user admin → `php artisan make:filament-user`

### **5. Membuat Model & Migrasi CRUD**

* model **Kegiatan** → `php artisan make:model Kegiatan -m`
* model **Siswa** → `php artisan make:model Siswa -m`
* edit file migrasi sesuai struktur tabel
* jalankan migrasi → `php artisan migrate`

### **6. Generate Filament Resource**

* `php artisan make:filament-resource Kegiatan --generate`
* `php artisan make:filament-resource Siswa --generate`

### **7. Storage Link**

* menjalankan → `php artisan storage:link`

### **8. Routing Halaman Publik (Opsional)**

* menambahkan route untuk halaman kegiatan publik di `web.php`

### **9. Menjalankan Aplikasi**

* menjalankan server → `php artisan serve`
* akses admin panel → `http://localhost:8000/admin`

<img width="1920" height="1043" alt="image" src="https://github.com/user-attachments/assets/3aa576ec-30e5-415c-ae4c-e112c5246023" />

---
