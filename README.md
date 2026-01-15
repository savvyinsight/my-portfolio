# my-portfolio

This repository contains a Hugo-based personal portfolio site.

Preview locally:

```bash
# serve with drafts
hugo server -D
# or serve the generated public/ folder
python3 -m http.server --directory public 8000
```

Build and deploy:

- The repository includes a GitHub Actions workflow at `.github/workflows/deploy.yml` that builds the site and deploys the generated `public/` directory to the `gh-pages` branch.
- Push to `main` to trigger CI and deploy.

Notes:

- `hugo.toml` `baseURL` is set to the GitHub Pages URL: `https://savvyinsight.github.io/my-portfolio/`.
- A copy of the theme CSS was added to `static/css/styles.css` so the site publishes `/css/styles.css`.

If you want a custom domain, add a `CNAME` file to `public/` (and to repo root in a future commit) and configure the domain in repository Pages settings.
