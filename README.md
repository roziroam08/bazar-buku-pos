# Kasir Bazar Buku (POS)

Aplikasi kasir (Point of Sale) untuk bazar buku. Frontend statis (HTML/CSS/JS) di GitHub Pages,
backend Google Apps Script + Google Sheets sebagai REST API.

## Fitur
- Login dengan peran Kasir dan Admin (token sesi, pengecekan peran di server)
- Kasir: cari produk, keranjang, diskon, Cash/QRIS/EDC, kembalian, struk cetak
- **Scan barcode ISBN** lewat kamera, scanner USB/Bluetooth, atau ketik ISBN
- Riwayat transaksi, katalog buku, periode bazar, laporan dan grafik, mode gelap
- Nomor transaksi atomik per hari: `INV/DDMMYY/P|N/XXXX`

## Struktur
```
index.html          halaman aplikasi
uji-barcode.html    10 barcode untuk uji coba scan
css/style.css       tema hijau toska
js/config.js        isi GAS_URL di sini
js/api.js           jembatan fetch ke Apps Script
js/scanner.js       scan barcode
js/app.js           logika aplikasi
img/                taruh login-bg.jpg (foto latar login)
```

Seluruh data pada demo ini fiktif.
