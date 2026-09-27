---
book: philemon
chapter: 1
stream: B
status: draft
purpose: pre-pilot time sample (METHODS §14); not counted toward coverage until redone under frozen methods
provenance:
  model: claude-opus-5-5
  command: /sweep-chapter Philemon 1
  prompt_version: .claude/commands/sweep-chapter.md @ c43a97d
  date: 2026-09-26
  discovery_stream: B
inputs:
  source: STEPBible TAGNT Act–Rev (CC BY 4.0), downloaded 2026-09-26 into data/source/ (not committed)
  comparisons: ASV, YLT, KJV (eng-kjv2006), BSB, WEB (engwebp), eBible.org VPL files, downloaded 2026-09-26
  not_consulted: NASB, ESV, NRSVue, NET, CSB, NIV, NLT, NABRE (copyrighted; per-verse lookup needed); any NWT edition
coverage:
  verses: 25
  # counted by regex over the classification table below, not by hand
  notable: 2
  uncertain: 7
  not_notable: 16
---

# Philemon 1: stream B sweep

Independent sweep: no other stream's results were read. NWT text was not consulted; every question that depends on it is marked `TODO-NWT`.

Textual notes below come from the edition columns in TAGNT (which marks readings in NA28, NA27, Tyndale House, SBL, WH, Tregelles, TR and Byzantine). The NWT's stated NT base is WH (METHODS §5.2, still to verify), so WH readings are called out.

## Verse classification

