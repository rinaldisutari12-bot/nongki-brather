# Nongki Brother – Kasir + Pesan via QR

Kasir angkringan (GitHub Pages + Firebase). Tidak ada data penjualan atau password di repo ini.

- `index.html` – kasir (login, meja, bil, biaya, rekap harian/bulanan, QR meja, pesanan masuk dari pelanggan)
- `order.html` – halaman pelanggan (dibuka lewat QR meja)
- `firestore.rules` – aturan keamanan database (tempel di Firebase Console > Firestore > Rules)
- `firebase-config.js` – identitas proyek Firebase (publik, aman)

## Pasang
1. Firebase > Firestore > Rules: tempel isi `firestore.rules`, pastikan email di `isKasir()` = email akun kasir, klik Publish.
2. Firebase > Authentication > Settings > User actions: matikan "Enable create (sign-up)".
3. Firebase > Authentication > Settings > Authorized domains: tambahkan `rinaldisutari12-bot.github.io`.
4. GitHub repo > Settings > Pages > Deploy from branch `main` / root.
5. Buka `https://rinaldisutari12-bot.github.io/nongki-brather/`, login, isi Menu dan Meja, lalu Menu > Tampilkan QR > Cetak.
