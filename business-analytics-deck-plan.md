# New deck: Econ, Python and jobs in the AI era (business analytics students)

Instructions for Claude Code. Build a new Quarto reveal.js deck in this repo (`Presentations26-27`), reusing existing slides and screenshots. **Do not ask for or create new screenshots.** Every image below already exists in the repo.

## Setup

1. Create the folder `2026-12-business-analytics/` (rename later if the date or venue changes) with the deck as `index.qmd`.
2. Follow `slide-kit/CLAUDE.md` for theme, components, voice and speaker notes. Read it first. Key points: academic and professional voice, no punch lines, no rhetorical triplets, no emdashes, one idea per slide, speaker notes as brief bullet reminders.
3. Front matter: copy from `2026-11-europea/index.qmd`, using `theme: [default, ../slide-kit/cdss-slides.scss]`. Footer: `"Business Analytics | [Venue] | Eric Van Dusen, UC Berkeley"`.
4. Copy only the images this deck uses into `2026-12-business-analytics/images/` (`logos/`, `screenshots/`, `figures/`).
5. Where a slide is marked REUSE, copy the slide markdown from the named deck and adapt the wording lightly for a business analytics audience. Keep the existing image classes (`.shot`, `.profile-slide`, `.lite-slide` and so on).
6. Placeholders for things Eric must fill in: `[DATE]`, `[VENUE]`, and any `[VERIFY]` claim. Do not invent statistics about jobs or hiring. If a slide needs a figure that is not in an existing deck, leave a `[VERIFY: ...]` note in the speaker notes.

## Sources to reuse from

- `2026-11-jupyter-europea/index.qmd` (Nov 19 Jupyter talk): path into notebooks, Data 8, connectors, Data 88E, before/after, Python packages, otter feedback, Colab, Spain chart exercise.
- `2026-11-europea/index.qmd` (Nov 4 AI and Education talk): Daily Cal grading slide, PrairieLearn (Econ 148), Tao, small open models, small models in the browser.
- Also available locally, outside this repo, if useful: `~/Documents/GitHub/Colombia-26-slides` (Bogotá: Econ 148 examples, "skills for the AI era" slides, vibecession notebook) and `~/Documents/GitHub/AI_Edu_Talk_Oct26` (Amsterdam: three levels of compute, browser demo). Check them for slide text before writing new text.

## Audience and message

Business analytics students. Rough length: [LENGTH, assume 30 minutes, about 25 slides].

The argument, in order:

1. Economics and Python fit together: Berkeley teaches economics through notebooks (Data 88E, Econ 148).
2. Jobs in the AI era increasingly expect Python, data skills and working fluency with AI tools, alongside domain knowledge.
3. Step one: learn to vibecode, that is, to build analyses with an AI assistant, while still reading and checking the code.
4. Step two: work with small models directly, to understand the harness concepts that sit around every AI product (tokens, chat roles, system prompts, context and memory, tools, evaluation).

## Slide plan

### Opening

1. **Title** `{.title-dark}`. Title: "Economics, Python and AI: Skills for Analytics Work". Subtitle: "Data 88E, Econ 148 and learning to work with models". Byline with `[DATE]`, `[VENUE]`, github link. Logos: `uc-berkeley.svg`, `cdss.svg`.
2. **Plan for today.** REUSE the structure of "Plan for today" from `2026-11-jupyter-europea`. Four parts: Economics in notebooks; Skills for jobs in the AI era; Step one: vibecoding; Step two: small models and the harness.

### Part 1: Economics in notebooks

3. `## Part 1 {.section-dark}` divider: "Economics in notebooks".
4. **My path into notebooks.** REUSE from `2026-11-jupyter-europea` (`EVD_development.png`). Shorten to the international development to notebooks story.
5. **Data 8: Foundations of Data Science.** REUSE from `2026-11-jupyter-europea` (`data8-logo.png`, `inferential-thinking-textbook.png`).
6. **The Data Science Connectors model.** REUSE (`connectors.png`).
7. **Data 88E: Economic Models.** REUSE (`data88e-notebook.png`).
8. **Start from an existing assignment.** REUSE "Start from your existing assignments" (`before-after.png`, class demand survey to demand curve). Good fit for business students: survey data in a spreadsheet becomes a demand curve.
9. **Econ 148: Data Science for Economists.** New text slide, or reuse from `Colombia-26-slides` if a version exists. Use `.cards` with three examples:
   - Forecasting: ARIMA, Prophet and Chronos-2 on Zillow rent and CPI data.
   - ML fairness: income prediction on Folktables/ACS data with SHAP explanations.
   - Survival analysis: time to reemployment for displaced workers, IPUMS CPS with lifelines.
   Speaker notes: classic econometrics next to a foundation model on the same data.
10. **Frequent assessment in Econ 148.** REUSE "PrairieLearn for frequent assessment" from `2026-11-europea` (`PraireLearn_SS.png`). Trim to one point: students practice pandas code with immediate feedback.
11. **The Python stack.** REUSE "Learning a new Python package" logo slide from `2026-11-jupyter-europea` (Jupyter, NumPy, pandas, scikit-learn, PyTorch logos). For analytics students, note that the same stack runs in Colab, Databricks (`databricks-logo.svg` is in the kit) and JupyterHub.

