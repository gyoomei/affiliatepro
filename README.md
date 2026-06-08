# ⚡ AffiliatePro

### Brand-Powered Affiliate Post Generator — 74 Real Design Systems

Generate stunning affiliate product cards using design tokens extracted from 74 real-world brand websites. Pick a brand style, fill in your product details, and export HTML code or social media captions — all in a single zero-dependency HTML file.

[![Live Demo](https://img.shields.io/badge/Live-Demo-000?style=for-the-badge&logo=github)](https://gyoomei.github.io/affiliatepro/)
[![Try Now](https://img.shields.io/badge/Try-Now-6366f1?style=for-the-badge&logo=googlechrome)](https://gyoomei.github.io/affiliatepro/)
[![Brands](https://img.shields.io/badge/Brands-74-10b981?style=for-the-badge)](#brand-collection)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)

---

## 📖 The Problem

Creating affiliate product posts that look professional is tedious. You need matching colors, typography, responsive layouts, and proper disclosure — for every product, across every platform. Most tools give you generic templates that don't match any real brand's design language.

## ✨ How it works

```
You pick:     Linear design system
You fill:     Product name, price, image, affiliate link
You get:      Production-ready HTML card + social media caption
```

**That's the entire UX** — pick a brand, fill in details, export.

## 🎯 Core Features

| Capability | Detail |
|---|---|
| Brand Design Systems | 74 real brands (Stripe, Linear, Vercel, Tesla, Nike, Spotify...) |
| Card Layouts | 4 layouts: Vertical, Horizontal, Minimal, Featured |
| HTML Export | Copy-paste ready responsive HTML code |
| Social Captions | Auto-generated captions with hashtags and affiliate disclosure |
| Price Display | Sale price, original price, automatic discount % badge |
| Dark/Light Theme | Toggle between dark and light app themes |
| Save Products | localStorage persistence for quick access |
| Brand Search | Filter brands by name instantly |

## 🏗️ Architecture

```
┌─────────────────────────────────────────────┐
│  Brand Tokens → Card Template → HTML Export  │
│  (74 brands)   (4 layouts)    (clipboard)    │
└─────────────────────────────────────────────┘
```

## 💡 Architecture Decisions

**Why single HTML?** Zero build step, zero dependencies. Opens in any browser, deploys anywhere — GitHub Pages, Netlify, or just a file:// URL.

**Why client-side only?** No server needed. All brand tokens are embedded in JS. localStorage for persistence. No API keys, no tracking.

**Why 74 brand tokens?** Real design systems produce better-looking cards than generic templates. Linear's near-black canvas + lavender accent reads completely different from Stripe's navy + indigo gradient.

## 🧪 Try these examples

| Brand | Product | Layout |
|---|---|---|
| Linear | SaaS subscription | Vertical |
| Stripe | Payment terminal | Horizontal |
| Tesla | Model Y referral | Featured |
| Nike | Running shoes | Minimal |
| Spotify | Premium gift card | Vertical |

## 🛠️ Stack

- **Frontend:** Vanilla JavaScript, single HTML file (~38KB)
- **Design Tokens:** Extracted from [VoltAgent/awesome-design-md](https://github.com/VoltAgent/awesome-design-md) (88K+ stars)
- **Fonts:** [Sora](https://fonts.google.com/specimen/Sora) + [Nunito](https://fonts.google.com/specimen/Nunito) + [JetBrains Mono](https://fonts.google.com/specimen/JetBrains+Mono)
- **Storage:** localStorage for saved products
- **Hosting:** GitHub Pages (zero infra cost)

## 🚀 Quick Start

```bash
git clone https://github.com/gyoomei/affiliatepro.git
open affiliatepro/index.html
```

## 📄 License

MIT — Use freely for personal and commercial projects.

---

**Design tokens from [VoltAgent/awesome-design-md](https://github.com/VoltAgent/awesome-design-md) · 74 brands · Single HTML · Zero dependencies**
