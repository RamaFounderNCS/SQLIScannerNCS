---
title: "[Bug] Logout tidak menghapus session cookie"
labels: [bug, auth]
---

## Deskripsi
Setelah klik logout, user masih bisa mengakses dashboard lewat URL langsung.

## Langkah Reproduksi
1. Login sebagai admin
2. Klik logout
3. Akses ulang /dashboard

## Expected
Session harus dihancurkan saat logout.

---
