# Kitoz Burger — Website

A dark, premium single-page site for Kitoz Burger with a 3D hero burger,
a full bilingual (EN/ES) menu, per-item customization, and cart-to-WhatsApp
ordering. Pure static site — no backend required.

## Structure

```
index.html         # the page
favicon.svg        # burger tab icon
.nojekyll          # serve files as-is (no Jekyll)
css/styles.css     # dark & premium theme
js/
  ├── i18n.js      # English / Spanish dictionary + helpers
  ├── data.js      # 👈 YOUR business info + menu (edit this)
  ├── app.js       # menu rendering, cart, customizer & ordering
  └── scene.js     # the 3D hero burger (Three.js)
```

## Edit your content

Everything customer-facing lives in **`js/data.js`** — business info, menu
items, prices, and the customizer options. UI text lives in `js/i18n.js`.

## Deploy

Deploys to GitHub Pages automatically via `.github/workflows/deploy-pages.yml`.
One-time: repo **Settings → Pages → Source: "GitHub Actions"**.
Live at: https://jcchavez650.github.io/Kitoz_Burger/
