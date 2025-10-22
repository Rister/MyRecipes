# Gemini Code Assistant Context

## Directory Overview

This directory contains the source code for a personal recipe book, titled "Jeremy's Favorite Recipes". The book is written in LaTeX, utilizing the `cuisine` package to format the recipes in a structured and visually appealing way.

### LaTeX Document Structure

*   **Document Class**: The project uses the `book` document class (`\documentclass{book}`), which is suitable for longer documents with chapters and sections.
*   **Page Layout**: The `geometry` package is used to customize page margins and dimensions (`\usepackage[inner=1.5in,outer=1in,top=0.75in,bottom=0.75in]{geometry}`).

## Key Files

*   **`main.tex`**: This is the main LaTeX file for the project. It contains all the recipe content, including ingredients and instructions for various dishes. The file uses the `\documentclass{book}` and imports the `cuisine` package for recipe typesetting.

*   **`README.md`**: A brief file stating the purpose of the repository.

*   **`.gitignore`**: A standard LaTeX `.gitignore` file, which lists temporary and generated files (like `.aux`, `.log`, `.pdf`) that should be excluded from version control.

## Cuisine Package Specifics

The `cuisine` LaTeX package introduces several specialized commands for recipe typesetting:

*   **`\newstep`**: This command is used to delineate distinct steps within a recipe's instructions, helping to organize the method section clearly.
*   **`\freeform`**: When used within a `recipe` environment, this command alters the default behavior of the `cuisine` package, allowing for a more flexible layout where ingredients are not automatically placed in the margin.
*   **`\X`**: Used to represent the multiplication symbol (e.g., `9\X 13 pan` renders as "9×13 pan").
*   **`\0`**: A shorthand for the degree symbol (e.g., `350\0 F` renders as "350°F").
*   **`\fr{numerator}{denominator}`**: Used for typesetting fractions (e.g., `\fr{1}{2}` renders as "1/2").
*   **Ingredient Commands**: The package provides several commands for listing ingredients:
    *   **`\ingredient[<qty>]{<unit>}{<item>}`** or **`\ing[<qty>]{<unit>}{<item>}`**: These are used for quantified ingredients, typically displayed in the margin next to the relevant recipe step.
    *   **`\Ingredient{<item>}`** or **`\Ing{<item>}`**: These are used for ingredients that are not quantified in the standard way, or for optional ingredients. They are generally displayed inline with the recipe text.

## Usage and Building

This is a LaTeX project. To compile it into a PDF document, you will need a LaTeX distribution (like TeX Live, MiKTeX, or MacTeX) installed on your system.

The typical command to build the project is:

```bash
pdflatex main.tex
```

You may need to run the command more than once to ensure all cross-references and the table of contents are generated correctly.
