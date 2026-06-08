# Catalog-Z — HTML5 / CSS3 Clone

A **pixel-perfect, dependency-free clone** of the [TemplateMo 556 Catalog-Z](https://templatemo.com/tm-556-catalog-z) photo-catalog template, rebuilt entirely with **HTML5**, **CSS3 Flexbox**, and a tiny sprinkle of vanilla JavaScript.

---

## ✨ Features

| Feature | Detail |
|---|---|
| **Zero CSS frameworks** | No Bootstrap, no Tailwind — 100 % vanilla CSS |
| **Flexbox layouts** | Navbar, gallery grid, footer — all Flexbox |
| **Responsive** | 4 → 3 → 2 → 1 column breakpoints |
| **Page loader** | Animated spinner + curtain slide-away |
| **Hero parallax** | CSS `background-attachment: fixed` |
| **Ming hover effect** | Caption slides in from below on card hover |
| **Semantic HTML5** | `<nav>`, `<main>`, `<article>`, `<figure>`, `<footer>` |
| **Accessible** | ARIA roles, `aria-label`, visible focus rings |
| **SEO ready** | `<title>`, `<meta description>`, single `<h1>` per page |
| **Deployment ready** | Static site — works on Netlify, Vercel, GitHub Pages |

---

## 📁 Project Structure

```
catalog-z/
├── index.html          ← Main page (photos gallery)
├── css/
│   └── style.css       ← All styles (design tokens → components → responsive)
├── images/
│   ├── hero.jpg
│   ├── img-01.jpg
│   ├── img-02.jpg
│   ├── ...
│   └── img-16.jpg
└── README.md
```

---

## 🚀 Local Setup

No build step needed — this is a pure static site.

### Option 1 – Open directly in browser
```bash
# Simply double-click index.html, or right-click → Open With → Browser
```

### Option 2 – Local dev server (recommended for `background-attachment: fixed`)
```bash
# Using Python (pre-installed on most systems)
cd catalog-z
python -m http.server 8080
# Open → http://localhost:8080

# OR using Node.js npx serve
npx serve .
# Open → http://localhost:3000
```

---

## ☁️ Deployment

### Netlify (drag & drop)
1. Go to [netlify.com](https://netlify.com) → **Add new site → Deploy manually**
2. Drag and drop the entire `catalog-z/` folder onto the upload area
3. Your site is live instantly ✅

### Netlify (CLI)
```bash
npm install -g netlify-cli
netlify deploy --dir=catalog-z --prod
```

### Vercel
```bash
npm install -g vercel
cd catalog-z
vercel --prod
```

### GitHub Pages
1. Push this repository to GitHub
2. Go to **Settings → Pages → Source → Deploy from a branch → `main` / `(root)`**
3. Your site is live at `https://<username>.github.io/<repo-name>/` ✅

---

## 🎨 Design System (CSS Custom Properties)

All colours, spacing and typography are defined as CSS variables in `:root` at the top of `css/style.css`:

| Token | Value | Purpose |
|---|---|---|
| `--color-primary` | `#007bff` | Blue accent (headings, links, buttons) |
| `--color-nav-bg` | `#222222` | Navbar background |
| `--color-footer-bg` | `#333333` | Footer background |
| `--color-footer-text` | `#999999` | Muted footer text |
| `--font-base` | `'Roboto', sans-serif` | Global typeface |
| `--navbar-h` | `56px` | Navbar height |
| `--transition` | `0.3s ease` | Global transition speed |

---

## 📐 Responsive Breakpoints

| Breakpoint | Columns | Trigger |
|---|---|---|
| Desktop (≥ 1200 px) | 4 columns | default |
| Large tablet (≤ 1199 px) | 3 columns | `max-width: 1199px` |
| Tablet (≤ 767 px) | 2 columns | `max-width: 767px` |
| Mobile (≤ 575 px) | 1 column | `max-width: 575px` |

---

## 🖼️ Image Credits

All images are sourced from the original [TemplateMo 556 Catalog-Z](https://templatemo.com/tm-556-catalog-z) template which is distributed free for personal and commercial use.

---

## 📝 License

Original template by [TemplateMo](https://templatemo.com) — free for personal and commercial use.  
This clone is for educational / portfolio purposes.
