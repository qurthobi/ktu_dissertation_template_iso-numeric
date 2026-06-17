# KTU Dissertation LaTeX Template

This is a comprehensive LaTeX dissertation template designed for PhD students at the Kaunas University of Technology (KTU).

This repository provides a structured and customizable template for writing PhD dissertations

The template is designed to simplify academic writing while maintaining a professional dissertation layout compatible with KTU formatting practices.

---

# Features

## Academic Formatting

- Professional dissertation layout
- B5-like page geometry
- Customized headers and footers
- Structured chapter formatting
- Figure and table styling
- Automatic table of contents generation

## Bibliography Support

- `biblatex` integration
- ISO 690:2021-style numeric citations
- Biber backend support
- Easy reference management

## Glossaries and Acronyms

- Acronym support using `glossaries`
- Symbols and terminology lists
- Automatic glossary generation

## Writing Convenience

- Modular chapter structure
- Separate folders for figures, tables, and appendices
- UTF-8 compatible
- Overleaf compatible
- Works with TeX Live and MiKTeX

---

# Repository Structure

```text
.
├── main.tex                    # Main dissertation file
├── bibliography.bib            # Bibliography database
├── ktu_thesis_style.sty        # Main KTU style package
├── summaryLT/                  # Lithuanian summary section
├── chapters/                   # Dissertation chapters
└── README.md
```

---

# Getting Started

## 1. Clone the Repository

```bash
git clone https://github.com/qurthobi/ktu_dissertation_template.git
cd ktu_dissertation_template
```

Or download the repository ZIP directly from GitHub.

---

# Requirements

Recommended LaTeX distributions:

- TeX Live 2024+
- MiKTeX
- MacTeX
- Overleaf

Main packages used:

- `biblatex`
- `glossaries`
- `fancyhdr`
- `titlesec`
- `tocloft`
- `graphicx`
- `amsmath`

---

# Compilation

## Recommended Method — latexmk

```bash
latexmk -pdf main.tex
```

## Manual Compilation

```bash
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
```

---

# Using Overleaf

1. Download the repository ZIP
2. Upload it to Overleaf
3. Set `main.tex` as the main document
4. Compile using `pdfLaTeX`
5. Enable Biber if needed

---

# Bibliography

References are stored in:

```text
bibliography.bib
```

Example citation:

```latex
\cite{example2025}
```

The template uses:

- `biblatex`
- numeric citation style
- Biber backend

---

# Glossaries and Acronyms

Example acronym definition:

```latex
\newacronym{ai}{AI}{Artificial Intelligence}
```

Usage in text:

```latex
\gls{ai}
```

---

# Figures and Tables

Example figure insertion:

```latex
\begin{figure}[ht]
    \centering
    \includegraphics[width=0.8\textwidth]{figures/example.png}
    \caption{Example figure}
\end{figure}
```

Example table:

```latex
\begin{table}[ht]
\centering
\caption{Example table}
\begin{tabular}{cc}
A & B \\
\end{tabular}
\end{table}
```

---

# Lithuanian Summary Section

The repository includes a Lithuanian dissertation summary section located in:

```text
summaryLT/
```

Example file:

```text
summaryLT/2_skyrius.tex
```

This section can be customized according to KTU dissertation submission requirements.

---

# Customization

You can modify:

- Fonts
- Margins
- Chapter formatting
- Header/footer styles
- Caption formatting
- Table of contents layout
- Glossary appearance

Main customization file:

```text
ktu_thesis_style.sty
```

---

# Recommended Workflow

1. Write each chapter separately inside `chapters/` (for ENGLISH parts) and `summaryLT` (for LITHUANIAN parts)
2. Store figures in `images/`
3. Maintain references in `bibliography.bib`
4. Compile regularly using any LaTeX compiler (Preferably Overleaf.com)
5. Use Git for version control

---

# Example Output

You may include:

- Sample dissertation PDF
- Cover page screenshots
- Example table of contents
- Example glossary page

Example output location:

```text
output/dissertation.pdf
```

---

# Troubleshooting

## Bibliography not appearing

Run:

```bash
biber main
```

Then recompile the document twice.

## Glossary not showing

Compile glossary files or use:

```bash
makeglossaries main
```

---

# Contributing

Contributions are welcome.

You can contribute by:

- reporting issues,
- improving formatting,
- fixing compilation problems,
- enhancing KTU compliance,
- or improving documentation.

Please open an issue or submit a pull request.

---

# License

This project is distributed under the MIT License unless stated otherwise.

---

# Author

Ahmad Qurthobi

GitHub: https://github.com/qurthobi

---

# Acknowledgements

This was inspired by several open-source LaTeX templates and dissertation projects. Special thanks go to https://dominyk4s.github.io/KTU-LaTeX/ for providing the main inspiration.
