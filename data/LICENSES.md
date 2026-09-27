# Data licenses

**Status:** draft — license terms retrieved by an AI agent on 2026-09-26 and not yet confirmed by a person (METHODS §8.2, §17). Nothing here is legal advice.

**Provenance:** model `claude-opus-5-5`, Claude Code session (no slash command), task "METHODS §17 license check", prompt version: none (ad hoc).

Each row records where the terms were read, what they say (paraphrased), and what that means for this project. "Bulk use" means scripts may download, store and process the whole dataset (METHODS §5.3–5.4, §13).

## Source-language data

| Dataset | Where the terms were read | License (as stated) | Bulk use | Conditions and notes |
|---|---|---|---|---|
| STEPBible-Data: TAGNT, TAHOT, TBESG, TBESH, TFLSJ | Repo README and the header of the TAGNT Mat–Jhn file, github.com/STEPBible/STEPBible-Data | CC BY 4.0 | Yes | Credit "STEP Bible" with a link to www.STEPBible.org. Changes to the data should be recorded and made visible to later users. **Don't use** the `TTESV` file in `Tagged-Bibles/`: its filename marks it CC BY-NC, and it tags the ESV, which is copyrighted. The TAGNT header says it covers words from NA27/28, TR, SBL, Tyndale House, Byzantine, WH and Tregelles, which is relevant to §5.2 but not checked verse by verse. |
| Macula Greek | `LICENSE.md`, github.com/Clear-Bible/macula-greek | CC BY 4.0 (© Biblica, Inc.) | Yes, with an exception | Required attribution: "MACULA Greek Linguistic Datasets, available at https://github.com/Clear-Bible/macula-greek/". The bundled parts have their own terms: Nestle1904 (see its repo), SBLGNT (CC BY 4.0), and Berean glosses (public domain). **Open question:** the UBS MARBLE word-sense attributes (`@ln`, `@domain`) are marked "used with permission", not CC BY. Don't redistribute those attributes until a person confirms we may. |
| Macula Hebrew | `LICENSE.md`, github.com/Clear-Bible/macula-hebrew | CC BY 4.0 (© Biblica, Inc.) | Yes, with an exception | Required attribution: "MACULA Hebrew Linguistic Datasets, available at https://github.com/Clear-Bible/macula-hebrew/". The WLC text is copyable without restriction per tanach.us; the Groves Center syntax and OpenScriptures morphology are CC BY 4.0. **Open question:** the Semantic Dictionary of Biblical Hebrew attributes (`@sdbh`, `@lexdomain`, `@coredomain`, `@contextualdomain`) are marked "used with permission" (UBS). Same caution as for Macula Greek. |
| ETCBC BHSA | `README.md` (License section) and `LICENSE`, github.com/ETCBC/bhsa | **Data: CC BY-NC 4.0.** Code: MIT | Yes, non-commercial only | Cite the persistent identifier 10.17026/dans-z6y-skyh. Commercial use needs consent from the German Bible Society. **Decided 2026-09-26:** the project is non-commercial (author's decision), so BHSA use is within the license. |
| Text-Fabric (software) | GitHub license metadata, github.com/annotation/text-fabric | MIT | n/a (software) | Only the metadata was checked; the license file itself wasn't read. |
| SBLGNT | `README.md` and `LICENSE`, github.com/Faithlife/SBLGNT (formerly LogosBible/SBLGNT) | CC BY 4.0 (© 2010 SBL and Logos Bible Software) | Yes | The README's version history dates the move to CC BY 4.0 to v1.1 (2022-12-19); older copies were under the SBLGNT EULA, so use v1.1 or later. v1.2 (2023-07-10) added John 7:53–8:11. |
| MorphGNT (SBLGNT parsing) | `README.md`, github.com/morphgnt/sblgnt | Parsing and lemmas: **CC BY-SA 3.0**. Text: the README still cites the old SBLGNT EULA. | Avoid unless needed | The share-alike clause could extend to derived instance tables. It isn't in the METHODS §5.4 list, and STEPBible and Macula cover the same ground. |
| Westcott–Hort 1881 (Robinson digital text) | `README.md`, github.com/byztxt/greektext-westcott-hort | Public domain ("Copy freely") | Yes | Primary author Maurice A. Robinson; maintainer Ulrik Sandborg-Petersen. The repo was last updated 2017-05-23. **Not yet confirmed:** that this text matches the printed 1881 edition, including how it handles WH's brackets and marginal readings. Check this against a scan of the 1881 printing before relying on it for §5.2 base-text comparisons. |

## Open-licensed translations (bulk use allowed, METHODS §5.3)

| Translation | Where the terms were read | License (as stated) | Conditions and notes |
|---|---|---|---|
| ASV | ebible.org/find/details.php?id=eng-asv | Public domain | None |
| YLT | ebible.org/find/details.php?id=engylt | Public domain | None |
| WEB | ebible.org/find/details.php?id=engwebp | Public domain | "World English Bible" is an eBible.org trademark. A changed text may not be called the WEB. |
| KJV | ebible.org/find/details.php?id=eng-kjv2006 | Public domain (outside the UK) | Under Crown letters patent, printing it in the UK or importing printed copies needs permission. This doesn't affect online use. |
| BSB | berean.bible/terms.htm, berean.bible/licensing.htm | Dedicated to the public domain on 2023-04-30 | Attribution is appreciated but not required. |
| JPS 1917 | ebible.org/find/details.php?id=engjps | Public domain | None |

## Not yet checked

- Nestle1904 (github.com/biblicalhumanities/Nestle1904): its README says each subfolder has its own terms. Check this only if we use Macula's Nestle1904 trees.
- Macula's MARBLE and SDBH "used with permission" data (see above).
- tanach.us WLC license page: only Macula's summary of it was read, not the page itself.
- jw.org terms of use: a separate §17 item.
