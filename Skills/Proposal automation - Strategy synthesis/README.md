# RFP Response - Strategy Synthesis

**Phase 2 of 4 — Strategy**

Reads multiple input documents — the populated RFP Tracker, past proposals, a salesperson-authored Win Strategy Brief, capability statements, and a Win/Loss Debrief — and synthesizes them into two deliverables: a **recommended Table of Contents** and a **Content Strategy Brief**. Also produces an explicit competitive-positioning recommendation (price / capability / delivery risk) and a page-budget allocation table that governs how much space each section gets in the draft.

Nothing in Phase 3 should be drafted without an approved output from this skill.

---

## Where it fits

```
Phase 1: [RFP Response - Extraction] → [RFP Response - Content Finder]
                    ↓
         (human gate: confirm tracker + mappings)
Phase 2: [RFP Response - Strategy Synthesis]
                    ↓
         (human gate: approve ToC + strategy before drafting)
Phase 3: [RFP Response - Content Generation]
Phase 4: [RFP Response - Proposal Review] → [Compliance Review] → [Quality & Tone Review]
```

---

## Inputs

- Populated **RFP Tracker** SharePoint List (Phase 1 complete)
- **Past Proposals** — 2–3 documents from the Past Proposals Library (same solution domain preferred)
- **Win Strategy Brief** — salesperson-authored document with client context, competitive dynamics, and deal-specific differentiators
- **Capability Statements** — 2–3 firm-authored documents describing relevant services and methodologies
- **Win/Loss Debrief** — lessons learned from past similar deals

## Output

A **Strategy Brief** Word document saved to the deal subfolder in the WIP Collaboration Folder, containing:
- Coverage Map (every RFP row mapped to a ToC section)
- Submission Checklist (procedural rules for the pursuit team)
- Recommended Table of Contents with strategic rationale annotations
- Page Budget Table
- Full Content Strategy Brief (situation summary, value proposition, competitive positioning, strategic themes, tone guidance, risk/neutralization strategy, content gaps, section-by-section drafting notes)

---

## Before you use this

1. Fill in the **Firm Profile** block at the top of `SKILL.md`.
2. Create the **WIP Collaboration Folder** in SharePoint — see `SETUP.md`.
3. Have the salesperson complete the Win Strategy Brief before running. Without it, the competitive positioning analysis will be significantly less targeted.

> Running this skill with the Firm Profile placeholders left blank will produce generic, unusable output.
