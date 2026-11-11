
# LaTeX Documentation

## 1. Introduction to LaTeX

### What is LaTeX?

LaTeX is a document preparation system built upon the TeX typesetting system. It is commonly used for preparing high-quality documents, academic research papers, technical reports, and books.

### Why Use LaTeX?

- It is free to use and easily portable.
- Offers professionally formatted document layouts.
- Simplifies the process of writing mathematical expressions.
- Supports different output formats.
- Automatically manages references, footnotes, tables of contents, and bibliographies.

### LaTeX Tools

LaTeX can be accessed using both offline software and online platforms.

| Offline Tools | Online Tools |
|---|---|
| MiKTeX | Overleaf |
| TeX Live | Papeeria |
| TeXstudio | CoCalc |

### Input and Output

LaTeX source code is written in a plain text file having the `.tex` extension. It contains the actual document content along with various LaTeX commands.

Some commonly used output formats are:

- PDF (`.pdf`)
- DVI (`.dvi`)
- PostScript (`.ps`)
- Rich Text Format (`.rtf`)

## 2. Basic Document Structure

A standard LaTeX document consists of three essential components:

```latex
\documentclass{article}

\begin{document}

This is my first LaTeX document.

\end{document}
```

### Explanation

- `\documentclass{article}` – Specifies the category or type of document.
- `\begin{document}` – Indicates where the actual document content begins.
- `\end{document}` – Marks the completion of the document content.

### Document Classes

The `\documentclass` command determines the basic format and structure of a document.

| Class | Purpose |
|---|---|
| `article` | Used for short documents and research papers |
| `report` | Suitable for detailed reports and longer documents |
| `letter` | Used for writing formal letters |

### Document Class Options

Additional options can be provided within square brackets to customize the document.

Example:

```latex
\documentclass[12pt,a4paper]{article}
```

- `12pt` sets the font size to 12 points.
- `a4paper` selects A4 as the page size.
- `article` defines the document type.

## 3. Adding Title, Author and Date

LaTeX includes specific commands for defining the title, author's name, and date of a document.

### Important Commands

- `\title{}` – Sets the title of the document.
- `\author{}` – Defines the name of the author.
- `\date{}` – Specifies the document date.
- `\maketitle` – Prints the title, author, and date in the document.

### Important Points

- The title, author, and date information should be declared before `\begin{document}`.
- The `\maketitle` command should be used after `\begin{document}`.
- The `\today` command automatically inserts the current date.

## 4. Comments and Page Styles

### Comments in LaTeX

Comments allow users to write additional notes or explanations in the source code. These comments are ignored during compilation and are not displayed in the final document.

LaTeX uses the `%` symbol to indicate a comment.

Example:

```latex
\documentclass{article}

\begin{document}

This text is processed.

% This is a comment.
This text is also processed.

\end{document}
```

Whenever LaTeX encounters `%`, it ignores the remaining portion of that particular line.

## 5. Hyphenation

LaTeX automatically divides words when required to maintain proper text alignment and formatting.

The `\-` command can be used to manually specify possible positions where a word can be split.

Example:

```latex
manu\-script
data\-base
micro\-processor
```

The word will only be divided at the specified position if a line break is required there.

## 6. Font Sizes

LaTeX offers several predefined commands that can be used to modify the size of text.

| Command | Font Size |
|---|---|
| `\tiny` | Tiny |
| `\small` | Small |
| `\normalsize` | Normal |
| `\large` | Large |
| `\Large` | Larger |
| `\LARGE` | Very large |
| `\huge` | Huge |
| `\Huge` | Largest |

These commands can be applied to change the font size of the text enclosed within their braces.

## 7. Text Alignment

LaTeX provides three commonly used environments to control the alignment of text:

- `flushleft` – Places text along the left margin.
- `center` – Positions text at the centre of the page.
- `flushright` – Aligns text with the right margin.

## 8. Lists in LaTeX

LaTeX supports three main types of lists for organizing information:

