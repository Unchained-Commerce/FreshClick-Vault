

```markdown
# FreshClick Vault 🔓
### The AfriSphere Digital Wealth Store

> **A division of FreshClick Media** · Built for the AfriSphere · Powered by Traffic + Ads = Money

[![Pages](https://img.shields.io/badge/Pages-14_HTML-d4af37?style=flat-square&labelColor=0a0b0f)](.)
[![Books](https://img.shields.io/badge/Free_Books-6_Titles-4ade80?style=flat-square&labelColor=0a0b0f)](.)
[![Packages](https://img.shields.io/badge/Business_in_a_Box-4_Tiers-a78bfa?style=flat-square&labelColor=0a0b0f)](.)
[![License](https://img.shields.io/badge/License-Proprietary-ef4444?style=flat-square&labelColor=0a0b0f)](.)
[![Status](https://img.shields.io/badge/Status-Live-22c55e?style=flat-square&labelColor=0a0b0f)](.)

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Live Site](#-live-site)
- [Site Architecture](#-site-architecture)
- [File Structure](#-file-structure)
- [Page Reference](#-page-reference)
- [Product Catalog](#-product-catalog)
- [URL Parameter Reference](#-url-parameter-reference)
- [Technology Stack](#-technology-stack)
- [Google Apps Script Setup](#-google-apps-script-setup)
- [Email Delivery System](#-email-delivery-system)
- [Design System](#-design-system)
- [WhatsApp Integration](#-whatsapp-integration)
- [SEO Configuration](#-seo-configuration)
- [Deployment Guide](#-deployment-guide)
- [Customization Guide](#-customization-guide)
- [Contact & Support](#-contact--support)

---

## 🌍 Overview

**FreshClick Vault** is the e-commerce and content delivery arm of **FreshClick Media** — a digital publisher focused on teaching Africans to earn USD income online using free tools, free traffic, and strategic ad monetization.

### What This Site Does

| Function | Details |
|---|---|
| **Publishes** | 6 free digital books on African digital wealth |
| **Sells** | 4 "Business in a Box" packages ($27–$247) |
| **Captures** | Email addresses with Google Apps Script backend |
| **Delivers** | Free PDFs automatically via email |
| **Converts** | Free book readers into paid box customers |
| **Serves** | The entire AfriSphere (15+ countries documented) |

### The Core Formula

```
Traffic + Ads = Money
```

Every piece of content on this site teaches, demonstrates, or delivers this formula.

---

## 🔗 Live Site

```
https://freshclickmedia.github.io/freshclick-vault/
```

| Page | URL |
|---|---|
| Store Homepage | `/index.html` |
| Download Portal | `/download.html` |
| Success Page | `/success.html` |

---

## 🏗 Site Architecture

```
FreshClick Vault
│
├── 🏪 STORE (index.html)
│   ├── Hero + Stats
│   ├── Tab Filter (All / Books / Boxes)
│   ├── Free Books Section ──────────────────┐
│   └── Business in a Box Section ──────┐    │
│                                       │    │
├── 📚 FREE BOOK DETAIL PAGES           │    │
│   ├── Traffic Is The New Oil ◄────────┼────┘
│   ├── Pinterest Goldmine ◄────────────┤
│   ├── Adsterra Decoded ◄──────────────┤
│   ├── Blog Like a Lumora ◄────────────┤
│   ├── The Niche Finder ◄──────────────┤
│   ├── Currency Liberation ◄───────────┤
│   └── Complete Bundle ◄──────────────┘
│         │
│         └── All link to ──► download.html
│
├── 💼 BOX DETAIL PAGES
│   ├── Starter Box ($27) ◄─────────────┐
│   ├── Growth Box ($67) ◄──────────────┤
│   ├── Empire Box ($127) ◄─────────────┤
│   └── Mogul Box ($247) ◄─────────────┘
│         │
│         └── All order via ──► WhatsApp
│
├── 📥 DOWNLOAD PORTAL (download.html)
│   ├── Auto-detects book from ?book= param
│   ├── Shows 3D book cover
│   ├── Email capture form
│   ├── Google Apps Script → Sheet + Email
│   └── On submit ──► success.html
│
└── ✅ SUCCESS PAGE (success.html)
    ├── Auto-detects type (book/box) from ?type=
    ├── Book mode → green theme + spam notice + box upsell
    └── Box mode → gold theme + WA support + books cross-sell
