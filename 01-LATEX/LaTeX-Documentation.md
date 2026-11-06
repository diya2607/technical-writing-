
# ✨ LATEX — COMPLETE LEARNING NOTES

<p align="center">
  <b>TECHNICAL WRITING | MODULE 01</b>
</p>

> LaTeX is a document preparation system used to create professional documents with structured formatting, mathematical equations, tables, references and more.

---

## 📑 TABLE OF CONTENTS

1. Introduction to LaTeX
2. Basic Document Structure
3. Document Classes
4. Packages
5. Text Formatting
6. Sections and Subsections
7. Lists
8. Mathematical Equations
9. Tables
10. Images and Figures
11. Labels and References
12. Bibliography and Citations
13. Page Layout
14. Compilation
15. Common Commands
16. Advantages and Applications

---

## 01. INTRODUCTION TO LATEX

- LaTeX is built on top of the TeX typesetting system.
- It is widely used for academic, scientific and technical documents.
- It uses commands to control document structure and formatting.
- It separates content from presentation.

**Popular platforms:**
- Overleaf
- TeXstudio
- MiKTeX
- TeX Live

## 02. BASIC DOCUMENT STRUCTURE

Every basic LaTeX document follows this structure:

```latex
\documentclass{article}

\usepackage{amsmath}
\usepackage{graphicx}

\begin{document}

\title{My First LaTeX Document}
\author{Your Name}
\date{\today}

\maketitle

\section{Introduction}
Welcome to LaTeX!

\end{document}
```

**Important commands:**

| Command | Purpose |
|---|---|
| `\documentclass{article}` | Defines document type |
| `\usepackage{}` | Imports packages |
| `\begin{document}` | Starts document |
| `\end{document}` | Ends document |
| `\maketitle` | Displays title information |

## 03. DOCUMENT CLASSES

Document classes determine the overall structure of a document.

| Class | Application |
|---|---|
| `article` | Articles and short reports |
| `report` | Long reports |
| `book` | Books |
| `letter` | Letters |
| `beamer` | Presentations |

Example:

```latex
\documentclass[12pt,a4paper]{article}
```

## 04. PACKAGES

Packages provide additional features.

| Package | Purpose |
|---|---|
| `amsmath` | Mathematical equations |
| `graphicx` | Inserting images |
| `geometry` | Page margins |
| `xcolor` | Colours |
| `hyperref` | Hyperlinks |
| `booktabs` | Professional tables |
| `listings` | Source code formatting |
| `array` | Advanced table formatting |
| `float` | Figure positioning |
| `fancyhdr` | Headers and footers |

Example:

```latex
\usepackage{graphicx}
\usepackage{amsmath}
\usepackage{xcolor}
```

## 05. TEXT FORMATTING

```latex
\textbf{Bold Text}

\textit{Italic Text}

\underline{Underlined Text}

\emph{Emphasised Text}

\texttt{Monospaced Text}
```

Line break:

```latex
First line.\\
Second line.
```

New paragraph: leave a blank line in the source.

## 06. SECTIONS AND SUBSECTIONS

```latex
\section{Introduction}

\subsection{Background}

\subsubsection{Basic Concepts}
```

For an unnumbered heading:

```latex
\section*{Acknowledgement}
```

## 07. LISTS

**Bulleted list:**

```latex
\begin{itemize}
  \item First point
  \item Second point
  \item Third point
\end{itemize}
```

**Numbered list:**

```latex
\begin{enumerate}
  \item First step
  \item Second step
  \item Third step
\end{enumerate}
```

**Description list:**

```latex
\begin{description}
  \item[LaTeX] Document preparation system.
  \item[TeX] Typesetting system.
\end{description}
```

## 08. MATHEMATICAL EQUATIONS

LaTeX is especially useful for mathematical typesetting.

**Inline equation:**

```latex
The equation is $a^2+b^2=c^2$.
```

**Displayed equation:**

```latex
\[
a^2+b^2=c^2
\]
```

**Fractions:**

```latex
\[
\frac{a+b}{c}
\]
```

**Square roots:**

```latex
\[
\sqrt{x^2+y^2}
\]
```

**Summation:**

```latex
\[
\sum_{i=1}^{n} i
\]
```

**Integration:**

```latex
\[
\int_0^1 x^2\,dx
\]
```

**Matrices:**

```latex
\[
A =
\begin{bmatrix}
1 & 2 \\
3 & 4
\end{bmatrix}
\]
```

**Aligned equations:**

```latex
\begin{align}
x+y &= 10 \\
x-y &= 2
\end{align}
```

## 09. TABLES

```latex
\begin{tabular}{|c|c|c|}
\hline
Name & Subject & Marks \\
\hline
Aman & Maths & 90 \\
Riya & Science & 85 \\
\hline
\end{tabular}
```

Column alignment:
- `l` = Left
- `c` = Centre
- `r` = Right
- `|` = Vertical line

## 10. INSERTING IMAGES

First import:

```latex
\usepackage{graphicx}
```

Then insert:

```latex
\begin{figure}[htbp]
\centering
\includegraphics[width=0.6\textwidth]{image.png}
\caption{Sample Image}
\label{fig:sample}
\end{figure}
```

Important commands:
- `\includegraphics` inserts an image.
- `\centering` centres it.
- `\caption` adds a caption.
- `\label` creates a reference point.

## 11. LABELS AND REFERENCES

```latex
\section{Introduction}
\label{sec:intro}

Refer to Section~\ref{sec:intro}.
```

Labels can be used for sections, figures, tables and equations.

## 12. BIBLIOGRAPHY AND CITATIONS

A basic manual bibliography:

```latex
\begin{thebibliography}{9}

\bibitem{book}
Author Name,
Title of the Book,
Publisher, Year.

\end{thebibliography}
```

Cite the source:

```latex
\cite{book}
```

**BibTeX:** A tool for managing references using a separate `.bib` file.

Example:

```bibtex
@book{example,
  author = {Author Name},
  title = {Example Book},
  year = {2024},
  publisher = {Example Publisher}
}
```

## 13. PAGE LAYOUT

```latex
\usepackage[a4paper,margin=1in]{geometry}
```

Useful page commands:

```latex
\newpage
\clearpage
\tableofcontents
\listoffigures
\listoftables
```

Headers and footers can be customised using `fancyhdr`.

## 14. COMPILATION

Compilation converts LaTeX source code into a formatted document, commonly PDF.

Common engines:

- pdfLaTeX
- XeLaTeX
- LuaLaTeX

Typical Overleaf workflow:

1. Create a project.
2. Write LaTeX code.
3. Click Recompile.
4. Check the PDF preview.
5. Correct errors.
6. Download the PDF.

## 15. SPECIAL CHARACTERS

Some characters have special meanings in LaTeX.

| Character | Command |
|---|---|
| % | `\%` |
| $ | `\$` |
| & | `\&` |
| # | `\#` |
| _ | `\_` |
| { | `\{` |
| } | `\}` |
| \ | `\textbackslash` |

## 16. ADVANTAGES OF LATEX

- Professional document formatting.
- Excellent mathematical typesetting.
- Automatic numbering.
- Easy cross-referencing.
- Structured document creation.
- Suitable for academic publications.

## 🎯 LEARNING OUTCOME

Through LaTeX, I learned how to create structured documents, format text, insert mathematical equations, prepare tables, add images and references, and generate professional PDF documents.

---

**END OF MODULE 01 | LATEX**
