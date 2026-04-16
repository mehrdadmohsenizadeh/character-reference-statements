# CDSS Criminal Record Exemption — RCFE Application Document Package

## Applicant: Mehrdad Mohsenizadeh
## Facility Type: RCFE (Residential Care Facility for the Elderly)
## Deadline: April 21, 2026

---

## Overview

This repository contains all documents required for the CDSS Criminal Record Exemption application, including the written statement of rehabilitation, cover letter, three LIC 301E character reference templates, and a comprehensive submission checklist.

## Repository Structure

```
├── REFINED_PROMPT.md                          # Master prompt for generating/refining documents
│
├── documents/                                 # Markdown versions (reference/drafts)
│   ├── 01_COVER_LETTER.md
│   ├── 02_STATEMENT_PART1-4.md
│   ├── 03-05_LIC_301E_TEMPLATES.md
│   └── SUBMISSION_CHECKLIST.md
│
├── latex/                                     # LaTeX project (upload to Overleaf)
│   ├── main.tex                               # Master assembler — compiles all documents
│   ├── styles/
│   │   └── cdss-exemption.sty                 # All packages, colors, environments, commands
│   ├── config/
│   │   └── variables.tex                      # All editable variables (names, dates, etc.)
│   └── content/
│       ├── cover-letter.tex                   # Formal cover letter to CPMB
│       ├── statement-part1.tex                # Statement Sections I-II (Accountability, Incident 1)
│       ├── statement-part2.tex                # Statement Sections III-IV (Incident 2, Rehabilitation)
│       ├── statement-part3.tex                # Statement Sections V-VI (Professional, Career Pivot)
│       ├── statement-part4.tex                # Statement Sections VII-IX (Vision, Conclusion)
│       ├── reference-a.tex                    # LIC 301E — Supervisor/Owner
│       ├── reference-b.tex                    # LIC 301E — Professional Colleague
│       └── reference-c.tex                    # LIC 301E — Community Contact
```

## LaTeX Project — How to Use with Overleaf

1. **Upload** the entire `latex/` folder to a new Overleaf project
2. **Set compiler** to pdfLaTeX (Project Settings)
3. **Edit** `config/variables.tex` to fill in all `\placeholder{}` fields (shown in red in the PDF)
4. **Personalize** reference templates in `content/reference-*.tex` (choose appropriate relationship options in Reference C)
5. **Compile** `main.tex` to generate the complete PDF
6. **To compile individual documents:** comment out `\input{}` lines in `main.tex` for documents you don't need

### Architecture (like a website)

| Layer | File | Analogy |
|-------|------|---------|
| **CSS / Styles** | `styles/cdss-exemption.sty` | All formatting, colors, environments, commands |
| **Config / Env Vars** | `config/variables.tex` | All editable data (names, dates, addresses, etc.) |
| **Content / Templates** | `content/*.tex` | Pure text — references variables, uses style environments |
| **Router / Index** | `main.tex` | Assembles everything into one PDF |

## Markdown Versions

The `documents/` folder contains plain-text Markdown versions for quick reference and editing outside of LaTeX.

## How to Submit

1. **Fill in** all placeholder fields in `config/variables.tex`
2. **Send** reference templates to your three references along with blank LIC 301E forms
3. **Gather** all proof-of-completion certificates and court compliance documentation
4. **Compile** the LaTeX project to PDF
5. **Upload** the complete packet through the Guardian portal by April 21, 2026
6. **Retain** copies of everything for CDPH CNA background check (expected later)

## Submission Methods

- **Primary (Recommended):** Upload via https://guardian.dss.ca.gov/Applicant
- **Secondary (Backup):** Mail to 744 P Street, M.S. T9-15-62, Sacramento, CA 95814, ATTN: CPU 5 / KG

## Key Contacts

- CPMB Phone: 888-422-5669
- CPMB Email: CPMB_CP5@dss.ca.gov
