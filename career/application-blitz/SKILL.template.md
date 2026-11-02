---
name: application-blitz
description: Tailor the candidate's one-page resume to a specific job posting using only their approved bullet bank, and report which job requirements it refused to claim. Use when they shares a job link or description and asks for a resume, application materials, or "blitz".
---

# Application Blitz

Turn one job posting into a tailored one-page resume (.docx) plus a short fit report. **Every claim must come from the approved bank below. Wording may be tuned; facts may not.**

## Inputs

- A job posting (link or pasted text). If it's a link, open it. If it can't be opened, ask their to paste the text. Never tailor from a title alone.
- Optional: "with cover letter", "short version", or a track they wants forced.

## Layer 1: Narrative (who should the reader see?)

Read the posting and pick **one** track, then say in one line: *"For this role, the reader should see the candidate as …"*

| Track | Pick when the role is about | Summary row |
|---|---|---|
| **AI PM** | AI/ML/GenAI products, personalization, recommendation, data products, platform requirements | SUM-1 |
| **Strategy & Ops** | strategy, business operations, chief of staff, transformation, operating rhythm, planning, investment | SUM-2 |
| **Product strategy & GTM** | go-to-market, product marketing, growth, launches, adoption | SUM-3 |

**Abort instead of writing a resume** (and explain why in two lines) if the role needs hands-on ML/software engineering, a mandatory engineering degree with no alternative, 10+ years of direct PM experience, or is pure sales. Forcing a story onto a bad fit is how a resume starts lying.

## Layer 2: Composer (which evidence, in what order?)

1. **Extract** the posting's core requirements (must-haves) and secondary keywords. Record which are already covered by the base resume *before* tailoring.
2. **Score every approved bullet** against the track and the posting: +3 if the track is in its Tracks list (or "All"), +1 per core requirement it genuinely evidences, +0.5 per secondary keyword. Ties: keep the one with the stronger number.
3. **Select within line budgets** (one page, 10pt Arial, normal margins):

| Section | Bullets |
|---|---|
| Most recent role | 4–5 |
| Previous role, same company | 1–2 |
| Earlier company | 2–3 |
| Current projects / consulting | 1 each |
| Education | 1–3 |

Order bullets inside each role by score. Keep roles reverse-chronological. Never use the same evidence twice.

## Layer 3: Tailor (how does each sentence read?)

Adjust wording toward the posting's vocabulary, one bullet at a time. Every rewrite must pass **all** gates. If any gate fails, use the approved bank text unchanged.

| Gate | Rule |
|---|---|
| **Protected facts** | Every item in the bullet's Protected facts appears verbatim (same number, same unit, same scope). |
| **No new claims** | No new numbers, tools, clients, outcomes, team sizes or responsibilities not already in that bullet. |
| **No scope inflation** | Never upgrade verbs (supported→led, helped set→set, aligned→led, contributed→owned) and never widen scope (one division → company-wide). |
| **No titles they hasn't held** | Never describe their as a Product Manager or Product Marketing Manager. Use their real titles. |
| **Banned labels** | Words the candidate has asked never to see (list them in the bank). |
| **Length** | No rewrite longer than the bank text + 10%. Aim to keep each bullet to 2 lines (≈ 230 characters). |
| **Fixed slots** | Header, company names and descriptors, titles, dates, education and skills are never reworded. |

Shortening is allowed (removing words while keeping every protected fact).

## Output

1. **The resume as .docx**: one page, Arial 10pt, matching the fixed layout below. File name: `the candidate_Purswani_Resume_<Company>.docx`.
2. **Fit report** (in chat, short):
   - Track chosen and the one-line narrative
   - Requirement coverage before → after tailoring
   - **Declined:** every core requirement or keyword they can't truthfully claim, and why. Several declined *core* requirements = say plainly that the role is a stretch.
   - Bullets used (IDs), and any bullet where tailoring was rejected by a gate
3. **Cover letter** only if asked: ≤ 250 words, built from the same selected bullets, no new facts.

Never submit an application, never contact anyone.

## Fixed layout

Header, company names, titles, dates, education and skills go here, exactly as they should appear. These are never reworded.

## Approved bullet bank (fictional sample)

Replace with your own bullets. Only rows you have approved go here.

### Summaries
- **SUM-1 · AI PM:** Digital product strategist with 6+ years in personalization and experimentation across the GCC. Owned the rollout of a recommendation engine to 500K+ customers.
  - Protected: 6+ years · 500K+

### Example Retail Group, Manager
- **EXP-1 · All:** Scaled a customer value program from pilot to 8 brands, delivering AED 20M+ annual incremental revenue measured against control groups
  - Protected: 8 brands · AED 20M+ · measured against control
- **EXP-3 · AI PM:** Owned the rollout of a recommendation engine to 500K+ customers, aligning data, engineering and vendor teams on integration requirements; revenue per recipient reached 2× control
  - Protected: 500K+ · 2× control · "owned the rollout" (not "built")

### Cut (never use)
- Any figure that doesn't match its source · any title not held
