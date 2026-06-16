# RFP Response - Proposal Review

**Phase 4 of 4 — Review**

An automated pre-flight audit that runs against the generated proposal draft before any human reviewer opens it. Checks three dimensions that are invisible to a casual read: whether the draft followed the approved strategy, whether every RFP requirement is actually addressed in what was written (not just in the approved ToC), and whether the content is grounded in the firm's source material or may have been hallucinated.

Produces a **Review Report** Word document that tells the reviewer exactly where to focus — and confirms what has already been verified — so the human review session is efficient rather than exploratory.

---

## Where it fits

```
Phase 1: [RFP Response - Extraction] → [RFP Response - Content Finder]
Phase 2: [RFP Response - Strategy Synthesis]
Phase 3: [RFP Response - Content Generation]
                    ↓
Phase 4: [RFP Response - Proposal Review] → [Compliance Review] → [Quality & Tone Review]
                    ↓
         (human gate: final review & submission)
```

Runs first in Phase 4, before Compliance Review and Quality & Tone Review.

---

## Inputs

- **Generated proposal draft** (.docx, Phase 3 output) in the deal's WIP Collaboration Folder subfolder
- **Strategy Brief** (.docx, Phase 2 output) — approved ToC, strategic themes, tone guidance, section-by-section drafting notes
- **RFP Tracker** SharePoint List — all columns populated including Available Content and Source 1/2/3

## Output

A **Review Report** Word document (`[ClientName]_Review_Report_[Date].docx`) saved to the deal subfolder, containing:
- Overall status: **READY FOR HUMAN REVIEW** or **REQUIRES REVISION BEFORE REVIEW**
- Strategy fidelity findings (ToC structure, theme coverage, tone, drafting-note compliance)
- Draft Coverage Map (every RFP row classified as Covered / Placeholdered / Thin / Missing)
- Content sourcing confidence ratings per section (flags potential hallucinations)
- Placeholder Register (every placeholder with owner and priority)
- Prioritised action list for the pursuit team

> All findings go into the Report document — nothing is output to chat.

---

## Before you use this

1. Fill in the **Firm Profile** block at the top of `SKILL.md`.
2. Phase 3 must be complete and the draft saved to the WIP Collaboration Folder before this skill runs.
3. Confirm which file is the current draft if multiple versions exist in the subfolder — the skill will ask if it cannot determine this.
