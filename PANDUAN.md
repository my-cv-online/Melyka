# Panduan Setup Portfolio Melyka

## Struktur Folder Repo

```
repo-anda/
├── index.html              ← file utama (sudah selesai)
├── sitemap.xml             ← ganti YOUR-USERNAME & YOUR-REPO
├── robots.txt              ← ganti YOUR-USERNAME & YOUR-REPO
├── favicon.png             ← buat di favicon.io (huruf M, warna #f4a7b9)
├── apple-touch-icon.png    ← dari favicon.io
├── PANDUAN.md              ← hapus setelah selesai setup
└── assets/
    ├── photo-1.jpg         ← FOTO 1: Hero (portrait full body, 360×500px)
    ├── photo-2.jpg         ← FOTO 2: About (kasual/hangat, 300×400px)
    ├── photo-3.jpg         ← FOTO 3: Education (formal/rapi, 300×400px)
    ├── photo-4.jpg         ← FOTO 4: Contact (senyum, 300×420px)
    └── CV-Melyka.pdf       ← CV dalam format PDF
```

## Langkah Setup

### 1. Ganti placeholder di index.html
Cari & ganti semua teks berikut:
- `YOUR-USERNAME` → username GitHub Anda
- `YOUR-REPO`     → nama repo GitHub Anda
- `email@gmail.com`      → email asli Melyka
- `628XXXXXXXXXX`        → nomor WA asli (format internasional, tanpa +)
- `username_melyka`      → username Instagram asli

### 2. Ganti placeholder kontak di sitemap.xml & robots.txt
Sama seperti langkah 1.

### 3. Upload foto
Buat folder `assets/` di repo, lalu upload 4 foto portrait.
Cara ganti placeholder foto di index.html — cari komentar:
  ╔═══ FOTO 1 — HERO ═══╗
Hapus seluruh <div class="photo-placeholder">...</div>
Ganti dengan tag <img> sesuai instruksi di dalam komentar.

### 4. Buat Favicon
Buka https://favicon.io/favicon-generator/
- Text    : M
- Background: Rounded
- Font    : Plus Jakarta Sans / DM Sans
- Font Color: #FFFFFF
- BG Color  : #f4a7b9
- Font Size : 90

Download & upload favicon.png + apple-touch-icon.png ke root repo.

### 5. Commit & Push
```bash
git add .
git commit -m "feat(portfolio): initial release Melyka personal portfolio

- Add complete single-page portfolio with SEO optimization
- Add JSON-LD Person schema for Google rich results
- Add Open Graph and Twitter Card meta tags
- Add 6-section layout: Hero, About, Skills, Experience, Education, Contact
- Add custom soft feminine design system (rose/blush/sage palette)
- Add photo placeholders with clear replacement instructions
- Add scroll animations and custom cursor
- Add sitemap.xml and robots.txt"
git push origin main
```

### 6. Submit ke Google Search Console
- Buka: https://search.google.com/search-console
- Tambah property URL Anda
- Submit sitemap: https://YOUR-USERNAME.github.io/YOUR-REPO/sitemap.xml

