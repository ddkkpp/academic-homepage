# Kunpeng Ding — Academic Homepage

A responsive, dependency-free academic homepage published through GitHub Pages.

## Repository contents

- .github/workflows/deploy.yml: GitHub Pages deployment workflow.
- public/index.html: page content and profile links.
- public/style.css: responsive layout and styling.
- public/assets/profile.jpg: supplied profile photo.
- public/assets/favicon.svg: site favicon.
- public/cv.pdf: supplied CV, openable in a browser preview or available to download.
- public/papers/ATC2026_RSM.pdf: ATC 2026 paper.

## Deploy

The workflow deploys the public directory on pushes to main and supports manual runs. In repository Settings → Pages, select GitHub Actions as the build and deployment source.

Published site: https://ddkkpp.github.io/academic-homepage/

## Preview

Open public/index.html directly, or run this command from the repository root:

    python -m http.server 8000 --directory public

Then visit http://localhost:8000.

## Profile links

- Google Scholar: https://scholar.google.com/citations?user=GgBCIJIAAAAJ&hl=en
- CNIPA patent search: https://pss-system.cponline.cnipa.gov.cn/conventionalSearch (search CN116846603A).
- HPR-DS, NetRT, SLP, and RPBV link to their DOI/publisher pages in public/index.html.

The page lists five publications. MCM is shown separately as ongoing research.
