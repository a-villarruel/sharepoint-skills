# RFP Response - Compliance Review

**Phase 4 of 4 — Review**

A rule-based compliance check that runs against the salesperson-reviewed draft before publication. Checks for language that misrepresents the firm's role or positioning, commitments the firm cannot or should not make, missing required disclosures, and violations of the procurement's submission standards. Logs every finding to the **Review Findings** SharePoint List and annotates the draft document inline so the reviewer knows exactly where to look and what to fix.

**No proposal proceeds to publication until all High severity findings are resolved.**

This skill is strictly rule-based — it does not make subjective judgments about tone or writing quality. Those are handled by the Quality & Tone Review skill.

---

## Where it fits

```
Phase 1: [RFP Response - Extraction] → [RFP Response - Content Finder]
Phase 2: [RFP Response - Strategy Synthesis]
Phase 3: [RFP Response - Content Generation]
                    ↓
Phase 4: [RFP Response - Proposal Review] → [RFP Response - Compliance Review] → [Quality & Tone Review]
                    ↓
         (human gate: final review & submission)
```

Runs after Proposal Review, before Quality & Tone Review.

---

## Inputs

- **Salesperson-reviewed draft** — must be saved in the WIP Collaboration Folder after human corrections. Do not run against the raw Phase 3 draft.
- **RFP Tracker** SharePoint List — Submission Rules rows are used for procurement compliance checks
- **Review Findings** SharePoint List — must exist for logging
- The firm's **style and compliance guide** (source of truth for prohibited terms and required language)

## Output

- New items logged in the **Review Findings** SharePoint List, one per finding, with severity, location, verbatim text, and recommended fix
- Inline annotations added to the draft document at each finding's location
- A summary to the user: findings by severity, all High findings listed, page count vs. RFP limit, links to the annotated draft and findings list

---

## Before you use this

1. Fill in the **Firm Profile** block at the top of `SKILL.md`.
2. **Replace the example compliance rules** in `SKILL.md` with your firm's actual rules. The skill ships with illustrative examples for an advisory firm — they will not be correct for your firm as-is.
3. Create the **Review Findings** SharePoint List — see `SETUP.md` for the column schema.
4. All Phase 3 placeholders must be filled before this skill runs — it cannot compliance-check a placeholder.

> High severity findings block publication. A salesperson who believes a High finding is incorrect must escalate to an authorized approver — the skill will not downgrade a finding without human sign-off.
