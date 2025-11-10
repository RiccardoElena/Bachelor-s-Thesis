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

First-order logic is undecidable, but several decidable fragments have been identified that retain useful expressive power while guaranteeing termination. The fluted fragment is one such subset, characterized by specific variable ordering constraints in quantified formulae.

This thesis implements and evaluates a decision procedure for the fluted fragment within the Vampire theorem prover. The implementation required three main components: a preprocessing stage that transforms input formulae into the required fluted clause form through structural naming, an adapted literal selection strategy compatible with fluted resolution, and a separation inference rule for handling non-strongly fluted clauses applying dynamic renaming.

The experimental evaluation used both existing TPTP benchmark problems and a custom test generator producing 15,000 synthetic problems. While only 151 naturally occurring fluted problems were found in TPTP, testing revealed that the fluted implementation often matches or outperforms standard Vampire resolution on these problems. The synthetic benchmarks provided more extensive evaluation, showing that specialized preprocessing optimizations can benefit performance even when falling back to standard resolution techniques.

The work demonstrates that implementing decision procedures for specific fragments within general-purpose theorem provers is feasible and can provide computational advantages by exploiting structural properties of the input problems.

## Structure

The thesis is organized as follows:

- **Introduction** - Context and motivation of the work
- **Chapter 1** - Introduction to First Order Logic
- **Chapter 2** - Introduction to Resolution Calculu
- **Chapter 3** - In-depth analysis of the decision procedure for the Fluted Fragment implemented
- **Chapter 4** - Overview on the Vampire Theorem Prover Architecture and core feature
- **Chapter 5** - Detailed analysis of the implementation of the procedure
- **Chapter 6** - Implementation benchmarking using the TPTP library
- **Chapter 7** - Implementation of a problem generator for further benchmarking
- **Conclusions** - Summary and future work
- **Appendix** - Additional Charts and tables reporting specific datas
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
