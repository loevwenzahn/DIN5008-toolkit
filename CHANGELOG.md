# Changelog

## [1.0.0] - 2026-07-06

Initial public release of DIN5008 Toolkit, a LaTeX/XeLaTeX toolkit for DIN 5008 Form A and Form B oriented letters, including applications, business correspondence, authority-oriented correspondence, and formal correspondence.

### Added

- Five curated presets for application, business, authority-oriented, legal/formal, and minimal correspondence workflows:
  - `application-de` / `application-en`
  - `business-de` / `business-en`
  - `authority-de` / `authority-en`
  - `legal-de` / `legal-en`
  - `minimal-de` / `minimal-en`
- Public `\UsePreset{...}` workflow.
- Separate Form A and Form B layout selection with `\UseLetterForm{A}` and `\UseLetterForm{B}`.
- Validated six-digit HEX overrides for accents, color-block segments, text, lines, fold marks, notices, and links.
- `LetterBody` environment for editable letter content.
- One-line `\DefineRecipient{key}{...}` workflow for reusable address book recipients, with a visible notice for unknown keys.
- Log-only demo-data reminder when draft mode is off and `content.tex` is compiled; opt out with `\CheckDemoDatafalse`.
- Fictional sender, recipient, reference, and attachment demo data.
- English and German guide source files for all five modes.
- PDF and PNG preview material for the README gallery.
- Compact Overleaf quickstart.
- Overleaf-friendly project structure.
- Local `latexmk` / XeLaTeX build path.
- LPPL-1.3c and CC BY 4.0 license split with `NOTICE` file.

### Notes

- The toolkit is oriented toward DIN 5008 Form A and Form B letter geometry, but is not DIN-certified.
- The Legal / Formal preset is a formal correspondence layout and does not provide legal advice.
- All included example data is fictional and neutralized.