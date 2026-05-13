# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository purpose

This repository is the source of a **Jupyter Book** for the course *Física Mecánica* (FISB4020/541) at Universidad Tecnológica Metropolitana. It is not a software project — it is a course ebook composed of MyST Markdown files, Jupyter notebooks, PDFs (guides, past exams, slides), and figures. The built site is published to GitHub Pages at https://fespinozav.github.io/FisicaMecanica/. All student-facing prose is written in **Spanish**; preserve that language when editing or adding content.

## Build and preview

The book is built with `jupyter-book` (pinned to `<2` in [requirements.txt](requirements.txt)) plus `sphinx-proof`. A local `.venv/` already exists.

```bash
# One-time setup
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt

# Build the book (HTML output goes to _build/html/)
jupyter-book build .

# Force a full clean rebuild if TOC/config changes aren't reflected
jupyter-book build --all .
# or
jupyter-book clean . && jupyter-book build .

# Preview locally
open _build/html/index.html
```

Notebook execution is **disabled** at build time (`execute_notebooks: off` in [_config.yml](_config.yml)) — outputs must be saved into the `.ipynb` files before committing, or the rendered page will show empty cells.

## Architecture of the book

The structure is controlled by two files at the repo root; changes to file layout almost always require updating both:

- **[_config.yml](_config.yml)** — Jupyter Book / Sphinx config. Sets Spanish (`language: es`), enables MyST extensions (`amsmath`, `dollarmath`, `colon_fence`, etc.), wires `sphinx-proof` (used for theorems/proofs), and excludes `.venv`, `_build`, `references/`. `only_build_toc_files: true` means **any new content file must be added to `_toc.yml` or it will not be built.**
- **[_toc.yml](_toc.yml)** — the table of contents. `root: README` means the repo `README.md` is the book landing page. The TOC is organized into captioned parts:
  - *Sobre el curso* — intro and bibliography notes
  - *Unidades* — the canonical UTEM units (`contents/utem/unidad1.md` … `unidad8.md`) plus `guias_trabajo.md` and `anexo_python.md`. **These are the primary teaching artifacts students read.**
  - *Problemas y proyectos* — applied problems and prior exams
  - *Bases de la mecanica* / *Modelacion y temas avanzados* — supplementary chapters under `contents/mechanics/`

The `contents/` directory is split by provenance, which matters when editing:

- `contents/utem/` — original/adapted material for this course (UTEM). Free to reorganize.
- `contents/mechanics/` — supplementary chapters covering numerical modeling, oscillations, gravitation, Lagrangian formulation, etc.
- `contents/phy321/` — material derived from Morten Hjorth-Jensen / Scott Pratt's PHY321 (CC0-licensed; see `PHY321_LICENSE_CC0.txt`). Used as conceptual reference.
- `contents/notebooks/`, `contents/evaluations/`, `contents/presentations/` — Jupyter notebooks for controls, PDFs of past exams/pautas, and lecture slides. Most PDFs are linked from Markdown rather than rendered.
- `contents/images/`, `_static/` — figures and static assets.
- `references/` — excluded from build; do not link to files inside.

See [contents/phy321/source_attribution.md](contents/phy321/source_attribution.md) for the editorial rules on adapting external material — preserve attributions when modifying anything under `contents/phy321/`.

## Authoring conventions

- Files are **MyST Markdown** (`.md`), not plain CommonMark. Math uses `$...$` / `$$...$$` (enabled via `dollarmath`); admonitions and proofs use MyST directives via `colon_fence`. Don't switch a file to a different math syntax.
- Cross-references between chapters use relative paths (e.g., `[Unidad 2](contents/utem/unidad2.md)`); the README itself uses these as well.
- When adding a new unit or chapter file, register it in [_toc.yml](_toc.yml) **and** add a link from [README.md](README.md) if it belongs in the public landing page index.
- `figures.ipynb` at the repo root is a scratch notebook for generating figures, not part of the book build.

## What not to touch without intent

- `_build/` is generated output — never edit by hand; rebuild instead.
- `.venv/` is local environment — don't commit changes to it (already gitignored).
- PDFs under `contents/presentations/` and `contents/evaluations/` are binary artifacts authored elsewhere; treat them as opaque assets.
