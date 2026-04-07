# SaiJaiEval

Marketing website for [SaiJaiEval](https://eval.saijaiai.com), an AI solutions competition platform built by SaiJaiAI.

Built with [Jekyll](https://jekyllrb.com/) using the [Chirpy](https://github.com/cotes2020/jekyll-theme-chirpy/) theme. Deployed on GitHub Pages at `eval.saijaiai.com`.

## Development

**Prerequisites:** Ruby, Bundler, Git

```bash
# Install dependencies
bundle install

# Serve locally (http://localhost:4000)
bundle exec jekyll serve

# Build for production
bundle exec jekyll build
```

## Structure

- `index.html` — Custom landing page with SaiJaiEval branding
- `_posts/` — Blog posts (Jekyll naming convention: `YYYY-MM-DD-title.md`)
- `_tabs/` — Navigation pages (about, archives, categories, tags)
- `_data/` — Contact and social sharing configuration
- `_config.yml` — Main Jekyll and theme configuration
- `assets/` — Static assets

## Deployment

Automatically deploys to GitHub Pages on push to `main`. Custom domain configured via `CNAME`.

## License

[MIT](https://github.com/cotes2020/chirpy-starter/blob/master/LICENSE)
