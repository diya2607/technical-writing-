
# 🎨 BEAMER — PRESENTATION DESIGN WITH LATEX

<p align="center">
  <b>TECHNICAL WRITING | MODULE 02</b>
</p>

> Beamer is a LaTeX document class used to create professional presentations and slides in PDF format.

---

## 📑 TABLE OF CONTENTS

1. Introduction to Beamer
2. Basic Structure
3. Title Slide
4. Frames and Slides
5. Themes
6. Colour Themes
7. Fonts
8. Text Formatting
9. Lists
10. Blocks
11. Columns
12. Images
13. Tables
14. Mathematical Equations
15. Overlays and Animations
16. Two-Column Layouts
17. Navigation Symbols
18. Compilation
19. Advantages

## 01. INTRODUCTION

Beamer allows users to prepare presentations using LaTeX commands.

**Features:**
- Professional slide layouts.
- Automatic numbering.
- Mathematical equations.
- Themes and colour schemes.
- Blocks and columns.
- Step-by-step content display.

## 02. BASIC STRUCTURE

```latex
\documentclass{beamer}

\usetheme{Madrid}

\title{My Presentation}
\author{Your Name}
\institute{My College}
\date{\today}

\begin{document}

\begin{frame}
\titlepage
\end{frame}

\begin{frame}{Introduction}
Welcome to my presentation!
\end{frame}

\end{document}
```

## 03. TITLE SLIDE

Important commands:

```latex
\title{Presentation Title}
\subtitle{Presentation Subtitle}
\author{Your Name}
\institute{College Name}
\date{\today}
```

Display the title slide:

```latex
\begin{frame}
\titlepage
\end{frame}
```

## 04. FRAMES AND SLIDES

A frame represents a presentation unit.

```latex
\begin{frame}{Introduction}

This is my first slide.

\end{frame}
```

Each frame generally creates a slide, although overlays can produce multiple PDF pages from one frame.

## 05. THEMES

Themes control the overall appearance of the presentation.

Common themes:

```latex
\usetheme{Madrid}
\usetheme{Berlin}
\usetheme{CambridgeUS}
\usetheme{Warsaw}
\usetheme{Boadilla}
\usetheme{Copenhagen}
\usetheme{Darmstadt}
\usetheme{Frankfurt}
```

The theme should be selected according to the presentation style.

## 06. COLOUR THEMES

```latex
\usecolortheme{default}
\usecolortheme{seahorse}
\usecolortheme{dolphin}
\usecolortheme{beaver}
\usecolortheme{orchid}
```

Custom colours:

```latex
\definecolor{myblue}{RGB}{20,80,150}

\setbeamercolor{frametitle}{
  bg=myblue,
  fg=white
}
```

## 07. FONT THEMES

```latex
\usefonttheme{professionalfonts}
\usefonttheme{serif}
\usefonttheme{structurebold}
```

These change the presentation's typography.

## 08. TEXT FORMATTING

```latex
\textbf{Bold Text}

\textit{Italic Text}

\underline{Underlined Text}

\alert{Important Text}
```

## 09. LISTS

Bulleted list:

```latex
\begin{itemize}
\item Introduction
\item Objectives
\item Conclusion
\end{itemize}
```

Numbered list:

```latex
\begin{enumerate}
\item First
\item Second
\item Third
\end{enumerate}
```

## 10. BLOCKS

Blocks highlight important information.

**Normal block:**

```latex
\begin{block}{Definition}
Beamer is used to create presentations.
\end{block}
```

**Alert block:**

```latex
\begin{alertblock}{Important}
Remember this concept!
\end{alertblock}
```

**Example block:**

```latex
\begin{exampleblock}{Example}
This is an example.
\end{exampleblock}
```

## 11. COLUMNS

Columns divide a slide into multiple sections.

```latex
\begin{columns}

\column{0.5\textwidth}
Left Column Content

\column{0.5\textwidth}
Right Column Content

\end{columns}
```

Useful for comparisons, images and explanations.

## 12. INSERTING IMAGES

```latex
\usepackage{graphicx}
```

Inside a frame:

```latex
\begin{frame}{My Image}

\centering

\includegraphics[width=0.6\textwidth]{image.png}

\end{frame}
```

## 13. TABLES

```latex
\begin{frame}{Student Results}

\begin{tabular}{|c|c|}
\hline
Name & Marks \\
\hline
Aman & 90 \\
Riya & 85 \\
\hline
\end{tabular}

\end{frame}
```

## 14. MATHEMATICAL EQUATIONS

Beamer supports mathematical notation from LaTeX.

```latex
\begin{frame}{Mathematics}

\[
E = mc^2
\]

\[
a^2+b^2=c^2
\]

\end{frame}
```

## 15. OVERLAYS AND ANIMATIONS

Overlays reveal content in stages.

**Using `\pause`:**

```latex
\begin{frame}{Learning Steps}

Step 1: Introduction

\pause

Step 2: Explanation

\pause

Step 3: Conclusion

\end{frame}
```

**Using overlay specifications:**

```latex
\begin{itemize}
\item<1-> Introduction
\item<2-> Concepts
\item<3-> Conclusion
\end{itemize}
```

Other useful overlay commands:

- `\only<2>{...}`
- `\uncover<2->{...}`
- `\visible<2->{...}`
- `\onslide<2->{...}`

These control when content appears on different overlay pages.

## 16. TWO-COLUMN LAYOUT

```latex
\begin{frame}{Comparison}

\begin{columns}

\column{0.48\textwidth}
\textbf{Advantages}
\begin{itemize}
\item Easy formatting
\item Professional slides
\end{itemize}

\column{0.48\textwidth}
\textbf{Features}
\begin{itemize}
\item Themes
\item Blocks
\end{itemize}

\end{columns}

\end{frame}
```

## 17. NAVIGATION SYMBOLS

Hide navigation symbols:

```latex
\setbeamertemplate{navigation symbols}{}
```

Display a frame counter:

```latex
\setbeamertemplate{footline}[frame number]
```

## 18. COMPILATION

1. Open Overleaf or another LaTeX editor.
2. Select the Beamer document class.
3. Write the presentation code.
4. Choose a theme.
5. Add frames and content.
6. Compile the document.
7. Preview and download the PDF.

## 19. ADVANTAGES OF BEAMER

- Professional academic presentations.
- Consistent slide design.
- Supports equations and tables.
- Customisable themes.
- Reusable presentation templates.
- Easy integration with LaTeX.

## 🎯 LEARNING OUTCOME

Through Beamer, I learned to design structured presentations, create title slides, organise frames, customise themes, use blocks and columns, insert images and display content step by step using overlays.

---

**END OF MODULE 02 | BEAMER**
