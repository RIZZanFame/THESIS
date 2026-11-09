# Thermal Debonding of Adhesive Joints in EV Battery Pack Disassembly

*A parametric simulation study of localized heating windows for releasing bonded cells without thermal runaway*

## Project

This repository contains the LaTeX source for Matteo Rizzolio's bachelor's thesis in the Sino-German Mechanical and Energy Engineering (CDHK) program, School of Mechanical Engineering and Robotics, Tongji University.

The thesis is planned to study localized heating as a way to release adhesive-bonded cells during electric-vehicle battery-pack disassembly, while keeping cell temperatures below a defined safety criterion. Its planned scope includes transient heat-conduction modelling, finite-element model verification, and a parametric study of feasible heating conditions.

**Status:** The manuscript is a work in progress. Several sections in `main.tex` are placeholders; this repository does not yet present completed, validated simulation results.

## Repository contents

- `main.tex` — root thesis file; contains the preamble, front matter, and the ordered `\input` calls used to assemble the document.
- `chapters/` — one `.tex` source file for each of the eight thesis chapters.
- `appendices/` — one `.tex` source file for each appendix.
- `figures/tongji_logo.png` — logo used on the title page.
- `main.pdf` — a compiled thesis PDF. Regenerate it after source changes before treating it as current.

No simulation source code, input datasets, or generated simulation results are currently included.

## Build the PDF

Install a LaTeX distribution such as TeX Live or MiKTeX, including the packages used by the source (`geometry`, `setspace`, `amsmath`, `amssymb`, `amsthm`, `graphicx`, `booktabs`, `float`, `hyperref`, and `cleveref`). From the repository root, run:

```sh
pdflatex main.tex
pdflatex main.tex
```

The second run updates the table of contents and lists. Alternatively, if `latexmk` is installed:

```sh
latexmk -pdf main.tex
```

## Citation and reuse

No formal citation metadata or reuse license is provided yet. If citing this work, identify the author, thesis title, Tongji University, and the final submission year. Please do not assume permission to reuse thesis text or figures in the absence of a license.
