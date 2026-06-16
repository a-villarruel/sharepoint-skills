# RFP Response - Content Generation

**Phase 3 of 4 — Drafting**

Drafts the proposal section by section using the approved Strategy Brief as its blueprint. For each section it reads the relevant source documents in full before writing — never drafting from summaries alone. It uses one of three modes per section based on what source material is available: **Adapt** (strong source match), **Synthesize** (material exists across multiple documents), or **Placeholder** (no source material — inserts a structured, descriptive placeholder rather than inventing content).

Enforces the firm's role boundary and vendor stance throughout. Every mandatory RFP requirement is tracked in a per-section register and must be explicitly answered in the prose. The output is a complete Word document ready for Phase 4 review.

---

## Where it fits

```
Phase 1: [RFP Response - Extraction] → [RFP Response - Content Finder]
Phase 2: [RFP Response - Strategy Synthesis]
                    ↓
         (human gate: approved Strategy Brief required before this skill runs)
Phase 3: [RFP Response - Content Generation]
                    ↓
Phase 4: [RFP Response - Proposal Review] → [Compliance Review] → [Quality & Tone Review]
```

---

## Inputs

- **Strategy Brief** (.docx, Phase 2 output) — approved ToC, Coverage Map, strategic themes, tone guidance, section-by-section drafting notes, Page Budget Table
- **RFP Tracker** SharePoint List — Category, Available Content, Source 1/2/3 columns populated
- **Source documents** referenced in the Source columns — must be accessible and readable in full
- **WIP Collaboration Folder** deal subfolder with write access

## Output

A **Proposal Draft** Word document (`[ClientName]_Proposal_Draft_v1_[Date].docx`) saved to the deal subfolder, containing all approved sections, an Exceptions & Assumptions section, appendices, and clearly marked placeholders for any content requiring human or SME input.

---

## Before you use this

1. Fill in the **Firm Profile** block at the top of `SKILL.md` — the role boundary and vendor stance rules apply to every word drafted.
2. Phase 2 must be complete and the Strategy Brief approved by the salesperson/pursuit lead before this skill runs.
3. All source documents in the RFP Tracker Source columns must be accessible to the agent.

> This skill will never invent facts, statistics, or case studies. If source material does not exist, it inserts a placeholder. Do not run it expecting it to fill gaps the firm does not have content for.
