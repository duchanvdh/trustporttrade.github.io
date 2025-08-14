# TrustPort Trade B.V. — Website

A single-page, Bootstrap-based website for **TrustPort Trade B.V.** ready for free hosting on **GitHub Pages**.

## 1) Create the repository
1. On GitHub, create a **public** repository named **`trustporttrade.github.io`** (or use your existing account name if different).
2. Upload all files from this folder to the **main** branch.

> The site will be served at `https://<YOUR_GH_USERNAME>.github.io/` automatically.

## 2) Enable GitHub Pages
- Go to **Settings → Pages** and confirm the source is **Branch: main / root**.
- Optionally enable **Enforce HTTPS** once available.

## 3) Configure your custom domain
- In **Settings → Pages**, set **Custom domain** to: `trustporttrade.eu` (this creates/updates a `CNAME` file in the repo).
- In your DNS provider, add the following records for the **apex/root** domain (`trustporttrade.eu`):

**A records (IPv4)**  
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

**Optional AAAA records (IPv6)**  
```
2606:50c0:8000::153
2606:50c0:8001::153
2606:50c0:8002::153
2606:50c0:8003::153
```

- Add a **CNAME** for `www.trustporttrade.eu` pointing to `<YOUR_GH_USERNAME>.github.io`.

DNS changes can take up to **24 hours** to propagate.

## 4) Contact form (Formspree)
- Create a free account at Formspree and get your **Form ID**.
- In `index.html`, replace `FORM_ID` in the form `action="https://formspree.io/f/FORM_ID"` with your actual ID.
- Submissions will be emailed to you and visible in your Formspree dashboard.

## 5) Customize content
- Update text in the **About**, **Services**, **Why TrustPort**, and **Contact** sections.
- Replace `assets/logo.svg` with your real logo (keep the same filename), or update the `<img>` path in the navbar.
- Tweak styles in `assets/style.css` (colors, spacing, etc.).

## 6) Optional
- Add analytics (e.g., Plausible/GA) via a script tag in `index.html`.
- Add a `robots.txt` or `sitemap.xml` if needed.

---

© 2025 TrustPort Trade B.V. — All rights reserved.
