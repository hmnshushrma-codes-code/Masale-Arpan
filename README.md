# 🌶 Masale Arpan — Pure Hand-Pounded Spices

> **Authentic Indian spices, crafted on our own machine, delivered fresh across India.**

![FSSAI](https://img.shields.io/badge/FSSAI-20826005001031-green?style=flat-square)
![Est](https://img.shields.io/badge/Established-April%202026-orange?style=flat-square)
![Location](https://img.shields.io/badge/Gurugram-Haryana%2C%20India-blue?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-lightgrey?style=flat-square)

---

## About

**Masale Arpan** is a small-batch, farm-to-kitchen spice brand based in Gurugram, Haryana. We built our own cold-pounding machine in-house, source raw spices directly from farms in Rajasthan, Kerala and Kashmir, and pack everything fresh — with zero fillers, no artificial colour, and no preservatives.

This repository contains the complete front-end website for our online store — a single-file HTML/CSS/JS app with full cart, address form, checkout, and WhatsApp/email ordering.

---

## Business Details

| Field | Details |
|---|---|
| **Brand** | Masale Arpan |
| **Established** | April 2026 |
| **Address** | 1040/31-A, Laxman Vihar Phase-1, Near Shiv Mandir, Gurugram, Haryana |
| **FSSAI Licence** | 20826005001031 |
| **Phone** | +91 92660 95118 |
| **Email** | arpanment@gmail.com |
| **WhatsApp** | [wa.me/919266095118](https://wa.me/919266095118) |

---

## Features

- **Product catalogue** — 9 products (Haldi, Coriander, Lal Mirch in 50g / 100g / 250g) with real product images
- **Category filter tabs** — filter by spice type
- **Cart** — add/remove items, live subtotal, delivery fee (free above ₹499)
- **Promo codes** — `MASALE10` (10% off), `WELCOME50` (₹50 off)
- **Full checkout form** with validation:
  - Name, 10-digit mobile, email
  - Flat, street, city, state (all Indian states), 6-digit PIN, landmark, delivery instructions
- **4 payment methods** — Cash on Delivery, UPI/GPay, Bank Transfer, WhatsApp Order
- **Order via email** — pre-filled `mailto:` to arpanment@gmail.com with full order details
- **Order via WhatsApp** — pre-filled message with cart and address to +91 92660 95118
- **Success screen** — order ID, delivery estimate, address confirmation, WhatsApp tracking link
- **About Us section** — our story, machine, FSSAI details
- **Responsive** — works on mobile and desktop
- **Floating WhatsApp button** — always visible

---

## File Structure

```
masale-arpan/
├── index.html        ← Main website (single file, self-contained)
├── logo.png          ← Brand logo (place your logo here)
└── README.md         ← This file
```

> **Note:** Place your logo file as `logo.png` in the root folder. The site will automatically use it in the navbar, About section, and footer. If the file is missing, it gracefully falls back to a spice emoji.

---

## Getting Started

### Run locally

Just open `index.html` in any browser — no build step, no dependencies, no server needed.

```bash
git clone https://github.com/YOUR_USERNAME/masale-arpan.git
cd masale-arpan
open index.html   # macOS
# or
start index.html  # Windows
```

### Deploy to GitHub Pages

1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/ (root)`
4. Your site will be live at `https://YOUR_USERNAME.github.io/masale-arpan`

### Deploy to Netlify (free, recommended)

1. Drag and drop the folder at [netlify.com/drop](https://app.netlify.com/drop)
2. Get an instant live URL — no account needed for basic deploy

---

## Customisation

All key values are at the top of the `<script>` block in `index.html`:

```js
const OWNER_EMAIL = 'arpanment@gmail.com';   // Order notification email
const WA_NUMBER   = '919266095118';           // WhatsApp number (no +, no spaces)
```

Products are in the `PRODUCTS` array — edit names, prices, images, and categories there.

Promo codes are in the `applyPromo()` function — add or change codes as needed.

---

## Tech Stack

| Layer | Choice |
|---|---|
| HTML | Semantic HTML5 |
| CSS | Custom properties, CSS Grid, Flexbox — no framework |
| JS | Vanilla ES6 — no libraries, no bundler |
| Fonts | Playfair Display + DM Sans (Google Fonts) |
| Images | Hosted on ibb.co (your product photos) |
| Orders | `mailto:` + WhatsApp deep link |

---

## Screenshots

> Add screenshots of your live site here after deployment.

---

## Roadmap

- [ ] Razorpay / UPI payment gateway integration
- [ ] Order tracking page
- [ ] Product review section
- [ ] WhatsApp Business API for automated order confirmation
- [ ] Inventory management

---

## Licence

MIT © 2026 Masale Arpan

---

*Built with ❤️ in Gurugram, Haryana*
