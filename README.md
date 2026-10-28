# Aoran Zhang — academic website

Personal academic website built with [al-folio](https://github.com/alshedivat/al-folio) and Jekyll.

- Website: https://aoranzhangmia.github.io/
- Direct CV: https://aoranzhangmia.github.io/Aoran_Zhang_Academic_CV.pdf

## Updating content

- Biography: `_pages/about.md`
- Publications: `_bibliography/papers.bib` (set `selected={true}` to feature a paper on the homepage)
- Research: `_pages/research.md`
- Web CV: `_pages/cv.md`
- Downloadable CV: replace `Aoran_Zhang_Academic_CV.pdf`, keeping its filename unchanged
- News: add a dated Markdown file under `_news/`
- Contact and profile links: `_data/socials.yml`

The site intentionally has no portrait. Analytics and comments are disabled.

## Local build

Use Ruby 3.3.5 and Node.js 22 or later:

```sh
bundle install
bundle exec jekyll serve
```

Open http://localhost:4000/. For production output, run `JEKYLL_ENV=production bundle exec jekyll build`.

## Publishing

GitHub Pages uses GitHub Actions. Every push to `main` runs `.github/workflows/deploy.yml`, builds the site, and publishes it. Wait for the workflow to succeed before checking the public URL.

## Attribution

The al-folio template is MIT licensed; its original license is preserved in `LICENSE`. Personal content and CV remain the author's work.
