# sutra-whitepaper
This repository contains the complete LaTeX files, bibliography, figures, and necessary scripts to compile the paper. SUTRA introduces a novel dual-transformer approach that decouples concept learning and language learning.


## Repository Structure
.
├── README.md
├── arxiv.sty
├── images
├── main.tex
└── references.bib

## How to Compile

To generate the PDF from the LaTeX source, follow these steps:

### Using `pdflatex` and `bibtex`
```sh
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
