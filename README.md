# Airlie Beach Veterinary Surgery

Static website — Airlie Beach Veterinary Surgery, Cannonvale QLD.

## Colours (matched to logo)

| Token | Hex | Usage |
|---|---|---|
| Primary teal | `#2a8a8a` | Buttons, nav active, borders |
| Mid teal | `#5ab5b5` | Hover states, icons |
| Pale teal | `#e8f5f5` | Card backgrounds, badges |
| Dark teal | `#0a3d4f` | Hero section, after-hours band |
| Orchid purple | `#c4a8d4` | Accent (matches logo orchid) |
| Sand | `#d4c4a0` | Warm neutral backgrounds |
| Deep navy | `#1e2d4b` | Heading text |

## Structure

```
airlie-beach-vet/
├── index.html              →  /
├── 404.html                →  auto-served for missing pages
├── services/index.html     →  /services/
├── about/index.html        →  /about/
├── contact/index.html      →  /contact/
├── images/                 →  drop photos here
├── .htaccess               →  Apache hosting config
└── README.md
```

## GitHub Pages deployment

1. Push repo to GitHub
2. Settings → Pages → Deploy from branch → main → / (root)
3. Live at `https://yourusername.github.io/airlie-beach-vet/`

For custom domain: add domain in Settings → Pages → Custom domain,
then point DNS A records to GitHub's IPs:
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

## Adding images

Place photos in `/images/`. From root pages:
```html
<img src="images/clinic.webp" alt="Airlie Beach Veterinary Surgery" loading="lazy">
```
From subpages (services/, about/, contact/):
```html
<img src="../images/clinic.webp" alt="..." loading="lazy">
```

Recommended sizes: Hero 1600px · Team/clinic 900px · Cards 600px · All WebP format.
Free compression: squoosh.app

## Logo files
- `AirlieBeachVets_Logo.png` — full logo with text
- `AirlieBeachVets_No_text.png` — icon only (for favicon, app icon)
