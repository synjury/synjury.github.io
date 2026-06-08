# synjury.github.io

Informational landing page for **Synjury** — a chain-neutral, stake-secured AI-jury arbitration
protocol for agentic payments. Served via GitHub Pages.

- **Live (default):** https://synjury.github.io/
- **Custom domain:** https://synjury.xyz (see `CNAME`; requires DNS — below)
- Plain static HTML/CSS, no build step (deploy from `main` branch, root). Migrate to a static-site
  generator later if the content grows.

## Deploy
GitHub Pages → Settings → Pages → Source: **Deploy from a branch**, branch `main`, folder `/ (root)`.
`.nojekyll` disables Jekyll processing so files are served as-is.

## Custom domain (synjury.xyz)
At your DNS provider, for the apex `synjury.xyz` add four **A** records to GitHub Pages:
`185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
(and optionally a `CNAME` for `www` → `synjury.github.io`). Then Settings → Pages → Custom domain
→ `synjury.xyz`, and enable **Enforce HTTPS** once the cert provisions.
