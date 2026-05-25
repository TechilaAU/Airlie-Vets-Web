# Airlie Beach Veterinary Surgery

Static website for Airlie Beach Veterinary Surgery, Cannonvale QLD.

## 📁 Structure

```
airlie-beach-vet/
├── index.html              # Homepage  →  /
├── 404.html                # Error page → auto-served for missing pages
├── services/
│   └── index.html          # Services   →  /services/
├── about/
│   └── index.html          # About Us   →  /about/
├── contact/
│   └── index.html          # Contact    →  /contact/
├── images/                 # Drop photos here
├── css/                    # Future stylesheets
├── js/                     # Future scripts
├── .htaccess               # Apache hosting config (ignored by GitHub Pages)
└── README.md
```

## 🚀 GitHub Pages deployment

1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Source: **Deploy from branch** → `main` → `/ (root)`
4. Click **Save** — site is live in ~60 seconds
5. URL: `https://yourusername.github.io/airlie-beach-vet/`

**Custom domain** (airliebeachvet.com.au):
- Add your domain under Settings → Pages → Custom domain
- Point your DNS `A` records to GitHub's IPs:
  ```
  185.199.108.153
  185.199.109.153
  185.199.110.153
  185.199.111.153
  ```
- Or add a `CNAME` record: `www → yourusername.github.io`

## 🎨 Brand colours

| Token | Hex | Usage |
|---|---|---|
| Primary purple | `#b89aea` | Buttons, icons, accents |
| Dark purple | `#7c4db8` | Hover states |
| Purple tint | `#f0ebfa` | Card backgrounds |
| Cream | `#faf7f2` | Page backgrounds |
| After-hours navy | `#2c3e6b` | After-hours sections |

**Fonts:** Playfair Display + DM Sans (Google Fonts)

## 📸 Adding images

Place photos in `/images/` and reference them:

```html
<img src="/images/team.webp" alt="Our veterinary team" loading="lazy">
```

From subpages (services, about, contact) use:
```html
<img src="../images/team.webp" alt="Our veterinary team" loading="lazy">
```

**Recommended sizes:**
| Image | Width | Format |
|---|---|---|
| Hero | 1600px | WebP |
| Team / clinic | 900px | WebP |
| Service cards | 600px | WebP |
| Favicon | 32px + 180px | PNG |

Free compression: [squoosh.app](https://squoosh.app)

## 📞 Clinic details

- **Phone:** 07 4946 1631
- **Address:** 58 Shute Harbour Road, Cannonvale QLD 4802
- **Hours:** Mon–Fri 8:30am–5:30pm · Sat 10:30am–12pm · Sun & After Hours available
