# 🧡 Jagonya Shopee — Affiliate Storefront

### Rekomendasi Produk Skincare, Makeup & Parfum Terbaik

Shopee affiliate product storefront dengan tampilan marketplace profesional. Product grid, flash sale, kategori filter, search, sort, dan SEO optimized. Single HTML, zero dependencies.

[![Live Demo](https://img.shields.io/badge/Live-Demo-ee4d2d?style=for-the-badge&logo=github)](https://gyoomei.github.io/affiliatepro/)
[![Try Now](https://img.shields.io/badge/Try-Now-ee4d2d?style=for-the-badge&logo=googlechrome)](https://gyoomei.github.io/affiliatepro/)
[![Products](https://img.shields.io/badge/Products-20+-10b981?style=for-the-badge)](#features)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)

---

## 📖 The Problem

Membuat halaman affiliate Shopee yang profesional biasanya butuh Next.js, Tailwind, dan hosting berbayar. Affiliate tools yang ada cuma generate card biasa — bukan storefront lengkap dengan kategori, flash sale, dan search.

## ✨ How it works

```
Buka:         https://gyoomei.github.io/affiliatepro/
Lihat:        Product grid dengan filter kategori
Search:       Cari produk favoritmu
Klik:         Langsung ke Shopee affiliate link
```

**That's the entire UX** — buka, cari, klik, beli.

## 🎯 Core Features

| Capability | Detail |
|---|---|
| Product Grid | Responsive grid dengan hover effect |
| Flash Sale | Countdown timer + horizontal scroll |
| Kategori | Skincare, Makeup, Parfum, Haircare |
| Search | Real-time product search |
| Sort | Rekomendasi, Terlaris, Terbaru, Harga ↑↓ |
| Discount Badge | Auto-hitung % OFF dari harga asli |
| Rating & Sold | Bintang + jumlah terjual |
| SEO | Schema.org, Open Graph, meta tags |
| Mobile | Fully responsive sampai 375px |
| Sidebar | Kategori sidebar + promo gratis ongkir |

## 🏗️ Architecture

```
┌────────────────────────────────────────────────┐
│  Header (Search) → Hero → Categories → Grid    │
│  Flash Sale → Sidebar → Sort → Product Cards   │
│  Trust Section → Footer → Schema.org JSON-LD   │
└────────────────────────────────────────────────┘
```

## 💡 Architecture Decisions

**Why single HTML?** Zero build step, zero dependencies. Deploy di GitHub Pages, Netlify, atau langsung buka file. SEO-friendly dengan meta tags dan structured data.

**Why Shopee style?** User Indonesia familiar dengan UI Shopee. Orange theme, product cards dengan rating + sold count, flash sale countdown — semua elemen yang bikin user trust dan klik.

**Why client-side?** Tidak perlu server. Data produk di-embed di JS. Ganti produk tinggal edit array PRODUCTS.

## 🧪 Customization

Edit array `PRODUCTS` di dalam `<script>` untuk menambah/mengubah produk:

```javascript
{
  name: "Nama Produk",
  img: "https://gambar-produk.jpg",  // kosongkan untuk placeholder
  price: 45000,                       // harga jual
  original: 60000,                    // harga asli (untuk hitung diskon)
  rating: 4.8,                        // rating bintang
  sold: 12000,                        // jumlah terjual
  category: "skincare",               // skincare|makeup|parfum|haircare
  link: "https://s.shopee.co.id/xxx", // Shopee affiliate link
  flash: true                         // tampilkan di Flash Sale
}
```

## 🛠️ Stack

- **Frontend:** Vanilla JavaScript, single HTML file (~25KB)
- **Font:** [Roboto](https://fonts.google.com/specimen/Roboto)
- **Colors:** Shopee Orange (#ee4d2d) + Red (#d0011b)
- **SEO:** Schema.org JSON-LD, Open Graph, Twitter Cards
- **Hosting:** GitHub Pages (zero infra cost)

## 🚀 Quick Start

```bash
git clone https://github.com/gyoomei/affiliatepro.git
open affiliatepro/index.html
```

## 📄 License

MIT — Use freely for personal and commercial projects.

---

**Built with 🧡 for Shopee affiliates · Single HTML · Zero dependencies · SEO Optimized**
