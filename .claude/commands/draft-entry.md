---
description: Draft an entry from a candidate
argument-hint: <reference, e.g. John 1:1>
---

Draft an entry for $ARGUMENTS following METHODS §9.2 and the rules in CLAUDE.md.

1. Read the candidate notes for this verse in `work/candidates/` and any related generated tables.
2. Layer 1:
   - Source text with its edition, the NWT's stated base text, and any variants across editions. Set `difference_type`.
   - Morphological gloss and contextual semantic range.
   - NWT renderings: `TODO-NWT` for each edition in METHODS §5.1 relevant to the verse.
   - Comparison renderings: fill open-licensed texts from `data/source/`; mark others `TODO-lookup`.
   - Watch Tower publications about the verse: only ones you can retrieve and confirm; otherwise list as `unverified`.
3. Assessment: propose triggers and L, T, R, confidence with a one-line justification each in a comment. C comes from generated data only.
4. Layer 2: leave the strongest-case fields for `/steelman`. List positions with named holders and sources.
5. Leave Layer 3 empty.
6. Set `status: draft` and fill provenance.

Write to `content/entries/<book>/<chapter>-<verse>.md`, then run validation and fix errors. Summarize what still needs human input.
