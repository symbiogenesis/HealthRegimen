# Working notes for this repo

Everything here is a **working draft**. The markdown files are the current state of the analysis, nothing more. Git holds the history; the documents do not.

## The rule that matters most: no revision history in the prose

Write every document as if it had always said what it now says. When you change a score, a flag, a section, or a conclusion, **replace the old text with the new text and state the current reasoning** — do not narrate the edit.

Never write, in any doc:

- Version stamps in titles or headers — "Revised", "Revision 3", "v2", "draft 4"
- "What changed" / "Summary of changes" / changelog sections, promoted-demoted-added-cut lists
- Inline edit markers — "corrected this revision", "raised from E3", "NEW ROW", "flag changed from AVOID to MONITOR", "down from AVOID", "— new"
- Arguments against a former version of the same doc — "the previous version treated X as…", "earlier drafts said…", "this replaced the four-axis model", "restored after being dropped"
- Retained-for-comparison framing — "kept for the old view", "the score is unchanged"

Instead:

| Instead of | Write |
|---|---|
| "Inclisiran was over-graded at E5; it drops to E4." | "Inclisiran sits at E4: it was approved on LDL-C lowering alone and its outcomes trials have not reported." |
| "Flag changed from AVOID to MONITOR this revision, because…" | "Why MONITOR rather than AVOID: …" |
| "Why this replaced the four-axis version." | "Why the model has this shape." |
| "Metformin phases cleanly, so the score is unchanged." | "Metformin phases cleanly, so it still scores 4." |

The test: a reader seeing the file for the first time should never learn that a different version existed.

## What is *not* revision history, and should stay

- Comparisons to the **AgingBiotech source table** and its omissions — that is an external document being critiqued.
- Trial and field history — ITP hits that failed to replicate, retracted premises (taurine), pending readouts. That is science, not editing.
- The single date line under the title. One "as of" stamp is fine; a version number is not.
- Discussion of the user's own proposed protocols (the methionine plan, the block-cycling hypothesis) and which objections they answer. That is analysis of a live idea, not a record of edits to this repo.

## Housekeeping

- Keep the two files cross-linked: [anti-aging-inventory.md](anti-aging-inventory.md) holds framework, grouped inventory, interactions and protocols; [therapeutics-by-mechanism.md](therapeutics-by-mechanism.md) holds row-level reasoning. Scores must agree across both — change a score in one, change it in the other and in the flat list at §2.7.
- Filenames describe content, never status. No `-revised`, `-v2`, `-final` or similar markers on new files.
- Scoring convention: `E × B = score`, safety is a veto flag (`ok` / `monitor` / `AVOID`), effort is a tag outside the score.
