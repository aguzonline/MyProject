# Perjalanan Lintas Batas

Website statis jurnal solo traveler Indonesia. HTML, CSS, dan JavaScript tanpa build tools.

## Jalankan lokal
Buka `index.html` langsung di browser.

## GitHub
1. Buat repository baru di GitHub.
2. Dari folder proyek, jalankan:

```bash
git init
git add .
git commit -m "Initial Perjalanan Lintas Batas"
git branch -M main
git remote add origin https://github.com/USERNAME/REPO.git
git push -u origin main
```

Ganti `USERNAME/REPO` dengan milik Anda.

## Coolify (Dockerfile)
1. Buat resource **New Resource > Application** dari repository GitHub.
2. Pilih branch `main` dan build pack **Dockerfile**.
3. Dockerfile location: `/Dockerfile`; port aplikasi/container: `80`.
4. Tambahkan domain pada konfigurasi aplikasi dan arahkan DNS ke server Coolify.
5. Klik **Deploy**. Coolify membangun image Nginx dan melayani website melalui port 80.

## Catatan
- Foto di halaman memakai URL eksternal, jadi membutuhkan koneksi internet. Untuk produksi, ganti dengan foto berlisensi yang disimpan di folder `assets/`.
- Form kontak membuka aplikasi email pengunjung (`mailto:`), bukan mengirim ke server. Tentukan alamat email tujuan di `index.html` jika diperlukan.
- Dropdown destinasi mengarah ke bagian cerita/galeri yang tersedia, belum ke halaman detail terpisah.
