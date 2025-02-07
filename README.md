# SUTRA Whitepaper
This repository contains the complete LaTeX files, bibliography, figures, and necessary scripts to compile the paper. SUTRA introduces a novel dual-transformer approach that decouples concept learning and language learning.


## Repository Structure

- `README.md` - This file
- `SUTRA-Whitepaper.pdf` - PDF of pre-compiled whitepaper
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
```

## Table of Contents
- [Introduction](#Introduction)
- [SUTRA's Dual Transformer Architecture](#sutra-models-comes-in-multiple-flavors)
- [Quantitative Evaluation](#repository-structure)

### Introduction

In this paper, we introduce SUTRA, multilingual Large Language Model architecture capable
of understanding, reasoning, and generating text in over 50 languages. SUTRA’s design uniquely
decouples core conceptual understanding from language-specific processing, which facilitates scalable
and efficient multilingual alignment and learning. Employing a Mixture of Experts framework
both in language and concept processing, SUTRA demonstrates both computational efficiency and
responsiveness. Through extensive evaluations, SUTRA is demonstrated to surpass existing models
like GPT-3.5, Llama2 by 20-30% on leading Massive Multitask Language Understanding (MMLU)
benchmarks for multilingual tasks. SUTRA models are also online LLMs that can use knowledge
from the internet to provide hallucination-free, factual and up-to-date responses while retaining their
multilingual capabilities. Furthermore, we explore the broader implications of its architecture for the
future of multilingual AI, highlighting its potential to democratize access to AI technology globally
and to improve the equity and utility of AI in regions with predominantly non-English languages.
Our findings suggest that SUTRA not only fills pivotal gaps in multilingual model capabilities but
also establishes a new benchmark for operational efficiency and scalability in AI applications.


### SUTRA's Dual Transformer Architecture

SUTRA is a novel multilingual large language model architecture that is trained by decoupling concept
learning from language learning. The input is processed through a multilingual concept encoder, followed by the
concept model and finally through a multilingual concept decoder to generate the output response.

![SUTRA API Logo](images/inference_pass.png)
