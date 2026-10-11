# Fastender - PHP Native Multi-Page

Konversi dari file Fastender HTML asli menjadi struktur multi-page PHP. Tampilan dan data demo mengikuti file HTML referensi, dengan penyesuaian interaksi untuk halaman PHP. Hash routing `#/...` diganti menjadi file PHP nyata.

## Struktur
- index.php — Beranda
- katalog.php — Katalog
- detail.php — Detail produk (`detail.php?id=0`, dst.)
- keranjang.php — Keranjang
- pemesanan.php / po.php — Form pemesanan (po.php alias untuk kompatibilitas tautan)
- lacak.php — Status pesanan
- login.php — Login admin
- admin.php — Dashboard admin
- includes/header.php — head + app container
- includes/footer.php — penutup dokumen
- includes/config.php — konfigurasi DB opsional
- assets/css/style.css — seluruh CSS dari file asli
- assets/js/app.js — seluruh JavaScript/data/fungsi dari file asli yang sudah disesuaikan untuk multi-page

## Cara menjalankan
1. Taruh folder `Fastender_PHP_Native` di `htdocs` XAMPP.
2. Jalankan Apache.
3. Buka `http://localhost/Fastender_PHP_Native/`.
4. Jangan membuka file `.php` dengan double-click; PHP harus dijalankan melalui Apache/XAMPP.

Catatan: versi ini adalah tahap migrasi multi-page. Data demo masih dikelola oleh JavaScript/localStorage seperti file asli; database MySQL/PHP server-side belum diaktifkan. Filter ukuran, urutan terbaru/terlama, keranjang, detail produk, dan edit produk tersimpan di browser. Foto produk bisa diunggah lewat form admin; produk demo memakai ilustrasi kategori karena file HTML referensi tidak menyertakan foto produk asli.
