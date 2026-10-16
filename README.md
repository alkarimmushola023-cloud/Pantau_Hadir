# Pantau Hadir — Sistem Absensi Pekerja Proyek

Aplikasi absensi berbasis web **100% client-side** (tanpa backend/server). Data disimpan di `localStorage` browser, sehingga bisa langsung dijalankan dengan membuka `index.html` atau di-hosting di **GitHub Pages**, Netlify, Vercel, dll.

## Cara Menjalankan

1. Upload seluruh folder ini ke repository GitHub.
2. Aktifkan **GitHub Pages** (Settings → Pages → deploy from branch `main` / root).
3. Buka URL Pages yang diberikan.

> Catatan: fitur **kamera & GPS** hanya aktif di koneksi **HTTPS** (GitHub Pages sudah HTTPS) atau `localhost`. Jika dibuka langsung via `file://`, kamera tidak akan aktif tapi absen tetap bisa dilakukan tanpa foto.

## Akun Demo (sudah ter-seed otomatis saat pertama dibuka)

### Admin
| Field | Nilai |
|---|---|
| ID Perusahaan | `PTJB01` |
| ID Pengguna | `admin` |
| Kata Sandi | `admin123` |

### Pekerja (20 akun)
| Field | Nilai |
|---|---|
| ID Perusahaan | `PTJB01` |
| NIK | `P0001` s.d. `P0020` |
| Kata Sandi | `123456` |

Data awal berisi 20 pekerja + riwayat absensi 14 hari terakhir. Untuk mereset ke data awal, hapus storage situs di browser (DevTools → Application → Local Storage → Clear).

## Fitur

**Admin:**
- Dashboard dengan statistik real-time (total pekerja, hadir, terlambat, alpha) + grafik tren 7 hari + jam live.
- Data Pekerja: tambah, edit, hapus, cari, filter lokasi, pagination, ekspor CSV.
- Rekapitulasi Absensi: filter nama/tanggal/status, lihat bukti foto, ekspor CSV, cetak (print).

**Pekerja:**
- Login dengan NIK.
- Absen masuk & pulang dengan selfie (kamera depan) + lokasi GPS.
- Status keterlambatan otomatis (batas masuk 07:30).
- Riwayat absensi pribadi.

## Struktur File

```
index.html                  — Landing page (pilih role)
admin-login.html            — Login admin
pekerja-login.html          — Login pekerja
admin-dashboard.html        — Dashboard admin
data-pekerja.html           — CRUD data pekerja
tambah-pekerja.html         — Form tambah/edit pekerja
rekapitulasi-absensi.html   — Rekap & filter absensi
pekerja-dashboard.html      — Absen selfie pekerja
absen-sukses.html           — Konfirmasi absen berhasil
error.html                  — Halaman error 404
assets/css/style.css        — Stylesheet bersama (desain modern)
assets/js/app.js            — Logika aplikasi (database localStorage)
```

## Hak Cipta
© 2026 Pantau Hadir — Sistem Absensi Pekerja Proyek.
