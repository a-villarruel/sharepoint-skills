# RFP Response - Quality & Tone Review

**Phase 4 of 4 — Review**

A structured editorial review that assesses how the proposal reads — whether it sounds like the firm, whether the narrative holds together as a coherent argument, whether each section earns its place, and whether the language is specific and confident enough to persuade an evaluator. Runs after Compliance Review and salesperson corrections. Logs findings to the **Review Findings** SharePoint List and annotates the draft inline.

This is not a spell-checker. It is a calibrated editorial review against the firm's configurable voice standards, the approved strategy, and the buyer's evaluation audience.

---

## Where it fits

```
Phase 1: [RFP Response - Extraction] → [RFP Response - Content Finder]
Phase 2: [RFP Response - Strategy Synthesis]
Phase 3: [RFP Response - Content Generation]
                    ↓
Phase 4: [RFP Response - Proposal Review] → [Compliance Review] → [RFP Response - Quality & Tone Review]
                    ↓
         (human gate: final review & submission)
```

Runs last in Phase 4, after Compliance Review findings have been addressed.

---

## Inputs

- **Compliance-reviewed and salesperson-corrected draft** from the WIP Collaboration Folder
- **Review Findings** SharePoint List — existing Compliance findings for this proposal (to avoid re-flagging)
- **Content Strategy Brief** (Phase 2 output) — the approved strategy the draft is assessed against

## Output

- New items logged in the **Review Findings** SharePoint List: narrative coherence gaps (High), tone and structural issues (Medium), line-level language patterns (Low)
- Inline annotations added to the draft at each finding's location
- A summary to the user covering: findings by severity, High findings listed explicitly, differentiator coverage (confirmed vs. absent), terminology consistency, proportionality assessment vs. evaluation criteria weighting, links to the annotated draft and findings list

---

## Before you use this

1. Fill in the **Firm Profile** block at the top of `SKILL.md` — particularly `NAMED METHODOLOGY`, `VALUE MODEL`, and `VOICE`, which drive the editorial standards.
2. **Replace the example voice standards** in `SKILL.md` with your firm's actual standards. The skill ships with illustrative examples for a precise, risk-disciplined advisory voice — these will not match your firm's voice as-is.
3. Run after Compliance Review, not before — this skill checks quality, not rule compliance.
4. The **Review Findings** SharePoint List must exist — see `SETUP.md`.

> High findings from this skill indicate structural problems (narrative coherence gaps, missing critical differentiators) that require section-level rewrites, not line edits.
