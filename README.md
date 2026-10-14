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

The homepage follows the layout of [Yi Ren's homepage](https://rayeren.github.io/): a profile sidebar, blue links and venue labels, paper figures beside citations on desktop, and a single column on mobile. The original AcadHomepage MIT license is retained.

Publication metadata is in `_data/publications.yml`, rendered by `_includes/publications.html`. Biography, research projects, education, and skills are in `_pages/about.md`. The content follows the base CV; a submitted RA-L paper is described as submitted rather than published.

The publication thumbnails display complete figures at their natural aspect ratios, without cropping or stretching them in CSS:

| File | Source |
| --- | --- |
| `images/papers/tro2026-fig1.png` | Figure 1, Ma et al., *IEEE Transactions on Robotics* (2026), [DOI](https://doi.org/10.1109/TRO.2026.3710397). |
| `images/papers/natcomm2026-fig1.png` | Figure 1, Lai et al., *Nature Communications* (2026), [DOI](https://doi.org/10.1038/s41467-026-74225-3), unchanged, [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). |
| `images/papers/tii2024-fig2.png` | Figure 2, Su et al., *IEEE Transactions on Industrial Informatics* (2024), [DOI](https://doi.org/10.1109/TII.2024.3423458), unchanged, [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/). |
| `images/papers/arso2024-fig1.png` | Figure 1, Wang, Ma, and Ren, *IEEE ARSO* (2024), [DOI](https://doi.org/10.1109/ARSO60199.2024.10557802). |

Figure source credits appear beside each paper on the page. Earlier placeholder files are retained but are no longer displayed.
