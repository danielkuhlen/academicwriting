# ![](_figures/academicwriting_hex.png){width="80"} Academic Writing with Quarto

This template provides researchers with a project structure that supports an integrated, reproducible, and transparent writing process. `academicwriting` consolidates Quarto templates for academic articles, abstracts, pre-analysis plans, conference presentations, and R&R memos, keeping all files in a clean, organized structure. If you’ve ever struggled to streamline your projects, this may help.

The basic idea of `academicwriting` is to provide a comprehensive framework for writing research article, consolidating all necessary components into a single project. By organizing all data wrangling, analysis, and writing in one place, this framework ensures that (1) every part of the research project references the same data—allowing for streamlined analysis and a more efficient writing process—and (2) co-authors and readers can clearly understand the processes behind the project.

In practice, all project outputs—such as the paper manuscripts, conference presentations, R&R memos—rely on the same data and bibliography files. The templates also include writing guides and best-practice examples to support both the technical and substantive aspects of writing. :dizzy:

The template synthesizes work from other researchers. The paper and abstract quarto templates are adapted from [Christopher Kenny’s](https://christophertkenny.com) template, available [here](https://github.com/christopherkenny/nature). The abstract features a wording template by [Fabrizio Gilardi](https://fabriziogilardi.org), available [here](https://fabriziogilardi.org/resources/papers/good-abstracts.pdf).

## What You Need to Use This

To use this template, you should have:

-   [TinyTeX](https://yihui.org/tinytex/) installed
-   [Quarto](https://quarto.org/docs/get-started/) installed

## The Structure

![](_figures/template_structure.png)

### Data

This folder stores all relevant data. The `input` folder contains all raw files, while the `output` folder is for files that have already been processed or analyzed.

-   /data
    -   /input
    -   /output

### Wrangling

This folder is for scripts used during the data wrangling process. The template includes an example R script.

-   /wrangling
    -   /example_script.R

### Bibliography

This folder stores all the literature you reference in your project. I recommend connecting Zotero (with the Better BibTeX extension) to this folder, which will automatically export all citations.

-   /bibliography
    -   /bib.bib

### Figures

This folder stores all figures you create.

-   /figures
    -   /example_figure.png

### Paper

This folder contains the template by Christopher Kenny for writing an academic article. The format is a slightly modified Nature style.

-   /paper
    -   /paper.qmd (This is the core file. Rendering this produces the PDF.)
    -   /sections (This is where you write the different sections.)
        -   /introduction.qmd
        -   /theory.qmd
        -   /casestudy.qmd
        -   /methods.qmd
        -   /results.qmd
        -   /conclusion.qmd
        -   /appendix.qmd
    -   /extensions (Stores TeX files for formatting)

The output will then look like this: ![](_figures/paper.png)

### Abstract

-   /abstract
    -   /abstract.qmd (This is the core file. Rendering this produces the PDF)
    -   /extensions (Stores TeX files for formatting)

The output will then look like this:\
![](_figures/abstract.png)

### Presentation

-   /presentation -/presentation.qmd (Core File. Rendering this produces the HTML Slides)

The output will then look like this: ![](_figures/presentation.png)
