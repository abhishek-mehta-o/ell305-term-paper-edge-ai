# ELL305 Term Paper — Architectural Trade-offs in Edge AI Inference

## Structure
- `main.tex` — top-level document, includes all chapters in order
- `chapters/` — one `.tex` file per chapter (edit these, not `main.tex`, day to day)
- `bib/references.bib` — BibTeX file, re-exported from Zotero as sources are added
- `figures/` — TikZ/CircuiTikZ diagrams and any exported images

## Submission plan (checkpoints)
| Version | Chapters | Target date |
|---|---|---|
| v0.1 | 00 Abstract (skeleton only) + 01 Introduction + 02 ISA Foundations + 03 Processor Design | — |
| v0.2 | + 04 Power & Thermal + 05 Memory Hierarchy | — |
| v0.3 | + 06 SIMD Acceleration + 07 Case Studies | — |
| v1.0 | + 08 Synthesis, full Abstract, final polish | Nov 11, 2026 |

## Workflow
1. Write/edit inside `chapters/`.
2. Compile locally or on Overleaf to check output.
3. Commit and push to GitHub after each work session (small, frequent commits).
4. Tag each submitted version in git (`git tag v0.1`) before submitting the PDF to Gradescope.
5. Add new sources to Zotero as you find them; re-export `bib/references.bib` before each submission.

## Compilation
Requires a LaTeX distribution with pdflatex + bibtex (or Overleaf, which handles this automatically):
```
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```
