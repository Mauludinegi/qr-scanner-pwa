# QR Code Scanner PWA (Ringan & Cepat untuk Android / Web)

Aplikasi Web Progresif (PWA) untuk scan QR code yang dirancang seringan mungkin tanpa build tool yang berat, langsung siap pakai dan bisa di-install ke layar utama Android (Add to Home screen / Install App).

## ✨ Fitur Utama
1. **PWA Standalone & Offline Ready**: Menggunakan Service Worker & Web App Manifest.
2. **Ringan & Cepat**: Tanpa framework berlebih, menggunakan `html5-qrcode` yang cepat dan hemat baterai.
3. **Dukungan Kamera Android Lengkap**:
   - Deteksi kamera otomatis (default: kamera belakang).
   - Tombol **Putar Kamera** (depan/belakang).
   - Tombol **Flash / Torch** untuk kondisi minim cahaya (jika didukung perangkat).
4. **Scan dari Galeri / Gambar**: Bisa upload file foto QR code langsung.
5. **Feedback Interaktif**:
   - Animasi laser bidik real-time.
   - Suara beep & getaran haptic saat scan berhasil.
6. **Aksi Cepat Hasil Scan**:
   - Deteksi otomatis link URL -> Tombol "Buka URL".
   - Salin ke clipboard.
   - Web Share API (bisa langsung kirim ke WhatsApp, Telegram, dll).
   - Riwayat scan tersimpan di perangkat lokal (`localStorage`).

## 🚀 Cara Menjalankan

### Menggunakan Python (Lokal / Jaringan Wi-Fi):
Jalankan perintah ini di direktori project:
```bash
python3 -m http.server 8080 --bind 0.0.0.0
```

Lalu buka di browser:
- Di komputer: `http://localhost:8080`
- Di HP Android (dalam 1 jaringan Wi-Fi): `http://<IP-KOMPUTER-ANDA>:8080`

> **Catatan Izin Kamera di Android (HTTPS/Localhost):**
> Browser Android memerlukan konteks aman (**HTTPS** atau **localhost**) untuk mengizinkan akses kamera.
> - Jika ingin dicoba langsung dari HP Android secara leluasa, Anda bisa mendeploy folder ini ke penyedia hosting gratis seperti **Cloudflare Pages**, **Vercel**, **GitHub Pages**, atau **Firebase Hosting** (semuanya otomatis HTTPS gratis).
> - Di Android Chrome, setelah dibuka via HTTPS, klik menu titik tiga (⋮) -> pilih **"Install app"** / **"Tambahkan ke Layar Utama"**. Aplikasi akan menjadi seperti aplikasi native Android.
