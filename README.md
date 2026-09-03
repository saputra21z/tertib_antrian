# Tertib Antrian — situs web

Situs statis untuk aplikasi **Tertib Antrian** (Google Play). Dipublikasikan lewat
GitHub Pages.

## Struktur

| Halaman | File | URL (setelah publish) |
|---|---|---|
| Beranda | `index.html` | `https://<username>.github.io/<repo>/` |
| Kebijakan Privasi | `playstore/index.html` | `https://<username>.github.io/<repo>/playstore/` |
| Hapus Akun & Data | `hapus-akun.html` | `https://<username>.github.io/<repo>/hapus-akun.html` |

`style.css` dipakai bersama oleh ketiga halaman. `.nojekyll` mencegah GitHub
memproses file dengan Jekyll.

## Publikasi (GitHub Pages)

Dari folder `docs/` ini:

```bash
git remote add origin https://github.com/<username>/<repo>.git
git push -u origin main --force        # --force bila repo sudah punya commit lain
```

Lalu di repo GitHub: **Settings → Pages** → Source: **Deploy from a branch** →
Branch **main**, folder **/ (root)** → Save. Tunggu ±1 menit.

## Isi di Google Play Console

- **Kebijakan → Konten aplikasi → Kebijakan Privasi** → `https://<username>.github.io/<repo>/playstore/`
- **Keamanan Data → Delete account URL** → `https://<username>.github.io/<repo>/hapus-akun.html`

## Memperbarui

```bash
git add . && git commit -m "update" && git push
```
