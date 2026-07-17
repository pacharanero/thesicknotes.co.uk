# thesicknotes.co.uk

Static website for The Sicknotes, a 4-piece swingabilly rock band from Yorkshire. Migrated from Canva to a dependency-free static site hosted on GitHub Pages.

## Local development

```sh
s/up        # serves on http://localhost:8000
s/up 3000   # serves on http://localhost:3000
```

## Structure

- `index.html` - single-page site with all content
- `styles.css` - all styling
- `assets/fonts/` - High Cruiser font (woff) + fonts.css
- `assets/media/` - all images (logo, band photos, social icons, gallery)
- `CNAME` - custom domain for GitHub Pages
- `.nojekyll` - disables Jekyll processing on Pages
- `.github/workflows/pages.yml` - GitHub Actions deploy workflow

## Deployment

Pushing to `main` triggers the GitHub Actions workflow which deploys the site to GitHub Pages. The Pages source must be set to "GitHub Actions" in the repo settings.

## Font

The site uses [High Cruiser](https://www.cdnfonts.com/high-cruiser.font) by TypeFairy (personal use license). The woff file is bundled locally in `assets/fonts/`.

## DNS

The custom domain `thesicknotes.co.uk` is managed on Cloudflare. See the deployment instructions for CNAME records pointing to `pacharanero.github.io`.