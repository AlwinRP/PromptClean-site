# PromptClean website

The landing page (`index.html`) and privacy policy (`privacy.html`) for the PromptClean Chrome extension. Plain HTML and one stylesheet: no build step, no scripts, no third-party fonts or analytics.

## Before publishing

Fill in the highlighted placeholders (they render with a yellow background):

- `privacy.html`: publisher name and contact email
- `index.html` and `privacy.html` footers: contact email
- `index.html`, "For your IT team": the link to the public source code (or remove the row)
- `index.html`, "Get PromptClean": the Chrome Web Store link, and point the "Add to Chrome" button at it

## Publish on GitHub Pages

1. Create a public GitHub repository and push this folder to it.
2. In the repository: **Settings → Pages → Build and deployment → Deploy from a branch**, branch `main`, folder `/ (root)`.
3. Put the resulting address (for example `https://<user>.github.io/promptclean-site/`) in the Chrome Web Store listing as the homepage, and `…/privacy.html` as the privacy policy.

## Images

`assets/icon-128.png` and `assets/favicon.png` are copied from the extension repository (`icons/`), where `brand/render-assets.mjs` renders them. Re-copy them if the icon changes. The before/after on the landing page is HTML, not an image, so it stays readable on phones; keep it in step with what Compress actually outputs.
