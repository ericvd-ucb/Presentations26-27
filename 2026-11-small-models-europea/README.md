# Small Models in the Browser

This deck uses its own theme (`small-models.scss`), not the shared slide-kit theme, so it is not part of the project render (its source is `small-models-browser.qmd`, not `index.qmd`).

To rebuild, render it outside the project so `_quarto.yml` does not add the slide-kit theme, then copy the output into `docs/2026-11-small-models-europea/`:

1. Copy this folder somewhere outside the repo and run `quarto render small-models-browser.qmd`.
2. Copy `small-models-browser.html` to `docs/2026-11-small-models-europea/index.html`, along with `small-models-browser_files/` and `images/`.
