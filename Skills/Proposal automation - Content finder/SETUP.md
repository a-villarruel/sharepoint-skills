# Setup & Configuration

Complete these steps once before running any skill. They take ~30 minutes.

---

## 1. Fill in the Firm Profile

Every `SKILL.md` opens with a **Firm Profile** block. Fill it in identically
across all seven skills (or maintain it in one place and paste it in). The skills
read these values as the source of truth for who your firm is and how it writes.

```
## Firm Profile (REQUIRED — fill in before use)

- FIRM NAME:            [e.g., Northwind Consulting]
- WHAT THE FIRM DOES:   [one sentence — e.g., "management consulting; we advise
                         and design, we do not build or operate systems"]
- ROLE BOUNDARY:        [what the firm will NOT claim to do — e.g., "not a
                         software vendor; not an implementation/managed-services
                         provider". Leave blank if no boundary applies.]
- VENDOR STANCE:        [e.g., "vendor-neutral — we recommend no specific
                         product" OR "we resell/implement Product X"]
- SPECIALIZATION:       [domains the firm credibly claims — e.g., "supply-chain
                         and operations transformation"]
- NAMED METHODOLOGY:    [optional — e.g., "our 5-step Diagnose→Deliver method";
                         leave blank if none]
- VALUE MODEL:          [optional — the through-line your proposals argue;
                         leave blank if none]
- VOICE:                [3–5 adjectives — e.g., "precise, confident,
                         evidence-led, plain-language"]
```

Anywhere a skill says `[FIRM NAME]`, `[ROLE BOUNDARY]`, `[SPECIALIZATION]`, etc.,
it is reading from this block.

---

## 2. Create the SharePoint objects

The skills share a small set of SharePoint Lists and document libraries. Names
below are **defaults** — rename them if you like, but use your chosen names
consistently across all skills (each skill references them in its Prerequisites).

### Lists

**RFP Tracker** — one row per extracted RFP item. Columns:

| Column | Type |
|---|---|
| Item | Multiple lines of text |
| Category | Choice: Question / Mandatory Requirement / Submission Rule / Evaluation Criterion / Administrative Certification |
| Mandatory | Yes/No |
| Source Location | Single line of text (page/section of the RFP) |
| Owner | Person |
| Status | Choice: Not Started / In Progress / Complete |
| Available Content | Multiple lines of text |
| Source 1 | Hyperlink |
| Source 2 | Hyperlink |
| Source 3 | Hyperlink |

**Review Findings** — one row per review issue. Columns:

| Column | Type |
|---|---|
| Proposal | Single line of text (or lookup to a Proposals list) |
| Review Type | Choice: Compliance / Quality & Tone |
| Severity | Choice: High / Medium / Low |
| Rule Category | Single line of text |
| Location | Single line of text |
| Finding | Multiple lines of text |
| Verbatim text | Multiple lines of text |
| Recommended fix | Multiple lines of text |
| Status | Choice: Open / Resolved |
| Resolved by | Person |

### Document libraries

| Library (default name) | Holds |
|---|---|
| **Capability Library** | Firm-authored methodology, capability statements, case-study abstracts |
| **Content Asset Library** | Slides, FAQs, proposal fragments, boilerplate sections |
| **Past Proposals Library** | Prior submitted proposals |
| **Standard Positions** | Reusable positions: IP/data-rights, pricing, exceptions & assumptions templates |

### Working folder

| Folder (default name) | Purpose |
|---|---|
| **WIP Collaboration Folder** | Per-deal working folder; each deal gets a subfolder named `[ClientShort]_[RFPShort]_[Year]`. All phase outputs save here. |

---

## 3. Object-name map (single source of truth)

If you rename anything, record it here and update the Prerequisites section of
each skill to match.

| Role | Name in your tenant |
|---|---|
| Tracking list | RFP Tracker |
| Findings list | Review Findings |
| Capability content | Capability Library |
| Reusable assets | Content Asset Library |
| Prior proposals | Past Proposals Library |
| Reusable positions | Standard Positions |
| Per-deal working folder | WIP Collaboration Folder |

---

## 4. Review the shipped examples

- **compliance-review** ships with example prohibited-language and disclosure
  rules. They are illustrative — replace them with your firm's actual rules.
- **quality-tone-review** ships with example voice standards. Replace with yours.
