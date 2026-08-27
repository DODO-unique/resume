# Gaurav Mali - Resume

This repository contains the source files for Gaurav Mali's resume, written in
LaTeX.

## Building

Compile the resume with `pdflatex`:

```bash
pdflatex main.tex
```

The generated resume is written to `main.pdf`. Auxiliary LaTeX build files are
ignored by Git.

## Project structure

- `main.tex` - document entry point and contact details
- `preamble.tex` - packages, typography, layout, and link styling
- `sections/` - project, education, and skills sections
- `sample.md` - Markdown version of the resume content

## Requirements

- A LaTeX distribution such as TeX Live or MiKTeX
- Packages used by the document: `geometry`, `helvet`, `hyperref`,
  `enumitem`, `titlesec`, `xcolor`, `changepage`, and `ulem`