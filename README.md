# MUST Final Year Project Proposal LaTeX Template

**[Chinese version / 中文版本](./README_CN.md)**

This repository provides a LaTeX version of the **Final Year Project Proposal** template for the School of Computer Science and Engineering, Faculty of Innovation Engineering, Macau University of Science and Technology (MUST).

The template was reconstructed from the official Microsoft Word template with the goal of reproducing its layout and formatting as faithfully as possible.

## Usage

The template is designed to be compiled with **XeLaTeX**.

### Overleaf

1. Upload the project files to Overleaf.
2. Open **Menu → Settings**.
3. Set the compiler to:

   ```text
   XeLaTeX
   ```

4. Use `main.tex` as the main document.
5. Recompile the project.

## Project Structure

```text
.
├── main.tex
├── must_proposal.sty
├── reference.bib
├── mustplain.bst
├── assets/
│   ├── image1.jpeg
│   └── water-fall.jpg
└── fonts/
```

- `main.tex`  
  Main document. Edit the project information and proposal content here.
- `must_proposal.sty`  
  Defines the page layout, typography, cover page, table of contents, headings, and other formatting.
- `mustplain.bst`
  Defines the citation format.
- `reference.bib`  
  Stores the bibliography entries used by the proposal. References can be cited in `main.tex` using `\cite{...}`. The reference list is automatically sorted alphabetically by the surname of the first author.
- `assets/`  
  Contains image assets required by the template.
- `fonts/`  
  Used for locally supplied fonts when the required fonts are not available in the compilation environment.

## Fonts

This template uses the original fonts of the Word template in order to preserve the formatting as closely as possible.

In particular, **Calibri is not available by default on Overleaf**.

If compilation fails because Calibri cannot be found, please obtain the Calibri font files yourself from a legitimate source and place them in the `fonts/` directory.

The expected filenames are:

```text
fonts/calibri.ttf
fonts/calibrib.ttf
fonts/calibrii.ttf
fonts/calibriz.ttf
```

corresponding to:

- Calibri Regular
- Calibri Bold
- Calibri Italic
- Calibri Bold Italic

Due to copyright restrictions, the font files themselves are **not distributed with this repository**. Please obtain the required fonts through appropriate and legitimate sources by yourselves.

The template does not silently substitute Calibri with another font, since doing so may change line wrapping, spacing, and the overall layout.

## Editing the Proposal

Basic project information can be edited in `main.tex`, including:

```latex
\projecttitle{...}
\studentname{...}
\studentno{...}
\supervisor{...}
\proposaldate{...}
```

The proposal content can then be written in the corresponding sections:

- Abstract
- Contributions
- Introduction
- Objectives
- Related Work
- Methodology
- Required Hardware and Software
- Project Planning
- References

## Notes

This template aims to reproduce the official Word template as closely as possible. Minor rendering differences may still exist because Microsoft Word and XeLaTeX use different typesetting and PDF rendering engines.

Please avoid modifying `must_proposal.sty` unless you need to intentionally change the template formatting.

## Contact

If you encounter any issues when using this template, please contact:

**Aaron**: zechengq@student.must.edu.mo

## Disclaimer

This repository provides an unofficial LaTeX reconstruction of the corresponding MUST Final Year Project Proposal template and is not officially released, endorsed, or maintained by Macau University of Science and Technology.

Although this template has been carefully designed to reproduce the official Microsoft Word template as closely as possible, Microsoft Word and XeLaTeX use different typesetting and rendering mechanisms. Therefore, the output cannot be guaranteed to be 100% identical to the official Word document in all circumstances.

Users are responsible for checking the latest formatting requirements and submission guidelines issued by the University before formal submission. The authors of this repository are not responsible for any formatting discrepancies, non-compliance with submission requirements, submission-related issues, or other consequences arising from the use of this template.

The name and logo of Macau University of Science and Technology remain the property of their respective rights holders and are included solely for the purpose of reproducing the academic template.

Microsoft fonts, including Calibri, are not distributed with this repository. Users should obtain any required fonts from appropriate and legitimate sources.
