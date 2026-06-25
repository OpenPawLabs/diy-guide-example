# diy-guide-example

A complete, working example of a DIY guide embedded in a plain HTML page and
published to GitHub Pages — no build step or coding required. It consumes the
[`openpawlabs/diy-guide-embedder`](https://github.com/OpenPawLabs/diy-guide-embedder)
script.

Live demo: https://openpawlabs.github.io/diy-guide-example/

## What's here

```
index.html            # the page — one <script> tag + a <diy-guide> element
guide/
  guide.mdx           # the guide, edited with the DIY Guides authoring tool
  images/             # images referenced by the guide (./images/...)
.github/workflows/    # publishes the files to GitHub Pages on push
```

The whole page is just:

```html
<diy-guide src="./guide/guide.mdx"></diy-guide>
<script src="https://openpawlabs.github.io/diy-guide-embedder/embed.js" defer></script>
```

## Make it your own

1. Use this repository as a template (or download it as a zip and create your own
   GitHub repository from the files).
2. Edit `guide/guide.mdx` with the
   [DIY Guides authoring tool](https://openpawlabs.github.io/diy-guides-authoring-tool/),
   adding your images under `guide/images/`.
3. Commit and push. GitHub Pages publishes your guide automatically.

Enable GitHub Pages once under **Settings → Pages → Source: GitHub Actions**.
