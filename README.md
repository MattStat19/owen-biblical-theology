# Theologoumena Pantodapa — English Translation

A complete English translation of John Owen's *Theologoumena Pantodapa, sive De Natura, Ortu, Progressu, et Studio Verae Theologiae, Libri Sex* (Biblical Theology), translated from the Latin text of William H. Goold's edition (Edinburgh: T. & T. Clark, 1862).

## Contents

- `Owen_Biblical_Theology_COMPLETE.docx` — the full translation in one Word document (~275,000 words): the Epistle to the Reader and all six books, with chapter arguments, Owen's section numerals, and the 1862 printed page numbers retained in brackets, e.g. `[ p. 156 ]`.
- `Owen_Biblical_Theology_COMPLETE.json` — the same translation as structured JSON: metadata, front matter, and six books, each with chapters (digressions as their own entries) and typed blocks (`page`, `argument`, `paragraph` with `section` numerals), addressable as book/chapter/section.
- `translation/` — **the source of truth**: the complete translation as numbered markdown files (`01`–`48`), Epistle through Book VI, plus the style guide. All edits and reviews happen here; the Word document and JSON are generated from these files.
- `scripts/compile.py` — rebuilds `Owen_Biblical_Theology_COMPLETE.docx` and `.json` from `translation/`. Run `python3 scripts/compile.py` from the repo root after any edit (requires `python-docx`).
- `chapters/` — archival: the original 35 chapter-part Word files for the Epistle and Books I–II, as first produced. Superseded by `translation/`; kept for provenance.
- `source/` — the Latin source: Goold's 1862 text as plain text and as the original Word document.

## Workflow

All changes are made on feature branches and merged to `main` by pull request. The review loop: edit the relevant file in `translation/`, run `scripts/compile.py`, commit both the markdown and the regenerated deliverables, open a PR, and review the markdown diff.

## The work

Owen's six books treat: (I) theology in general and natural theology, its corruption and loss, with the digression on universal grace and the refutation of Bellarmine's notes of the church; (II) the restoration of theology after the fall: the protevangelium, the first church, Cain, the Enoshian reformation, and the flood; (III) the Noachic theology and the origin and progress of idolatry, including British idolatry and the Druids; (IV) the Abrahamic and Mosaic theology, with digressions on the origin of letters and the ancient Hebrew script; (V) the corruption and restoration of the Mosaic theology, the Ezraitic reformation, and digressions on the Hebrew vowel points, the Septuagint, the Targums, and Jewish rites; (VI) evangelical theology properly so called, the gospel church and its apostasy, and the study of theology.

## Translation notes

- Greek and Hebrew are translated, with transliterations in brackets where the argument turns on the original wording.
- Verse quotations are rendered as quoted prose with citations.
- Fidelity was verified against the Latin source at the section level: every Roman-numeral section in the Latin is present in the translation, and the two tables of the printed edition (the seven Noachic precepts, Book III ch. I; Seneca's *Apocolocyntosis* verse, Book III ch. XI) are included.
