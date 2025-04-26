# Atlantis Auto Swap Bot

🤖 Bot ini dirancang untuk mengotomatiskan perdagangan token pada AtlantisDEX di Monad testnet. Dengan skrip ini, Anda dapat melakukan swap token dengan mudah melalui antarmuka baris perintah (CLI).


## 🚀 Fitur
- **Otomatisasi Swap Token**: Swap token di AtlantisDEX dengan cepat dan mudah.
- **Pilihan Token**: Mendukung berbagai token seperti ATLANTIS, WETH, USDC, WMONAD, CHOG, MOLANDAK, MOYAKI, dan MONAD.
- **Estimasi Harga dan Gas**: Menampilkan estimasi jumlah token yang diterima dan biaya gas sebelum transaksi.
- **Keamanan Wallet**: Membaca kunci pribadi dari file `privatekeys.json` untuk menjaga keamanan.
- **Antarmuka CLI**: Input sederhana melalui terminal untuk memilih token dan jumlah swap.

## 🛠 Prasyarat
Sebelum menjalankan bot, pastikan Anda memiliki:
- [Node.js](https://nodejs.org/) terinstal (versi 16 atau lebih baru).
- Akun dengan saldo Monad di testnet.
- Kunci pribadi yang disimpan di file `privatekeys.json`.
- Dependensi Node.js seperti `ethers`, `axios`, `readline`, dan `fs`.

## 📦 Instalasi
Ikuti langkah-langkah berikut untuk mengatur proyek:

1. **Kloning Repositori**:
   ```bash
   git clone https://github.com/Yuurichan-N3/Atlantis-Auto-Swap.git
   cd Atlantis-Auto-Swap
   ```

2. **Instal Dependensi**:
   ```bash
   npm install ethers axios
   ```

3. **Buat File Konfigurasi**:
   Buat file `privatekeys.json` di direktori proyek dengan format berikut:
   ```json
   {
     "PRIVATE_KEY": "kunci_pribadi_anda"
   }
   ```
   **Catatan**: Jangan pernah bagikan kunci pribadi Anda!

4. **Jalankan Bot**:
   ```bash
   node bot.js
   ```

## 🖥 Penggunaan
1. Jalankan skrip dengan perintah `node bot.js`.
2. Ikuti petunjuk di terminal:
   - Pilih nomor token yang ingin dijual (1-8).
   - Pilih nomor token yang ingin dibeli (1-8).
   - Masukkan jumlah token yang akan di-swap (contoh: `0.99`).
3. Bot akan:
   - Memeriksa saldo wallet Anda.
   - Mengambil estimasi harga dari API AtlantisDEX.
   - Menampilkan ringkasan transaksi (jumlah token yang diterima dan biaya gas).
   - Mengeksekusi transaksi setelah konfirmasi.

## ⚠️ Peringatan
- **Gunakan di Testnet**: Bot ini dirancang untuk Monad testnet. Jangan gunakan di mainnet tanpa pengujian menyeluruh.
- **Keamanan**: Pastikan `privatekeys.json` aman dan tidak dibagikan.
- **Biaya Gas**: Pastikan saldo cukup untuk biaya gas dan transaksi.

## 📜 Lisensi
Script ini didistribusikan untuk keperluan pembelajaran dan pengujian. Penggunaan di luar tanggung jawab pengembang.

Untuk update terbaru, bergabunglah di grup **Telegram**: [Klik di sini](https://t.me/sentineldiscus).

## 💡 Disclaimer
Penggunaan bot ini sepenuhnya tanggung jawab pengguna. Kami tidak bertanggung jawab atas penyalahgunaan skrip ini.
