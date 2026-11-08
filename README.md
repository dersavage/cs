# Computer Science

Hugo blog using the [hugo-trainsh](https://hugo-trainsh.pages.dev/) theme.
Live at https://dersavage.github.io/cs/.

- Posts: `content/posts/*.md`
- Build locally: `hugo server`
- Deploys on every push to `main` via `.github/workflows/pages.yml`
- The theme is vendored in `themes/hugo-trainsh`, with one fix so it works under the `/cs/` subpath
  (the brand link and home link use `site.Home.RelPermalink`).
