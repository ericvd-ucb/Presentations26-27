# slide-kit

Shared theme, rules and images for Eric's Quarto reveal.js decks.

- `CLAUDE.md`: master copy of the slide style and voice rules. Copy into each new deck folder.
- `cdss-slides.scss`: master theme. Copy into each new deck folder.
- `images/`: reusable images. Copy only what a deck needs into that deck's own `images/` folder.

## Where things live

- This folder (`~/Documents/Vibecoding/slide-kit`) is the master copy of the kit. Edit the theme, rules and images here.
- `~/Documents/GitHub/Presentations26-27/slide-kit` is a copy for the published repo. Refresh it from here; don't edit it directly.

## Starting a new deck

1. Make a folder `~/Documents/Vibecoding/YYYY-MM-venue/` and copy in `CLAUDE.md` and `cdss-slides.scss`. Name the deck `index.qmd`.
2. Copy `images/logos/uc-berkeley.svg` and `images/logos/cdss.svg` into the deck's `images/` folder, plus any other images it uses.
3. New images go into this kit first, with a line in the index below. New theme classes go into this kit's `cdss-slides.scss` too.

## Moving a finished deck to the repo

1. Copy the deck folder into `~/Documents/GitHub/Presentations26-27/`.
2. If the theme changed, copy this kit's `cdss-slides.scss`, `CLAUDE.md`, `README.md` and `images/` into the repo's `slide-kit/` folder.
3. Render with `quarto render` from the repo root, add a row to the repo README, then commit and push with GitHub Desktop.

## Naming

Lowercase, hyphens, no spaces. Add a year to screenshots that will date: `datahub-login-2026.png`.

## Image index

