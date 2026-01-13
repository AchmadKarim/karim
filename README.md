```markdown
# CloudApp - LKS Cloud Computing 2026

Aplikasi web sederhana yang di-deploy ke layanan cloud computing untuk Lomba Kompetensi Siswa (LKS) SMK Ma'arif NU Tingkat Jawa Timur 2026.

## Informasi Peserta

| Item | Detail |
|------|--------|
| **Nama** | [NAMA LENGKAP PESERTA] |
| **No. Peserta** | [NOMOR PESERTA] |
| **Sekolah** | [NAMA SMK] |
| **Kompetensi** | [KOMPETENSI KEAHLIAN] |

## Deskripsi Aplikasi

CloudApp adalah aplikasi web yang mendemonstrasikan kemampuan dalam:
- Pembuatan halaman web dengan HTML5
- Desain responsif dengan CSS3
- Interaktivitas dengan JavaScript
- Integrasi dengan API publik
- Penyimpanan data lokal dengan LocalStorage
- Deployment ke layanan cloud (Vercel)

## Fitur Aplikasi

1. **Halaman Beranda**
   - Informasi tentang aplikasi
   - Fitur Quote of the Day (data dari API)
   - Fitur Catatan Sederhana (CRUD)

2. **Halaman About**
   - Profil pembuat
   - Keahlian yang digunakan
   - Informasi tentang aplikasi

3. **Fitur Tambahan**
   - Fetch data dari API publik (quotable.io)
   - CRUD dengan LocalStorage
   - Logging untuk monitoring

## Struktur Folder

```
lks-cloud-001/
├── assets/
│   └── images/          # Folder untuk gambar
├── css/
│   └── style.css        # File stylesheet
├── js/
│   └── app.js           # File JavaScript
├── index.html           # Halaman beranda
├── about.html           # Halaman tentang
├── .gitignore           # File untuk ignore git
└── README.md            # Dokumentasi (file ini)
```

## Teknologi yang Digunakan

- **HTML5** - Struktur halaman
- **CSS3** - Styling dan responsive design
- **JavaScript (ES6+)** - Interaktivitas dan logic
- **LocalStorage API** - Penyimpanan data lokal
- **Fetch API** - Mengambil data dari server
- **Git & GitHub** - Version control
- **Vercel** - Cloud deployment platform

## Cara Menjalankan Secara Lokal

### Metode 1: Langsung Buka di Browser
1. Download atau clone repository ini
2. Buka file `index.html` dengan browser (double-click)

### Metode 2: Menggunakan Live Server (VS Code)
1. Install extension "Live Server" di VS Code
2. Klik kanan pada `index.html`
3. Pilih "Open with Live Server"

### Metode 3: Menggunakan Python Simple Server
```bash
cd lks-cloud-001
python -m http.server 8000
```
Buka browser: `http://localhost:8000`

## Link Deployment

