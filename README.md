# blog

Source for my personal blog at <https://omusing.io>.

Markdown posts, rendered by [Jekyll](https://jekyllrb.com) with the [Chirpy](https://github.com/cotes2020/jekyll-theme-chirpy) theme, hosted on Cloudflare Pages.

## Writing

Add a file named `_posts/YYYY-MM-DD-title.md` with front matter (`title`, `date`, `categories`, `tags`) and push to `main`.

## Local preview

```sh
bundle install
bundle exec jekyll serve
```

## Deployment (Cloudflare Pages)

Cloudflare Pages builds the site from this repo on every push to `main`:

- Build command: `bundle exec jekyll build`
- Output directory: `_site`
- Environment variables: `JEKYLL_ENV=production`, `RUBY_VERSION=3.3.0`
- Custom domain: `omusing.io` (add under the project's Custom domains tab)

## Conventions

- Published posts: `_posts/YYYY-MM-DD-slug.md`.
- Work in progress: `_drafts/` (not built unless `--drafts` is passed). Start from `_drafts/_TEMPLATE.md`.
- Images: `assets/img/posts/<slug>/`.
- Front matter: `title`, `subtitle` (shown under the title and in listings), `description` (the snippet in listings and SEO).
- Ordering: newest first by front matter `date`. Include time and timezone offset so same-day posts sort reliably.
