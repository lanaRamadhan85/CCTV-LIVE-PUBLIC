# CCTV Monitoring System

Sebuah sistem pemantauan CCTV real-time berbasis web untuk Kota A. Aplikasi ini dibuat menggunakan HTML murni, Tailwind CSS untuk styling, dan HLS.js untuk memutar live streaming video.

## Fitur
- **Responsive Design**: Antarmuka pengguna yang dirancang khusus dengan Tailwind CSS agar tampil optimal di berbagai ukuran layar (desktop maupun mobile).
- **HLS Streaming**: Menggunakan pustaka *HLS.js* yang ringan dan andal untuk menampilkan aliran video *HTTP Live Streaming* (HLS).
- **Fullscreen Modal**: Modul tampilan penuh yang memungkinkan pengguna berfokus pada satu aliran video dalam ukuran yang leluasa.
- **Dynamic Configuration**: Dapat dengan mudah menambah, menghapus, atau mengedit data CCTV yang akan ditampilkan.

## Prasyarat
- Sebuah Web Browser modern (Google Chrome, Mozilla Firefox, Safari, Microsoft Edge).
- Koneksi internet (diperlukan untuk Tailwind CSS via CDN dan HLS.js via CDN).

## Struktur File
```
├── index.html       # File utama aplikasi web, memuat antarmuka & logika video player
├── assets/          
│   └── download.png # (File dihapus) Referensi placeholder gambar jika video/CCTV tidak dapat dimuat, dibiarkan di HTML namun file fisiknya telah dihapus.
```

## Cara Menjalankan Aplikasi
1. Clone atau unduh repositori ini ke komputer Anda.
2. Buka folder proyek (`CCTV WEB`).
3. Anda cukup melakukan klik ganda (double click) pada file `index.html` untuk membukanya di peramban web default Anda.

## Konfigurasi CCTV / URL Stream
Jika Anda ingin mengubah nama lokasi, daftar CCTV, atau URL *Live Stream*, silakan edit file `index.html`. Temukan bagian JavaScript berikut:

```javascript
// Array aliran CCTV
const cctvStreams = [
  { id: 'alamat-1', url: 'url 1' },
  { id: 'alamat-2', url: 'url 2' },
  // ... Tambahkan atau ubah data di sini
];
```
- Ubah `id` dengan format identifier yang unik.
- Ubah `url` dengan URL live streaming CCTV tujuan dengan format `.m3u8` (HLS format).

## Teknologi yang Digunakan
- **HTML5** & **JavaScript**: Sebagai kerangka utama dan logika fungsional aplikasi.
- **Tailwind CSS (CDN)**: Untuk mempercepat proses *styling* desain UI secara langsung dan elegan (Utility-First).
- **HLS.js (CDN)**: Pustaka JavaScript untuk memutar video HLS langsung di peramban.

## Lisensi
© CCTV Kota A 2026 | Instansi Terkait / Sistem Pemantauan CCTV Real-time