| Platform | URL |
|----------|-----|
| **Live App** | [https://lks-cloud-001.vercel.app](https://lks-cloud-001.vercel.app) |
| **GitHub Repo** | [https://github.com/username/lks-cloud-001](https://github.com/username/lks-cloud-001) |

## Screenshots

### Halaman Beranda
![Beranda](assets/images/screenshot-beranda.png)

### Halaman About
![About](assets/images/screenshot-about.png)

## Kendala dan Solusi

| No | Kendala | Solusi |
|----|---------|--------|
| 1 | CORS error saat fetch API | Menggunakan API yang sudah support CORS (quotable.io) |
| 2 | Layout tidak responsif di mobile | Menambahkan media queries untuk berbagai ukuran layar |
| 3 | Data hilang saat refresh | Menggunakan LocalStorage untuk menyimpan data secara persisten |

## Lisensi

Dibuat untuk keperluan LKS Cloud Computing 2026.

---

&copy; 2026 - [NAMA PESERTA] - LKS Cloud Computing SMK Ma'arif NU Jawa Timur
```

---

## 7. UPLOAD KE GITHUB

### 7.1 Inisialisasi Git Repository

Buka **Terminal** di VS Code (Ctrl + `) atau **Command Prompt**, lalu jalankan perintah berikut:

```bash
# Pindah ke folder proyek
cd D:\lks-cloud-001

# Inisialisasi git repository
git init
```

**Output yang diharapkan:**
```
Initialized empty Git repository in D:/lks-cloud-001/.git/
```

### 7.2 Menambahkan Semua File

```bash
# Tambahkan semua file ke staging
git add .

# Cek status (opsional)
git status
```

**Output git status:**
```
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   .gitignore
        new file:   README.md
        new file:   about.html
        new file:   css/style.css
        new file:   index.html
        new file:   js/app.js
```

### 7.3 Membuat Commit Pertama

```bash
git commit -m "Initial commit: LKS Cloud Computing project"
```

**Output yang diharapkan:**
```
[main (root-commit) abc1234] Initial commit: LKS Cloud Computing project
 6 files changed, 800 insertions(+)
 create mode 100644 .gitignore
 create mode 100644 README.md
 create mode 100644 about.html
 create mode 100644 css/style.css
 create mode 100644 index.html
 create mode 100644 js/app.js
```

### 7.4 Membuat Repository di GitHub

1. Buka `https://github.com` dan login
2. Klik tombol **"+"** di pojok kanan atas
3. Pilih **"New repository"**
4. Isi form:
   - **Repository name:** `lks-cloud-001` (sesuai nama folder)
   - **Description:** `LKS Cloud Computing - SMK Ma'arif NU 2026`
   - **Visibility:** Public
   - **JANGAN centang** "Add a README file" (kita sudah punya)
5. Klik **"Create repository"**

### 7.5 Menghubungkan Local Repository ke GitHub

Setelah membuat repository di GitHub, akan muncul instruksi. Jalankan perintah berikut:

```bash
# Tambahkan remote origin (ganti USERNAME dengan username GitHub kamu)
git remote add origin https://github.com/USERNAME/lks-cloud-001.git

# Rename branch ke main (jika belum)
git branch -M main

# Push ke GitHub
git push -u origin main
```

**Jika diminta login:**
- Masukkan username GitHub
- Untuk password, gunakan **Personal Access Token** (bukan password biasa)

### 7.6 Membuat Personal Access Token (Jika Diperlukan)

1. Buka GitHub > Settings (klik foto profil > Settings)
2. Scroll ke bawah, klik **"Developer settings"**
3. Klik **"Personal access tokens"** > **"Tokens (classic)"**
4. Klik **"Generate new token"** > **"Generate new token (classic)"**
5. Isi:
   - **Note:** `Git CLI`
   - **Expiration:** 90 days (atau sesuai kebutuhan)
   - **Scopes:** Centang `repo`
6. Klik **"Generate token"**
7. **COPY TOKEN** (hanya ditampilkan sekali!)
8. Gunakan token ini sebagai password saat git push

### 7.7 Verifikasi Upload

1. Buka `https://github.com/USERNAME/lks-cloud-001`
2. Pastikan semua file sudah ter-upload:
   - `.gitignore`
   - `README.md`
   - `about.html`
   - `index.html`
   - `css/style.css`
   - `js/app.js`

---

## 8. DEPLOY KE VERCEL

### 8.1 Login ke Vercel

1. Buka `https://vercel.com`
2. Klik **"Log In"**
3. Pilih **"Continue with GitHub"**
4. Authorize Vercel jika diminta

### 8.2 Import Project

1. Di dashboard Vercel, klik **"Add New..."** > **"Project"**
2. Di bagian **"Import Git Repository"**, cari repository `lks-cloud-001`
3. Klik **"Import"** pada repository tersebut

### 8.3 Konfigurasi Project

Pada halaman konfigurasi:

| Setting | Nilai |
|---------|-------|
| **Project Name** | `lks-cloud-001` (otomatis terisi) |
| **Framework Preset** | Other |
| **Root Directory** | `./` (biarkan default) |
| **Build Command** | (kosongkan) |
| **Output Directory** | (kosongkan) |

4. Klik **"Deploy"**

### 8.4 Proses Deployment

1. Tunggu proses deployment (biasanya 30-60 detik)
2. Vercel akan menampilkan log proses build
3. Jika sukses, akan muncul preview website

### 8.5 Akses Website

Setelah deploy berhasil:

1. Klik **"Continue to Dashboard"**
2. Di bagian **"Domains"**, akan ada URL seperti:
   - `https://lks-cloud-001.vercel.app`
   - `https://lks-cloud-001-username.vercel.app`
3. Klik URL untuk membuka website
4. **COPY URL ini** untuk dokumentasi

### 8.6 Troubleshooting Deployment

**Masalah: Build Error**
- Pastikan tidak ada error di kode HTML/CSS/JS
- Cek apakah semua file sudah ter-push ke GitHub

**Masalah: 404 Not Found**
- Pastikan file `index.html` ada di root folder
- Cek nama file (case-sensitive)

**Masalah: CSS/JS tidak loading**
- Cek path di HTML (harus relatif: `css/style.css`, bukan `/css/style.css`)
- Pastikan struktur folder benar

---

## 9. MEMBUAT DOKUMENTASI

### 9.1 Screenshot Aplikasi

1. Buka website yang sudah di-deploy
2. Ambil screenshot:
   - **Screenshot 1:** Halaman Beranda (desktop)
   - **Screenshot 2:** Halaman About (desktop)
   - **Screenshot 3:** Tampilan Mobile (opsional, tekan F12 > toggle device toolbar)

3. Simpan screenshot di folder `assets/images/`:
   - `screenshot-beranda.png`
   - `screenshot-about.png`
   - `screenshot-mobile.png`

### 9.2 Template Dokumentasi PDF

Buat dokumen Word/Google Docs dengan format berikut, lalu export ke PDF:

---

**DOKUMENTASI PROYEK LKS CLOUD COMPUTING**

**HALAMAN SAMPUL**
```
LOMBA KOMPETENSI SISWA (LKS)
SMK MA'ARIF NU TINGKAT JAWA TIMUR 2026

BIDANG: CLOUD COMPUTING

DOKUMENTASI PROYEK

Nama: [NAMA LENGKAP]
No. Peserta: [NOMOR PESERTA]
Sekolah: [NAMA SMK]
```

---

**DAFTAR ISI**
1. Deskripsi Aplikasi
2. Fitur Aplikasi
3. Teknologi yang Digunakan
4. Struktur Folder
5. Langkah Deployment
6. Screenshot Aplikasi
7. Link Repository & Deploy
8. Kendala dan Solusi

---

**1. DESKRIPSI APLIKASI**

CloudApp adalah aplikasi web yang dibuat untuk memenuhi tugas LKS Cloud Computing. Aplikasi ini mendemonstrasikan kemampuan dalam pengembangan web dan deployment ke layanan cloud.

Tujuan aplikasi:
- Menampilkan informasi tentang pembuat
- Mendemonstrasikan integrasi dengan API publik
- Menyediakan fitur CRUD sederhana
- Menerapkan praktik keamanan dasar

---

**2. FITUR APLIKASI**

| No | Fitur | Deskripsi |
|----|-------|-----------|
| 1 | Halaman Beranda | Menampilkan informasi utama dan fitur aplikasi |
| 2 | Halaman About | Menampilkan profil pembuat |
| 3 | Quote of the Day | Mengambil quote dari API publik |
| 4 | Catatan Sederhana | CRUD menggunakan LocalStorage |
| 5 | Responsive Design | Tampilan menyesuaikan ukuran layar |
| 6 | Logging | Mencatat aktivitas aplikasi |

---

**3. TEKNOLOGI YANG DIGUNAKAN**

- HTML5: Struktur halaman web
- CSS3: Styling dan responsive design
- JavaScript ES6+: Interaktivitas dan logic aplikasi
- Git: Version control
- GitHub: Hosting repository
- Vercel: Cloud deployment platform
- LocalStorage API: Penyimpanan data lokal
- Fetch API: Mengambil data dari server

---

**4. STRUKTUR FOLDER**

```
lks-cloud-001/
├── assets/
│   └── images/
├── css/
│   └── style.css
├── js/
│   └── app.js
├── index.html
├── about.html
├── .gitignore
└── README.md
```

---

**5. LANGKAH DEPLOYMENT**

**Langkah 1: Persiapan**
- Install Git dan VS Code
- Buat akun GitHub dan Vercel

**Langkah 2: Membuat Proyek**
- Buat folder proyek dengan struktur yang benar
- Buat file HTML, CSS, dan JavaScript

**Langkah 3: Upload ke GitHub**
```bash
git init
git add .
git commit -m "Initial commit"
git remote add origin [URL_REPO]
git push -u origin main
```

**Langkah 4: Deploy ke Vercel**
- Login ke Vercel dengan GitHub
- Import repository
- Klik Deploy

**Langkah 5: Verifikasi**
- Akses URL yang diberikan Vercel
- Pastikan semua fitur berfungsi

---

**6. SCREENSHOT APLIKASI**

[Sisipkan Screenshot Beranda]
Gambar 1. Tampilan Halaman Beranda

[Sisipkan Screenshot About]
Gambar 2. Tampilan Halaman About

[Sisipkan Screenshot Mobile - Opsional]
Gambar 3. Tampilan Mobile

---

**7. LINK REPOSITORY & DEPLOY**

| Jenis | URL |
|-------|-----|
| GitHub Repository | https://github.com/[USERNAME]/lks-cloud-001 |
| Live Application | https://lks-cloud-001.vercel.app |

---

**8. KENDALA DAN SOLUSI**

**Kendala 1: CORS Error saat Fetch API**
- Deskripsi: Browser memblokir request ke API karena kebijakan CORS
- Solusi: Menggunakan API yang sudah mendukung CORS (quotable.io)

**Kendala 2: Layout Berantakan di Mobile**
- Deskripsi: Elemen-elemen tidak tertata rapi saat dibuka di HP
- Solusi: Menambahkan media queries untuk ukuran layar mobile

**Kendala 3: Data Catatan Hilang saat Refresh**
- Deskripsi: Data yang diinput hilang ketika halaman di-refresh
- Solusi: Menggunakan LocalStorage untuk menyimpan data secara persisten

**Kendala 4: Git Push Ditolak**
- Deskripsi: Tidak bisa push ke GitHub karena authentication error
- Solusi: Membuat Personal Access Token dan menggunakannya sebagai password

---

### 9.3 Export ke PDF

**Dari Microsoft Word:**
1. File > Save As
2. Pilih format PDF
3. Klik Save

**Dari Google Docs:**
1. File > Download
2. Pilih PDF Document (.pdf)

---

## 10. CHECKLIST AKHIR

### 10.1 Checklist File

| No | Item | Status |
|----|------|--------|
| 1 | `index.html` ada dan bisa dibuka | [ ] |
| 2 | `about.html` ada dan bisa dibuka | [ ] |
| 3 | `css/style.css` ada dan ter-link | [ ] |
| 4 | `js/app.js` ada dan ter-link | [ ] |
| 5 | `.gitignore` ada | [ ] |
| 6 | `README.md` ada dan lengkap | [ ] |
| 7 | Data peserta sudah diisi di about.html | [ ] |
| 8 | Data peserta sudah diisi di README.md | [ ] |

### 10.2 Checklist Fungsionalitas

| No | Item | Status |
|----|------|--------|
| 1 | Navigasi Beranda <-> About berfungsi | [ ] |
| 2 | Quote berhasil dimuat dari API | [ ] |
| 3 | Tombol "Quote Baru" berfungsi | [ ] |
| 4 | Bisa menambah catatan baru | [ ] |
| 5 | Bisa menghapus catatan | [ ] |
| 6 | Catatan tersimpan setelah refresh | [ ] |
| 7 | Tampilan responsif di mobile | [ ] |
| 8 | Console tidak ada error (kecuali log) | [ ] |

### 10.3 Checklist GitHub

| No | Item | Status |
|----|------|--------|
| 1 | Repository sudah dibuat | [ ] |
| 2 | Semua file sudah ter-push | [ ] |
| 3 | Repository bersifat Public | [ ] |
| 4 | README.md tampil dengan benar | [ ] |
| 5 | Tidak ada file sensitif ter-upload | [ ] |

### 10.4 Checklist Deployment

| No | Item | Status |
|----|------|--------|
| 1 | Website berhasil di-deploy | [ ] |
| 2 | URL bisa diakses publik | [ ] |
| 3 | HTTPS aktif (ada gembok) | [ ] |
| 4 | Semua halaman bisa dibuka | [ ] |
| 5 | CSS dan JS ter-load dengan benar | [ ] |
| 6 | Fitur API berfungsi | [ ] |
| 7 | Fitur CRUD berfungsi | [ ] |

### 10.5 Checklist Dokumentasi

| No | Item | Status |
|----|------|--------|
| 1 | Screenshot beranda ada | [ ] |
| 2 | Screenshot about ada | [ ] |
| 3 | Link GitHub dicantumkan | [ ] |
| 4 | Link deploy dicantumkan | [ ] |
| 5 | Langkah deployment ditulis | [ ] |
| 6 | Kendala & solusi ditulis (min 2) | [ ] |
| 7 | Dokumentasi sudah di-export ke PDF | [ ] |

---

## RINGKASAN PENILAIAN

| Kategori | Poin Max | Cara Mendapat Poin Penuh |
|----------|----------|--------------------------|
| **Fungsi Aplikasi Web** | 30 | Buat 2 halaman, navigasi berfungsi, responsif, ada fitur API/CRUD |
| **Kualitas Kode** | 15 | Struktur folder rapi, HTML valid, CSS tidak redundan |
| **Deployment Cloud** | 25 | Repo terhubung Vercel, deploy sukses, link bisa diakses |
| **Logging** | 5 | Implementasi console.log yang relevan |
| **Keamanan Dasar** | 5 | Ada .gitignore, tidak ada credential, HTTPS aktif |
| **Dokumentasi** | 15 | Deskripsi, langkah, screenshot, link, kendala |
| **Kerapian** | 5 | Ikuti semua instruksi, nama file benar |
| **TOTAL** | **100** | |

---

## TIPS SUKSES

1. **Kerjakan berurutan** - Ikuti langkah dari awal sampai akhir
2. **Test setiap tahap** - Jangan lanjut jika ada error
3. **Simpan sering** - Ctrl+S di VS Code
4. **Commit bertahap** - Jangan commit sekali di akhir
5. **Baca error message** - Pesan error biasanya memberitahu masalahnya
6. **Gunakan DevTools** - F12 di browser untuk debug
7. **Backup penting** - Copy folder proyek sebelum eksperimen
8. **Manajemen waktu** - Alokasikan waktu untuk setiap tahap

---

**SELAMAT MENGERJAKAN DAN SEMOGA SUKSES!**

---

*Dokumentasi ini dibuat untuk persiapan LKS Cloud Computing SMK Ma'arif NU Tingkat Jawa Timur 2026*
