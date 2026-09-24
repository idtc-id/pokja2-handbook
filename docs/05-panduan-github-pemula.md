# 05 — Panduan GitHub untuk Pemula

Tidak perlu jadi programmer untuk berkontribusi. Sebagian besar kontribusi di Pokja 2 berupa **dokumen, data, dan diskusi** yang bisa dilakukan lewat browser.

## 1. Buat akun & bergabung

1. Daftar di <https://github.com/signup>.
2. Aktifkan **two-factor authentication** (Settings → Password and authentication).
3. Kirim **username** GitHub ke pengurus Pokja 2.
4. Terima undangan organisasi `idtc-id` melalui email atau <https://github.com/idtc-id>.

## 2. Istilah penting

| Istilah | Arti sederhana |
|---|---|
| **Repository (repo)** | Folder proyek beserta riwayat perubahannya |
| **Issue** | Catatan tugas, pertanyaan teknis, atau laporan masalah |
| **Discussion** | Forum tanya jawab dan ide |
| **Branch** | Salinan kerja agar perubahan tidak langsung mengubah versi utama |
| **Pull Request (PR)** | Usulan perubahan yang direview sebelum digabung |
| **Markdown (.md)** | Format teks sederhana untuk dokumen di GitHub |

## 3. Ikut diskusi

Buka repo `pokja2-handbook` → tab **Discussions** → pilih kategori → **New discussion**.

## 4. Membuat issue

Buka repo → tab **Issues** → **New issue** → pilih template → isi → **Submit**.

## 5. Mengedit dokumen lewat web (tanpa instal apa pun)

1. Buka file `.md` yang ingin diubah → klik ikon ✏️ (**Edit this file**).
2. Ubah teks. Klik **Preview** untuk melihat hasilnya.
3. Klik **Commit changes…** → pilih *Create a new branch… and start a pull request* → **Propose changes**.
4. Isi template PR → **Create pull request**. Reviewer akan memeriksa dan menggabungkan.

## 6. Mengunggah file kecil

Buka folder tujuan → **Add file → Upload files** → seret file → pilih *create a new branch* → **Propose changes**.
Ingat: file ≤ 50 MB dan patuhi [kebijakan data](04-kebijakan-data.md).

## 7. Dasar Markdown

```markdown
# Judul
## Subjudul
**tebal**, *miring*
- butir daftar
1. daftar bernomor
[teks tautan](https://contoh.id)
| Kolom 1 | Kolom 2 |
|---|---|
| isi | isi |
```

## 8. Untuk yang ingin memakai git di komputer

Gunakan **GitHub Desktop** (<https://desktop.github.com>) atau git CLI:
```bash
git clone https://github.com/idtc-id/<repo>.git
git checkout -b docs/perubahan-saya
# ... ubah file ...
git add .
git commit -m "Jelaskan perubahan"
git push -u origin docs/perubahan-saya
```
Lalu buka Pull Request di GitHub.
