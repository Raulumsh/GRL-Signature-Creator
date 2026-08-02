# GRL Email Signature Creator

Internal tool for Granite River Labs employees to generate consistent HTML email signatures.

## Features

- Three templates: Modern, Classic, Minimal
- Live preview with instant updates
- Photo upload (local file or URL)
- Brand color picker
- Copy as rich text or raw HTML
- Download as `.html` file
- Dark mode support
- Saves your details to `localStorage` (browser-only, nothing hits a server)

## Deploy to Vercel

### Option 1 — GitHub CI/CD (recommended)

1. Create a new repo on GitHub: `GRL-Signature-Creator`
2. Push this folder:
   ```bash
   cd grl-signature-creator
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/Raulumsh/GRL-Signature-Creator.git
   git push -u origin main
   ```
3. Go to [vercel.com/new](https://vercel.com/new), import the repo, deploy.
4. Your signature tool will be live at `https://grl-signature-creator.vercel.app`

### Option 2 — Vercel CLI (one-shot)

```bash
cd grl-signature-creator
npx vercel --yes
```

## Custom domain (optional)

In the Vercel dashboard → Project Settings → Domains, add e.g. `signature.graniteriverlabs.com` and update your DNS.

## Project structure

```
grl-signature-creator/
├── index.html      ← The entire app (single file, zero dependencies)
├── vercel.json     ← Vercel config (headers, caching, rewrites)
└── README.md
```
