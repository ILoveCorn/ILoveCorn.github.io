# Yan Ma (马彦)

Personal academic homepage, built with [AcadHomepage](https://github.com/RayeRen/acad-homepage.github.io) and published with GitHub Pages.

Site: https://ilovecorn.github.io

This repository is a user site (`ILoveCorn.github.io`). `baseurl` is empty so the site is served from the domain root. Publish the default branch with GitHub Pages (source: repository root).

## Local preview

```bash
bundle install
bundle exec jekyll serve --host 0.0.0.0 --port 4000
```

`run_server.sh` starts the same server with live reload (`hawkins`).

## Docker

```bash
docker build -t jekyll-site .
docker run -p 4000:4000 --rm -v "$(pwd)":/usr/src/app jekyll-site
```

## Google Scholar citations

The workflow in `.github/workflows/google_scholar_crawler.yaml` writes citation data to the `google-scholar-stats` branch. Add a repository secret named `GOOGLE_SCHOLAR_ID` with value `H2TMh68AAAAJ`, then enable Actions. Until that branch exists, the page shows the Scholar link without a citation count.

## Figures

`images/papers/natcomm2026-fig1.png` is Figure 1 of Lai et al., *Nature Communications* (2026), https://doi.org/10.1038/s41467-026-74225-3, used unchanged under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

Temporary light figure cards in `images/papers/` (`placeholder-tro-2026.png`, `placeholder-tii-2024.png`, `placeholder-arso-2024.png`, `placeholder-oct-skin.png`, `placeholder-vla-2026.png`, 972×509) fill publication and project entries that do not yet have a figure. Replace each file when a real image is available.
