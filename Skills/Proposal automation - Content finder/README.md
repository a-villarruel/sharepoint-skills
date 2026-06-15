# RFP Response - Content Finder

**Phase 1 of 4 — Intake & Mapping**

Searches the firm's SharePoint content libraries to find existing material that matches each row in the RFP Tracker. Classifies each row as administrative (pass/fail legal or corporate qualifier) or substantive (approach, methodology, references, pricing, etc.), routes substantive rows to the most relevant libraries, scores and ranks matches, then writes the results back to the tracker — a plain-language summary in the **Available Content** column and clickable source links in three **Source** hyperlink columns.

The source links are what the Content Generation skill follows in Phase 3 to read the full documents before drafting. The summaries are for human review at the Phase 1 gate.

---

## Where it fits

```
Phase 1: [RFP Response - Extraction] → [RFP Response - Content Finder]
                    ↓
         (human gate: review tracker + approve mappings)
Phase 2: [RFP Response - Strategy Synthesis]
Phase 3: [RFP Response - Content Generation]
Phase 4: [RFP Response - Proposal Review] → [Compliance Review] → [Quality & Tone Review]
```

---

## Inputs

- Populated **RFP Tracker** SharePoint List (output of RFP Response - Extraction)
- Read access to the firm's four content libraries:
  - **Capability Library** — methodology, capability statements, case-study abstracts
  - **Content Asset Library** — slides, FAQs, proposal fragments, boilerplate
  - **Past Proposals Library** — prior submitted proposals
  - **Standard Positions** — reusable positions on IP/data rights, pricing, exceptions

## Output

Updated **RFP Tracker** with Available Content summaries and Source 1/2/3 hyperlinks populated for every row. Rows with no matching content are flagged as **No Match** — these require SME or salesperson input before Phase 3.

---

## Before you use this

1. Fill in the **Firm Profile** block at the top of `SKILL.md`.
2. Create the four content libraries and the RFP Tracker List columns (Available Content + Source 1/2/3 as Hyperlink type) — see `SETUP.md`.
3. The Source columns **must be Hyperlink type** (not plain text) for the clickable links to work.

> Running this skill with the Firm Profile placeholders left blank will produce generic, unusable output.
