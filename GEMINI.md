# GEMINI.md: MyRecipes

## Directory Overview

This directory contains the LaTeX source for a recipe book titled "Jeremy's Favorite Recipes". The project uses the `cuisine` LaTeX package to format the recipes.

## Key Files

*   `main.tex`: This is the main LaTeX file for the recipe book. It contains all the recipe content and uses the `cuisine` package for formatting.
*   `README.md`: A short file that describes the project.
*   `.gitignore`: Standard git ignore file.

## Usage

To generate the recipe book, you will need a LaTeX distribution (like TeX Live, MiKTeX, or MacTeX) installed on your system. You can then compile `main.tex` to produce a PDF file.

For example, using `pdflatex`:

```bash
pdflatex main.tex
```

This may need to be run multiple times to resolve all cross-references.
