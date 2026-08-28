# StructWeaver — CHI 2027 Papers

Fresh project aligned with the official **ACM Conference Proceedings Primary Article Template** (`acmart` **v2.20**, 2026/08/16) and [CHI 2027 Publication Formats](https://chi2027.acm.org/chi-publication-formats/).

## Main file

`sigconf-authordraft.tex` (CHI Overleaf naming)

```latex
% Review / PCS (current)
\documentclass[manuscript,review,anonymous]{acmart}

% After acceptance / TAPS
% \documentclass[sigconf]{acmart}
```

## Template files (from ACM / borisveytsman/acmart)

| File | Role |
|------|------|
| `acmart.cls` | ACM class v2.20 |
| `ACM-Reference-Format.bst` | Numbered ACM references |
| `acm-jdslogo.png` | Class asset |

## Content

| File | Role |
|------|------|
| `sigconf-authordraft.tex` | Paper body |
| `sample-base.bib`, `related_work.bib`, `software.bib` | Bibliography |
| `fig/*.pdf`, `fig/*.png` | Figures used in the paper |

## CHI notes

- Submissions must be **single-column** for review (`manuscript`). Wrong format can be desk-rejected.
- Abstract ≤ **150** words; body typically **5k–8k** words; above **12k** needs strong justification.
- Deadline (AoE): **10 September 2026**.
- Overleaf setup: open ACM template → keep `sigconf-authordraft.tex` → delete unused sample `.tex` files.

## Build

```bash
pdflatex sigconf-authordraft.tex
bibtex sigconf-authordraft
pdflatex sigconf-authordraft.tex
pdflatex sigconf-authordraft.tex
```

Or set Overleaf main document to `sigconf-authordraft.tex`.