```

---

## 📁 File Structure

```
freshclick-vault/
│
├── index.html                          # Store homepage
├── download.html                       # Universal email capture portal
├── success.html                        # Universal success/thank-you page
│
├── download-traffic-is-the-new-oil.html   # Book 1 detail page
├── download-pinterest-goldmine.html       # Book 2 detail page
├── download-adsterra-decoded.html         # Book 3 detail page
├── download-blog-like-a-lumora.html       # Book 4 detail page
├── download-niche-finder.html             # Book 5 detail page
├── download-currency-liberation.html      # Book 6 detail page
├── download-complete-bundle.html          # Bundle detail page
│
├── starter-box.html                    # Paid: Starter Box ($27)
├── growth-box.html                     # Paid: Growth Box ($67)
├── empire-box.html                     # Paid: Empire Box ($127)
├── mogul-box.html                      # Paid: Mogul Box ($247)
│
├── README.md                           # This file
│
├── assets/
│   ├── images/
│   │   ├── favicon.ico
│   │   ├── og-vault.jpg
│   │   ├── og-traffic-oil.jpg
│   │   ├── og-pinterest-goldmine.jpg
│   │   ├── og-adsterra-decoded.jpg
│   │   ├── og-blog-lumora.jpg
│   │   ├── og-niche-finder.jpg
│   │   ├── og-currency-liberation.jpg
│   │   ├── og-bundle.jpg
│   │   ├── og-starter-box.jpg
│   │   ├── og-growth-box.jpg
│   │   ├── og-empire-box.jpg
│   │   └── og-mogul-box.jpg
│   └── books/
│       ├── traffic-is-the-new-oil.pdf
│       ├── pinterest-goldmine.pdf
│       ├── adsterra-decoded.pdf
│       ├── blog-like-a-lumora.pdf
│       ├── niche-finder.pdf
│       ├── currency-liberation.pdf
│       └── freshclick-vault-complete-bundle.zip
│
└── google-apps-script/
    └── Code.gs                         # Email capture + delivery backend
```

---

## 📄 Page Reference

### Free Content Pages

| # | File | Book | Color Accent | Unique Sections |
|---|---|---|---|---|
| 1 | `download-traffic-is-the-new-oil.html` | Traffic Is The New Oil | Orange `#ea580c` | Formula box, 4 case studies, 6 audience cards |
| 2 | `download-pinterest-goldmine.html` | Pinterest Goldmine | Red `#ef4444` | Stats row (450M users), pin anatomy grid |
| 3 | `download-adsterra-decoded.html` | Adsterra Decoded | Blue `#3b82f6` | 6 ad format cards with revenue tier tags |
| 4 | `download-blog-like-a-lumora.html` | Blog Like a Lumora | Purple `#7c3aed` | 48hr timeline, 5 required pages checklist |
| 5 | `download-niche-finder.html` | The Niche Finder | Amber `#d97706` | 10 niche category cards, 4 data-point grid |
| 6 | `download-currency-liberation.html` | Currency Liberation | Green `#10b981` | 15-country grid, 6 payment rails |
| 7 | `download-complete-bundle.html` | Complete Bundle | Gold gradient | Interactive 6-book stack, reading order, learning paths |

### Paid Product Pages

| # | File | Product | Price | Color Accent | Notable Features |
|---|---|---|---|---|---|
| 8 | `starter-box.html` | Starter Box | $27 | Cyan `#22d3ee` | Minimal, entry-level, platform picker grid |
| 9 | `growth-box.html` | Growth Box | $67 | Green `#22c55e` | "Most Popular" banner, floating icon animation |
| 10 | `empire-box.html` | Empire Box | $127 | Purple `#a78bfa` | ROI calculator, rotating box animation, testimonials |
| 11 | `mogul-box.html` | Mogul Box | $247 | Gold `#d4af37` | Gold particle field, mentorship section, 4-point ROI |

### System Pages

| File | Purpose | Mode Detection |
|---|---|---|
| `download.html` | Email capture + PDF delivery | `?book=` URL parameter |
| `success.html` | Post-conversion confirmation | `?type=` + `?id=` + `?email=` / `?name=` |
| `index.html` | Store homepage | Tab filter (JS) |

---

## 🛍 Product Catalog