### Part 2: Skills for jobs in the AI era

12. `## Part 2 {.section-dark}` divider: "Skills for jobs in the AI era".
13. **What changes when AI writes code.** REUSE the Daily Cal slide "Grading homework in math at Berkeley" from `2026-11-europea` (`dailycal_MathGrades.png`), reframed: AI tools can now do much of the routine work in a course or a job, so what is left to learn?
14. **Skills that keep their value.** REUSE from `Colombia-26-slides` if present (the "know Python / ask an inferential question / know how to debug" slides), condensed to one `.chips` or `.cards` slide:
    - Read and write Python, because AI tools produce code you have to check.
    - Ask an inferential question: prediction versus cause and effect.
    - Debug and test: AI-generated code often fails without an error message.
    - Know the domain: economics or business knowledge is what makes a result meaningful.
    Speaker notes: `[VERIFY]` any claim about employer demand before adding a number.
15. **There is more analysis to do, not less.** REUSE "Terence Tao: the frontier keeps expanding" from `2026-11-europea` (`tao-math-2-caltech-2026.png`). Point: AI expands the set of questions people can work on.

### Part 3: Step one, vibecoding

16. `## Part 3 {.section-dark}` divider: "Step one: vibecoding".
17. **What vibecoding means.** New text slide. Describe it plainly: describing an analysis in natural language and having an AI assistant write the code, then running, reading and revising it. Use `.flow .flow-navy` with steps: describe the question; generate code; run it; read and check it; revise. Add a `.bottom-question`: "How do you know the code is right?"
18. **Exercise: can we reproduce this chart?** REUSE "Can we reproduce this chart?" from `2026-11-jupyter-europea` (`migracion.jpeg`). Frame it as a vibecoding task: start from a published chart, find the data, rebuild it.
19. **The result in a notebook.** REUSE "Notebook basics in Colab" (`colab-interface.png`), trimmed to show the rebuilt chart by Spanish president's term.
20. **A larger example: the vibecession notebook.** New slide using `qr-colombia-26-nb.svg`. Text: sources data from APIs, builds a dataset, compares consumer sentiment with fundamentals, runs a time series model. Built for students in Bogotá, October 2026. Reuse wording from `Colombia-26-slides` if available.
21. **Checking AI-written code with tests.** REUSE "Feedback through autograding" (`otter-feedback.png`). Point: a test shows that a function named `square` actually cubes its input. Tests are how you check vibecoded work.

### Part 4: Step two, small models and the harness

22. `## Part 4 {.section-dark}` divider: "Step two: small models and the harness".
23. **Small open models as teaching tools.** REUSE from `2026-11-europea` (`huggingface-ollama-jupyter-combined.png`). Merge in the main point from "Why small open models?": a model that runs on a laptop or in a browser can be inspected.
24. **A small model in a notebook.** New slide using `jupyterhub-small-lm-notebook.png` (from the kit). Caption: small Qwen model loaded on JupyterHub.
25. **What a harness is.** New slide, `.chips` or `.build-stack` layers. Products like ChatGPT or Claude are a model plus a harness around it. Working with a small model makes each layer visible:
    - Tokens: text becomes numbers.
    - Chat format: system, user and assistant roles.
    - System prompt and settings (temperature).
    - Context and memory: what the model sees on each turn.
    - Tools: letting the model call code or search.
    - Evaluation: testing outputs for accuracy and bias.
    Speaker notes: maps to the small-models-lite notebook series (starter sampler, model cards, chat format, tokens, memory, SAT test taker).
26. **Small models in the browser.** REUSE "Small models in the browser" `{.lite-slide}` from `2026-11-europea` (`qr-small-models-lite.svg`, `jupyterlite-wordmark.svg`). Speaker notes: live demo if wifi allows, have fallback.
27. **Three levels of compute.** REUSE from `AI_Edu_Talk_Oct26` if present (browser, campus hub, public compute, `.stairs`). If not easy to find, skip this slide.
28. **A new course: Understanding AI with small models.** Short text slide on Data 88I, the 2-unit connector in development: runs in JupyterLite, on JupyterHub, or with students' own Ollama; covers bias, evaluation, training data, privacy and API costs. Hedge: "in development".

### Close

29. **Where to start.** `.cards` with QR codes: `qr-small-models-lite.svg`, `qr-colombia-26-nb.svg`, `qr-jupyterlite-ai.svg`, plus the Data 8 textbook link. Suggested steps: open a notebook in Colab, rebuild one chart with an AI assistant, then run a small model and look at its tokens.
30. **Thank you.** REUSE from `2026-11-europea`.

## Before finishing

- Render with `quarto render 2026-12-business-analytics/index.qmd` and check every slide for overflow. Split or trim rather than shrinking text.
- List all `[VERIFY]`, `[DATE]`, `[VENUE]` placeholders for Eric at the end.
- Add a row to the root `README.md` talks table.
- Do not commit; Eric commits with GitHub Desktop.
