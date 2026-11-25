# Semantic model AI-readiness check

A single static page. No server, no build step, nothing is uploaded: the check runs in the visitor's browser.

Accepts a Power BI Project `.SemanticModel` folder (TMDL), a `model.bim` file, or `.tmdl` files.
A `.pbix` cannot be read in a browser; the page explains how to convert it.

## Publish with GitHub Pages
1. Create a repository and upload `index.html` and `.nojekyll` to the main branch.
2. Settings > Pages > Build and deployment > Deploy from a branch > main > / (root) > Save.
3. After a minute the page is live at `https://<owner>.github.io/<repo>/`.

The scoring lives in the script block at the top of `index.html` (function `analyze`).
