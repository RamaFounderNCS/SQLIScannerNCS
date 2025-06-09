---
title: "[Feature] Tambahkan Auto-Detection Payload untuk SQL Injection"
labels: [enhancement, feature, security]
---

## Deskripsi
Tambahkan mekanisme deteksi otomatis terhadap jenis SQL Injection berdasarkan respon server (boolean, time-based, error-based, dll).

## Tujuan
- Mempermudah pengguna dalam memilih metode injeksi
- Meningkatkan akurasi pemindaian

## Solusi yang Diusulkan
Gunakan pendekatan berbasis pola respon dan delay waktu untuk klasifikasi otomatis.

## Tambahan
Tambahkan opsi toggle "Auto Detect" di UI.

---
