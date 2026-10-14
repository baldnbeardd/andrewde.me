# andrewde.me

Personal site for Andrew DeGarmo. Plain HTML/CSS, no build step, deployed to GitHub Pages by `.github/workflows/pages.yml` on every push to `main`.

## One-time setup
1. Repo **Settings → Pages → Source: GitHub Actions**.
2. Under **Custom domain** enter `andrewde.me` (the `CNAME` file already sets it) and tick **Enforce HTTPS** once the certificate is issued.
3. At your DNS provider, point the domain at GitHub Pages:
   - `A` records for `@`: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - `CNAME` for `www`: `<your-github-username>.github.io`
   - Remove the old Convertri records.

## Editing
Everything lives in `index.html`. Colors and fonts are CSS variables at the top of the `<style>` block.
To self-host the headshot, add it as `assets/andrew-degarmo.png` and update the `<img src>` and `og:image`.
