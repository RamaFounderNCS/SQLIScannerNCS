---
title: "[Bug] Scan tidak jalan ketika input menggunakan port URL"
labels: [bug, critical]
---

## Deskripsi
Scan tidak bekerja ketika URL target memiliki port custom seperti `http://target.com:8080`.

## Langkah Reproduksi
1. Masukkan URL: `http://testphp.vulnweb.com:8080`
2. Jalankan scan
3. Tidak ada respon

## Expected Result
Scan berjalan normal untuk URL dengan port.

---
