---
name: job-hunter
description: Sweep GCC job sources and target-company career pages for Chandni's AI PM, Strategy & Ops and PMM roles, score fit, and return a review digest with a direct link to every role. Use when she says "hunt", "find roles", "any new jobs", or names a company to check.
---

# Job Hunter

Find open roles that fit Chandni's search, score them, and show her a ranked digest. **Never add anything to her tracker unless she names the rows to add.**

## 1. Who this is for

- Chandni Purswani, Abu Dhabi. NYU Stern MBA (Strategy & AI), graduating Dec 2026.
- 6+ years in personalization, customer data and experimentation products at Majid Al Futtaim and Nexa Digital.
- Locations: Abu Dhabi and Dubai. Flag (don't drop) roles elsewhere in the GCC or remote-from-UAE.

## 2. Role types and weights

| Rank | Role type | Weight | Title signals |
|---|---|---|---|
| 1 | AI PM | 1.00 | AI Product Manager, Product Manager (AI / ML / GenAI / data / platform for AI products), Senior PM in an AI company |
| 2 | Strategy & Ops | 0.85 | Strategy & Operations, Strategy Manager, Business Operations, Chief of Staff to a product/AI leader, AI Strategy, AI Transformation |
| 3 | PMM | 0.70 | Product Marketing Manager, Growth PM, Go-to-market lead for an AI or digital product |

Any other PM role (non-AI) counts as AI PM's neighbour: weight 0.80.

**Seniority:** keep Manager, Senior Manager, Senior PM, Lead. **Exclude:** intern, graduate, junior, associate/assistant titles, Director and above, VP, Head of (unless the posting asks for ≤ 8 years' experience). **Exclude:** technical program manager, project manager, engineering roles, pure sales.

## 3. Target companies

Tier sets the company weight. Search every Tier 1 company's own careers page on every run; Tier 2 on every run if time allows; Tier 3 only when she asks.

- **Tier 1 · weight 1.00 (applied / enterprise AI, Abu Dhabi):** Inception (G42), Presight, ai71, Microsoft (Abu Dhabi), The Applied AI Company (AAICO)
- **Tier 2 · weight 0.85 (AI-forward consumer tech and payments):** Careem, Talabat, Visa (CEMEA), Property Finder, G42 and its other companies (e.g. Core42)
- **Tier 3 · weight 0.70 (watchlist):** Dubai Holding, Bayut / Dubizzle, other VC-backed GCC scale-ups with an AI product
- **Not on the list:** weight 0.60. Still surface strong fits.

Chandni does not want traditional consumer businesses (banks, retailers, airlines, government apps) as primary targets. Surface their roles only if they are clearly AI product roles, and mark them "off-thesis".

## 4. Sources

Use several; each has different blind spots.

1. Each target company's official careers page (find it by searching "<company> careers"; use the company's own domain or its applicant tracking system, not a reposting site)
2. LinkedIn Jobs (search results pages via web search)
3. Bayt, GulfTalent, NaukriGulf, Indeed UAE
4. Wellfound and VC portfolio job boards for startups

Useful searches: `"AI product manager" Abu Dhabi`, `"product manager" AI Dubai`, `"strategy and operations" AI Abu Dhabi`, `"product marketing manager" AI UAE`, plus `<company> careers product manager`.

Open the posting itself before scoring it. Never score from a search snippet alone, and never list a role whose posting you could not open or whose date suggests it has closed.

## 5. Score

`fit score = role weight × company weight × freshness × 100`, rounded.

Freshness: posted ≤ 7 days 1.00 · 8–14 days 0.90 · 15–30 days 0.75 · 31–60 days 0.50 · older 0.40 · unknown 0.60. A "New" badge on the company's own job board counts as 8–14 days. If a reposting site and the original disagree on the date, trust the original.

Aggregator pages (job boards that copy postings) often stay up after a role is filled. When the role came from one, also check the company's own page; if it says filled, closed, or no longer exists, drop it and count it under "closed".

Then adjust, and say why in one line:
- +5 if the posting asks for personalization, experimentation / A/B testing, customer data / CDP, recommendation systems, marketplace or loyalty experience (her strongest evidence)
- +5 if it mentions GCC / regional market experience
- −10 if it requires Arabic fluency (flag it; don't drop it)
- −10 if it requires hands-on ML engineering or a computer science degree as a hard requirement

**Caps:** at most 2 roles per company in one digest (keep the highest scoring). Drop anything scoring under 40.

## 6. Dedupe against the tracker

The tracker is a Google Sheet named **"Job Pipeline"** in her Google Drive, with columns:
`Date added | Company | Role | Role type | Location | Posted | Fit score | Link | Status | Notes`

Before showing results, read the sheet and drop any role whose Link (or Company + Role) is already there. If the sheet doesn't exist, say so and offer to create it; don't create it unasked.

## 7. Output: the digest

Lead with one line: how many roles were found, how many survived filtering, how many were already tracked.

**Top picks**: a table, highest score first:

| # | Score | Role | Company | Location | Posted | Why it fits | Link |

- Every row must have a direct link to the posting itself. A role without a working link is not listed.
- "Why it fits" is one line in plain language, tied to her real experience. Don't call her background "CRM"; say personalization, customer data, experimentation or lifecycle products.

**By company**: Tier 1 first, then Tier 2, then others, so she can see which company is worth effort today.

**Flags**: Arabic required, off-thesis, outside UAE, unclear posting date.

**Skipped**: one line with counts by reason (too senior, too junior, wrong function, closed, duplicate).

End with: *"Reply with the numbers you want added to the tracker."*

## 8. Promotion (only after she replies)

Append only the rows she named to "Job Pipeline", with Status = "To apply" and today's date. Confirm what was added. Never change or delete existing rows.

## 9. Rules

- Review-first: the digest is the output. The tracker is a decision record, not a scratchpad.
- Never apply to anything, contact anyone, or send anything.
- Never invent a role, a date, a salary or a link. If unsure, leave it out or mark it unclear.
- If she names a company ("hunt Presight"), search only that company, but go deeper: all open roles in product, strategy and AI, even below the score cut-off, marked as such.
