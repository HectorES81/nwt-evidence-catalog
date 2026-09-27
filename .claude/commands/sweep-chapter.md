---
description: Discovery stream B — sweep one chapter for candidates
argument-hint: <Book> <chapter>
---

Sweep $ARGUMENTS for candidates (METHODS §6.1, stream B).

1. Load the source text for the chapter from `data/source/` (tagged Greek or Hebrew with lemmas and morphology) and the open comparison texts.
2. Do not read other streams' results for this chapter (`work/candidates/`, generated tables, edition diffs) before finishing. This sweep is meant to be independent.
3. For each verse, consider: lexical choices (METHODS §7.1 T1), constructions (T2), supplied words (T3), punctuation and segmentation (T5), and any item on the lemma and construction list (§6.2).
4. Classify each verse as `notable`, `not-notable` or `uncertain`. For `notable` and `uncertain`, give one or two sentences on what and why, naming the trigger code.
5. You do not have NWT text. Where the question depends on the NWT rendering, write `TODO-NWT` and what needs checking.
6. Note any lemma or construction that seems worth adding to §6.2.

Write the result to `work/candidates/<book>-<chapter>.md` with a header recording the model, date and command. Update the coverage record for the chapter. Do not create entries.
