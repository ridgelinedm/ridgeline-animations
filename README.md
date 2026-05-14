# Ridgeline Animations

HTML animations embedded on [ridgelinedigitalmarketing.com](https://ridgelinedigitalmarketing.com), served via GitHub Pages.

Each animation lives in its own folder and is loaded into the marketing site via `<iframe>`.

## Current animations

| Animation | Folder | Live URL |
|---|---|---|
| The SEO / GEO problem | [`seo-geo-problem/`](./seo-geo-problem/) | https://ridgelinedm.github.io/ridgeline-animations/seo-geo-problem/ |

## Adding a new animation

1. Create a new folder at the repo root (e.g. `my-new-animation/`).
2. Add a self-contained `index.html` inside it (inline CSS and JS — no build step).
3. Commit to `main`. GitHub Pages publishes automatically within a minute or two.
4. Embed on the Webflow site with:
   ```html
   <iframe
     src="https://ridgelinedm.github.io/ridgeline-animations/my-new-animation/"
     style="width: 100%; height: 560px; border: none; display: block;"
     loading="eager"
     title="Descriptive title">
   </iframe>
   ```
5. Add a row to the table above.

## Hosting

GitHub Pages is configured to serve from the `main` branch, root folder. Pushing to `main` triggers a redeploy.
