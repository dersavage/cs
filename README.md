# Computer Science

Hugo blog using the [Contour](https://themes.gohugo.io/themes/hugo-contour/) theme.
Live at https://dersavage.github.io/cs/.

- Posts: `content/posts/*.md`
- Build locally: `hugo server` (Hugo extended 0.160+)
- Deploys on every push to `main` via `.github/workflows/pages.yml`
- The theme is vendored unmodified in `themes/contour` (without its example site and screenshots).
  Site-level overrides live outside it:
  - `layouts/home.html` + `assets/css/home-intro.css`: show the body of `content/_index.md` on the landing page
  - `layouts/_partials/logo.html`: smaller logo font so the 16-character title fits, and no empty kicker chip
- `/blog/` redirects to `/posts/` (alias in `content/posts/_index.md`)
