# marcusjp.com

Personal portfolio website for Marcus Pratley built with Astro.

## Tech Stack

- **Framework**: Astro 5.14.8 (static site generator)
- **TypeScript**: Strict mode via astro/tsconfigs/strict
- **Integrations**: @astrojs/sitemap for SEO
- **Analytics**: GoatCounter (marcusjpcom.goatcounter.com)
- **Hosting**: GitHub Pages via GitHub Actions

## Commands

```bash
npm run dev      # Start dev server
npm run build    # Build for production
npm run preview  # Preview production build
```

## Project Structure

```
src/pages/index.astro  # Single-page site with all content
public/
  tactical.jpg         # Desktop hero background
  crop.jpg             # Mobile hero background
  favicon.png
  robots.txt
```

## Architecture

Single-page portfolio with four sections (software, photography, singing, contact) revealed via JS navigation. Content toggles visibility rather than routing. Includes noscript fallback for SEO/accessibility.

Email obfuscation via data attributes to prevent scraping.

## Deployment

Push to `main` triggers GitHub Actions workflow that builds and deploys to GitHub Pages. Site URL: https://marcusjp.com

## WIP / Known TODOs

- Photography portfolio section marked as "-- photo portfolio WIP --" (src/pages/index.astro:115)
