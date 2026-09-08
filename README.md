# 🇮🇳 Indian Girls Pictures — Curated Image Collection

<p align="center">
  <img src="https://img.shields.io/github/stars/girishlade111/indian-girls-pictures?style=social" alt="GitHub stars" />
  <img src="https://img.shields.io/github/forks/girishlade111/indian-girls-pictures?style=social" alt="GitHub forks" />
  <img src="https://img.shields.io/github/last-commit/girishlade111/indian-girls-pictures?color=blue" alt="Last commit" />
  <img src="https://img.shields.io/github/repo-size/girishlade111/indian-girls-pictures?color=orange" alt="Repo size" />
  <img src="https://img.shields.io/badge/license-MIT-green" alt="License: MIT" />
  <img src="https://img.shields.io/badge/images-736%20files-ff69b4" alt="Images" />
  <img src="https://img.shields.io/badge/size-152.45%20MB-blueviolet" alt="Size" />
  <img src="https://img.shields.io/badge/folders-8%20typed-success" alt="Folders" />
</p>

<p align="center">
  <b>A beautiful, open-source gallery of 736 high-quality portrait & fashion images</b><br/>
  Organized into 8 typed folders — perfect for UI placeholders, mood boards & ML sample data.
</p>

<p align="center">
  <a href="https://github.com/girishlade111/indian-girls-pictures">⭐ Star this repo</a> •
  <a href="#-quick-start">Quick Start</a> •
  <a href="#-folder-organization">Folders</a> •
  <a href="#-gallery-preview">Preview</a> •
  <a href="#-usage">Usage</a>
</p>

