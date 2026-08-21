# Courseware QA Report — v6.0

**Course:** Scrum Master Fundamentals for High-Performing Teams  
**Course code:** TGS-2024045803  
**Release date:** 22 August 2026  
**Result:** PASS for local build and publication readiness

## A. Scope and programme alignment

- Five learning outcomes from the course page are preserved and mapped to Topics 1–5.
- Skills Framework reference: Business Agility, ICT-BIN-4038-1.1.
- Delivery remains two days / 16 hours, comprising 14 training hours and two assessment hours.
- Assessment instruments are Written Assessment (1 hour) and Case Study (1 hour).
- No practice exam is included.
- Canonical learner-resource label is **Activities**; no lab folder is present.

## B. Single-source alignment

- The slide deck, Learner Guide, Lesson Plan, activities, and assessments were generated from `courseware/build/course_data.py`.
- The legacy v5 deck was used as the coverage floor.
- Current Scrum terminology is anchored to the November 2020 Scrum Guide.
- Source coverage and generated-image provenance are recorded in `SOURCE-COVERAGE-v6.0.md`.
- `slide_map.json` is generated with the deck and consumed by the Lesson Plan.

## C. Deck QA

| Check | Evidence | Result |
|---|---:|---|
| Slide count | 149 | PASS |
| Rendered pages | 149 | PASS |
| Native editable PowerPoint charts | 3 | PASS |
| ImageGen workplace visuals | 6 | PASS |
| Slide transitions | 149 / 149 | PASS |
| Out-of-canvas shapes | 0 | PASS |
| Activity overview slides | 10 | PASS |
| Click-by-click procedure leakage on activity slides | 0 | PASS |
| Placeholder / TODO / prohibited practice-exam text | 0 | PASS |

All slides were rendered to PNG contact sheets and visually inspected. The cover, administrative slides, section dividers, content patterns, activity overviews, charts, and closing slides are legible and free of clipping or overlap. Detailed procedures are confined to the Learner Guide and activity packs.

## D. Learner Guide and Lesson Plan QA

- Learner Guide: 19 rendered pages; includes detailed activity procedures, browser-tool guidance, evidence requirements, acceptance criteria, facilitator prompts, and troubleshooting.
- Lesson Plan: 8 rendered pages; includes two-day schedule, duration, teaching method, exact slide references, activity-folder references, topic breakdown, and activity alignment.
- Both documents passed the Google Docs title-residue sanitizer and were visually inspected after PDF rendering.

## E. Activity QA

| Check | Evidence | Result |
|---|---:|---|
| Individual activity folders | 10 | PASS |
| Files per activity folder | 8 | PASS |
| Activity PDFs | 30 | PASS |
| Excel workbooks | 10 | PASS |
| Mock-data CSV files | 10 | PASS |
| Workbook formula errors after recalculation | 0 | PASS |
| Editable Excel charts in Activity 07 | 2 | PASS |

Every activity is self-contained and includes a detailed README, scenario, checklist, editable workbook, and mock data. All 30 PDFs were opened and their first pages were visually inspected; the activity sets have consistent branding, readable typography, and complete acceptance criteria.

## F. Assessment QA

### Written Assessment

Seven open-ended questions cover K1–K7 exactly once. Candidate paper and trainer answer key are separate documents.

### Case Study

Five questions cover all abilities:

| Question | Ability coverage |
|---|---|
| Q1 | A3 |
| Q2 | A7 |
| Q3 | A4, A5 |
| Q4 | A2, A6 |
| Q5 | A1 |

The legacy five-question structure and one-hour duration were retained. The previous A6 coverage omission was corrected by explicitly mapping Q4 to A2 and A6.

The rendered assessment set passed `verify_assessment.py`: cover-only page 1, candidate information/instructions/grading on page 2, content from page 3, LMS upload link present, no “For Official Use Only”, and answer-key blocks complete.

## G. Privacy and release gates

- Candidate papers may be learner-facing.
- Answer keys are trainer-only and must not be linked into LMS-TMS or committed to GitHub.
- `.env`, reference files, build scripts, QA scratch renders, and assessment keys are excluded from the public repository.
- Drive, LMS-TMS dry-run, and GitHub read-back evidence are recorded during publication and are not implied by this local PASS.

