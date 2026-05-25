# Airlie Beach Veterinary Surgery — Website

Static HTML website for Airlie Beach Veterinary Surgery, Cannonvale QLD.

## 📁 Project Structure

```
airlie-beach-vet/
├── index.html          # Homepage
├── services.html       # Services page
├── about.html          # About Us page
├── contact.html        # Contact page
├── 404.html            # Custom 404 error page
├── images/             # Add all photos here (see naming guide below)
│   └── .gitkeep
├── css/                # Reserved for any extracted stylesheets
│   └── .gitkeep
├── js/                 # Reserved for any extracted scripts
│   └── .gitkeep
├── .htaccess           # Apache: clean URLs + 404 routing + caching
├── _redirects          # Netlify: clean URLs + 404 routing
└── README.md           # This file
```

## 🚀 Deployment Options

### Option A — GitHub Pages (free)
1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Set source to `main` branch, root folder
4. Your site is live at `https://yourusername.github.io/airlie-beach-vet/`
5. For a custom domain (airliebeachvet.com.au), add it under **Custom domain**

> **Note:** GitHub Pages doesn't support `.htaccess`. Clean URLs work differently —
> GitHub Pages will serve `404.html` automatically for missing pages, but
> `/services` won't resolve unless you rename files to folders (see below).

**For true clean URLs on GitHub Pages**, rename files to folder/index pattern:
```
services.html  →  services/index.html
about.html     →  about/index.html
contact.html   →  contact/index.html
contact.html   →  contact/index.html
```
Then `/services/` resolves cleanly. The `.htaccess` file is ignored by GitHub Pages.

### Option B — Traditional hosting (Hostinger, SiteGround, cPanel)
1. Upload all files to `public_html/` via FTP or File Manager
2. The `.htaccess` file handles clean URLs and 404 routing automatically
3. Make sure `.htaccess` is visible in your FTP client (enable hidden files)

### Option C — Netlify (free, recommended over GitHub Pages)
1. Connect your GitHub repo in Netlify dashboard
2. Build command: *(leave blank)*
3. Publish directory: `/` (root)
4. The `_redirects` file handles clean URLs and 404 routing automatically
5. Add your custom domain in **Domain settings**

---

## 🎨 Brand

| Token | Value | Usage |
|---|---|---|
| Primary purple | `#b89aea` | Buttons, accents, icons |
| Dark purple | `#7c4db8` | Hover states |
| Light purple tint | `#f0ebfa` | Card backgrounds, badges |
| Cream | `#faf7f2` | Page backgrounds |
| After-hours navy | `#2c3e6b` | After-hours banner |
| Bark / warm brown | `#6b4f3a` | Stat badge |

**Fonts:** Playfair Display (headings) + DM Sans (body) — loaded from Google Fonts

---

## 📸 Adding Images

Drop photos into the `/images/` folder. Recommended naming and sizes:

| File name | Where used | Ideal width |
|---|---|---|
| `hero-bg.webp` | Homepage hero background | 1600px |
| `clinic-exterior.webp` | About page, building shot | 1200px |
| `team.webp` | About page, team photo | 900px |
| `vet-[name].webp` | Individual team member | 600px |
| `dog-consultation.webp` | Services hero | 1200px |
| `logo.svg` | Nav + footer logo mark | SVG |
| `favicon.png` | Browser tab icon | 32×32 + 180×180 |

**Free compression tool:** [squoosh.app](https://squoosh.app) — convert to WebP and resize before uploading.

Reference images in HTML like:
```html
<img src="images/team.webp" alt="Airlie Beach Veterinary Surgery team" loading="lazy">
```

Or as a CSS background:
```css
background-image: url('images/hero-bg.webp');
```

---

## 📞 Clinic Details

- **Phone:** 07 4946 1631
- **Address:** 58 Shute Harbour Road, Cannonvale QLD 4802
- **Hours:** Mon–Fri 8:30am–5:30pm · Sat 10:30am–12pm · Sun & After Hours: available

---

## 🛠 Moving to WordPress (future)

When ready to move to WordPress + Elementor:
1. Install WordPress on hosting
2. Install **Astra** theme (free) + **Elementor** page builder (free)
3. Use this HTML as the visual reference to recreate pages in Elementor
4. Install **WPForms Lite** for the contact form
5. All content is editable from the WordPress dashboard — no code needed

---

*Built with plain HTML/CSS/JS — no frameworks, no build tools, no dependencies.*