| File | What it is | Source |
|---|---|---|
| logos/uc-berkeley.svg | UC Berkeley wordmark (white; needs a dark background) | https://brand.berkeley.edu/wp-content/themes/gallantry/dist/imgs/logo-uc-berkeley.svg |
| logos/cdss.svg | CDSS logo (theme inverts it to white on the title slide) | https://cdss.berkeley.edu/sites/all/themes/cdss/images/DESKTOP_SECTIONS/HEADER-FOOTER/CDSS_LOGO.svg |
| logos/data8-logo.png | Data 8 logo | https://www.data8.org/fa24/data8logo.png |
| logos/jupyterlite-wordmark.svg | JupyterLite wordmark | JupyterLite project |
| logos/databricks-logo.svg | Databricks logo, stacked (red mark, black wordmark; needs a light background) | https://commons.wikimedia.org/wiki/File:Databricks-logo.svg |
| logos/alpaca-logo.png | Alpaca wordmark (yellow mark, black text; needs a light background) | https://alpaca.markets/static/images/email/logo-plain.png |
| logos/jupyter-logo.svg | Jupyter logo (orange and grey; light background) | https://commons.wikimedia.org/wiki/File:Jupyter_logo.svg |
| logos/jupyter-logo-white.svg | Jupyter logo, white text and light moons, orange kept (for dark backgrounds, e.g. title slide) | Made from logos/jupyter-logo.svg for the UEM talk, Nov 2026 |
| logos/numpy-logo.svg | NumPy logo, 2020 version (blue; light background) | https://commons.wikimedia.org/wiki/File:NumPy_logo_2020.svg |
| logos/pandas-logo.svg | pandas logo (navy wordmark; light background) | https://commons.wikimedia.org/wiki/File:Pandas_logo.svg |
| logos/scikit-learn-logo.svg | scikit-learn logo, small (orange and blue) | https://commons.wikimedia.org/wiki/File:Scikit_learn_logo_small.svg |
| logos/pytorch-logo.svg | PyTorch logo (black wordmark; light background) | https://commons.wikimedia.org/wiki/File:PyTorch_logo_black.svg |
| logos/github-logo.svg | GitHub Invertocat mark (black; light background) | https://commons.wikimedia.org/wiki/File:GitHub_Invertocat_Logo.svg |
| logos/huggingface-ollama-jupyter-combined.png | Hugging Face, Ollama and Jupyter logos combined | Made for the Amsterdam talk, Oct 2026 |
| screenshots/inferential-thinking-textbook.png | Data 8 textbook landing page | inferentialthinking.com |
| screenshots/jupyterhub-small-lm-notebook.png | Notebook loading a small Qwen model on JupyterHub | Eric's screenshot, Oct 2026 |
| screenshots/data8-lecture01-sp18.png | First slide of Data 8 Lecture 1, Spring 2018 | https://www.data8.org/materials-sp18/lec/lec01PDF.pdf |
| screenshots/tao-math-2-caltech-2026.png | Terence Tao, "Math 2.0" title slide, AIM Public Lecture, Caltech, Oct 2026 | https://teorth.github.io/tao-web/slides/math-2-0-caltech-2026.pdf |
| screenshots/dailycal_MathGrades.png | Daily Californian, "AI use leads UC Berkeley math professor to see no point in grading homework" (Borcherds), Oct 23, 2026 | https://www.dailycal.org |
| screenshots/DSUS_lunchtalks.png | DSUS lightning talks program: Pardos, Adhikari, Bray, Ousterhout, DeNero, Garcia | CDSS Data Science Undergraduate Studies |
| screenshots/PraireLearn_SS.png | PrairieLearn question, Econ 148 Spring 2026 (pandas fill-in-the-blank) | https://www.prairielearn.com |
| screenshots/cbtffull.jpeg | Computer-Based Testing Facility, Moffitt Library, UC Berkeley (small, 300px) | |
| screenshots/pensive.png | Pensieve AI grading interface on handwritten physics work | Pensieve |
| screenshots/61a_bot.png | ACM DL page, "61A Bot Report" (Zamfirescu-Pereira et al., SIGCSE TS 2025) | https://doi.org/10.1145/3641554.3701864 |
| screenshots/EVD_development.png | Collage from the International Development course: outcomes by treatment arm, diarrhea prevalence by round, photo of a community water source | Eric's course materials |
| screenshots/intl-dev-notebook.png | International Development course notebook, Lec9.2-waterguard.ipynb (treatment arms, group by arm), fa25-student repo on GitHub | Eric's screenshot, Nov 2026 |
| screenshots/intl-dev-chart.png | Bar chart of mean self-reported WaterGuard use by treatment arm, from the same notebook | Eric's course materials |
| screenshots/connectors.png | Connectors Library: connector course notebook repos (Child Development, City Planning, Civil Eng, Cog Sci, Data 88 EconModels, Genetics, Demography) | Eric's screenshot, Nov 2026 |
| screenshots/data88e-notebook.png | Data 88E Economic Models Textbook, Cobb-Douglas utility with budget constraint (3D plot, dark theme) | Eric's screenshot, Nov 2026 |
| screenshots/before-after.png | Data 88E fall 2024 demand survey: Google Sheet responses, same data read into a notebook table, plotted demand curve (wide strip) | Eric's course materials |
| screenshots/otter-feedback.png | otter-grader feedback in a notebook: grader.check("q4") on a wrong square function, failing test with expected output | Eric's screenshot, Nov 2026 |
| screenshots/lopez-jupytercon.png | JupyterCon talk, M. López-Caniego et al. (ESAC, Madrid): "Closing the loop from astronomical data exploration to scientific discovery using the Jupyterverse" (video frame, subtitles cropped) | JupyterCon video |
| screenshots/lopez-esa-docs.png | euclid-jupyter-notebooks, Getting_started.ipynb: how to access Euclid data (mounted volumes table) | GitHub |
| screenshots/acosta-protein.png | Poster, Acosta and Del Arco (UEM), "AI-guided therapeutic peptide design: a challenge-based learning experience in biomedical education," ICERI 2026 (portrait) | Javier Acosta |
| screenshots/lorca.png | Eric at LORCA (Laboratorio Optimizado de Recursos de Computación Avanzada), Universidad Europea de Madrid; phone badge removed | Eric's photo, Nov 2026 |
| screenshots/migracion.jpeg | Spanish news graphic, "Récord de empleo en los últimos años": EPA employed and Social Security affiliates 1996-2026 by presidential term, headline on 18-19% job growth (portrait) | El Diario, Instagram: https://www.instagram.com/p/DeXZ-VrGlI6/ |
| screenshots/colab-interface.png | spain_economy_by_term.ipynb in Google Colab (dark theme): toolbar, employment plotting cell, chart shaded by presidential term | Eric's screenshot, Nov 2026 |
| screenshots/maria_cruz.png | María Cruz Gaya López (UEM), meteoritos_pandas_profesor.ipynb: Computación Científica I, NASA Meteorite Landings project (Spanish) | universidad-europea-collab repo |
| screenshots/jose_naveiro.png | José Naveiro (UEM), metal_cutting_demo.ipynb: cutting speed and spindle speed for turning a steel shaft | universidad-europea-collab repo |
| figures/qr-jupyterlite-ai.svg | QR code to the JupyterLite AI demo | jupyterlite.github.io/ai |
| figures/qr-small-models-lite.svg | QR code to the Small Models in the Browser JupyterLite site | https://ericvd-ucb.github.io/small-models-lite/ |
| figures/qr-colombia-26-nb.svg | QR code to the Colombia-26-NB notebook repository | github.com/ericvd-ucb/Colombia-26-NB |

## Wanted

Cloudbank logo, 2i2c logo, NSF logo, NAIRR logo, DataHub screenshot, Cloudbank Classroom screenshot.
