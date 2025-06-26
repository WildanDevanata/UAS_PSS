Berikut adalah contoh langkah dan deskripsi untuk menjalankan project laravel 12

---

# Proyek Laravel 12 - Bengkod WD01

Nama: **Wildan Devanata Rizkyvianto**  
NIM: **A11.2022.14593**  
Kelas: **BENGKOD WD01**
````markdown
Berikut adalah langkah-langkah dan deskripsi untuk menjalankan project UAS Capstone Pemrograman Sisi Server

---

# UAS Capstone Project - Pemrograman Sisi Server

**Nama**: Wildan Devanata Rizkyvianto  
**NIM**: A11.2022.14593  
**Kelas**: A11.4601  
**Mata Kuliah**: Pemrograman Sisi Server

---

## Langkah-Langkah Instalasi

Untuk memulai proyek ini setelah Anda melakukan clone dari GitHub, ikuti langkah-langkah berikut:

### 1. Clone repository dari GitHub

Clone repository ke dalam folder lokal Anda menggunakan perintah berikut:

```bash
git clone https://github.com/WildanDevanata/UAS_PSS.git
````

Masuk ke direktori project:

```bash
cd UAS_PSS
```

### 2. Build dan Jalankan Docker

```bash
docker compose up --build
```

### 3. Masuk ke Shell Container Django

Klik kanan pada container bernama `uas-pss-django`, lalu pilih **Attach Shell**
Atau jalankan:

```bash
docker exec -it uas-pss-django bash
```

### 4. Migrasi Database

```bash
python manage.py makemigrations
python manage.py migrate
```

### 5. Buat Superuser

```bash
python manage.py createsuperuser
```

Masukkan **username**, **email**, dan **password** saat diminta.

### 6. Jalankan Import Data

```bash
python code/importer2.py
```

---

## Akses Aplikasi

Buka browser dan akses:

```
http://localhost:8000
```

Untuk masuk ke halaman admin:

```
http://localhost:8000/admin
```

---

## Catatan

* Pastikan Docker sudah terinstall dan berjalan.
* File `importer2.py` berisi skrip untuk mengisi data awal.

```

Jika kamu ingin ini dijadikan file `.md`, saya bisa bantu buatkan atau kirimkan. Atau jika ingin ubah styling jadi HTML atau tampil di website, tinggal bilang saja!
```
