# Catatan — folder ini adalah GitHub Profile README

Repo ini **wajib** bernama sama persis dengan username GitHub:
`fitrinuryatinningrum`. Kalau nama repo berbeda, README-nya tidak akan
muncul di halaman profil.

## Isi

| File | Keterangan |
|---|---|
| `README.md` | README profil yang tampil di github.com/fitrinuryatinningrum |
| `.github/workflows/snake.yml` | Workflow yang meng-generate animasi ular kontribusi |

## GitHub Actions

Repo ini sudah punya 1 workflow yang berjalan otomatis:

- **snake.yml** — meng-generate ulang animasi ular kontribusi (`Platane/snk`)
  setiap 6 jam, lalu mempublikasikannya ke branch `gh-pages` dan mengunggah
  SVG/GIF sebagai artifact.

Untuk menjalankan manual: **Actions → Generate contribution snake animation → Run workflow**

> Karena branch `gh-pages` dipakai workflow, jangan pakai branch itu untuk
> source code — cukup biarkan workflow yang menimpanya.

## Push ke GitHub

```powershell
cd C:\Users\sweet-potato\github-profile
git remote add origin https://github.com/fitrinuryatinningrum/fitrinuryatinningrum.git
git push -u origin main
```

## Sebelum publish

- [ ] Ganti URL LinkedIn di `README.md` (header + section "Let's Connect")
- [ ] Ganti link kartu Featured Projects ke URL repo masing-masing
- [ ] Sesuaikan persentase skill & progress bar sesuai kondisi terbaru