- `itemize` – Produces a list with bullet points.
- `enumerate` – Generates a list with numbered items.
- `description` – Creates a list containing labels followed by their descriptions.

## 9. Trivlist Environment

The `trivlist` environment is used to create a basic list without displaying bullets or numbering.

Example:

```latex
\begin{trivlist}
\item First item without label
\item Second item
\end{trivlist}
```

Every `\item` command represents a separate entry in the list.

## 10. Page Breaks

LaTeX provides commands that help control the placement of content across different pages.

- `\newpage` – Immediately begins a new page.
- `\clearpage` – Starts a new page after processing all pending figures and tables.

## 11. Section and Subsection

LaTeX offers commands to divide a document into different sections and subsections, making its structure more organized.

**Example:**

```latex
\section{Introduction}
\subsection{Background}
\section{Methods}
```

LaTeX automatically assigns numbers to sections and subsections.

## 12. Lengths and Spaces in LaTeX

LaTeX provides commands for inserting horizontal and vertical spaces within a document.

**Example:**

```latex
\hspace{1cm} % Adds horizontal space
\vspace{1cm} % Adds vertical space
```

- `\hspace` is used to insert horizontal spacing.
- `\vspace` is used to insert vertical spacing.

## 13. BibTeX in LaTeX

BibTeX is a reference management tool used to organize citations and generate bibliographies in LaTeX documents.

**Example:**

```latex
\bibliographystyle{plain}
\bibliography{references}
```

- The `bibliographystyle` command determines the formatting style of the bibliography.
- The `bibliography` command imports references from a `.bib` file.

## 14. Colours in LaTeX

The `xcolor` package allows users to apply different colours to text within a LaTeX document.

**Example:**

```latex
\usepackage{xcolor}

\textcolor{red}{Red Text}
\textcolor{blue}{Blue Text}
```

## 15. Backgrounds and Highlights

LaTeX provides the `\colorbox` and `\fcolorbox` commands to highlight specific text using background colours and borders.

**Example:**

```latex
\colorbox{yellow}{Important Text}
\fcolorbox{red}{white}{Highlighted Text}
```

- `\colorbox` adds a coloured background behind the given text.
- `\fcolorbox` creates a coloured border along with a background colour.

## 16. Important LaTeX Symbols

LaTeX includes predefined commands for inserting Greek alphabets and various mathematical symbols.

### Greek Letters

| Symbol | Command |
|---|---|
| α | `\alpha` |
| β | `\beta` |
| γ | `\gamma` |
| δ | `\delta` |
| θ | `\theta` |
| λ | `\lambda` |
| μ | `\mu` |
| ν | `\nu` |
| π | `\pi` |
| ρ | `\rho` |
| σ | `\sigma` |
| τ | `\tau` |
| φ | `\phi` |
| ψ | `\psi` |
| ω | `\omega` |
| η | `\eta` |
| Δ | `\Delta` |
| Ω | `\Omega` |
| Σ | `\Sigma` |
| Γ | `\Gamma` |

### Mathematical Symbols

| Symbol | Command |
|---|---|
| ∞ | `\infty` |
| ≤ | `\leq` |
| ≥ | `\geq` |
| ≠ | `\neq` |
| ≈ | `\approx` |
| × | `\times` |
| ÷ | `\div` |
| ± | `\pm` |
| √ | `\sqrt{}` |
| ∑ | `\sum` |
| ∫ | `\int` |
| ∂ | `\partial` |
| ∇ | `\nabla` |
| ∈ | `\in` |
| ∉ | `\notin` |
| ∩ | `\cap` |
| ∪ | `\cup` |
| → | `\rightarrow` |
| ⇒ | `\Rightarrow` |
| ≡ | `\equiv` |

## Conclusion

LaTeX is an effective document preparation system widely used for producing professional, technical, and scientific documents. It offers a wide range of features for formatting text, writing mathematical equations, designing tables, inserting figures, and managing references. Its structured approach makes it a useful tool for creating well-organized and high-quality documents.
