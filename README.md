# LaTeX Templates Collection

A curated collection of highly functional, beautifully formatted, and modern LaTeX templates for various academic and professional use cases. 

All templates have been configured to support **XeLaTeX**, which provides built-in support for UTF-8 and modern font rendering.

[🇨🇳 中文说明 (Chinese Readme)](README_zh.md)

## Included Templates

### 1. Academic Paper (`Academic_Paper/`)
A standard, professional two-column LaTeX template, modeled after top-tier conferences (like IEEE/ACM). 
- **Features**: Dual-column layout, robust author/affiliation formatting (`authblk`), modern table and figure setups (`booktabs`), and BibTeX integration (`natbib`).
- **Structure**: Pre-split into multiple `sections/` (Introduction, Related Work, Methodology, Experiments, Conclusion) for easy collaborative writing via Git.

### 2. Academic Report (`Academic_Report/`)
A comprehensive, single-column A4 report template designed for university assignments, project reports, and dissertations.
- **Features**: Clean structure, custom header/footer layout (`fancyhdr`), code snippet highlighting (`listings`), and an organized methodology/results section. 

### 3. Academic Homework (`Academic_Homework/`)
A clean and structured template specifically for solving mathematical or algorithmic homework assignments.
- **Features**: Custom "Solution" environments with framed boxes (`mdframed`), standard theorem packages, and a clean header for student and course information.

### 4. LaTeX Practice (`LaTeX_Practice/`)
A complete functional sandbox demonstrating standard LaTeX capabilities. Excellent for beginners learning LaTeX syntax.
- **Features**: Includes examples for basic text formatting, inline and block math equations, lists, standard tables, and image insertion.

## Compilation Usage

It is highly recommended to compile these documents using **XeLaTeX** to ensure proper rendering (especially for any CJK characters if needed in the future, as the `ctex` package is pre-included natively).

### Command Line
Navigate to the desired directory and run:

```bash
xelatex main.tex
bibtex main      # If the template includes a references.bib
xelatex main.tex
xelatex main.tex
```

### Editors (VSCode / TeXShop / TeXstudio)
Ensure your default compiler or "recipe" is set to use **XeLaTeX**. The files include the `%!TEX TS-program = xelatex` magic comment, which should automatically force most modern editors to use the correct engine.

## Contribution & Collaborative Writing
The `Academic_Paper` template separates the content into the `sections/` directory. By doing this, multiple authors can work on different `.tex` files simultaneously without causing massive Git merge conflicts.