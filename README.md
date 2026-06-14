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
