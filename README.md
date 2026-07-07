# Raleigh Foosball

The website for the Raleigh Foosball community — weekly Tornado and Bonzini
DYP tournaments at Snookers Billiards, Raleigh, NC.
  
Built with [Astro](https://astro.build) (static output, Vite under the hood).

## Develop

```sh
npm install
npm run dev        # dev server at localhost:4321
npm run build      # static build to dist/
npm run preview    # serve the production build locally
```

## Deploy

Pushing to `master` triggers `.github/workflows/deploy.yml`, which builds the
site and publishes it to GitHub Pages.

One-time repo setup: **Settings → Pages → Source: GitHub Actions**, then add
the custom domain `raleighfoosball.com` (and point DNS at GitHub Pages).

## Structure

- `src/pages/` — index, about-powerkick, contact-us
- `src/layouts/Base.astro` — shared head, nav, footer
- `src/styles/global.css` — design tokens ("Table Lights" theme)
- `src/assets/` — photos + crest, optimized by `astro:assets` at build time
