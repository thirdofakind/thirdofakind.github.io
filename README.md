# Hadley's Portfolio (Jekyll + GitHub Pages)

A clean, fast portfolio using the **minima** theme. Includes:
- Projects collection (`_projects/`) with individual pages
- Blog posts (`_posts/`) for notes & case studies
- About & Contact pages
- SEO + RSS out of the box

## Quick Deploy (GitHub Pages)
1. Create a new repo and push these files.
2. In **Settings → Pages**, set:
   - **Source**: `main` (or your default branch)
   - **Folder**: `/ (root)`
3. Save. Wait ~1–2 minutes, then your site will be live at:
   `https://<your-username>.github.io/<repo>` or `https://<your-username>.github.io` if you name the repo `<your-username>.github.io`.

## Edit Content
- Projects live in `_projects/`. Add more `.md` files with front matter.
- Blog posts go in `_posts/` (use `YYYY-MM-DD-title.md`).
- Update social links in `_config.yml` under `minima.social_links`.
- Replace images in `assets/img/` and update paths in project pages.

## Local Preview (optional)
If you have Ruby installed:
```bash
bundle install
bundle exec jekyll serve
```
Open http://127.0.0.1:4000
