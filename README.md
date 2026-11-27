# All things CS

Hugo blog using the [Contour](https://themes.gohugo.io/themes/hugo-contour/) theme.
Live at https://dersavage.github.io/cs/.

- Posts: `content/posts/*.md`
- Build locally: `hugo server` (Hugo extended 0.160+)
- Deploys on every push to `main` via `.github/workflows/pages.yml`
- The theme is vendored unmodified in `themes/contour` (without its example site and screenshots).
  Site-level overrides live outside it:
  - `layouts/home.html` + `assets/css/home-intro.css`: show the body of `content/_index.md` on the landing page
  - `layouts/_partials/logo.html`: no empty kicker chip
  - `layouts/_partials/copyright.html`: copyright shows the author (`params.author`)
  - `layouts/_partials/head.html`: defaults to dark theme instead of following the OS setting
  - `assets/js/contour.js`: the landing-page terrain (canvas `#terrain`) slowly animates
- Colours: Pip-Boy green `#1aff80` on near-black (`params.fg` / `params.bg` in `hugo.toml`)
- `/blog/` redirects to `/posts/` (alias in `content/posts/_index.md`)
