# Project rules for Claude Code

This repository is an evidence catalog of interpretive choices in the New World Translation (NWT). `METHODS.md` is the authority. If anything here conflicts with it, `METHODS.md` wins. Read the relevant sections of `METHODS.md` before any content task.

## Hard rules

1. **Never write NWT text from memory.** Leave NWT renderings as `TODO-NWT` with the edition needed. A person fills them in with evidence.
2. **Never publish a citation you have not retrieved.** If you cannot open and confirm a source, mark it `unverified: true` and say what you could not confirm. Never invent authors, titles, pages or quotations.
3. **Never write counts, ratios or occurrence lists by hand.** Run or extend a script in `scripts/`. Generated files in `data/generated/` are never hand-edited.
4. **No motive language.** Do not write that a rendering was chosen to support a doctrine, or use "biased," "dishonest," "deceptive," "agenda" or similar. Record the rendering, its support, its consistency, and what Watch Tower published (R-scale, METHODS §7.4).
5. **Keep the layers separate.** Layer 1 is checkable fact only. Layer 2 attributes every argument to a named holder with a source. Layer 3 commentary is the author's; do not draft it unless asked, and mark any draft as a draft.
6. **Strongest case for the NWT first.** Write it as a knowledgeable defender would, never as a strawman.
7. **Don't write "scholars agree"** unless a consensus is documented with sources. Otherwise name the positions.
8. **Separate textual from translational differences.** Check the NWT's stated base text (METHODS §5.2) before calling anything a translation choice.
9. **Your output is a draft.** Set `status: draft` at most. Never set `reviewed` or `verified`.
10. **Record provenance** on every entry you touch: model, command, prompt version, discovery stream.
11. **Don't bulk-copy copyrighted translations.** Quote per verse only. Instance tables store only the rendered word or phrase.
12. **Paraphrase sources** rather than quoting; keep any quotation short and cited.

## Source hierarchy (METHODS §8.1)

Primary texts → standard lexicons and grammars → peer-reviewed scholarship → other scholarship → positions (apologetics on any side, reported in Layer 2 only) → leads (websites, forums; never cited as evidence).

## Layout

- `content/entries/<book>/<chapter>-<verse>.md` — entries
- `content/phenomena/<slug>.md` — pattern analyses
- `content/controls/<slug>.md` — control entries
- `content/peculiarities/<book>.yaml` — triggers without a doctrinal link
- `work/candidates/<book>-<chapter>.md` — sweep output
- `data/bibliography.json` — CSL-JSON; cite by key
- `data/generated/` — script output only
- `schemas/` — validate every content file against these
- `scripts/` — Python generators and validators

## Commands

- `/sweep-chapter <Book> <chapter>` — discovery stream B
- `/draft-entry <reference>` — draft an entry from a candidate
- `/steelman <reference>` — strongest case for and against
- `/check-citations <path>` — verify citations in a file

## After editing content

Run schema validation (`python scripts/validate.py <path>`) and fix every error before finishing.
