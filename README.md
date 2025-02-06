# sutra-whitepaper
This repository contains the complete LaTeX files, bibliography, figures, and necessary scripts to compile the paper. SUTRA introduces a novel dual-transformer approach that decouples concept learning and language learning.


## Repository Structure

- `README.md` - This file
- `arxiv.sty` - ArXiv style file for formatting
- `images/` - Directory containing figures and diagrams
- `main.tex` - Main LaTeX source file
- `references.bib` - Bibliography file with references

## How to Compile

To generate the PDF from the LaTeX source, follow these steps:

### Using `pdflatex` and `bibtex`
```sh
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
