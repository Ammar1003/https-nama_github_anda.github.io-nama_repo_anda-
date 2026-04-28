# 🛡 SY HalalTrack Dashboard

Sistem pengurusan sijil halal, latihan, dan kesihatan staf — hosted di GitHub Pages.

## 🌐 Pautan Website
Selepas setup, website anda akan tersedia di:
```
https://YOUR_GITHUB_USERNAME.github.io/YOUR_REPO_NAME/
```

---

## 📁 Struktur Fail

```
repo/
├── index.html    ← Dashboard utama (jangan ubah)
├── data.json     ← SEMUA DATA disimpan di sini (ini yang anda edit)
└── README.md     ← Panduan ini
```

---

## 🚀 Cara Setup (Buat Sekali Sahaja)

### Langkah 1 — Buat Akaun GitHub
Pergi ke [github.com](https://github.com) dan daftar akaun percuma.

### Langkah 2 — Buat Repository Baru
1. Klik butang **"New"** (hijau) di GitHub
2. Namakan repo: contoh `sy-halaltrack`
3. Pilih **Public** (supaya semua orang boleh akses)
4. Klik **"Create repository"**

### Langkah 3 — Upload Fail
1. Dalam repo baru anda, klik **"uploading an existing file"**
2. Drag & drop ketiga-tiga fail: `index.html`, `data.json`, `README.md`
3. Klik **"Commit changes"**

### Langkah 4 — Aktifkan GitHub Pages
1. Pergi ke **Settings** (tab atas repo)
2. Skrol ke bawah ke bahagian **"Pages"** (menu kiri)
3. Di bawah **"Branch"**, pilih `main` → folder `/root`
4. Klik **Save**
5. Tunggu 1-2 minit, website anda akan live!

### Langkah 5 — Kemaskini index.html
Buka `index.html` dan tukar 2 baris ini:
```javascript
const GITHUB_USER = 'YOUR_GITHUB_USERNAME';  // ← tukar kepada username GitHub anda
const GITHUB_REPO = 'YOUR_REPO_NAME';        // ← tukar kepada nama repo anda
const ADMIN_PASSWORD = 'admin123';           // ← tukar kepada kata laluan anda
```

Upload semula `index.html` ke GitHub.

---

## ✏️ Cara Kemaskini Data

### Cara A — Edit Terus di GitHub (Mudah)
1. Pergi ke repo GitHub anda
2. Klik fail `data.json`
3. Klik ikon **pensil** (Edit)
4. Edit data dalam format JSON
5. Klik **"Commit changes"**
6. Website akan update dalam beberapa saat

### Cara B — Guna Dashboard Admin (Lebih Mudah)
1. Buka website anda
2. Klik **"🔐 Log Masuk Admin"**
3. Masukkan kata laluan anda
4. Tambah / edit / padam rekod seperti biasa
5. Klik **"⬇ Export Data"** → **"Download data.json"**
6. Upload fail `data.json` yang baru ke GitHub (gantikan yang lama)

---

## 🔐 Keselamatan

| Pengguna | Boleh Buat Apa |
|----------|----------------|
| **Semua orang** | View dashboard, tengok data |
| **Admin (anda)** | Tambah, edit, padam rekod |

Kata laluan admin boleh ditukar dalam fail `index.html` pada baris:
```javascript
const ADMIN_PASSWORD = 'kata-laluan-baru-anda';
```

---

## ❓ Soalan Lazim

**Q: Data saya hilang selepas close browser?**
A: Perubahan yang dibuat dalam dashboard perlu di-export dan di-upload semula ke GitHub. Ikut Cara B di atas.

**Q: Website saya tidak update walaupun dah upload data.json baru?**
A: Tekan `Ctrl+Shift+R` untuk hard refresh browser. GitHub Pages mungkin ambil masa 1-2 minit untuk update.

**Q: Boleh ke tukar warna / logo?**
A: Ya, buka `index.html` dan edit bahagian CSS atau logo di bahagian `<header>`.
