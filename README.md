# ai-career-os

**AI agents I run my own job search on: built for the GCC, with a human approving every step.**

I'm finishing an NYU Stern MBA in Strategy & AI in Abu Dhabi and recruiting for AI product and strategy roles. Instead of using AI as a chatbot, I turned the repetitive parts of the search into small, reliable agents, each with clear rules about what it may and may not do.

| Agent | What it does | Status |
|---|---|---|
| [**job-hunter**](./career/job-hunter/) | Sweeps GCC job boards and target career pages for AI PM, Strategy & Ops and PMM roles; verifies every posting is live; scores fit; surfaces a digest for review | ✅ live |
| [**application-blitz**](./career/application-blitz/) | Tailors my resume from a bank of approved, fact-checked bullets, and reports every requirement it refused to claim | ✅ live |
| **networking-scout** | Ranks contacts at target companies by shared background, relevance and reachability | planned |
| **relationship-nurture** | Flags warm contacts going cold and drafts the follow-up as a Gmail draft | planned |

## Principles

1. **Drafts, never sends.** Every outbound message is a draft. Every tracker write is approved.
2. **Never invents.** No made-up roles, links, metrics or experience. When unsure, it says so.
3. **Built for the region.** GCC sources, Abu Dhabi's applied-AI ecosystem, and a market where warm introductions matter more than applications.
4. **Honest about fit.** Stretch roles are labelled as stretches, not hidden or inflated.

## How it runs

Each agent is a Claude skill: a plain-language instruction file (`SKILL.md`) that Claude follows, using web search and my Google Drive and Gmail. There are no servers or scrapers; the design work is in the rules.

## About me

Chandni Purswani · Strategy + AI · Abu Dhabi
6+ years building personalization, customer data and experimentation products across the GCC, including an AI recommendation engine shipped to 1M+ customers at Majid Al Futtaim.

[Portfolio](https://chandnipurswani.github.io) · [LinkedIn](https://www.linkedin.com/in/chandni-purswani)
