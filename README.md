# ZÉEN Studio — Website

Website company profile untuk **ZÉEN Studio** (formerly Batavia Studio).
Single-file static HTML + Tailwind CDN. Zero build, zero dependencies.

## 🚀 Deploy GRATIS (3 menit, no registrasi)

### Opsi 1: Netlify Drop (paling gampang — RECOMMENDED)
1. Buka **https://app.netlify.com/drop**
2. **Drag & drop folder `zeen-studio/`** ke halaman itu
3. Tunggu ~10 detik
4. Dapat URL live, misal: `https://zeen-studio-xyz.netlify.app`
5. Share URL ke klien/instagram 🎉

### Opsi 2: Vercel
1. Buka **https://vercel.com/new** → drag & drop folder `zeen-studio/`
2. Auto-detect static site → deploy
3. URL: `https://zeen-studio.vercel.app`

### Opsi 3: GitHub Pages
1. Buat repo baru → upload `index.html`
2. Settings → Pages → Deploy from `main` branch
3. URL: `https://username.github.io/zeen-studio/`

### Opsi 4: Cloudflare Pages
1. Buka **https://pages.cloudflare.com** → sign up free
2. Upload folder → deploy
3. URL: `https://zeen-studio.pages.dev`

## 🧪 Test Lokal

```bash
cd zeen-studio
python3 -m http.server 8000
# Buka http://localhost:8000
```

Atau double-click `index.html` (langsung buka di browser).

## ✏️ Yang Perlu Diganti Sebelum Live

Search-replace di `index.html` (semua `6281234567890` & `hello@zeenstudio.id` gampang banget):

| Placeholder | Ganti dengan | Lokasi |
|---|---|---|
| `6281234567890` (4 tempat) | No WhatsApp asli format `628xxx` | WA contact, floating button, footer, form submit |
| `hello@zeenstudio.id` | Email asli | Contact section, footer |
| `+62 812-3456-7890` | No WA format display | Contact section |
| `Jakarta, Indonesia` | Alamat studio lengkap | Contact section |
| `[HARGA]` (3 tempat) | Sesuai pricelist (misal `4.5`, `8`, `15`) | Pricing Bronze/Silver/Gold |
| `[Nama Klien]` / `[Nama Brand]` | Testimoni asli | Section Testimoni |
| Foto Unsplash (9 portfolio + 1 hero + 1 about) | Foto asli (upload ke `portfolio/` atau ImgBB/Cloudinary) | Section Hero, About, Portfolio |

> **Cari & replace cepet:** pakai Ctrl+H di code editor. Ganti `6281234567890` → nomor lo, semua beres.

## 🖼️ Cara Ganti Foto dengan Foto Sendiri

**Cara cepat (tetap URL):**
1. Upload foto ke **Cloudinary** atau **ImgBB** (instant, no signup)
2. Copy URL hasil upload
3. Replace URL Unsplash di `index.html`

**Cara proper (file lokal):**
1. Taruh foto di `portfolio/foto-1.jpg`, `portfolio/foto-2.jpg`, dst
2. Replace `https://images.unsplash.com/...` jadi `portfolio/foto-1.jpg`
3. Compress foto dulu di **https://tinypng.com** (max 300-500KB per foto)

## 🎨 Kustomisasi Cepat

**Warna** — Cari di `<script>tailwind.config = {...}`:
- `accent: '#c9a875'` → ganti ke warna brand lo (saat ini champagne gold)
- `base: '#0a0a0a'` → background utama
- `ink: '#f5f0e6'` → warna teks

**Font** — Link Google Fonts:
- Default: `Cormorant Garamond` (display/serif) + `Inter` (body)
- Alternatif: `Playfair Display` + `Manrope`

**Tagline** — Cari di hero: `Built from` & `meaning.`

## ✅ Checklist Sebelum Share

- [ ] Ganti WA `6281234567890` → no asli (4 tempat)
- [ ] Ganti email `hello@zeenstudio.id` → email asli
- [ ] Ganti `[HARGA]` di pricing → sesuai pricelist
- [ ] Ganti testimoni `[Nama Klien]` → nama asli
- [ ] Replace foto Unsplash (opsional, bisa nanti)
- [ ] Test mobile (DevTools → toggle device)
- [ ] Klik floating WA → pastikan link benar
- [ ] Test lightbox di portfolio
- [ ] Test form contact → submit → redirect ke WA

## 📐 Tech Stack

- HTML5 + Tailwind CSS (CDN) — zero build
- Vanilla JavaScript — no jQuery, no React, no libs
- Google Fonts (Cormorant Garamond + Inter)
- Unsplash placeholder images (replace dengan foto asli)
- Inline SVG favicon (zero asset)
- **File size:** ~40KB (super ringan, load < 1 detik)

## 🛠️ Struktur File

```
zeen-studio/
├── index.html        ← File utama (semua section di sini)
├── README.md         ← File ini
└── portfolio/        ← (opsional) taruh foto lokal di sini nanti
```

## 🌐 Custom Domain (Opsional, ~Rp 150rb/tahun)

1. Beli domain di **Namecheap** atau **Cloudflare Registrar** (lebih murah)
2. Di Netlify: **Site settings → Domain management → Add custom domain**
3. Ikuti instruksi update DNS
4. SSL otomatis (HTTPS) aktif dalam ~10 menit

---

Made with ✦ — *Built from meaning.*

<!-- trigger 1781364440 -->
