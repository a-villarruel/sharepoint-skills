# RFP Response - Extraction

**Phase 1 of 4 — Intake & Mapping**

Reads an incoming RFP document stored in SharePoint and populates a structured tracking list with every actionable item found — questions, mandatory requirements, submission rules, evaluation criteria, and administrative certifications. Each item is categorized, flagged as mandatory or not, and traced back to its source location in the document so the team can assign owners and track response progress.

Handles multi-document packages (RFP body, addenda, Q&A, attachments) and correctly applies addenda — later versions override earlier ones rather than appending.

---

## Where it fits

```
Phase 1: [RFP Response - Extraction] → [RFP Response - Content Finder]
                    ↓
         (human gate: review tracker)
Phase 2: [RFP Response - Strategy Synthesis]
Phase 3: [RFP Response - Content Generation]
Phase 4: [RFP Response - Proposal Review] → [Compliance Review] → [Quality & Tone Review]
```

---

## Inputs

- RFP document (PDF or Word) accessible in SharePoint
- Any addenda, attachments, or Q&A documents referenced in the package

## Output

A populated **RFP Tracker** SharePoint List — one row per extracted item, with columns for Category, Mandatory flag, Source Location, Owner, and Status. Ready for the Content Finder skill to run next.

---

## Before you use this

1. Fill in the **Firm Profile** block at the top of `SKILL.md` (firm name, role boundary, vendor stance, specialization, voice).
2. Create the **RFP Tracker** SharePoint List with the required columns — see `SETUP.md` for the full column schema.

> Running this skill with the Firm Profile placeholders left blank will produce generic, unusable output.