### Free Books

| # | ID | Title | Pages | Chapters | PDF |
|---|---|---|---|---|---|
| 1 | `traffic-is-the-new-oil` | Traffic Is The New Oil | — | 6 | `assets/books/traffic-is-the-new-oil.pdf` |
| 2 | `pinterest-goldmine` | Pinterest Goldmine | — | 8 | `assets/books/pinterest-goldmine.pdf` |
| 3 | `adsterra-decoded` | Adsterra Decoded | — | 7 | `assets/books/adsterra-decoded.pdf` |
| 4 | `blog-like-a-lumora` | Blog Like a Lumora | — | 9 | `assets/books/blog-like-a-lumora.pdf` |
| 5 | `niche-finder` | The Niche Finder | — | 6 | `assets/books/niche-finder.pdf` |
| 6 | `currency-liberation` | Currency Liberation | — | 10 | `assets/books/currency-liberation.pdf` |
| 7 | `complete-bundle` | The Complete Bundle | — | 48 total | `assets/books/freshclick-vault-complete-bundle.zip` |

### Business in a Box Packages

| Tier | ID | Price | Delivery | Socials | Posts | Key Differentiator |
|---|---|---|---|---|---|---|
| Starter | `starter-box` | $27 | 48hrs | 1 | — | Minimum viable business |
| Growth ⭐ | `growth-box` | $67 | 48-72hrs | 3 | 10 | Content + branding included |
| Empire | `empire-box` | $127 | 72hrs | 5 | 25 | Pinterest + 30-day support |
| Mogul | `mogul-box` | $247 | 5 days | 8 (all) | 50 | 60-day mentorship + strategy session |

### Upgrade Pricing (Credit System)

| From | To | Additional Cost |
|---|---|---|
| Starter → Growth | $27 → $67 | Pay $40 |
| Starter → Empire | $27 → $127 | Pay $100 |
| Starter → Mogul | $27 → $247 | Pay $220 |
| Growth → Empire | $67 → $127 | Pay $60 |
| Growth → Mogul | $67 → $247 | Pay $180 |
| Empire → Mogul | $127 → $247 | Pay $120 |

### Supported Social Platforms (Business in a Box)

| Platform | Starter | Growth | Empire | Mogul |
|---|---|---|---|---|
| 📌 Pinterest | Pick 1 | ✅ | ✅ | ✅ |
| 📓 Tumblr | Pick 1 | ✅ | ✅ | ✅ |
| 🐘 Mastodon | Pick 1 | Pick 1 | Pick 1 | ✅ |
| 👩‍💻 Dev.to | Pick 1 | Pick 1 | Pick 1 | ✅ |
| #️⃣ Hashnode | Pick 1 | Pick 1 | Pick 1 | ✅ |
| 🦋 Bluesky | Pick 1 | Pick 1 | ✅ | ✅ |
| ✈️ Telegram | Pick 1 | Pick 1 | ✅ | ✅ |
| 📢 Discord | Pick 1 | Pick 1 | Pick 1 | ✅ |

---

## 🔗 URL Parameter Reference

### `download.html` Parameters

| Parameter | Values | Description |
|---|---|---|
| `book` | See Book IDs below | Which book to show and deliver |

**Book IDs:**
```
traffic-is-the-new-oil
pinterest-goldmine
adsterra-decoded
blog-like-a-lumora
niche-finder
currency-liberation
complete-bundle
```

**Examples:**
```
download.html?book=traffic-is-the-new-oil
download.html?book=complete-bundle
download.html                             ← Shows dropdown selector
```

---

### `success.html` Parameters

| Parameter | Values | Required | Description |
|---|---|---|---|
| `type` | `book` or `box` | Yes | Determines page mode and theme |
| `id` | Product ID | Yes | Which product was acquired |
| `email` | Email address | Books only | Shown on confirmation card |
| `name` | First name | Optional | Personalized greeting |

**Example URLs:**
```
# Free Books
success.html?type=book&id=traffic-is-the-new-oil&email=chidi@gmail.com&name=Chidi
success.html?type=book&id=complete-bundle&email=amina@mail.com&name=Amina

# Business in a Box
success.html?type=box&id=starter-box&name=Kwame
success.html?type=box&id=growth-box&name=Blessing
success.html?type=box&id=empire-box&name=Tonderai
success.html?type=box&id=mogul-box&name=Brian
```

