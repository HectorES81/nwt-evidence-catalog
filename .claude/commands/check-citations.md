---
description: Verify every citation in a file
argument-hint: <path>
---

Check every citation in $ARGUMENTS.

For each bibliography key and source reference:
1. Confirm the work exists (author, title, year, publisher or journal) by retrieving it or a reliable catalog record.
2. Where the entry attributes a claim to it, confirm the source says that, if the text is accessible. Note the page or section.
3. Classify: `confirmed`, `exists-claim-unchecked` (work is real but the claim couldn't be checked), or `not-found`.

Set `unverified: true` on anything not `confirmed`. Never correct a citation by guessing. Report a table of results, and list what a person needs to check by hand (for example, print-only sources).
