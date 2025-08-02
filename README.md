# Bachelor's Thesis - Computer Science

A Bachelor's thesis project in Computer Science at the University of Naples "Federico II" (UniNA), built using the official [unina-thesis-template](https://github.com/luistar/unina-thesis-template).

## Thesis Information

**Title:** A fancy LaTeX template for your thesis at UniNA  
**Author:** Riccardo Elena  
**Student ID:** N86/4490  
**Supervisors:** Prof. Fabio Mogavero, Prof. Massimo Benerecetti  
**Academic Year:** 2024-2025  
**Degree Program:** Bachelor's in Computer Science  
**Department:** Dipartimento di Ingegneria Elettrica e Tecnologie dell'Informazione
**School:** Scuola Politecnica e delle Scienze di Base  

## Abstract

[Add your thesis abstract here - a brief summary of your research, methodology, and key findings]

## Structure

The thesis is organized as follows:

- **Abstract** - Summary of the work
- **Introduction** - Context and motivation
- **Chapter 1** - [Your first chapter title]
- **Chapter 2** - [Your second chapter title]
- **Conclusions** - Summary and future work
- **Appendix** - Additional materials
- **Bibliography** - References and citations

## Building the Document

This project uses LaTeX with biblatex for bibliography management. To compile:

```bash
pdflatex thesis
biber thesis
pdflatex thesis
pdflatex thesis
```

Or use latexmk for automatic compilation:

```bash
latexmk -pdf thesis.tex
```

## Template Features

This thesis leverages the unina-thesis-template which provides:

* Official UniNA front pages with the unina-frontespizio package
* Multiple typeface options
* Inline table of contents for chapters
* Custom commands for unnumbered sections
* Consistent styling for tables, algorithms, and code listings
* Built-in draft mode and todo utilities

## Repository Structure

```
├── thesis.tex              # Main thesis document
├── uninathesis.cls         # UniNA thesis class file
├── uninafrontespizio.sty   # Front page styling
├── _chapters/              # Thesis chapters
│   ├── 0-abstract.tex
│   ├── 0-introduction.tex
│   ├── 1-first-chapter.tex
│   ├── 2-second-chapter.tex
│   ├── 3-conclusions.tex
│   └── 4-appendix.tex
├── _bib/                   # Bibliography files
│   └── bibliography.bib
├── _figures/               # Figures and images
├── _utils/                 # Utility files and macros
│   └── macro.tex
└── _builds/                # Build artifacts (ignored by git)
```

## License

This thesis project is based on the unina-thesis-template, which is licensed under GPL v3. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

Special thanks to [Luigi Lucio Libero Starace](https://github.com/luistar), the creator of the [unina-thesis-template](https://github.com/luistar/unina-thesis-template), for providing an excellent LaTeX template for UniNA theses.