---

### Redirect from `download.html`

To redirect to `success.html` after form submission, update the `showSuccess()` function in `download.html`:

```javascript
// In download.html — replace showSuccess() body with:
function showSuccess(data) {
  var url = 'success.html'
    + '?type=book'
    + '&id=' + encodeURIComponent(data.bookId)
    + '&email=' + encodeURIComponent(data.email)
    + '&name=' + encodeURIComponent(data.firstName);
  window.location.href = url;
}
```

---

## ⚙️ Technology Stack

### Frontend

| Technology | Usage | Why |
|---|---|---|
| **HTML5** | Structure | Semantic, SEO-friendly |
| **CSS3** | All styling | Zero framework dependency |
| **Vanilla JavaScript** | All interactivity | No jQuery, no React, pure speed |
| **Google Fonts** | Typography | Plus Jakarta Sans + Space Grotesk |
| **CSS Custom Properties** | Design tokens | Easy theme customization |
| **Intersection Observer API** | Scroll animations | Performant, battery-friendly |
| **CSS Grid + Flexbox** | Layout | Modern, responsive |
| **CSS Animations** | UI polish | Hardware-accelerated |

### Backend

| Technology | Usage |
|---|---|
| **Google Apps Script** | Email capture, Sheet logging, PDF delivery |
| **Google Sheets** | Lead database |
| **Gmail API** (via Apps Script) | Email sending |
| **Google Drive** | PDF hosting |

### Hosting

| Platform | What's Hosted |
|---|---|
| **GitHub Pages** | All HTML/CSS/JS |
| **Google Drive** | PDF books |
| **Google Apps Script** | Backend API |

### Zero Dependencies

This site has **zero npm packages**, **zero node_modules**, **zero build steps**.

```bash
# To run locally:
open index.html
# That's it. No npm install. No webpack. No nothing.
```

---

## 📧 Google Apps Script Setup

### Step 1: Create Google Sheet

