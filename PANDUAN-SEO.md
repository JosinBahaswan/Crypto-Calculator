# 🔍 Panduan Setup SEO + Google Search Console
## CryptoCalc — Langkah demi Langkah

---

## 📁 File yang Perlu Diupload ke Domain Kamu

| File | Upload ke | Keterangan |
|------|-----------|------------|
| `crypto-calculator.html` | `https://[DOMAIN]/crypto-calculator.html` | Halaman utama |
| `sitemap.xml` | `https://[DOMAIN]/sitemap.xml` | Peta halaman untuk Google |
| `robots.txt` | `https://[DOMAIN]/robots.txt` | Izin crawler |
| `og-image.png` *(buat sendiri)* | `https://[DOMAIN]/og-image.png` | Gambar preview share (1200×630px) |

---

## 🔧 STEP 1 — Ganti Semua `[DOMAIN]`

Buka ketiga file, lalu **cari & ganti** teks `[DOMAIN]` dengan domain aslimu.

**Contoh:**
```
https://[DOMAIN]/sitemap.xml  →  https://cryptocalc.id/sitemap.xml
```

---

## 🖼️ STEP 2 — Buat OG Image (Preview Share)

Buat gambar ukuran **1200 × 630 px** dengan:
- Background gelap (#050a0e)
- Teks besar: "CryptoCalc"
- Subtitle: "Kalkulator Kripto Gratis"
- Logo/ikon crypto

Tools gratis: **Canva**, **Figma**, atau **Adobe Express**
Simpan sebagai `og-image.png` lalu upload ke root domain.

---

## 🌐 STEP 3 — Daftarkan ke Google Search Console

### A. Tambahkan Property
1. Buka → https://search.google.com/search-console
2. Klik **"Add property"**
3. Pilih **"URL prefix"** → masukkan `https://[DOMAIN]/`
4. Klik **Continue**

### B. Verifikasi Domain
Pilih metode **"HTML tag"**:
1. Google akan memberikan kode seperti:
   ```html
   <meta name="google-site-verification" content="abcXYZ123...">
   ```
2. Buka file `crypto-calculator.html`
3. Cari baris:
   ```html
   <meta name="google-site-verification" content="GANTI_DENGAN_KODE_VERIFIKASI_GOOGLE_SEARCH_CONSOLE">
   ```
4. Ganti bagian `GANTI_DENGAN_KODE_VERIFIKASI_...` dengan kode dari Google
5. Upload ulang file ke server
6. Kembali ke Search Console → klik **"Verify"**

### C. Submit Sitemap
1. Di Search Console, klik menu **"Sitemaps"** (sidebar kiri)
2. Klik **"Add a new sitemap"**
3. Ketik: `sitemap.xml`
4. Klik **Submit**
5. Tunggu status berubah jadi ✅ **Success**

---

## ⏱️ STEP 4 — Request Indexing

1. Di Search Console → **URL Inspection**
2. Masukkan URL: `https://[DOMAIN]/crypto-calculator.html`
3. Klik **"Request Indexing"**
4. Google biasanya mengindex dalam **1–7 hari**

---

## ✅ Checklist SEO Lengkap

```
[ ] Semua [DOMAIN] sudah diganti
[ ] og-image.png sudah dibuat dan diupload (1200×630px)
[ ] robots.txt bisa diakses di browser
[ ] sitemap.xml bisa diakses di browser
[ ] Google Search Console: property ditambahkan
[ ] Google Search Console: verifikasi berhasil ✅
[ ] Google Search Console: sitemap disubmit ✅
[ ] URL inspection: indexing diminta
[ ] Favicon sudah ada (opsional tapi direkomendasikan)
```

---

## 📊 Meta Tags yang Sudah Tercakup

| Kategori | Tag | Status |
|----------|-----|--------|
| Basic SEO | title, description, keywords, robots | ✅ |
| Google | google-site-verification, canonical | ✅ |
| Open Graph | og:title, og:description, og:image, og:url | ✅ |
| Twitter/X | twitter:card, twitter:image, twitter:title | ✅ |
| Structured Data | WebApplication, WebPage, FAQPage (JSON-LD) | ✅ |
| Performance | preconnect fonts | ✅ |
| Sitemap | sitemap.xml dengan priority & changefreq | ✅ |
| Robots | robots.txt dengan sitemap pointer | ✅ |

---

## 🔑 Target Keyword

| Keyword | Volume (est.) | Kesulitan |
|---------|--------------|-----------|
| kalkulator kripto | Tinggi | Sedang |
| kalkulator solana staking | Sedang | Rendah |
| DCA crypto indonesia | Sedang | Rendah |
| profit loss crypto calculator | Sedang | Rendah |
| break even crypto | Rendah | Sangat Rendah |

> 💡 **Tip**: Tambahkan konten blog/artikel tentang "cara staking Solana" atau "strategi DCA crypto" untuk meningkatkan authority domain dan ranking keyword ekor panjang.

---

*Dibuat untuk CryptoCalc — All client-side, no backend required.*
