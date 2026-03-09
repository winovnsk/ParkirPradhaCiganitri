# Pradha Ciganitri Parking

Website penyewaan lahan parkir dengan integrasi Google Sheets & Google Drive.

## 🚀 Fitur

- ✅ **Login & Register** - Terintegrasi dengan Google Sheets
- ✅ **Cek Ketersediaan Lahan** - Real-time dari Google Sheets
- ✅ **Pemesanan Online** - Dengan upload bukti pembayaran ke Google Drive
- ✅ **Admin Dashboard** - Kelola semua data (unit, penyewa, pembayaran)
- ✅ **Export PDF Laporan** - Laporan keuangan per bulan
- ✅ **Sistem Ulasan** - Feedback dari pengguna
- ✅ **WhatsApp Integration** - Tombol chat langsung ke admin

## 💳 Informasi Pembayaran

| Metode | Detail |
|--------|--------|
| **BCA** | 4380082794 a.n Agung Wicaksono |
| **DANA** | 08568xxxx1 |
| **QRIS** | Hubungi Admin |

## 📋 Setup Google Sheets

### 1. Buat Google Apps Script

1. Buka [script.google.com](https://script.google.com)
2. Buat project baru
3. Copy kode dari file `google-apps-script-full.js` yang ada di folder `pradha-full/`
4. Ganti `SHEET_ID` dan `DRIVE_FOLDER_ID` dengan milik Anda:
   - Sheet ID: `1gpLgAkN0Vf5LsohxHoA8Hcrug_oLNBvE7ObIJc5oofY`
   - Drive Folder ID: `13bXPdfhUCsycid_svPfg2IQ-hpgp67Do`

### 2. Deploy Web App

1. Klik **Deploy** → **New deployment**
2. **Type**: Web app
3. **Execute as**: Me
4. **Who has access**: Anyone
5. Copy URL Web App

### 3. Update API URL

Edit file `assets/index-*.js` dan cari `API_URL`, ganti dengan URL Web App Anda.

### 4. Inisialisasi Sheets

Jalankan fungsi `initializeSystem()` di Google Apps Script untuk membuat sheet-sheet yang diperlukan.

## 📁 Struktur Sheet Google Sheets

1. **User Login** - Data pengguna (email, password, role)
2. **Data Peserta** - Data penyewa
3. **Laporan Keuangan** - Riwayat pembayaran
4. **Ketersediaan** - Status unit parkir
5. **Ulasan** - Review pengguna
6. **Pesan Masuk** - Formulir kontak

## 👤 Default Admin

- **Email**: admin@pradhaciganitri.com
- **Password**: admin123

## 🛠️ Deploy ke GitHub Pages

1. Upload semua file di folder ini ke repository GitHub Anda
2. Aktifkan GitHub Pages di Settings → Pages
3. Pilih branch `main` dan folder root `/`

## 📝 License

© 2026 Pradha Ciganitri Parking
