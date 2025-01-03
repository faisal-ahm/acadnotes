# acadnotes.sty

`acadnotes.sty` is a versatile LaTeX package designed for academic and technical notes. It provides features like supersections, custom headers and footers, improved table of contents management, and appendix formatting. Perfect for reports, course notes, and other structured documents.

---

## Features

- **Supersections**: Organize your document with Roman-numbered "Part" divisions.
- **Custom Footers**: Define custom titles and authors for left and right footer sections.
- **Enhanced Appendix**: Distinct formatting and page numbering for appendices.
- **Table of Contents Control**: Limit the depth of TOC entries.
- **Customizable Chapter Titles**: Horizontal rules and spacing options.
- **Compact Lists**: Tighter spacing for bullet points and numbered lists.

---

## Installation

1. Download the `acadnotes.sty` file.
2. Place it in the same directory as your `.tex` file or in a directory recognized by your TeX distribution (e.g., `~/texmf/tex/latex/` for local installations).

---

## Usage

Include the package in your LaTeX document preamble:
```latex
\usepackage{acadnotes}
```

---

### Example

Below is an example LaTeX document using `acadnotes.sty`:

```latex
\documentclass{report}
\usepackage{acadnotes}

% Set custom footer content
\setfootertitle{Course Notes}
\setfooterauthor{John Doe}

\begin{document}

% Front Matter Setup
\title{Advanced Mathematics Notes}
\author{John Doe}
\date{\today}
\setupfrontmatter

% Supersections and Chapters
\supersection{Foundations}
\chapter{Introduction}
\section{Overview}

\supersection{Applications}
\chapter{Linear Algebra}
\section{Matrix Operations}

% Appendix
\appendix
\chapter{Supplementary Material}

\end{document}
```

---

## Features Breakdown

### Supersections
Supersections provide high-level divisions for your document, labeled as "Part I," "Part II," etc., and are automatically added to the Table of Contents (TOC).

Usage:
```latex
\supersection{Title of Part}
```

### Custom Footers
Define a title and author for the footer sections:
```latex
\setfootertitle{Footer Title}
\setfooterauthor{Author Name}
```

### Appendix Setup
The appendix starts on a new page with distinct formatting:
```latex
\appendix
\chapter{Appendix Title}
```

### Table of Contents Depth
By default, the TOC includes only chapters and sections. Adjust with:
```latex
\setcounter{tocdepth}{desired-depth}
```

---

## Documentation

For a detailed explanation of features and more examples, refer to the [compiled documentation](acadnotes-doc.pdf).

---

## Contributing

Contributions are welcome! Feel free to:
- Submit pull requests for new features or bug fixes.
- Report issues via the [GitHub Issues](https://github.com/your-username/acadnotes/issues) page.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Acknowledgments

- Inspired by academic and technical note-taking needs.
- Uses foundational LaTeX packages like `fancyhdr`, `titlesec`, and `hyperref`.

---

Happy TeXing! 🎉
