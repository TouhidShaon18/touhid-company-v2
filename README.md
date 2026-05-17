# Touhid & Company — Website

The official website for Touhid & Company (T&C), an integrated growth consultancy for global SMEs and founders.

**Stack:** Static HTML + CSS + vanilla JS · No build step · Deploys instantly on Vercel.

---

## 📁 Project Structure

```
tc-website/
├── index.html              # Home page
├── vercel.json             # Vercel deployment config
├── README.md               # This file
└── assets/
    ├── css/
    │   └── styles.css      # All styles (CSS variables at top)
    ├── js/
    │   └── main.js         # Mobile menu, small interactions
    └── images/             # Add your logo + images here
```

---

## 🚀 Deploy to Vercel (3 minutes)

1. **Create a GitHub repo** and push this folder to it:
   ```bash
   cd tc-website
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/tc-website.git
   git push -u origin main
   ```

2. **Go to [vercel.com](https://vercel.com)** → New Project → Import your GitHub repo.

3. **Click Deploy.** No build settings needed — Vercel auto-detects it as a static site.

4. Your site is live at `your-project.vercel.app`. Add a custom domain (`touhidandcompany.com`) in Vercel → Settings → Domains.

---

## ✏️ How to Edit

### Change colors, fonts, or spacing

Open `assets/css/styles.css`. At the very top under `:root {}` you'll find every color and size as a variable:

```css
:root {
  --color-sky-blue: #29ABE2;
  --color-parrot-green: #39B54A;
  --color-midnight: #1A1A2E;
  --font-serif: 'DM Serif Display', Georgia, serif;
  --font-sans: 'DM Sans', system-ui, sans-serif;
  --max-width: 1200px;
  --section-padding-y: 70px;
}
```

Change one value — every instance across the site updates automatically.

### Change text content

Open `index.html`. Sections are commented and clearly labeled:

```html
<!-- ===================== HERO ===================== -->
<!-- ===================== SERVICES ===================== -->
<!-- ===================== APPROACH ===================== -->
```

Edit anything between the tags. Save. Push to GitHub. Vercel auto-deploys.

### Add a new page

1. Duplicate `index.html` → rename to e.g. `about.html`.
2. Replace the section content between the header and footer.
3. The header `<nav>` already links to it (`/about.html`).

---

## 🎨 Brand Reference

**Colors**
- Sky Blue (primary): `#29ABE2`
- Parrot Green (secondary): `#39B54A`
- Midnight Navy: `#1A1A2E`
- Charcoal: `#374151`

**Fonts** (loaded from Google Fonts)
- Headings: DM Serif Display
- Body: DM Sans

**Tagline:** Build the System. Own the Growth.

---

## 📋 Pages To Build Next

- [ ] `about.html`
- [ ] `services.html` (hub) + 8 service sub-pages in `/services/`
- [ ] `case-studies.html` + individual case study template
- [ ] `portfolio.html` + project page template
- [ ] `blog.html` + single post template
- [ ] `contact.html`
- [ ] `strategy-call.html` (primary CTA destination)
- [ ] `privacy.html`, `terms.html`

---

## 🔧 Local Preview

No build step required. Just open `index.html` in a browser, or run a tiny local server:

```bash
# Python 3
python -m http.server 8000

# Or with Node
npx serve .
```

Then visit `http://localhost:8000`.

---

© 2026 Touhid & Company. All rights reserved.
