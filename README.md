# veronicasalazarrestrepo.com — GitHub Pages

Personal academic website. Plain HTML/CSS, no build step.

## Files

- `index.html` — home page
- `research.html` — working papers, work in progress, publications
- `style.css` — all styling (colors are CSS variables at the top)
- `photo.jpg` — **add this yourself**: your profile photo (roughly square or portrait, ≥500px wide)

## Publish on GitHub Pages

1. Create a repo named `veronicasalazar.github.io` (public) on github.com.
2. Add these files (drag-and-drop via "Add file > Upload files" works, no git needed).
3. Add your `photo.jpg`.
4. Repo Settings > Pages: source = `main` branch, `/ (root)`. Site goes live at `https://veronicasalazar.github.io` within a minute.

## Point your custom domain

1. Repo Settings > Pages > Custom domain: enter `www.veronicasalazarrestrepo.com`, save, and enable "Enforce HTTPS" once available.
2. At your domain registrar, set DNS:
   - `CNAME` record: `www` → `vsalazarr.github.io`
   - Four `A` records for the apex domain (`veronicasalazarrestrepo.com`): `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
3. In Google Sites, unpublish the old site once the new one is live (Settings > Custom domains, remove the domain first).

DNS changes can take up to 24h to propagate.

## Editing tips

- Add a paper: copy a `<div class="paper">…</div>` block in `research.html`.
- Change colors: edit the `--green`, `--gold`, `--bg` variables at the top of `style.css`.
- Update CV: replace the Dropbox link in both HTML files, or commit `cv.pdf` to the repo and link to `cv.pdf` instead (recommended — no more broken Dropbox links).
