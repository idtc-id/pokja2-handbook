# 02 — Alur Kerja Pilot

## 8 tahap pilot

| # | Tahap | Keluaran | Dokumen di repo pilot |
|---|---|---|---|
| 1 | Identifikasi pilot | Usulan pilot | Formulir usulan |
| 2 | Seleksi lokasi/mitra | Pilot terpilih & mitra berkomitmen | `docs/charter.md` (draf) |
| 3 | Perencanaan | Charter disetujui, KPI & baseline | `docs/charter.md`, `docs/kpi.md` |
| 4 | Integrasi data & teknologi | Arsitektur & pipeline data | `docs/arsitektur.md`, `data/catalog.yml` |
| 5 | Implementasi | MVP Digital Twin | `src/` |
| 6 | Pengujian | Hasil uji pengguna | `evaluation/uji-pengguna.md` |
| 7 | Evaluasi manfaat/dampak | Laporan dampak | `evaluation/laporan-dampak.md` |
| 8 | Dokumentasi & replikasi | Playbook replikasi | `playbook/` |

Setiap tahap punya **gerbang (gate)**: pilot lanjut ke tahap berikutnya setelah keluaran tahap sebelumnya ada di repo dan disetujui lead pilot + pemilik kasus.

## Ritme kerja

| Kegiatan | Frekuensi | Peserta | Keluaran |
|---|---|---|---|
| Sprint | 2 minggu | Tim pilot | Milestone GitHub tertutup |
| Sync tim pilot | 2 mingguan (30–45 menit) | Tim pilot | Notulen di `docs/notulen/` |
| Laporan ke Pokja | Bulanan | Lead pilot → pengurus | Update status 1 halaman |
| Diskusi rutin | 2 mingguan | Semua anggota | Rangkuman di `diskusi/` |
| Demo | Akhir siklus (±6 bulan) | Publik IDTC | Rekaman & materi |

## Board proyek

Setiap pilot memakai **GitHub Projects** (tampilan Board) dengan kolom:
`Backlog` → `Sprint ini` → `Dikerjakan` → `Review` → `Selesai`,
dan field **Tahap** (1–8) agar progres per tahap terlihat.

## Status pilot (laporan bulanan)

Gunakan format singkat:
- **Status**: 🟢 sesuai rencana / 🟡 ada hambatan / 🔴 terhambat
- **Capaian bulan ini**
- **Rencana bulan depan**
- **Hambatan & bantuan yang dibutuhkan**
