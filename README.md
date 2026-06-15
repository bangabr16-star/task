# TechSpark PWA

Isi folder ini sudah siap untuk dijadikan Progressive Web App (PWA).

## Cara pakai

1. Upload semua isi folder ini ke hosting HTTPS, misalnya GitHub Pages, Firebase Hosting, Vercel, Netlify, atau hosting biasa yang sudah SSL.
2. Buka `index.html` dari browser Chrome/Edge/Safari mobile.
3. Masuk ke Settings → Install App.
4. Kalau tombol install belum muncul, pakai menu browser: Add to Home screen / Install app.

## File penting

- `index.html` = aplikasi utama.
- `manifest.webmanifest` = identitas PWA, nama app, icon, warna, start URL.
- `service-worker.js` = cache offline dasar.
- `icons/` = icon aplikasi untuk Android/iOS.

## Catatan

- PWA tidak bisa aktif dari `file://` secara lokal. Harus lewat HTTPS atau localhost.
- Notifikasi versi ini tetap berjalan saat app terbuka. Untuk push notification saat app tertutup, perlu backend push notification.
- Data masih disimpan di `localStorage`, jadi gunakan fitur Backup Database sebelum pindah browser/perangkat.


## Alarm HP

Versi ini punya dua mode alarm:

1. Alarm in-app: bunyi/vibrate/popup saat TechSpark sedang terbuka.
2. Pasang Alarm HP: tombol jam di card task akan membuka aplikasi Clock/Alarm Android agar alarm tetap bunyi walaupun TechSpark tidak dibuka.

Catatan: browser/PWA tidak boleh memasang alarm sistem secara diam-diam. User tetap harus menekan tombol Pasang Alarm HP dan mengonfirmasi di aplikasi Clock/Alarm.
