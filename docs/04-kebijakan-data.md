# 04 — Kebijakan Data

## Prinsip

1. **Pemilik data menentukan.** Data mitra hanya dipakai sesuai izin tertulis pemiliknya.
2. **Git bukan tempat data besar.** Repo menyimpan metadata, skrip, sampel kecil, dan dokumentasi.
3. **Tercatat di katalog.** Setiap dataset yang dipakai pilot dicatat di `data/catalog.yml` repo pilot.

## Klasifikasi

| Kelas | Contoh | Boleh di repo public? | Penyimpanan |
|---|---|---|---|
| **Terbuka** | Data berlisensi terbuka, OSM, data yang sudah dipublikasikan | ✅ (jika kecil) | Repo / tautan sumber |
| **Terbatas** | Data mitra dengan izin terbatas | ❌ | Storage mitra/tim, akses per orang; repo private jika perlu |
| **Rahasia** | Data pribadi, infrastruktur vital, data yang dilarang dibagikan | ❌ | Tidak dibawa keluar sistem mitra |

## Ukuran file

- Repo: file ≤ **50 MB** (batas keras GitHub 100 MB per file).
- Sampel data untuk contoh/uji: kecil dan representatif.
- Data besar (LiDAR, point cloud, mesh, citra, model BIM penuh): simpan di storage (server mitra, cloud storage, dsb.) → catat tautan dan cara akses di katalog.

## Standar minimum metadata (`data/catalog.yml`)

```yaml
- id: lidar-kota-x-2025
  nama: Point cloud LiDAR Kota X
  pemilik: Bappeda Kota X
  kelas: terbatas            # terbuka | terbatas | rahasia
  lisensi: "Izin terbatas untuk pilot, surat no. ..."
  format: LAZ
  crs: EPSG:32750
  tahun: 2025
  ukuran: 120 GB
  lokasi: "Storage mitra — hubungi PIC data"
  pic: "Nama PIC"
  catatan: ""
```

## Lisensi

| Jenis | Lisensi default |
|---|---|
| Kode | MIT |
| Dokumentasi | CC BY 4.0 |
| Data | Mengikuti lisensi/izin pemilik data |

## Jika data sensitif terlanjur ter-upload

1. Segera hubungi pengurus.
2. Jangan hanya menghapus file — riwayat git masih menyimpannya. Pengurus akan membersihkan riwayat dan, bila perlu, menjadikan repo private sementara.
3. Beri tahu pemilik data.
