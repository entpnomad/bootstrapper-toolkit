# Bootstrapper Toolkit

A [Claude Code skills](https://docs.anthropic.com/en/docs/claude-code/skills) toolkit that helps founders evaluate business ideas with bootstrapper-first rigor. Built for founders who self-fund from customer revenue, not venture capital.

Powered by a curated reference library of business books — strategy, positioning, pricing, growth, unit economics, and more. The skills distill insights from dozens of books into structured analysis, so you get battle-tested frameworks without having to read the entire shelf yourself.

## What This Does

Type `/analyze-idea` in Claude Code and describe a business idea. The toolkit launches 10 specialized research agents in parallel, scores the idea against a quantitative framework, and synthesizes a strategic verdict — all grounded in real market data via web research.

Each dimension can also run standalone:

| Skill | What it does |
|-------|-------------|
| `/analyze-idea` | Full orchestrated analysis — runs all dimensions, scores, synthesizes |
| `/venture-sensei` | Brutal strategic mentorship and idea critique |
| `/bootstrap-oracle` | Structured scoring with unit economics and sanity gates |
| `/competitor-analysis` | 16-dimension competitive intelligence |
| `/market-size` | Bottom-up TAM/SAM/SOM with demand validation |
| `/problem-analysis` | Pain severity, willingness to pay, buyer persona clarity |
| `/solution-analysis` | Product fitness, differentiation, AI-substitute threat |
| `/gtm-strategy` | Beachhead, channels, distribution economics, first 100 customers |
| `/moat-analysis` | Defensibility, switching costs, user-investment lock-in |
| `/timing-analysis` | Market window, inflection points, incumbent vulnerability |
| `/business-model` | Revenue architecture, pricing, margin structure, offer design |
| `/financial-projections` | Cash flow, break-even, revenue stairs, stress tests |
| `/founder-fit` | Domain clarity, distribution access, execution tempo, 8-habits diagnostic |

## Philosophy

**Revenue is the only funding round.**

- No VC mindset, no exit-first thinking, no valuation theater
- Build things people pay for, then compound over decades
- The best moment to sell a good business is never

Code is cheap — AI coding tools mean a solo founder can ship what used to take a funded team. The bottleneck has shifted from "can we build it?" to **clarity** (do you know what's worth building?) and **distribution** (can you reach buyers?). Every skill in this toolkit weights these accordingly.

## Setup

1. Clone this repo
2. Open the project directory in Claude Code
3. Run any skill: `/analyze-idea`, `/venture-sensei`, `/competitor-analysis`, etc.

Skills are project-local (`.claude/skills/`), not global. They activate automatically when Claude Code opens this directory.

## Project Structure

```
bootstrapper-toolkit/
├── CLAUDE.md                          # Project conventions and skill architecture
├── .claude/skills/                    # All skills (project-local)
│   ├── _shared/                       # Shared philosophy and principles
│   ├── analyze-idea/                  # Orchestrator — runs all dimensions
│   ├── venture-sensei/                # Mentor — strategic critique
│   ├── bootstrap-oracle/              # Mentor — structured scoring
│   ├── competitor-analysis/           # Dimension skill
│   ├── market-size/                   # Dimension skill
│   ├── problem-analysis/              # Dimension skill
│   ├── solution-analysis/             # Dimension skill
│   ├── gtm-strategy/                  # Dimension skill
│   ├── moat-analysis/                 # Dimension skill
│   ├── timing-analysis/               # Dimension skill
│   ├── business-model/                # Dimension skill
│   ├── financial-projections/         # Dimension skill
│   └── founder-fit/                   # Dimension skill
└── references/                        # Curated business book library (PDFs) + INDEX.md
```

## Why This Exists

I used to do all of this manually.

For years, I evaluated business ideas the slow way — reading books, building spreadsheets, Googling market data across 20 tabs, running competitive analysis by hand. Every new idea meant weeks of research before I had enough signal to decide if it was worth building.

My frameworks got sharper with each business. MetricSpot taught me what distribution-first thinking actually means. RevenueHunt taught me that the idea matters less than the channel. A decade of building things nobody wanted — a digital marketing agency, failed products, ideas that burned months and went nowhere — taught me which questions actually matter. What finally worked: SaaS with freemium distribution. Two out of dozens.

But the process was still slow, manual, and locked in my head.

Then AI got good enough to change the equation. Not "summarize this article" good — good enough to run 10 research agents in parallel, pull real market data, score an idea against a quantitative framework, and synthesize a verdict that's better than what most consultants produce. In minutes, not weeks.

So I took every framework I'd built over a decade — the scoring rubrics, the competitive dimensions, the unit economics sanity checks, the founder-fit diagnostics — and turned them into Claude Code skills. The reference library is 30+ business books I actually read and applied. The scoring weights reflect what I learned building two profitable businesses from zero.

This toolkit is my decision-making process, automated. It's opinionated because I am.

## Credits

Created by [Alex Diaz](https://www.linkedin.com/in/revenuehunt/), co-founder of [RevenueHunt](https://www.revenuehunt.com/) — a 7-figure bootstrapped SaaS built without venture capital. The Oracle scoring skill was inspired by a framework from [Andrew Shackleford](https://www.linkedin.com/in/andrew-s-a175623/), a fellow [Dynamite Circle](https://dynamitecircle.com/) member.

Read the human-friendly version on [Founders Hub](https://founders.do).
