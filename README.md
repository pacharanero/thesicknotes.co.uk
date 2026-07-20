# thesicknotes.co.uk

Static website for The Sicknotes, a 4-piece swingabilly rock band from Yorkshire. Migrated from Canva to a dependency-free static site hosted on GitHub Pages.

## Local development

```sh
s/up        # serves on the first free port from 8000 to 8030
s/up 3000   # serves on the first free port from 3000 to 3030
s/lint      # validates local HTML and CSS asset references
```

## Structure

- `index.html` - single-page site with all content
- `styles.css` - all styling
- `assets/fonts/` - High Cruiser font (woff) + fonts.css
- `assets/media/` - all images (logo, band photos, social icons, gallery)
- `CNAME` - custom domain for GitHub Pages
- `.nojekyll` - disables Jekyll processing on Pages
- `.github/workflows/ci.yml` - static-site lint workflow
- `.github/workflows/pages.yml` - GitHub Actions deploy workflow

## Deployment

Pushing to `main` triggers the GitHub Actions workflow which deploys the site to GitHub Pages. The Pages source must be set to "GitHub Actions" in the repo settings.

## Font And Asset Provenance

The site uses [High Cruiser](https://creativemarket.com/typefairy/5493275-High-Cruiser-Modern-Bold-Sans) by TypeFairy. `assets/fonts/HighCruiser.woff` is the numerals-capable runtime font from the original Canva site, retained solely to reproduce the original website. It is not licensed here for independent reuse or redistribution.

The logo, band photography, and gallery imagery are proprietary to The Sicknotes and their respective copyright owners. The social-media marks remain the property of their respective owners.

## DNS

The custom domain `thesicknotes.co.uk` is managed on Cloudflare. See the deployment instructions for CNAME records pointing to `pacharanero.github.io`.

## Licence

The website code is licensed under [AGPL-3.0-or-later](LICENSE). Repository prose is licensed under CC-BY-SA-4.0. Media and the High Cruiser font have the separate restrictions described above and in [REUSE.toml](REUSE.toml).
