# Belajar Directus

Proyek ini mengatur instansi Directus dengan Docker Compose, menggunakan PostgreSQL sebagai basis data dan Redis sebagai penyimpanan cache. Directus adalah CMS Headless sumber terbuka dengan API dinamis dan panel admin yang kuat untuk mengelola konten Anda.

## Prasyarat

Pastikan Anda sudah menginstal Docker dan Docker Compose di sistem Anda.

## Pengaturan

### Klon Repositori

Klon repositori ini dan masuk ke direktori:

```
git clone https://github.com/dikahariss/belajar-directus.git
cd belajar-directus
```

### Konfigurasi Variabel Lingkungan

Ubah nilai default untuk **POSTGRES_PASSWORD**, **DB_PASSWORD**, **KEY**, dan **SECRET** di file docker-compose.yml agar unik dan aman.

### Mulai Layanan

Jalankan layanan menggunakan perintah:

```
docker-compose up -d
```

### Akses Directus

Setelah layanan berjalan, Directus dapat diakses melalui:

```
http://localhost:8055
```

### Menghentikan Layanan

Untuk menghentikan semua layanan, gunakan perintah:

```
docker-compose down
```

## Informasi Tambahan

- **Database**: Layanan PostgreSQL disiapkan dengan PostGIS.
- **Caching**: Layanan Redis digunakan oleh Directus untuk caching.
- **Catatan Keamanan**: Konfigurasi ini ditujukan untuk pengembangan dan mungkin tidak aman untuk produksi.
