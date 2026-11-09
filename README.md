# Kunpeng Ding — Academic Homepage

A lightweight, responsive, dependency-free academic homepage.

## Contents

```text
academic-homepage/
├── README.md
└── public/
    ├── index.html
    ├── style.css
    ├── assets/
    │   └── favicon.svg
    └── papers/
        └── ATC2026_RSM.pdf
```

## Deploy with Cloudflare Pages (Git integration)

1. Create a GitHub repository, for example `academic-homepage`, under the GitHub account you want to use (e.g. `kpding`).
2. Upload the contents of this folder to the repository. Keep the `public/` directory at the repository root.
3. In Cloudflare Dashboard, open **Workers & Pages → Create application → Pages → Connect to Git**.
4. Select the repository and configure:
   - Production branch: `main`
   - Framework preset: `None`
   - Build command: `exit 0`
   - Build output directory: `public`
5. Click **Save and Deploy**.

Cloudflare will publish the site at the project URL, typically `https://<project-name>.pages.dev`.
Each push to the production branch triggers a new deployment.

## Local preview

You can open `public/index.html` directly in a browser. For a local HTTP server, run:

```bash
cd public
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## Updating the CV

The CV section is intentionally a placeholder. When ready:

1. Put your PDF at `public/cv.pdf`.
2. In `public/index.html`, replace the disabled “CV PDF · Coming soon” span with:

```html
<a class="button button-light" href="./cv.pdf" target="_blank" rel="noopener">Download CV (PDF)</a>
```

## Publication links

- ATC 2026: the uploaded PDF is included locally at `public/papers/ATC2026_RSM.pdf`.
- HPR-DS, NetRT, SLP, and RPBV: linked to their DOI/publisher landing pages.
- Patent: linked to the USTC official patent listing.

## Notes

- The GitHub profile link in the page currently points to `https://github.com/kpding`. Change it in `public/index.html` if you want to show a different GitHub profile.
- The page lists five publications. MCM is shown separately as ongoing research, not as a published paper.
