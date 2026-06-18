# Matech Landing Page — Deployment Guide

This directory contains a static landing page for Matech (AI-Powered Materials Intelligence Platform).

## Files

- **`index.html`** — Main landing page (self-contained, semantic markup)
- **`styles.css`** — Responsive stylesheet (professional dark theme)
- **`DEPLOYMENT.md`** — This file

## Deployment Options

### Option 1: cPanel File Manager (Recommended for matech.co.ma)

1. Log in to your cPanel dashboard at your hosting provider (ADK)
2. Open **File Manager**
3. Navigate to the `public_html` folder (this is your document root for matech.co.ma)
4. Upload `index.html` and `styles.css` directly to `public_html/`
5. Verify by visiting `https://matech.co.ma` in your browser

**Notes:**
- Ensure DNS is fully propagated before testing
- If Google Workspace verification files are needed, place them in `public_html/` as well
- Keep `styles.css` in the same directory as `index.html`

### Option 2: GitHub Pages

If you want to serve the landing page from GitHub:

1. Go to repository settings → **Pages**
2. Select **Build and deployment** → Source: `Deploy from a branch`
3. Choose branch: `main` (or create a `gh-pages` branch)
4. Select folder: `/root` or `/docs` (depending on where you keep the files)
5. Save and wait ~1-2 minutes for deployment
6. Your site will be available at: `https://oussamaezzaher-debug.github.io/matech-materials-science-engine/`

### Option 3: Vercel (Recommended for future scaling)

1. Push this repository to GitHub (already done)
2. Go to [vercel.com](https://vercel.com) and sign in with GitHub
3. Click **Add New** → **Project**
4. Import the `matech-materials-science-engine` repository
5. Accept defaults and click **Deploy**
6. Once deployed, go to **Settings** → **Domains** → Add `matech.co.ma`
7. Update your DNS records to point to Vercel (they'll provide the CNAME)
8. Wait ~24-48 hours for DNS propagation

## Design Notes

- **Color Scheme**: Dark professional (suitable for technical/scientific audience)
- **Accent Color**: Cyan/electric blue (`#00d4ff`) — modern, tech-forward
- **Typography**: System fonts (fast loading, consistent across platforms)
- **Responsive**: Optimized for desktop, tablet, and mobile
- **Performance**: Lightweight (no JavaScript, no external dependencies)

## Future Enhancements

When you're ready to expand beyond the landing page:

- Add a **Blog** section for materials science insights
- Integrate **Email signup** for early access
- Add **Team** or **About** pages
- Implement a **Resource Library** (whitepapers, case studies)
- Add **Analytics** (Google Analytics, Vercel Analytics)

## Contact

- **hello@matech.co.ma** — General inquiries
- **info@matech.co.ma** — Business development

---

**Status**: Under Development  
**Last Updated**: 2026-06-18
