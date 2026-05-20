# NezzDev — Ultimate Sales Manager

![Version](https://img.shields.io/badge/version-2.0-blue.svg)
![Language](https://img.shields.io/badge/language-HTML%2FCSS%2FJS-yellow.svg)
![Status](https://img.shields.io/badge/status-Active-green.svg)

NezzDev adalah aplikasi web modern untuk mengelola penjualan, transaksi, dan pre-order dengan antarmuka yang elegan, responsif, dan user-friendly.

## 🚀 Fitur Utama

### 📊 Dashboard Overview
- Statistik pendapatan tahunan dan bulanan
- Grafik penjualan bulanan interaktif dengan animasi
- Rata-rata transaksi dan pendapatan per bulan
- Daftar transaksi terbaru
- Status pre-order real-time dengan badge status

### 💳 Manajemen Transaksi
- Tambah transaksi penjualan dengan detail lengkap
- Kategori produk (Produk, Jasa, Langganan, Lainnya)
- Filter berdasarkan tahun, bulan, dan pencarian
- Laporan penjualan harian dengan detail per tanggal
- Tren penjualan semua tahun dengan area chart
- Catatan transaksi untuk informasi tambahan

### 📦 Manajemen Produk
- Tambah produk baru dengan harga dan stok
- Kategori produk yang dapat disesuaikan
- Tracking stok barang
- Pilihan produk quick-select di form transaksi
- Grid view untuk semua produk

### 🛒 Pre-Order Management
- Kelola pre-order dari pelanggan
- Catat nomor telepon/WhatsApp
- Status pembayaran (Pending/Lunas) dengan toggle cepat
- Catatan detail (alamat, varian, dll)
- Filter by status dan pencarian nama pembeli
- Statistik total PO, lunas, pending, dan nilai total

### 🎨 Tema & Personalisasi
- **3 Tema Pilihan:**
  - 💜 **Purple Haze** (Default) - Elegan & modern dengan aksen ungu
  - 🌸 **Pink Glamour** - Gaya feminin dengan palet pink
  - ⚫ **Midnight Black** - Minimalis & clean dengan theme hitam
- Pengaturan tema disimpan otomatis
- Dropdown menu untuk ganti tema cepat

### ⚙️ Fitur Teknis
- Auto-save setiap perubahan
- Penyimpanan data dengan LocalStorage
- Loading screen dengan animasi matrix
- Login screen dengan validasi UI
- Responsive sidebar navigation
- Toast notification untuk feedback user

## 📖 Cara Penggunaan

### 🔐 Login
1. Buka file `Data.html` di browser
2. Anda akan melihar layar login dengan animasi
3. Masukkan **ID Admin** dan **Password** (untuk demo, gunakan any value)
4. Klik tombol **"Masuk"** atau tekan Enter
5. Sistem akan loading dengan animated progress bar
6. Dashboard akan muncul setelah loading selesai

### 📊 Akses Dashboard
Dari sidebar kiri, klik menu:
- **Overview** - Lihat ringkasan penjualan & statistik
- **Transaksi** - Kelola transaksi dan produk
- **Daftar Pre-Order** - Kelola pre-order pelanggan

### ➕ Tambah Transaksi
1. Ke menu **Transaksi**
2. Buka form "Tambah Transaksi Baru"
3. Isi field:
   - **Nama Pembeli** - Nama pelanggan
   - **Pilih Produk** - Dropdown dari daftar produk
   - **Atau Ketik Manual** - Jika produk belum ada
   - **Jumlah (Rp)** - Nominal harga
   - **Tanggal Transaksi** - Pilih tanggal
   - **Kategori** - Jenis transaksi
4. Klik **Simpan Transaksi**
5. Notifikasi akan muncul, data otomatis tersimpan

### 📦 Tambah Produk
1. Ke menu **Transaksi** (scroll ke bawah)
2. Buka form "Tambah Produk Baru"
3. Isi field:
   - **Nama Produk** - Nama produk/layanan
   - **Harga (Rp)** - Harga satuan
   - **Kategori** - Tipe produk
   - **Stok** - Jumlah stok (opsional)
   - **Deskripsi** - Deskripsi singkat
4. Klik **Simpan Produk**
5. Produk akan muncul di grid view

### 🛒 Tambah Pre-Order
1. Ke menu **Daftar Pre-Order**
2. Buka form "Tambah Pre-Order Baru"
3. Isi field:
   - **Nama Pembeli** - Nama pelanggan
   - **No. Telepon / WA** - Nomor kontak
   - **Qty** - Jumlah barang
   - **Harga per Unit (Rp)** - Harga satuan
   - **Status Pembayaran** - Pending atau Lunas
   - **Catatan** - Detail order/pengiriman
4. Klik **Simpan Pre-Order**

### 📅 Filter & Laporan
- **Filter Tahun/Bulan** - Pilih tahun dan bulan untuk melihat data spesifik
- **Pencarian** - Type nama pembeli atau produk untuk filter real-time
- **Laporan Harian** - Pilih tanggal spesifik untuk laporan harian
- **Filter Pre-Order** - Filter by status (Lunas/Pending)

### 🎨 Ganti Tema
1. Klik tombol **"Theme"** di topbar kanan
2. Pilih tema dari dropdown:
   - Pink Glamour
   - Purple Haze
   - Midnight Black
3. Tema akan berubah langsung dan disimpan

## 🛠️ Teknologi

| Teknologi | Kegunaan |
|-----------|----------|
| **HTML5** | Struktur markup dan semantic elements |
| **CSS3** | Styling, animasi, grid/flex layout |
| **Vanilla JavaScript** | Logic, interaktivitas, DOM manipulation |
| **LocalStorage API** | Penyimpanan data persistent |
| **Canvas API** | Animasi background, chart drawing |
| **Fetch API** | (Potential) untuk koneksi backend |

## 💾 Penyimpanan Data

### LocalStorage
- Semua data disimpan di `localStorage.nz2_fixed`
- Format: JSON string
- Struktur data:
  ```javascript
  {
    sales: [...],      // Daftar transaksi
    preorders: [...],  // Daftar pre-order
    products: [...]    // Daftar produk
  }
  ```

### Durasi Penyimpanan
- **Persistent** sampai browser cache dihapus
- **Tidak tersimpan** jika menggunakan Private/Incognito mode
- Setiap perubahan otomatis di-save

> ��️ **Catatan**: Untuk production, gunakan backend database (Firebase, MongoDB, etc)

## 🎨 Fitur Desain

### Animasi & Visual
- ✨ Background dengan gradient blob yang bergerak dinamis
- 🌟 Particle animation floating yang smooth
- 📊 Bar chart dengan animasi grow effect
- 💫 Smooth panel transition (slideUp + fade in)
- ⚡ Loading screen dengan matrix effect
- 🔔 Toast notification dengan animated appearance
- 🎯 Hover effects pada semua element interaktif
- 📉 Area chart dengan gradient fill

### Color Scheme
| Elemen | Warna | Hex |
|--------|-------|-----|
| Primary Accent | Purple | `#7c5cfc` |
| Secondary Accent | Light Purple | `#a78bfa` |
| Accent (Teal) | Teal | `#2dd4bf` |
| Success (Green) | Green | `#4ade80` |
| Warning (Amber) | Amber | `#fbbf24` |
| Error (Red) | Red | `#f87171` |

### Responsive Design
- 📱 Dioptimalkan untuk desktop dengan sidebar fixed
- 🖥️ Layout fleksibel dengan CSS Grid & Flexbox
- 📐 Typography responsive dengan rem units
- 🎯 Touch-friendly buttons dan input fields
- 🔄 Sidebar dapat di-customize width

## 🔧 Fitur Lanjutan

### Laporan Harian
- Pilih tanggal spesifik dari date picker
- Lihat total pendapatan dan jumlah transaksi hari itu
- Detail per transaksi dengan avatar buyer
- Auto-hide jika tidak ada data

### Filter & Pencarian
- **Filter Tahun** - Data 2024, 2025, 2026
- **Filter Bulan** - 12 bulan dengan nama Indonesia
- **Pencarian Real-time** - Filter by buyer name, product, atau note
- **Filter Pre-Order by Status** - Tampilkan Lunas/Pending saja

### Statistik & Analitik
- Total pendapatan tahun ini
- Total transaksi semua waktu
- Rata-rata per transaksi
- Rata-rata per bulan
- Pre-order yang pending vs lunas
- Pendapatan bulan ini

### Chart & Visualisasi
- **Bar Chart Bulanan** - Pendapatan per bulan dengan hover tooltip
- **Area Chart Tren** - Penjualan semua tahun
- Gradient colors untuk visual appeal
- Interactive dengan data tips

## 📊 Struktur Data

### Sales Object
```javascript
{
  id: timestamp,
  buyer: "Nama Pembeli",
  product: "Nama Produk",
  amount: 150000,
  category: "Produk",
  note: "Catatan",
  date: "2025-05-20",
  month: 4,        // 0-11
  year: 2025
}
```

### PreOrder Object
```javascript
{
  id: timestamp,
  buyer: "Nama Pembeli",
  phone: "081234567890",
  product: "Nama Produk",
  qty: 5,
  price: 50000,
  status: "pending" | "paid",
  note: "Detail order"
}
```

### Product Object
```javascript
{
  id: timestamp,
  name: "Nama Produk",
  price: 150000,
  category: "Produk Fisik",
  stock: 10,
  desc: "Deskripsi"
}
```

## ⌨️ Shortcuts & Tips

| Aksi | Cara |
|------|------|
| Save Form | Klik tombol "Simpan" atau tekan Enter di input terakhir |
| Delete Item | Klik icon trash di tabel (dengan konfirmasi) |
| Clear Filter | Pilih "Semua" di dropdown filter |
| Search | Type di input pencarian, hasil real-time |
| Toggle PO Status | Klik checkbox di tabel pre-order |
| Change Theme | Klik tombol "Theme" di topbar |

## 🎯 Keyboard Navigation

- `Tab` - Navigate antar elemen
- `Enter` - Submit form atau activate button
- `Esc` - Close dropdown menu (if any)

## 📝 Catatan Penting

1. **Data Local Only** - Data hanya di browser, tidak ada cloud sync
2. **No Backend** - Ini adalah frontend-only application
3. **Login Mock** - Login screen hanya untuk UI, tidak validasi real
4. **Browser Support** - Tested di Chrome, Firefox, Safari, Edge terbaru
5. **Theme Persistent** - Pilihan tema disimpan di localStorage
6. **Auto-timestamp** - Setiap transaksi auto-timestamp saat di-save

## 🚀 Deployment

### Local
1. Buka file `Data.html` dengan double-click atau drag ke browser
2. Atau gunakan local server: `python -m http.server 8000`

### Online
- Upload `Data.html` ke hosting (Vercel, Netlify, GitHub Pages)
- File adalah single-page, cukup satu file HTML saja
- Browser harus support LocalStorage (semua browser modern support)

## 📧 Info Developer

- **Created by**: AkuOness
- **Version**: 2.0
- **Last Updated**: 2025
- **Repository**: https://github.com/AkuOness/NezzDev

## 📄 Lisensi

Proyek ini open source dan dapat digunakan untuk keperluan personal maupun komersial.

---

**Selamat menggunakan NezzDev! 🎉**

Untuk fitur lebih lanjut atau kontribusi, silakan fork repository dan submit pull request.