1. Go to [sheets.google.com](https://sheets.google.com)
2. Create a new spreadsheet
3. Name it: `FreshClick Vault Leads`
4. Create a sheet named `Leads`
5. **Copy the Sheet ID** from the URL:
   ```
   https://docs.google.com/spreadsheets/d/YOUR_SHEET_ID_HERE/edit
   ```

### Step 2: Create Apps Script Project

1. Go to [script.google.com](https://script.google.com)
2. Click `New Project`
3. Paste the code from `google-apps-script/Code.gs`
4. Update configuration at the top:

```javascript
var SHEET_ID = 'YOUR_GOOGLE_SHEET_ID_HERE';  // ← Your Sheet ID
var SHEET_NAME = 'Leads';
var SENDER_NAME = 'FreshClick Vault';
var REPLY_TO = 'FreshClickmedia@gmail.com';
```

### Step 3: Update PDF Links

```javascript
var PDF_LINKS = {
  'traffic-is-the-new-oil': {
    title: 'Traffic Is The New Oil',
    url: 'https://drive.google.com/uc?export=download&id=YOUR_GDRIVE_FILE_ID',
    emoji: '⛽'
  },
  // Repeat for all 7 books/bundle
};
```

**To get a Google Drive file ID:**
```
Upload PDF to Drive → Right-click → Get link → Share → Copy

URL looks like:
https://drive.google.com/file/d/1BxiMVs0XRA5nFMdKvBdBZjgmUUqptlbs/view

Your file ID: 1BxiMVs0XRA5nFMdKvBdBZjgmUUqptlbs
```

### Step 4: Deploy as Web App

1. Click `Deploy` → `New Deployment`
2. Select type: `Web App`
3. Set `Execute as`: `Me`
4. Set `Who has access`: `Anyone`
5. Click `Deploy`
6. **Copy the deployment URL**

### Step 5: Update `download.html`

```javascript
// In download.html, find and replace:
var GOOGLE_SCRIPT_URL = 'https://script.google.com/macros/s/YOUR_DEPLOYMENT_ID_HERE/exec';

// Replace with your actual deployment URL:
var GOOGLE_SCRIPT_URL = 'https://script.google.com/macros/s/AKfycbxXXXXXXXXXXXXXXXX/exec';
```

### Step 6: Test

```bash
# Test the endpoint manually:
curl -X POST "YOUR_SCRIPT_URL" \
  -H "Content-Type: application/json" \
  -d '{"firstName":"Test","email":"test@email.com","country":"Nigeria","bookId":"traffic-is-the-new-oil","bookTitle":"Traffic Is The New Oil"}'
```

---

## 📊 Email Delivery System

### Data Captured Per Lead

| Column | Data | Example |
|---|---|---|
| Timestamp | ISO 8601 | `2025-01-15T10:30:00Z` |
| First Name | String | `Chidi` |
| Last Name | String | `Okafor` |
| Email | String | `chidi@gmail.com` |
| Country | String | `Nigeria` |
| WhatsApp | String | `+234 800 000 0000` |
| Book ID | Slug | `traffic-is-the-new-oil` |
| Book Title | String | `Traffic Is The New Oil` |
| Source | URL | `https://...download.html?book=...` |
| Referrer | URL or `direct` | `https://google.com/` |

### Email Template Features

- HTML email with dark theme
- Book emoji + title + download button
- "Other books" cross-sell section
- Business in a Box WhatsApp upsell
- Unsubscribe instructions
- Mobile-responsive layout

### Flow

```
User fills form → fetch() to Apps Script → Apps Script:
  1. Saves to Google Sheet
  2. Sends HTML email with PDF link
  3. Returns success
→ download.html redirects to success.html
```

### `no-cors` Note

`download.html` uses `mode: 'no-cors'` for the fetch request because
Google Apps Script doesn't support CORS preflight. This means:

- The response is always "opaque" (can't read it)
- We assume success and redirect
- The Apps Script still executes correctly
- Email still gets sent

---

## 🎨 Design System

### Color Palette

```css
/* Brand */
--gold:       #d4af37   /* Primary brand color */
--gold-light: #f4d03f   /* Lighter gold */
--gold-dark:  #c27803   /* Darker gold */

/* Backgrounds */
--bg-primary:   #0a0b0f  /* Main background */
--bg-secondary: #0d1117  /* Secondary sections */
--bg-tertiary:  #111827  /* Tertiary sections */

/* Text */
--text-primary:   #e8e0d4  /* Main text */
--text-secondary: #b8a99a  /* Secondary text */
--text-muted:     #8a7e70  /* Muted text */
--text-dim:       #6b6358  /* Dim text */
--text-faint:     #4a4339  /* Faint text */

/* Accent (per page) */
--accent: varies per product page

/* Status */
--green:  #4ade80  /* Success, free, earnings */
--red:    #ef4444  /* Errors, Pinterest */
--blue:   #5b9bd5  /* Info, Adsterra */
--orange: #e8943a  /* Warning, Traffic */
--purple: #a78bfa  /* Empire, Blog */
--cyan:   #22d3ee  /* Starter */
```

### Per-Page Accent Colors

| Page | Accent | Hex |
|---|---|---|
| Traffic Is The New Oil | Orange | `#ea580c` |
| Pinterest Goldmine | Red | `#ef4444` |
| Adsterra Decoded | Blue | `#3b82f6` |
| Blog Like a Lumora | Purple | `#7c3aed` |
| The Niche Finder | Amber | `#d97706` |
| Currency Liberation | Emerald | `#10b981` |
| Complete Bundle | Gold | `#d4af37` |
| Starter Box | Cyan | `#22d3ee` |
| Growth Box | Green | `#22c55e` |
| Empire Box | Purple | `#a78bfa` |
| Mogul Box | Gold | `#d4af37` |
| Success (book) | Green | `#4ade80` |
| Success (box) | Gold | `#d4af37` |

### Typography

```css
/* Display / Headings */
font-family: 'Space Grotesk', sans-serif;
/* Weights: 400, 500, 600, 700 */

/* Body / UI */
font-family: 'Plus Jakarta Sans', sans-serif;
/* Weights: 300, 400, 500, 600, 700, 800 */
```

### Border Radius Scale

```css
--radius-sm:   6px    /* Buttons, tags */
--radius-md:   10px   /* Cards, inputs */
--radius-lg:   14px   /* Large cards */
--radius-xl:   20px   /* Hero boxes */
--radius-full: 50px   /* Pills, badges */
```

### Animation Classes

```css
.an               /* Fade up animation target */
.an.visible       /* Triggered by IntersectionObserver */
.d1               /* 0.1s delay */
.d2               /* 0.2s delay */
.d3               /* 0.3s delay */
.d4               /* 0.4s delay */
```

---

## 💬 WhatsApp Integration

All orders and inquiries go through WhatsApp. Pre-filled messages are used throughout.

### WhatsApp Number

```
+263 77 967 4212
```

### Pre-filled Message URLs

```
# General inquiry
https://wa.me/263779674212

# Starter Box order
https://wa.me/263779674212?text=Hi%20FreshClick%20Vault%2C%20I%20want%20to%20order%20the%20STARTER%20BOX%20(%2427).%20Please%20send%20payment%20details.

# Growth Box order
https://wa.me/263779674212?text=Hi%20FreshClick%20Vault%2C%20I%20want%20to%20order%20the%20GROWTH%20BOX%20(%2467).%20Please%20send%20details.

# Empire Box order
https://wa.me/263779674212?text=Hi%20FreshClick%20Vault%2C%20I%20want%20to%20order%20the%20EMPIRE%20BOX%20(%24127).%20Please%20send%20payment%20details%20and%20let%27s%20discuss%20my%20niche.

# Mogul Box order
https://wa.me/263779674212?text=Hi%20FreshClick%20Vault%2C%20I%20want%20to%20order%20the%20MOGUL%20BOX%20(%24247).%20I%27m%20ready%20to%20build%20my%20digital%20empire.

# Book download feedback
https://wa.me/263779674212?text=Hi%2C%20I%20just%20downloaded%20a%20book%20from%20FreshClick%20Vault!

# Business in a Box inquiry (after reading free book)
https://wa.me/263779674212?text=Hi%20FreshClick%20Vault%2C%20I%20just%20downloaded%20a%20free%20book%20and%20I%27m%20interested%20in%20Business%20in%20a%20Box.
```

### Payment Methods Accepted

| Method | Notes |
|---|---|
| USDT (TRC20) | Preferred — instant confirmation |
| USDT (BEP20) | Also accepted |
| Wise Transfer | For larger amounts |
| Payoneer | Where available |
| EcoCash | Zimbabwe |
| Bank Transfer | SWIFT — larger amounts |
| MTN MoMo | West Africa |

---

## 🔍 SEO Configuration

### Meta Tags (All Pages)

Every page includes:
- `<title>` — unique per page
- `<meta name="description">` — unique per page
- `<meta name="keywords">` — relevant per page
- `<meta name="robots" content="index, follow">` (except success.html)
- `<link rel="canonical">` — absolute URL per page

### Open Graph (Social Sharing)

Every page includes:
- `og:type`
- `og:url`
- `og:title`
- `og:description`
- `og:image` — unique per page (1200×630px recommended)
- `og:site_name`

### Twitter Cards

Every page includes:
- `twitter:card` — `summary_large_image`
- `twitter:title`
- `twitter:description`
- `twitter:image`

### Success Page

```html
<meta name="robots" content="noindex, nofollow">
```

The success page is intentionally excluded from search engines.

### OG Images Needed

Create `1200×630px` images for each:

```
assets/images/
├── og-vault.jpg              # Store homepage
├── og-traffic-oil.jpg        # Book 1
├── og-pinterest-goldmine.jpg # Book 2
├── og-adsterra-decoded.jpg   # Book 3
├── og-blog-lumora.jpg        # Book 4
├── og-niche-finder.jpg       # Book 5
├── og-currency-liberation.jpg # Book 6
├── og-bundle.jpg             # Bundle
├── og-starter-box.jpg        # Starter
├── og-growth-box.jpg         # Growth
├── og-empire-box.jpg         # Empire
└── og-mogul-box.jpg          # Mogul
```

---

## 🚀 Deployment Guide

### GitHub Pages (Recommended)

```bash
# 1. Fork or clone this repo
git clone https://github.com/yourusername/freshclick-vault.git
cd freshclick-vault

# 2. Make your changes (update URLs, WhatsApp number, etc.)

# 3. Push to GitHub
git add .
git commit -m "Initial FreshClick Vault deployment"
git push origin main

# 4. Enable GitHub Pages
# GitHub → Settings → Pages → Branch: main → Root → Save

# 5. Your site is live at:
# https://yourusername.github.io/freshclick-vault/
```

### Custom Domain

```bash
# 1. Add CNAME file to root
echo "vault.freshclickmedia.com" > CNAME
git add CNAME && git commit -m "Add custom domain" && git push

# 2. In your DNS provider, add:
# CNAME vault → yourusername.github.io
# or
# A records pointing to GitHub Pages IPs
```

### Pre-Deployment Checklist

```
□ Update WhatsApp number throughout
□ Update email address (FreshClickmedia@gmail.com)
□ Update GitHub username in all canonical URLs
□ Update og:url meta tags on all pages
□ Add real OG images (1200×630px)
□ Upload PDFs to Google Drive + get file IDs
□ Set up Google Sheet + Apps Script
□ Update GOOGLE_SCRIPT_URL in download.html
□ Update PDF_LINKS in Code.gs
□ Test email capture end-to-end
□ Test success page with all parameter combinations
□ Add favicon.ico
□ Test on mobile (iOS + Android)
□ Test all WhatsApp links
```

### Environment Variables (There Are None)

All configuration is hardcoded in the HTML files. Before deploying, do a global search-and-replace for:

| Placeholder | Replace With |
|---|---|
| `yourusername` | Your GitHub username |
| `263779674212` | Your WhatsApp number (no +, no spaces) |
| `FreshClickmedia@gmail.com` | Your email address |
| `YOUR_DEPLOYMENT_ID_HERE` | Your Apps Script deployment ID |
| `YOUR_GOOGLE_SHEET_ID_HERE` | Your Google Sheet ID |
| `YOUR_FILE_ID_1` through `YOUR_FILE_ID_BUNDLE` | Your Google Drive file IDs |

---

## 🛠 Customization Guide

### Change Brand Colors

In any HTML file, find the `:root` block and update:

```css
:root {
  --gold: #d4af37;       /* Change primary brand color */
  --gold-light: #f4d03f;
  --gold-dark: #c27803;
}
```

### Add a New Free Book

1. Create `download-your-new-book.html` using an existing book page as template
2. Add to `BOOKS` object in `download.html`:
```javascript
var BOOKS = {
  // ... existing books ...
  'your-new-book': {
    emoji: '🔥',
    title: 'Your New Book',
    subtitle: 'The Subtitle',
    meta: ['📄 PDF', '📖 X Chapters', '⚡ Fast Read'],
    coverGradient: 'linear-gradient(160deg, #your, #colors, #here)',
    spineGradient: 'linear-gradient(180deg, #color1, #color2)',
    desc: 'Description shown on download form.'
  }
};
```
3. Add to `PRODUCTS` object in `success.html`
4. Add to `PDF_LINKS` in `Code.gs`
5. Add card to `index.html` store
6. Upload PDF to Google Drive

### Add a New Box Tier

1. Create `new-tier-box.html` using `starter-box.html` as template
2. Update the CSS `--tier` color variable
3. Add to `PRODUCTS` in `success.html`:
```javascript
'new-tier-box': {
  type:'box',
  emoji:'💎',
  title:'New Tier Box',
  sub:'Description · $XX',
  color:'gold',
  delivery:'X hours',
  price:'$XX'
}
```
4. Add card to `index.html` store

### Disable a Section

Any section wrapped in:
```html
<section class="...">...</section>
```
Can be hidden with:
```css
/* In the page's <style> block: */
.sx-upsell { display: none !important; }
```

---

## 📞 Contact & Support

### FreshClick Media

| Channel | Details |
|---|---|
| 💬 WhatsApp | [+263 77 967 4212](https://wa.me/263779674212) |
| 📧 Email | FreshClickmedia@gmail.com |
| 🌍 Website | https://freshclickmedia.github.io/freshclick-vault/ |

### For Customers

| Issue | Resolution |
|---|---|
| Didn't receive book email | Check spam → Message WhatsApp with email address |
| Wrong book delivered | Message WhatsApp with order details |
| Box order questions | WhatsApp is primary support channel |
| Upgrade request | Message WhatsApp — we apply credit |
| Technical issue on site | Email or WhatsApp with screenshot |

### For Developers

| Issue | Where to Look |
|---|---|
| Email not sending | Check Apps Script execution logs |
| Sheet not updating | Verify `SHEET_ID` and sheet name |
| PDF link broken | Re-upload to Drive, update sharing settings |
| Form submission fails | Check browser console + Apps Script logs |
| Page not displaying correctly | Hard refresh (Ctrl+Shift+R) |

---

## 📊 Analytics & Tracking

### Google Analytics (Optional Setup)

Add to the `<head>` of each page:

```html
<!-- Google Analytics 4 -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

### Track Book Downloads

In `download.html`, after successful form submission:

```javascript
// Add inside showSuccess():
if(typeof gtag !== 'undefined'){
  gtag('event', 'download', {
    event_category: 'Free Book',
    event_label: data.bookTitle,
    value: 0
  });
}
```

### Track Box Orders (WhatsApp Click)

```javascript
// Add to each WhatsApp order button:
onclick="gtag('event', 'click', {event_category: 'Box Order', event_label: 'Empire Box'})"
```

---

## 📜 Legal

### Content

All HTML, CSS, JavaScript, copy, and design in this repository is the
proprietary work of **FreshClick Media**. All rights reserved.

### Books

The free books distributed through this site are © FreshClick Media.
They may be read and shared freely but may not be resold, repackaged,
or published without written permission.

### Business in a Box

All "Business in a Box" services are delivered by FreshClick Media
personnel. Results are not guaranteed. Individual outcomes depend on
niche selection, content quality, and traffic effort.

---

## 🗺 Roadmap

### Phase 1 — Current (Complete)
- [x] Store homepage
- [x] 6 free book detail pages
- [x] Bundle page
- [x] 4 Business in a Box pages
- [x] Universal download portal with email capture
- [x] Universal success page
- [x] Google Apps Script backend
- [x] Mobile-responsive design
- [x] WhatsApp integration

### Phase 2 — Planned
- [ ] Blog section (`blog.html`) with SEO articles
- [ ] Individual blog post pages
- [ ] Affiliate program page
- [ ] Testimonials / wall of love page
- [ ] FAQ standalone page
- [ ] Sitemap.xml
- [ ] robots.txt

### Phase 3 — Future
- [ ] Member login area (premium content)
- [ ] Course pages
- [ ] Community forum integration
- [ ] Multi-language support (French for West Africa)
- [ ] Automated WhatsApp order notifications

---

## 📈 Performance

### Target Metrics

| Metric | Target |
|---|---|
| Lighthouse Performance | 90+ |
| First Contentful Paint | < 1.5s |
| Largest Contentful Paint | < 2.5s |
| Total Blocking Time | < 200ms |
| Cumulative Layout Shift | < 0.1 |
| Page Size | < 500KB per page |

### Optimization Notes

- **No JavaScript frameworks** — vanilla JS only
- **No external CSS** — all styles self-contained in `<style>` tags
- **Fonts** loaded via Google Fonts with `preconnect`
- **Images** should be WebP format, compressed to < 100KB
- **Animations** use CSS transforms (GPU-accelerated)
- **IntersectionObserver** for scroll animations (no scroll events)

---

*Built with 🖤 by FreshClick Media · For the AfriSphere · #TrafficIsTheNewOil*

---

**FreshClick Vault** · A division of **FreshClick Media**
```

---

**The README covers:**

| Section | Details |
|---|---|
| Overview | What the site is and does |
| Site architecture | Visual tree diagram of all pages and how they link |
| File structure | Complete folder and file map |
| Page reference | All 14 pages with accent colors and unique sections |
| Product catalog | All books, boxes, upgrade pricing, and social platform availability |
| URL parameter reference | Every `?param=` for `download.html` and `success.html` with examples |
| Technology stack | Frontend, backend, hosting — with zero dependencies note |
| Apps Script setup | 6-step guide with code snippets |
| Email delivery | Data captured, flow diagram, `no-cors` explanation |
| Design system | Full color palette, per-page accents, typography, border radius, animation classes |
| WhatsApp integration | All pre-filled message URLs + payment methods |
| SEO config | Meta tags, OG, Twitter cards, noindex on success page |
| Deployment | GitHub Pages steps, custom domain, pre-deployment checklist, find-and-replace table |
| Customization | How to add new books, boxes, change colors, disable sections |
| Contact | Customer support matrix + developer troubleshooting |
| Analytics | Optional GA4 setup + event tracking snippets |
| Legal | Content ownership, book distribution, box disclaimer |
| Roadmap | Phase 1 (complete) → Phase 2 → Phase 3 |
| Performance | Target metrics + optimization notes |
