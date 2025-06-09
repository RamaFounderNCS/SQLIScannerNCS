# SQLIScannerNCS 🛡️

**Advanced SQL Injection Scanner with Modern UI/UX – Professional Edition**

---

## 🔍 Table of Contents

1. [Overview](#overview)  
2. [Features](#features)  
3. [Architecture & Design](#architecture--design)  
4. [Installation](#installation)  
5. [Usage](#usage)  
6. [Configuration](#configuration)  
7. [Customization & Extension](#customization--extension)  
8. [Screenshots](#screenshots)  
9. [Security & Auth](#security--auth)  
10. [Contributing](#contributing)  
11. [Licensing](#licensing)  
12. [Contact & Support](#contact--support)  

---

## Overview

**SQLIScannerNCS** adalah aplikasi canggih untuk mendeteksi dan menganalisis potensi **SQL Injection** pada target web. Didesain dengan UI/UX modern premium, sistem login aman, dan fitur lengkap sesuai standar internasional.

✅ **Built for professionals**: Penetration tester, security engineer, atau developer yang peduli keamanan.  
🎯 **Goals**:  
- Identifikasi celah SQL Injection laboratorium  
- Antarmuka premium, mudah digunakan  
- Dilengkapi sistem autentikasi dasar

---

## Features

- 🔗 **Multiple Injection Types**: Blind, Union-based, Boolean, Error-based  
- 🖥️ **Modern GUI Dashboard**  
- 🔐 **Secure Login**: Username/password (`admin` / `adminncs` default, bisa diubah)  
- 🧩 **Custom Payload Builder**  
- 🧪 **Scan Report & Log**: Ekspor ke format CSV/JSON  
- 🌐 **Batch Target Support**  
- ⚙️ **Pluggable Modules**: Mudah diperluas  
- 🔄 **Session Handling**: Cookies & Token Auth  

---

## Architecture & Design

```
Client (Web Browser)
     ↓ HTTPS
───────────────────────────────────
Server Backend (Flask / Django / Node.js)
 ├─ Auth Module (Login / Session)
 ├─ Scanner Engine (Injection Logic)
 ├─ Payload Manager
 ├─ Reporting Engine
 └─ API Endpoints
───────────────────────────────────
Database (SQLite / PostgreSQL)
```

- **Frontend**: HTML5 | CSS3 | JS (+Framework seperti React/Vue)  
- **Backend**: RESTful API + Engine Accuracy  
- **Database**: Penyimpanan user, scan history, logs  

---

## Installation

1. **Clone repo**  
   ```bash
   git clone https://github.com/RamaFounderNCS/SQLIScannerNCS.git
   cd SQLIScannerNCS
   ```

2. **Setup environment**  
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   pip install -r requirements.txt
   ```

3. **Inisialisasi DB**  
   ```bash
   flask db init
   flask db migrate -m "Init schema"
   flask db upgrade
   ```

4. **Set konfigurasi**  
   Salin `.env.example` ke `.env` dan update variabel (SECRET_KEY, DB URI)

5. **Run server**  
   ```bash
   flask run --host=0.0.0.0 --port=5000
   ```
   Buka `http://localhost:5000`, login dengan `admin:adminncs`.

---

## Usage

### 1. Login  
Masuk ke dashboard menggunakan `admin / adminncs`. **(Ganti kredensial setelah instalasi)**

### 2. Mulai Scan  
- Masukkan target URL dan metode HTTP (GET/POST)  
- Pilih jenis injeksi dan payload  
- Jalankan scan dan pantau progres  
- Lihat hasil langsung di interface

### 3. Ekspor Hasil  
Klik tombol **Export** untuk mendapatkan laporan CSV/JSON.

### 4. Batch Scan  
Unggah daftar target (`.txt`) dan jalankan scan otomatis untuk setiap target.

---

## Configuration

| Parameter           | Default         | Description                               |
|---------------------|------------------|-------------------------------------------|
| SECRET_KEY          | random           | Kunci enkripsi session pengguna           |
| DATABASE_URL        | sqlite:///data.db | Lokasi database                           |
| ADMIN_USERNAME      | admin            | Username admin default                    |
| ADMIN_PASSWORD      | adminncs         | Password admin default (GANTI SEGERA)     |

Update `.env` untuk mengamankan aplikasi.

---

## Customization & Extension

- **Payload Injector**: Tambahkan file `.json` di folder `/payloads`  
- **Module NewInjection**: Tambahkan modul Python baru di `/modules/`  
- **Frontend UI**: Ubah file HTML/CSS/JS di `/templates` dan `/static`  
- **Dockerfile**: Siapkan kontainer Docker untuk deploy mudah

---

## Screenshots

*(Tambahkan screenshot UI dashboard, halaman scan, laporan)*  

---

## Security & Auth

- Gunakan **HTTPS** untuk akses publik  
- Setelah instalasi, **ganti kredensial default**  
- Batasi IP dan gunakan **firewall / VPN**  
- Rekam **log aktivitas dan audit trails**

---

## Contributing

1. Fork repository  
2. Buat branch fitur: `feature/nama-fitur`  
3. Commit dan push ke remote  
4. Buat Pull Request, sertakan detail dan test  
5. Diharapkan: penambahan modul terkait security & QA

---

## Licensing

Proyek ini dilindungi oleh [MIT License](LICENSE).

---

## Contact & Support

Untuk pertanyaan dan dukungan:  
📧 **rama@ncssecurity.com**  
📄 **GitHub Issues**: https://github.com/RamaFounderNCS/SQLIScannerNCS/issues

---

**Selamat mengamankan aplikasi Anda dengan SQLIScannerNCS!** 🎯
