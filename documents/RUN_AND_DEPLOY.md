Run and deploy the site

Prerequisite

- Install Hugo (extended): https://gohugo.io/getting-started/install/

Run locally (with drafts)

```bash
hugo server -D
# open http://localhost:1313
```

Build static output

```bash
hugo
# files in ./public
```

Deploy options

Option A — Any static hosting

1. Build: `hugo`
2. Upload the `public/` directory to your host

Option B — GitHub Pages (build locally)

1. `hugo` to build
2. Push `public/` to a `gh-pages` branch
3. In repo settings → Pages, select the `gh-pages` branch and `/` root

Option C — GitHub Pages (CI/CD)

- Add a GitHub Actions workflow that:
  - Runs `hugo` on pushes to `main`
  - Publishes the `public/` folder to GitHub Pages

Option D — Netlify / Vercel / Cloudflare Pages

- Connect this repository
- Build command: `hugo`
- Publish directory: `public`

Notes

- Site title/description in `hugo.toml`
- Favicons and `site.webmanifest` live in `static/`
- Default theme loads as dark unless a user preference is stored