| Verse | Class | Trigger | Note |
|---|---|---|---|
| 1 | not-notable | | |
| 2 | **notable** | T4, §6.2 | κατ᾽ οἶκόν σου ἐκκλησίᾳ: *kata* + *oikos* in the singular, where the sense is "the church at your house" in all five comparison texts. This is a comparison point for the §6.2 item "from house to house" (the *kata* + *oikos* construction at e.g. Acts 5:42, 20:20). `TODO-NWT`: rendering of κατ᾽ οἶκον here and of ἐκκλησία ("church" in ASV, KJV, BSB; "assembly" in YLT, WEB), in 1984 and 2013. Textual: ἀδελφῇ (WH, NA28) vs ἀγαπητῇ (TR, Byz); comparison texts split along those lines. |
| 3 | uncertain | §6.2 (*kyrios*) | κυρίου Ἰησοῦ Χριστοῦ: *kyrios* with an explicit referent to Jesus. An instance for the *kyrios* table; not expected to be notable on its own. `TODO-NWT`: confirm the rendering. |
| 4 | not-notable | | |
| 5 | uncertain | T5, textual | Two points. (a) Textual: WH and Tregelles read εἰς τὸν κύριον; NA28, SBL, TR and Byz read πρός. Any NWT difference from translations following NA28 here would be textual, not translational. (b) Order: "your love and the faith which you have toward the Lord Jesus and toward all the saints." ASV, WEB, YLT, KJV keep the Greek order; BSB regroups it as faith in the Lord Jesus and love for all the saints. `TODO-NWT`: which structure the NWT follows. No doctrinal link seen. |
| 6 | uncertain | T2 | A verse that's hard to construe. Open points: the genitive in ἡ κοινωνία τῆς πίστεώς σου ("fellowship of your faith", ASV/WEB/YLT; "communication", KJV; "partnership in the faith", BSB); the sense of ἐπίγνωσις; and εἰς Χριστόν ("unto Christ", ASV; "toward Christ Jesus", YLT; "in Christ", BSB). Textual: WH reads ἡμῖν and omits Ἰησοῦν (TR has ὑμῖν ... Ἰησοῦν). The comparison texts already diverge widely, so an NWT rendering is unlikely to be a lone outlier. No doctrinal link seen; if notable, it belongs in the peculiarity log. `TODO-NWT`: rendering of κοινωνία here, which also feeds a proposed §6.2 addition. |
| 7 | not-notable | | σπλάγχνα (also v12, v20) is idiom ("bowels" in KJV/YLT, "hearts" elsewhere); stylistic. Textual: ἔσχον (WH) vs ἔχομεν (TR), which explains "I had" vs "we have". |
| 8 | not-notable | | |
| 9 | uncertain | T1 | πρεσβύτης "old man / aged" in all five comparison texts. **Lead, unverified:** a conjectural reading πρεσβευτής ("ambassador") is reported to have been adopted by some translations. I couldn't confirm which, so the panel should be checked. No doctrinal link seen; peculiarity-log material at most. `TODO-NWT`: rendering. |
| 10 | not-notable | | Textual: WH lacks μου after δεσμοῖς. |
| 11 | not-notable | | Wordplay on Onesimus's name (ἄχρηστον / εὔχρηστον). Textual: first καί is in NA28/NA27 only, not WH. |
| 12 | not-notable | | Textual: TR/Byz add σὺ ... δὲ ... προσλαβοῦ ("thou therefore receive him", KJV, WEB, YLT); WH lacks it (ASV, BSB). Textual difference, not translational. |
| 13 | not-notable | | |
| 14 | not-notable | | |
| 15 | uncertain | §6.2 (*aiōnios*), T4 | ἵνα αἰώνιον αὐτὸν ἀπέχῃς: *aiōnios* used adverbially of a person's return ("for ever", ASV/KJV/WEB; "age-duringly", YLT; "for good", BSB). An instance for the *aiōnios* consistency table, where the non-eschatological context matters. `TODO-NWT`: rendering. Also πρὸς ὥραν ("for a season / a while / an hour"). |
| 16 | uncertain | §6.2 (*kyrios*), T4 | Two points. (a) ἐν κυρίῳ: referent not stated in the phrase (God or Christ). An instance for the *kyrios* table; `TODO-NWT`: rendering, and whether any NWT edition renders κύριος here with the divine name. (b) δοῦλος: "servant" (ASV, KJV, YLT) vs "slave" (BSB, WEB); an instance for a proposed *doulos* table. |
| 17 | not-notable | | |
| 18 | not-notable | | |
| 19 | not-notable | | |
| 20 | **notable** | §6.2 (*kyrios*), T4, textual | ἐν κυρίῳ ... ἐν Χριστῷ in parallel clauses. The ambiguous κύριος sits next to an explicit Χριστός, so this is a useful test case for how the *kyrios* referent is decided. Textual: WH and NA28 end with Χριστῷ; TR and Byz end with κυρίῳ (KJV, WEB, YLT "in the Lord" twice; ASV, BSB "in Christ"). `TODO-NWT`: rendering of both phrases in 1984 and 2013, and whether the divine name appears. |
| 21 | not-notable | | |
| 22 | not-notable | | |
| 23 | not-notable | | Textual: singular ἀσπάζεταί (WH) vs plural (TR). |
| 24 | not-notable | | |
| 25 | uncertain | §6.2 (*pneuma*), T1 | μετὰ τοῦ πνεύματος ὑμῶν: *pneuma* of a human group. All five comparison texts render "with your spirit". An instance for the *pneuma* table; notable only if the NWT renders it interpretively. `TODO-NWT`: rendering. Textual: ἡμῶν and ἀμήν are absent in WH and NA28 (BSB omits "Amen"; the others include it). The TR subscription ("written from Rome ...") is TR-only. |

## Proposed §6.2 additions

- **Construction: *kata* + *oikos*** (singular and plural). v2 gives a clear singular "at your house" use against which the §6.2 item "from house to house" can be compared. Arguably already implied by that item; adding the construction makes stream C able to generate it.
- **Lemma: *doulos*.** Rendering splits between "servant" and "slave" across the panel; relevant to the §6.2 item "faithful and discreet slave".
- **Lemma: *koinōnia* / *koinōnos*** (v6, v17). Worth a consistency table if stream C shows the NWT splitting its renderings; low priority.

## Notes for the time sample

- Setup (downloading TAGNT and the open texts, extracting the chapter) is one-time and is not part of the per-chapter cost.
- Every `TODO-NWT` above needs a person to look up the 1984 and 2013 NWT. That lookup is probably the main per-verse cost and is worth timing separately.
- The eight copyrighted panel translations were not consulted; a full stream B sweep needs them (per-verse lookup).
