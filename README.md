# Jelajah Sejarah Malang — versi statis

Website ini sudah diubah dari Laravel/PHP menjadi HTML, CSS, dan JavaScript statis sehingga bisa di-host gratis dengan GitHub Pages. Tidak membutuhkan PHP, Composer, database, atau proses build.

## Isi folder
- `index.html` — halaman utama
- `tempat/<slug>/index.html` — halaman detail setiap tempat
- `css/map.css` — stylesheet dari proyek asli
- `gambar/` — gambar tempat sejarah

## Cara deploy ke GitHub Pages
1. Buat repository GitHub baru.
2. Ekstrak ZIP ini, lalu unggah **isi folder** ini ke root repository (pastikan `index.html` berada di root, bukan di dalam folder lain).
3. Buka **Settings → Pages**.
4. Pada **Build and deployment**, pilih **Deploy from a branch**.
5. Pilih branch `main` dan folder `/(root)`, lalu tekan **Save**.
6. Tunggu proses deploy selesai. GitHub akan menampilkan URL website.

Semua tautan internal menggunakan path relatif sehingga mendukung URL GitHub Pages berbentuk `https://username.github.io/nama-repo/`. Carousel memakai Swiper dari CDN; jika internet/CDN tidak tersedia, gambar tetap dapat dibuka melalui daftar tempat di bawahnya.

## Catatan
Versi ini mempertahankan tiga tempat dan isi utamanya. Fungsi backend Laravel telah dihilangkan. Untuk menambah tempat, buat halaman detail baru di `tempat/<slug>/index.html` dan tambahkan kartu/slide di `index.html`.
