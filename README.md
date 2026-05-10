# kinbeat-web

Static landing page for [kinbeat.com](https://kinbeat.com/). Plain HTML, no build step — Vercel serves it as-is.

## Structure

```
.
├── index.html        # the entire page (inline CSS, inline SVG badges, JSON-LD)
├── logos/            # brand assets referenced from index.html
├── robots.txt
├── sitemap.xml
└── vercel.json       # security headers + long-cache for /logos/*
```

## Deploying to Vercel

1. Push this repo to GitHub (`sho-das/kinbeat-web`).
2. In Vercel: New Project → Import the repo → leave framework as "Other" → Deploy.
3. Add custom domain `kinbeat.com` in Project → Settings → Domains.

## Before launch — update these

- App Store URL (currently a placeholder `https://apps.apple.com/app/kinbeat/`).
- Play Store URL is already set to `com.kinbeat.android`; confirm before going live.
- `terms.html` and `privacy.html` are linked from the footer — copy them in from `kinbeat-android/app/src/main/assets/` when ready, or replace with hosted-elsewhere URLs.
