# Shrimp & Bits — Jekyll site

A Jekyll rebuild of selected posts from shrimpnbits.wordpress.com, using the standard `minima` theme.

## Deploy to GitHub Pages

1. Create a new GitHub repo (e.g. `shrimpnbits`).
2. Push this folder's contents to the `main` branch:
   ```bash
   git init
   git add .
   git commit -m "Initial Jekyll site"
   git branch -M main
   git remote add origin git@github.com:YOUR_USER/shrimpnbits.git
   git push -u origin main
   ```
3. In the repo, go to **Settings → Pages**, set **Source = Deploy from a branch**, **Branch = main / (root)**, save.
4. Your site appears at `https://YOUR_USER.github.io/shrimpnbits/`.
   - If you want it at `https://YOUR_USER.github.io/`, name the repo `YOUR_USER.github.io` instead and set `baseurl: ""` (already set).
   - If using a project repo, set `baseurl: "/shrimpnbits"` in `_config.yml`.

## Local preview

```bash
bundle install
bundle exec jekyll serve
```

## Adding more posts

Drop additional files into `_posts/` named `YYYY-MM-DD-slug.md` with the same front matter format. Images go under `assets/images/<slug>/`.
