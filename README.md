Berikut versi lengkap dari `README.md` yang sudah ditambahkan judul dan identitas:

````markdown
# UAS Capstone Project Pemrograman Sisi Server

**Nama**: WILDAN DEVANATA RIZKYVIANTO  
**NIM**: A11.2022.14593  
**Kelas**: A11.4601  
**Mata Kuliah**: Pemrograman Sisi Server

---

## 🐳 Menjalankan Aplikasi dengan Docker

Ikuti langkah-langkah berikut untuk menjalankan project ini menggunakan Docker:

### 1. Build dan Jalankan Container

```bash
docker compose up --build
````

### 2. Masuk ke Shell Container Django

Klik kanan pada container bernama `uas-pss-django`, lalu pilih **Attach Shell**
Atau gunakan perintah berikut di terminal:

```bash
docker exec -it uas-pss-django bash
```

### 3. Jalankan Perintah Migrasi Database

```bash
python manage.py makemigrations
python manage.py migrate
```

### 4. Buat Superuser

```bash
python manage.py createsuperuser
```

Masukkan username, email, dan password sesuai kebutuhan.

### 5. Jalankan Skrip Import Data

```bash
python code/importer2.py
```

---

## 🧑‍💻 Akses Halaman Admin

Setelah berhasil membuat superuser, buka halaman admin di browser:

```
http://localhost:8000/admin
```

Login menggunakan akun yang telah dibuat.

---

## 📂 Struktur Direktori (Opsional)

```
.
├── code/
│   └── importer2.py
├── docker-compose.yml
├── manage.py
└── ...
```

---

## 📝 Lisensi

Proyek ini dibuat untuk keperluan UAS dan bersifat open source untuk pembelajaran.

```

Jika kamu ingin saya bantu menyisipkan screenshot, diagram, atau penjelasan tambahan tentang fitur project-mu, tinggal beri tahu ya!
```
