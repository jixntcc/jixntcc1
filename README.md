# 🧠 InnerVault Journal  
> _A minimalist, evolving knowledge vault built with Jekyll and GitHub Pages._

---

## ✦ Overview

**InnerVault Journal** is my personal website and digital knowledge system — a place where thoughts, experiments, and creative systems are documented, refined, and shared.

Built on **Jekyll + GitHub Pages**, it is lightweight, open-source, and future-ready for expansion into a portfolio, SaaS, or marketplace.

---

## ✦ Features

- 🌓 **Dark Mode Toggle** – Smooth, persistent light/dark theme  
- 🧩 **Vault Feed Layout** – Clean post cards with dates and excerpts  
- 🔖 **Dynamic Category Filter** – Instantly sort posts by topic  
- 💡 **Responsive Design** – Optimized for mobile and desktop  
- 🧠 **Syntax Highlighting** – Custom Rouge dark theme for code  
- ⚙️ **Auto SEO + Sitemap** – Powered by `jekyll-seo-tag` and `jekyll-sitemap`  
- 🧰 **Extensible System** – Can evolve into a SaaS or marketplace framework

---

## ✦ File Structure

```bash
├── _includes/         # Reusable components (meta, icons, analytics)
├── _layouts/          # HTML templates
│   ├── default.html   # Global layout (header, footer, dark mode)
│   ├── page.html      # Standard content pages
│   └── post.html      # Blog post layout
├── _posts/            # Your blog entries (YYYY-MM-DD-title.md)
├── _sass/             # Internal Sass partials (auto imported)
├── images/            # Media & uploads
│
├── about.md           # About page
├── archive.md         # Full post index
├── index.md           # Homepage (Vault Feed)
├── _config.yml        # Site configuration
├── style.scss         # Main style (compiled by Jekyll)
│
├── LICENSE            # Open source license
└── README.md          # Project overview (this file)