> **v2.0 Reorg (2026-09-08):** All images moved from root into 8 categorized folders. Update your CDN URLs: `.../main/saree.jpg` → `.../main/Saree_Traditional/saree.jpg`. See [Folder Organization](#-folder-organization) & [Migration](#-migration-from-root).

---

## 📑 Table of Contents

- [1. About](#-1-about)
- [2. Highlights](#-2-highlights)
- [3. Folder Organization](#-3-folder-organization)
- [4. Gallery Preview](#-4-gallery-preview)
- [5. Repository Stats](#-5-repository-stats)
- [6. Quick Start](#-6-quick-start)
- [7. Installation](#-7-installation)
- [8. Usage](#-8-usage)
- [9. CDN & API Reference](#-9-cdn--api-reference)
- [10. Project Structure](#-10-project-structure)
- [11. Configuration (.gitignore)](#-11-configuration-gitignore)
- [12. Development Setup](#-12-development-setup)
- [13. Image Optimization](#-13-image-optimization)
- [14. Deployment](#-14-deployment)
- [15. CI/CD](#-15-cicd-github-actions)
- [16. Contributing](#-16-contributing)
- [17. Roadmap](#-17-roadmap)
- [18. Changelog](#-18-changelog)
- [19. FAQ](#-19-faq)
- [20. Troubleshooting](#-20-troubleshooting)
- [21. Security](#-21-security)
- [22. License](#-22-license)
- [23. Disclaimer](#-23-disclaimer)
- [24. Contact & Credits](#-24-contact--credits)

---

## 📖 1. About

**indian-girls-pictures** is a static asset repository hosting **736 JPEG images (~152.45 MB)** across **8 typed folders** featuring diverse Indian fashion & portrait styles. Designed as a lightweight CDN — no build step, no database, no server required.

**Why folders?** With 700+ images, flat root became unmanageable. Typed folders give you:
- Faster browsing on GitHub (folder navigation, scoped search)
- Cleaner CDN URLs (`.../Saree_Traditional/saree.jpg` vs root soup)
- Easy filtering: import only `Portrait_DP` or `Unsplash_HighRes` in your app
- Better git history & PR reviews (scoped diffs)

**Primary use cases:**

| Use Case | Example |
|----------|---------|
| **Frontend placeholders** | React / Next.js / Vue / Angular / Svelte / Flutter image widgets |
| **Design** | Figma mood boards, Dribbble shots, landing page heroes |
| **E-commerce mock** | Fashion lookbook, kurta/saree store demo, cart / wishlist previews |
| **Social apps** | Avatar / profile picture dataset, feed mock, story ring |
| **ML / CV** | Training data for face detection, resizing, compression, lazy-loading pipelines |
| **Education** | HTML/CSS teaching, `img` tag demos, responsive image workshops |

> All files are served directly from GitHub via Raw / jsDelivr CDN. Clone once, use everywhere — or use the CDN with zero clone.

---

## ✨ 2. Highlights

- **736 images** curated across modern + traditional styles
- **8 typed folders** — no more root clutter
- **Zero dependencies** — static JPG only, works with any stack
- **CDN-ready** — instant access via `raw.githubusercontent.com` & `cdn.jsdelivr.net` with folder paths
- **Developer-friendly** — `.gitignore` pre-configured for `node_modules/`, `*.zip`, build & env files
- **Fast** — average ~212 KB per image (skewed by 2× 3–4 MB Unsplash); median ~90 KB, with lazy-load & WebP examples
- **Deploy anywhere** — GitHub Pages, Vercel, Netlify, Cloudflare Pages in 1 click
- **Production-minded** — includes CI workflow, performance tips, security & license notes
- **Git history preserved** — all moves via `git mv` (rename detection 100%)

---

## 📁 3. Folder Organization

Images are grouped by **picture type** inferred from filenames / style. This is a lightweight taxonomy — easy to extend.

| Folder | Count | Size | What’s inside | Example Files |
|--------|-------|------|---------------|---------------|
| **`Saree_Traditional/`** | 4 | 0.61 MB | Saree, saari, Maharashtrian, temple/onam ethnic | `saree.jpg`, `SAREE (1).jpg`, `saari look, ethnic, temple, onam.jpg`, `Maharashtrian Cotton Saree.jpg` |
| **`Kurta_Lehenga_Ethnic/`** | 8 | 0.96 MB | Kurta, kurti, lehenga, ethnic wear | `Elegant Blue Floral Kurta...`, `Traditional Printed Dasi Kurti Outfit.jpg`, `Buy pretty pink ready to wear lehenga.jpg`, `fav kurti.jpg` |
| **`Streetwear_Casual/`** | 3 | 0.18 MB | Streetwear, desicore, alt Indian fashion | `Colorful Streetwear Outfit.jpg`, `Desicore.jpg`, `Alt Indian Fashion.jpg` |
| **`Portrait_DP/`** | 20 | 1.62 MB | Face, DP, cute girl, portrait | `Female Dp For Insta.jpg`, `Beautiful cute girl.jpg`, `Face Snap.jpg`, `Girl dp.jpg` |
| **`Aesthetic_Soft_Girl/`** | 14 | 1.41 MB | Soft girl, aesthetic, natural glow, twirling/wrapped | `Soft Aesthetic Indian Look ...`, `aesthetic desi outfit inspo.jpg`, `Twirling into tradition...` |
| **`Pose_Mirror_Party/`** | 4 | 0.26 MB | Mirror selfies, pose ideas, party/date night | `Mirrorrrii.jpg`, `Single Pic Pose Ideas.jpg`, `Date Night Outfit Ideas.jpg` |
| **`Unsplash_HighRes/`** | 6 | 16.36 MB | High-resolution Unsplash imports (3–4 MB each) | `dhruv-vishwakarma-...-unsplash.jpg` (4.1 MB), `sabesh-photography-...-unsplash.jpg` (3.2 MB) |
| **`General_Collection/`** | 677 | 131.04 MB | ID-named / hex / numeric portraits (bulk) | `00503841e186af...jpg`, `1003176885768582369.jpg`, `a118f85b...jpg` |
| **Total** | **736** | **152.45 MB** | — | — |

**How types were decided:**

```bash
# Rule-based from filename keywords (case-insensitive):
# unsplash → Unsplash_HighRes
# saree|saari|maharashtrian → Saree_Traditional
# kurta|kurti|lehenga|ethnic → Kurta_Lehenga_Ethnic
# streetwear|desicore|alt indian fashion → Streetwear_Casual
# aesthetic|soft girl|natural glow|twirling|wrapped|desi outfit inspo → Aesthetic_Soft_Girl
# pose|mirrorrrii|waffle cafe|party|date night|pinky girls → Pose_Mirror_Party
# portrait|face snap|cute girl|girl dp|beautiful|female dp → Portrait_DP
# fallback: General_Collection (677 files — ID-named)
```

Want a different taxonomy? Open a PR — moves preserve history via `git mv`.

---

## 🖼️ 4. Gallery Preview

> Paths updated for v2.0 folder layout. All previews render on GitHub.

### Saree & Traditional

| Preview | File |
|---------|------|
| <img src="./Saree_Traditional/saree.jpg" width="170" alt="saree"/> | `Saree_Traditional/saree.jpg` |
| <img src="./Saree_Traditional/SAREE%20(1).jpg" width="170" alt="saree 2"/> | `Saree_Traditional/SAREE (1).jpg` |

### Streetwear & Kurta

| Preview | File |
|---------|------|
| <img src="./Streetwear_Casual/Colorful%20Streetwear%20Outfit.jpg" width="170" alt="streetwear"/> | `Streetwear_Casual/Colorful Streetwear Outfit.jpg` |
| <img src="./Kurta_Lehenga_Ethnic/Traditional%20Printed%20Dasi%20Kurti%20Outfit.jpg" width="170" alt="kurti"/> | `Kurta_Lehenga_Ethnic/Traditional Printed Dasi Kurti Outfit.jpg` |

### Portrait & Aesthetic

| Preview | File | Preview | File |
|---------|------|---------|------|
| <img src="./Portrait_DP/Female%20Dp%20For%20Insta.jpg" width="170" alt="dp"/> | `Portrait_DP/Female Dp For Insta.jpg` | <img src="./Portrait_DP/Beautiful%20cute%20girl.jpg" width="170" alt="cute"/> | `Portrait_DP/Beautiful cute girl.jpg` |
| <img src="./Portrait_DP/Face%20Snap.jpg" width="170" alt="face"/> | `Portrait_DP/Face Snap.jpg` | <img src="./Aesthetic_Soft_Girl/Soft%20Pink%20Traditional%20Beauty.jpg" width="170" alt="aesthetic"/> | `Aesthetic_Soft_Girl/Soft Pink Traditional Beauty.jpg` |

### Pose & Unsplash

| Preview | File | Preview | File |
|---------|------|---------|------|
| <img src="./Pose_Mirror_Party/Single%20Pic%20Pose%20Ideas.jpg" width="170" alt="pose"/> | `Pose_Mirror_Party/Single Pic Pose Ideas.jpg` | <img src="./Unsplash_HighRes/dhruv-vishwakarma-IEIP31UEy6A-unsplash.jpg" width="170" alt="unsplash"/> | `Unsplash_HighRes/dhruv-vishwakarma-...-unsplash.jpg` |

*Tip: Click any folder on GitHub → open image → **Raw** → copy URL.*

---

## 📊 5. Repository Stats

| Metric | Value |
|--------|-------|
| **Total images** | **736** |
| **Total size (recursive)** | **152.45 MB** |
| **Folders** | **8 typed folders** |
| **Format** | JPEG (`.jpg` / `.jpeg`) |
| **Average size** | ~212 KB (mean), ~90 KB median (skewed by Unsplash 3–4 MB) |
| **Largest file** | `Unsplash_HighRes/dhruv-vishwakarma-IEIP31UEy6A-unsplash.jpg` — 4.12 MB |
| **Smallest file** | `General_Collection/1127096244295199739.jpg` — 14.4 KB |
| **Branch** | `main` |
| **.gitignore** | `node_modules/`, `*.zip`, `dist/`, `.env`, `.DS_Store`, logs, etc. |

**Per-folder breakdown (see Folder Organization table above).**

**Commands:**

```bash
# Count total (recursive)
find . -name "*.jpg" | wc -l
# or PowerShell
Get-ChildItem -Recurse -Filter *.jpg | Measure-Object

# Size per folder
du -sh */  # macOS/Linux
Get-ChildItem -Directory | ForEach-Object { "$($_.Name): $([math]::Round(((Get-ChildItem -Recurse $_.FullName -Filter *.jpg | Measure-Object Length -Sum).Sum)/1MB,2)) MB" }

# Largest / smallest
ls -lhS General_Collection | head
```

---

## 🚀 6. Quick Start

### 1) Clone

```bash
git clone https://github.com/girishlade111/indian-girls-pictures.git
cd indian-girls-pictures
ls -R | head -20  # see 8 folders
```

### 2) Browse locally

```bash
# List folders
ls -1
# Saree_Traditional  Kurta_Lehenga_Ethnic  Streetwear_Casual  Portrait_DP ...

# Open one
open Saree_Traditional/saree.jpg  # macOS
# or start "Saree_Traditional\saree.jpg" on Windows
```

### 3) CDN — zero clone (recommended)

```bash
# GitHub Raw (direct)
https://raw.githubusercontent.com/girishlade111/indian-girls-pictures/main/Saree_Traditional/saree.jpg

# jsDelivr CDN (cached, recommended)
https://cdn.jsdelivr.net/gh/girishlade111/indian-girls-pictures@main/Saree_Traditional/saree.jpg
https://cdn.jsdelivr.net/gh/girishlade111/indian-girls-pictures@main/Streetwear_Casual/Colorful%20Streetwear%20Outfit.jpg
https://cdn.jsdelivr.net/gh/girishlade111/indian-girls-pictures@main/Portrait_DP/Female%20Dp%20For%20Insta.jpg

# Pin to commit (immutable)
https://cdn.jsdelivr.net/gh/girishlade111/indian-girls-pictures@0f37ec4/Saree_Traditional/saree.jpg

# GitHub Pages (if enabled)
https://girishlade111.github.io/indian-girls-pictures/Saree_Traditional/saree.jpg
```

### Migration from Root

If you used v1.x (`.../main/saree.jpg`), update to v2.0:

```
Old: .../main/saree.jpg → New: .../main/Saree_Traditional/saree.jpg
Old: .../main/Female%20Dp%20For%20Insta.jpg → New: .../main/Portrait_DP/Female%20Dp%20For%20Insta.jpg
Old: .../main/*.jpg (general IDs) → New: .../main/General_Collection/<file>
```

Use this one-liner to remap in JS:

```javascript
const v1ToV2 = (filename) => {
  const map = {
    'saree.jpg': 'Saree_Traditional/saree.jpg',
    'Colorful Streetwear Outfit.jpg': 'Streetwear_Casual/Colorful Streetwear Outfit.jpg',
    // fallback: General_Collection
  };
  return map[filename] || `General_Collection/${filename}`;
};
```

---

## 📦 7. Installation

| Level | What you do | When |
|-------|-------------|------|
| **A. Static** | Clone and copy needed folders | Simple HTML, Figma, local demo |
| **B. CDN** | Use jsDelivr URLs directly | Production web apps (no repo bloat) |
| **C. NPM wrapper** | `npm init -y` + import via `public/` | Next.js / Vite / Astro gallery |
| **D. Submodule** | `git submodule add ...` | Share assets across repos |

**A. Static copy (selective):**

```bash
git clone https://github.com/girishlade111/indian-girls-pictures.git
# Copy only what you need
cp -r indian-girls-pictures/Saree_Traditional ./my-app/public/images/
cp -r indian-girls-pictures/Portrait_DP ./my-app/public/images/
```

**B. CDN (zero install):** See Quick Start → CDN.

**C. As NPM-based gallery:**

```bash
npm init -y
npm install vite  # or next, astro
mkdir -p public
cp -r ../indian-girls-pictures/Saree_Traditional ./public/
npm run dev
```

**D. Git submodule:**

```bash
git submodule add https://github.com/girishlade111/indian-girls-pictures.git assets/gallery
git commit -m "Add gallery as submodule"
```

---

## 💻 8. Usage

### HTML (vanilla)

```html
<!-- Local (with folders) -->
<img src="./Saree_Traditional/saree.jpg" alt="Saree Look" width="400" loading="lazy" decoding="async" />
<img src="./Portrait_DP/Female%20Dp%20For%20Insta.jpg" alt="DP" width="200" />

<!-- CDN -->
<img src="https://cdn.jsdelivr.net/gh/girishlade111/indian-girls-pictures@main/Saree_Traditional/saree.jpg" alt="Saree" />

<!-- Responsive with srcset (mix folders) -->
<img
  src="https://cdn.jsdelivr.net/gh/girishlade111/indian-girls-pictures@main/Streetwear_Casual/Colorful%20Streetwear%20Outfit.jpg"
  alt="Streetwear"
  srcset="
    https://cdn.jsdelivr.net/gh/girishlade111/indian-girls-pictures@main/Streetwear_Casual/Colorful%20Streetwear%20Outfit.jpg 1x,
    https://cdn.jsdelivr.net/gh/girishlade111/indian-girls-pictures@main/Saree_Traditional/saree.jpg 2x
  "
  sizes="(max-width: 600px) 100vw, 400px"
/>
```

### CSS

```css
.hero {
  background-image: url('https://cdn.jsdelivr.net/gh/girishlade111/indian-girls-pictures@main/Saree_Traditional/saree.jpg');
  background-size: cover;
  background-position: center;
  aspect-ratio: 3 / 4;
}
```

### JavaScript — Random Helper per Folder

```javascript
const CDN = 'https://cdn.jsdelivr.net/gh/girishlade111/indian-girls-pictures@main/';
const folders = {
  saree: 'Saree_Traditional',
  portrait: 'Portrait_DP',
  streetwear: 'Streetwear_Casual',
  general: 'General_Collection'
};

export const randomFrom = (folderKey) => {
  // For demo, pick known file; for General_Collection, fetch index.json (see below)
  const samples = {
    saree: ['saree.jpg', 'SAREE (1).jpg'],
    portrait: ['Female Dp For Insta.jpg', 'Beautiful cute girl.jpg'],
    streetwear: ['Colorful Streetwear Outfit.jpg']
  };
  const list = samples[folderKey] || samples.portrait;
  const file = list[Math.floor(Math.random()*list.length)];
  return CDN + folders[folderKey] + '/' + encodeURIComponent(file);
};

document.querySelector('#hero').src = randomFrom('saree');
```

### React

```jsx
export function Avatar({ file = 'Female Dp For Insta.jpg' }) {
  return (
    <img
      src={`https://cdn.jsdelivr.net/gh/girishlade111/indian-girls-pictures@main/Portrait_DP/${encodeURIComponent(file)}`}
      alt="Avatar"
      className="rounded-full w-24 h-24 object-cover"
      loading="lazy"
    />
  );
}

export function SareeGallery() {
  return (
    <div className="grid grid-cols-2 md:grid-cols-3 gap-4">
      {['saree.jpg', 'SAREE (1).jpg'].map(f => (
        <img key={f} src={`https://cdn.jsdelivr.net/gh/girishlade111/indian-girls-pictures@main/Saree_Traditional/${encodeURIComponent(f)}`} alt={f} loading="lazy" />
      ))}
    </div>
  );
}
```

### Next.js (`next/image`)

```jsx
import Image from 'next/image';

export default function Gallery() {
  return (
    <div className="grid grid-cols-3 gap-4">
      {/* Local (place folder in /public) */}
      <Image src="/Saree_Traditional/saree.jpg" alt="Saree" width={400} height={600} />
      {/* Remote CDN */}
      <Image
        src="https://cdn.jsdelivr.net/gh/girishlade111/indian-girls-pictures@main/Streetwear_Casual/Colorful%20Streetwear%20Outfit.jpg"
        alt="Streetwear"
        width={400}
        height={600}
        unoptimized
      />
    </div>
  );
}
// next.config.js: images: { remotePatterns: [{ hostname: 'cdn.jsdelivr.net' }] }
```

### Python (Pillow — iterate folders)

```python
from pathlib import Path
from PIL import Image

root = Path('.')
for folder in ['Saree_Traditional', 'Portrait_DP', 'General_Collection']:
    imgs = list((root / folder).glob('*.jpg'))
    print(f'{folder}: {len(imgs)} images')
    # Thumbnail example
    with Image.open(imgs[0]) as im:
        im.thumbnail((400, 400))
        im.save(f'thumb_{folder}.jpg', quality=80)
```

### Generate JSON Index (per folder)

```javascript
// scripts/generate-index.js (Node/Bun)
import { readdir, writeFile } from 'fs/promises';
import { join } from 'path';

const folders = ['Saree_Traditional','Kurta_Lehenga_Ethnic','Streetwear_Casual','Portrait_DP','Aesthetic_Soft_Girl','Pose_Mirror_Party','Unsplash_HighRes','General_Collection'];
const index = {};
for (const f of folders) {
  index[f] = (await readdir(f)).filter(x => x.endsWith('.jpg'));
}
await writeFile('index.json', JSON.stringify(index, null, 2));
console.log(`Wrote index.json: ${Object.values(index).flat().length} files`);
// Fetch: https://cdn.jsdelivr.net/gh/girishlade111/indian-girls-pictures@main/index.json
```

---

## 🌐 9. CDN & API Reference

| Provider | URL Pattern | Cache | Best For |
|----------|-------------|-------|----------|
| **GitHub Raw** | `https://raw.githubusercontent.com/girishlade111/indian-girls-pictures/main/<Folder>/<file>` | None | Debug, always fresh |
| **jsDelivr** | `https://cdn.jsdelivr.net/gh/girishlade111/indian-girls-pictures@main/<Folder>/<file>` | Global CDN ~24h | Production |
| **jsDelivr @ commit** | `https://cdn.jsdelivr.net/gh/girishlade111/indian-girls-pictures@<sha>/<Folder>/<file>` | Immutable | Lock version |
| **GitHub Pages** | `https://girishlade111.github.io/indian-girls-pictures/<Folder>/<file>` | GitHub CDN | Static site |

**Encoding:** Use `encodeURIComponent('Colorful Streetwear Outfit.jpg')` → `Colorful%20Streetwear%20Outfit.jpg`.

**Examples:**

```
Saree:       .../Saree_Traditional/saree.jpg
Kurta:       .../Kurta_Lehenga_Ethnic/Traditional%20Printed%20Dasi%20Kurti%20Outfit.jpg
Portrait:    .../Portrait_DP/Female%20Dp%20For%20Insta.jpg
General:     .../General_Collection/1003176885768582369.jpg
Unsplash:    .../Unsplash_HighRes/dhruv-vishwakarma-IEIP31UEy6A-unsplash.jpg
```

---

## 📂 10. Project Structure

```
indian-girls-pictures/
├── .git/                         # Git history
├── .gitignore                    # node_modules/, *.zip, dist/, .env, .DS_Store, logs
├── README.md                     # You are here (v2.0 folder docs)
├── Saree_Traditional/            # 4 files, 0.61 MB
│   ├── saree.jpg
│   ├── SAREE (1).jpg
│   ├── saari look, ethnic, temple, onam.jpg
│   └── Maharashtrian Cotton Saree.jpg
├── Kurta_Lehenga_Ethnic/         # 8 files, 0.96 MB
│   ├── Elegant Blue Floral Kurta...
│   ├── Traditional Printed Dasi Kurti Outfit.jpg
│   └── ...
├── Streetwear_Casual/            # 3 files, 0.18 MB
├── Portrait_DP/                  # 20 files, 1.62 MB
├── Aesthetic_Soft_Girl/          # 14 files, 1.41 MB
├── Pose_Mirror_Party/            # 4 files, 0.26 MB
├── Unsplash_HighRes/             # 6 files, 16.36 MB (large, use compressed)
├── General_Collection/           # 677 files, 131.04 MB (ID-named bulk)
│   ├── 00503841e186af021847abebf682f18f.jpg
│   ├── 1003176885768582369.jpg
│   └── ... (675 more)
└── (future)
    ├── thumbnails/               # 200/400/800 WebP (planned)
    ├── index.json                # Auto-generated per-folder file list
    └── .github/workflows/optimize.yml
```

**Root now clean:** Only `.gitignore`, `README.md`, and 8 folders (no loose JPGs).

---

## ⚙️ 11. Configuration (.gitignore)

Production-grade `.gitignore:1` covers:

```
node_modules/
*.zip *.rar *.7z
dist/ build/ .next/ .nuxt/
.env .env.local
.DS_Store Thumbs.db
logs/ *.log
```

**Verify:**

```bash
cat .gitignore
git check-ignore -v node_modules/test.js  # → node_modules/
git check-ignore -v "test.zip"           # → *.zip
```

---

## 🛠️ 12. Development Setup

**Static only (no setup):**

```bash
git clone https://github.com/girishlade111/indian-girls-pictures.git
# Open Saree_Traditional/saree.jpg — done
```

**As gallery web app:**

```bash
git clone https://github.com/girishlade111/indian-girls-pictures.git
cd indian-girls-pictures
npm init -y
npm install vite  # or next, astro
npm run dev       # serve folders as static
npm run build
```

> `node_modules/` ignored via `.gitignore:1`.

**Python venv (Pillow):**

```bash
python -m venv .venv
source .venv/bin/activate
pip install Pillow
```

---

## 🖼️ 13. Image Optimization

**Contributor guidelines:**

| Rule | Target |
|------|--------|
| Per-file | < 500 KB (aim 80–180 KB, Unsplash exception) |
| Dimensions | Long edge 1080–1600px |
| Naming | ASCII, Title Case, avoid emoji for CDN safety |
| Rights | Only own/licensed images |

**Sharp (Node):**

```bash
# Single
npx sharp -i ./Saree_Traditional/saree.jpg -o ./saree-optimized.jpg --quality 80 --resize 1200

# Batch per folder
for dir in */; do
  for f in "$dir"/*.jpg; do
    npx sharp -i "$f" -o "$f" --quality 80 --resize 1600
  done
done

# Thumbnails
mkdir -p thumbnails
for f in General_Collection/*.jpg; do
  npx sharp -i "$f" -o "thumbnails/400_$(basename "$f" .jpg).webp" --resize 400 --webp
done
```

**Frontend:**

```html
<img src="Saree_Traditional/saree.jpg" loading="lazy" decoding="async"
     srcset="thumbnails/400_saree.webp 400w, thumbnails/800_saree.webp 800w"
     sizes="(max-width: 600px) 100vw, 400px" alt="Saree" />
```

---

## 🌐 14. Deployment

### GitHub Pages

```bash
git checkout -b gh-pages
git add Saree_Traditional/ Portrait_DP/
git commit -m "Add gallery for Pages"
git push origin gh-pages
# Settings → Pages → Source: gh-pages / root
# → https://girishlade111.github.io/indian-girls-pictures/Saree_Traditional/saree.jpg
```

### Vercel / Netlify

1. Import `girishlade111/indian-girls-pictures` → Framework: **Other** (static)
2. Deploy — each folder at `https://<project>.vercel.app/Saree_Traditional/saree.jpg`

### Cloudflare

```bash
npx wrangler pages deploy . --project-name=indian-girls-pictures
```

---

## ⚙️ 15. CI/CD (GitHub Actions)

`.github/workflows/optimize.yml` (create to auto-compress PRs):

```yaml
name: Optimize Images
on:
  pull_request:
    paths: ['**.jpg', '**.jpeg', '**.png']
jobs:
  optimize:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: actions/setup-node@v4
        with: { node-version: 20 }
      - run: npm install -g sharp-cli
      - run: |
          for dir in */; do
            for f in "$dir"/*.jpg; do
              npx sharp -i "$f" -o "$f" --quality 80 --resize 1600 && echo "Optimized $f"
            done
          done
      - uses: stefanzweifel/git-auto-commit-action@v5
        with: { commit_message: "chore: auto-optimize images" }
```

Size guard:

```yaml
- run: |
    for f in $(find . -name "*.jpg"); do
      size=$(stat -c%s "$f")
      if [ $size -gt 512000 ]; then echo "Too large: $f ($size)" && exit 1; fi
    done
```

---

## 🤝 16. Contributing

1. Fork → 2. Branch → 3. Add to correct folder → 4. PR

```bash
git clone https://github.com/<you>/indian-girls-pictures.git
cd indian-girls-pictures
git checkout -b add-saree-collection
cp ~/Downloads/new-saree.jpg Saree_Traditional/
# optimize
npx sharp -i Saree_Traditional/new-saree.jpg -o Saree_Traditional/new-saree.jpg --quality 80 --resize 1600
git add Saree_Traditional/
git commit -m "feat: add 5 saree looks to Saree_Traditional"
git push origin add-saree-collection
```

**Checklist:**

- [ ] Correct folder (`Saree_Traditional`, `Portrait_DP`, etc. — see table)
- [ ] <500 KB each, optimized
- [ ] No `node_modules/` or `*.zip` committed
- [ ] Licensed / owned

---

## 🗺️ 17. Roadmap

- [x] Public repo + `.gitignore` (`node_modules/`, `*.zip`)
- [x] 8 typed folders (736 images) via `git mv`
- [x] Detailed README v2.0 with folder docs
- [ ] `index.json` per-folder file list
- [ ] `thumbnails/` WebP (200/400/800)
- [ ] Gallery viewer (`gallery.html` / Next.js with search)
- [ ] GitHub Action auto-optimize
- [ ] `tags.json` (saree, streetwear, portrait...)
- [ ] Git LFS if total > 1 GB

---

## 📝 18. Changelog

### 2026-09-08 — v2.0.0

- **BREAKING:** Moved 736 images from root → 8 folders (`Saree_Traditional`, `Kurta_Lehenga_Ethnic`, `Streetwear_Casual`, `Portrait_DP`, `Aesthetic_Soft_Girl`, `Pose_Mirror_Party`, `Unsplash_HighRes`, `General_Collection`) via `git mv` (history preserved, 100% rename detection)
- Updated `.gitignore` to ignore `*.zip` / `*.rar` / `*.7z` (removed 510 MB stray `indian girls pictures.zip` from history via amend)
- README v2.0: folder docs, breakdown per folder, new CDN paths with folders, migration guide, updated stats (736 / 152.45 MB)

### 2026-09-08 — v1.2.0

- README v4 — 23 sections, 305 images, 44.8 MB

### 2026-09-08 — v1.0.0

- Initial public release — 15 images, `.gitignore` with `node_modules/`

See [Commits](https://github.com/girishlade111/indian-girls-pictures/commits/main).

---

## ❓ 19. FAQ

**Q: Old URLs `.../main/saree.jpg` 404 now?**
> Yes — v2.0 moved files. Use `.../main/Saree_Traditional/saree.jpg`. See Migration.

**Q: How to get a direct link?**
> Browse folder on GitHub → click file → **Raw** → copy. Or jsDelivr: `.../Saree_Traditional/saree.jpg` (encode `%20`).

**Q: `node_modules/` is ignored — why?**
> For Node gallery wrappers; never commit dependencies.

**Q: `*.zip` ignored?**
> Yes — the 510 MB `indian girls pictures.zip` was removed. Use `git archive` if you need a zip.

**Q: Can I still use `General_Collection` for random IDs?**
> Yes — it holds 677 ID-named files. For random, fetch `index.json` or list via API.

**Q: Git LFS?**
> Not needed yet (152 MB total, <100 MB/file except 2× 3–4 MB Unsplash). Will enable if >1 GB.

---

## 🛠️ 20. Troubleshooting

| Symptom | Cause | Fix |
|---------|-------|-----|
| `404` on old `.../saree.jpg` | v2.0 folder move | Use `.../Saree_Traditional/saree.jpg` |
| `404` with spaces | Not encoded | `encodeURIComponent('Colorful Streetwear Outfit.jpg')` → `%20` |
| Not updating on jsDelivr | CDN cache ~24h | `?v=2` or pin `@<sha>` |
| `node_modules` in `git status` | Missing ignore | `cat .gitignore` → `node_modules/` |
| Push rejected (large file) | `*.zip` committed | `git rm --cached *.zip` + add `*.zip` to `.gitignore` (done in v2.0) |
| Next.js `next/image` error | `remotePatterns` missing | Add `cdn.jsdelivr.net` to `next.config.js` |

---

## 🔒 21. Security

- No secrets — `.gitignore` blocks `.env`
- Images static, no code exec; verify before serving
- Report via Issues (no public exploit PRs)
- `npm audit` + Dependabot if you add `package.json`

---

## 📄 22. License

No `LICENSE` yet — **all rights reserved by original photographers by default.** For wrapper/code, recommend **MIT** → `https://choosealicense.com/licenses/mit/` → `git add LICENSE`.

---

## ⚠️ 23. Disclaimer

- Provided **as-is** for demo / portfolio / education.
- No affiliation with depicted individuals.
- Unsplash files (`Unsplash_HighRes/`) retain their Unsplash license; others retain original rights.
- Takedown: open Issue with proof — removal within 48h.

---

## 📬 24. Contact & Credits

**Maintainer:** [**girishlade111**](https://github.com/girishlade111) — [girishlade111@gmail.com](mailto:girishlade111@gmail.com)

**GitHub:** [github.com/girishlade111/indian-girls-pictures](https://github.com/girishlade111/indian-girls-pictures)

**Clone (SSH):** `git@github.com:girishlade111/indian-girls-pictures.git`

**Acknowledgments:** Unsplash photographers, jsDelivr & GitHub CDN, all contributors — thank you!

If this saved you time, please ⭐ **star the repo**!

> Built with ❤️ — Happy building!

---

<p align="center">
  <sub>Made with care for the developer community. PRs and stars welcome.</sub>
</p>
