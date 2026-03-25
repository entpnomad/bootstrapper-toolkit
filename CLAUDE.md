# Bootstrapper Toolkit — Business Strategy Skills

Business strategy skills toolkit for bootstrapped founders, built as Claude Code skills.

Created by [Alex Diaz](https://www.linkedin.com/in/revenuehunt/), co-founder of [RevenueHunt](https://www.revenuehunt.com/) — a 7-figure self-funded SaaS that helps ecommerce stores build product recommendation quizzes to increase conversions and collect zero-party data. This toolkit condenses the same bootstrapping philosophy we used to grow RevenueHunt from zero to profitability without a dollar of outside funding.

## Project Structure

```
bootstrapper-toolkit/
├── CLAUDE.md                 # This file
├── references/               # Business books (PDFs) — knowledge base
│   └── INDEX.md              # Pre-indexed book catalog for progressive disclosure
└── .claude/                  # Project-level Claude config
```

## Skills (in .claude/skills/)

### `/venture-sensei`
Brutal, bullshit-free business strategist. Evaluates ideas with real-world frameworks, drawing on the reference library. Created by the founders of RevenueHunt.com.

### `/bootstrap-oracle`
Structured business idea evaluator. Scores ideas on 9 weighted factors, runs a 5PM filter, produces a structured output with unit economics, cash-flow analysis, and sanity gates. Calibrated to bootstrapped business reality. Oracle scoring inspired by a framework from [Andrew Shackleford](https://www.linkedin.com/in/andrew-s-a175623/).

### `/analyze-idea`
Orchestrated business idea analysis. Runs 10 dimension skills for deep factual research, applies Oracle scoring with full context, then synthesizes a strategic verdict with Venture Sensei's interpretive voice. Use this for the most thorough critique.

### `/competitor-analysis`
Deep competitive intelligence. Analyzes competitors across 16 dimensions — funding, team location, pricing, SEO, ads, reviews, tech stack, product, and more. Red ocean philosophy: competition is validation, VC-backed competitors are an advantage.

### `/gtm-strategy`
Go-to-market strategy for bootstrappers. Eight-dimension analysis: beachhead & ICP, GTM motion, channel strategy (Bullseye), positioning & message-market fit, funnel & conversion, distribution economics, first 100 customers plan, and compounding scale path.

### `/moat-analysis`
Defensibility and switching cost analysis. Nine-dimension assessment: user-investment lock-in, network effects, data moats, distribution moats, counter-positioning, economies of scale, regulatory/compliance, relationship/trust, and process power. Core principle: design products where usage creates investment, and investment creates lock-in.

### `/problem-analysis`
Problem existence and pain validation. Nine-dimension assessment: problem evidence, pain severity, pain frequency, current solutions & workarounds, willingness to pay, urgency & trigger events, buyer persona clarity, problem scope, and the hair-on-fire test. Plus six binary validation gates. Core principle: assumption is the enemy, evidence is the standard.

### `/solution-analysis`
Product fitness and solution validation. Nine-dimension assessment: value proposition clarity, solution-problem fit, minimum product achievability, differentiation reality, switching motivation, time-to-value, retention & habit potential, substitute vulnerability, and solution conviction. Plus six validation gates including an explicit AI-substitute test. Core principle: when code is cheap, "can we build it?" is never the question — "is this the right thing to build?" is.

### `/founder-fit`
Founder-business fit assessment. Nine-dimension assessment: domain clarity, distribution access, execution tempo & 8-habits diagnostic, time & energy budget, financial runway, relationship & trust capital, ambition calibration, psychological readiness, and founder-business fit synthesis. Plus seven validation gates. Core principle: this is not a personality test — it's a collision analysis between who you are and what the business demands. Technical skills are nearly irrelevant; clarity, distribution, and relationships are everything.

### `/financial-projections`
Financial viability for bootstrappers. Nine-dimension assessment: revenue model clarity, unit economics & margins, cash-flow profile, break-even path (three-tier), revenue stairs, AI-native cost structure, pricing power, stress resilience, and founder sustainability. Plus six validation gates and Profit-First allocation. Core principle: revenue is the only funding round — model the founder's survival, not just the business's.

### `/timing-analysis`
Market timing and entry window assessment. Nine-dimension assessment: strategic inflection points, technology adoption stage, buyer behavior shifts, market window & entry timing, regulatory & policy catalysts, supply-side disruption, demand urgency, incumbent vulnerability windows, and bootstrapper timing fit. Plus five validation gates. Core principle: you can build at any time, but you can't create the wave — timing is about reading forces already in motion.

### `/swot`
Quick SWOT analysis with bootstrapper lens. Produces a structured strengths/weaknesses/opportunities/threats matrix with evidence, strategic implications (S+O, S+T, W+O, W+T cross-references), and prioritized action recommendations. Gateway tool — run this first for a fast strategic read, then go deep with dimension skills where it matters.

### `/idea-comparison`
Multi-idea comparison matrix. Side-by-side scoring of 2-4 business ideas on 8 weighted dimensions (problem clarity, market validation, distribution access, cash-flow speed, founder fit, competition gap, revenue ceiling, effort to test). Produces a ranked recommendation with trade-off analysis and kill criteria.

### `/user-personas`
ICP and buyer persona card generator. Produces 2-3 detailed persona cards (primary buyer, secondary buyer, anti-persona) with demographics, psychographics, behavior patterns, pain story, buying triggers, objections, and targeting criteria. Includes beachhead drift check and persona-to-action map.

### `/positioning`
Positioning and pitch copy generator. Produces ready-to-paste copy: positioning canvas (Obviously Awesome framework), one-liner, elevator pitch, homepage hero copy (3 options), value propositions, positioning statement, taglines, cold email opener, and language bank (customer pain phrases, words to use/avoid). NOT analysis — usable marketing artifacts.

### `/content-strategy`
Content and distribution strategy generator. Produces content pillars, 15 specific content ideas with ready-to-publish titles, 20 SEO keywords with volume/difficulty estimates, 90-day content calendar, channel-specific tactics (SEO, community, social, email), and a distribution checklist per content piece. BOFU-first strategy for bootstrappers.

### `/launch-plan`
30/60/90-day execution roadmap. Synthesizes all prior skill outputs into a chronological plan: weekly action items with deliverables, decision gates at Day 30/60/90, phase exit criteria, kill criteria, tools/resources list with costs, and estimated 90-day budget. Most powerful after running dimension skills — converts analysis into sequenced actions.

### `/risk-assessment`
Risk matrix and pre-mortem analysis. Seven-dimension risk assessment (market, competitive, execution, financial, platform/tech, regulatory, founder/team). Pre-mortem exercise with three failure stories. Blind spot detection (3-5 risks the founder isn't thinking about). Ranked risk matrix (10-15 risks with severity x likelihood). Five validation gates. Core principle: founders are optimists — this skill injects structured pessimism before real money is on the line.

### `/sanity-check`
Lightweight decision filter. Applies 6 bootstrapper principles (clarity, distribution, manual-first, lock-in, opportunity cost, compounding) to ANY founder decision. One-page output: verdict, minimalist version, primary risk, this week's action. No research phase — fast and opinionated. Can also review output of other skills.

## Skill Architecture — Modular Analysis Suite

The toolkit is a modular analysis and execution suite with five skill archetypes. Each business dimension gets its own standalone skill, independently invocable and composable. Generator and meta skills produce actionable artifacts from analysis outputs.

### Orchestrator Skills
- `/analyze-idea` — Runs multiple dimension skills, cross-references results, synthesizes verdict

### Mentor Skills
- `/venture-sensei` — Broad strategic mentorship, idea critique, business advice
- `/bootstrap-oracle` — Structured scoring, unit economics, sanity gates

### Dimension Skills (one per business aspect)
| Skill | Status | What it analyzes |
|-------|--------|-----------------|
| `/competitor-analysis` | **Live** | Competitor landscape, positioning, vulnerabilities, pricing, team, funding |
| `/market-size` | **Live** | TAM/SAM/SOM/TRM, bottom-up sizing, beachhead identification, demand signals, revenue ceiling, market dynamics & risks |
| `/problem-analysis` | **Live** | Problem existence & evidence, pain severity, willingness to pay, buyer personas, urgency triggers, validation gates, founder-vs-reality gap |
| `/solution-analysis` | **Live** | Product fitness, value prop clarity, differentiation, MPA, substitutes, AI-substitute threat, switching motivation, retention |
| `/gtm-strategy` | **Live** | Beachhead & ICP, GTM motion, channels (Bullseye), positioning & message-market fit, funnel, distribution economics, first 100 customers, compounding scale |
| `/timing-analysis` | **Live** | Why now, market readiness, adoption stage, inflection points, regulatory catalysts, entry windows, incumbent vulnerability, bootstrapper timing fit |
| `/business-model` | **Live** | Revenue model architecture, pricing architecture, unit economics, offer design, revenue quality, margin structure, cash flow dynamics, scalability & leverage, business model risks. Plus five validation gates |
| `/founder-fit` | **Live** | Founder-business fit, domain clarity, distribution access, execution tempo, 8-habits diagnostic, time/runway, relationships, ambition calibration, psychological readiness |
| `/moat-analysis` | **Live** | Defensibility, switching costs, user-investment lock-in, network effects, data moats, distribution moats, counter-positioning, real vs. fake moat classification |
| `/financial-projections` | **Live** | Cash flow, break-even, revenue stairs, unit economics, pricing power, stress tests, founder sustainability, 24-month projections |
| `/risk-assessment` | **Live** | Pre-mortem exercise, ranked risk matrix, blind spot detection, 7-dimension risk assessment (market, competitive, execution, financial, platform/tech, regulatory, founder/team). Plus five validation gates |

### Generator Skills (produce actionable artifacts)
| Skill | Status | What it produces |
|-------|--------|-----------------|
| `/swot` | **Live** | SWOT matrix with evidence, strategic implications (S+O, S+T, W+O, W+T), prioritized actions, deep-dive recommendations |
| `/user-personas` | **Live** | 2-3 detailed persona cards (primary buyer, secondary buyer, anti-persona), targeting criteria, beachhead drift check, persona-to-action map |
| `/positioning` | **Live** | Positioning canvas, one-liner, elevator pitch, homepage hero copy (3 options), value propositions, taglines, cold email opener, language bank |
| `/content-strategy` | **Live** | Content pillars, 15 titled content ideas, 20 SEO keywords, 90-day content calendar, channel tactics, distribution checklist, AI discoverability strategy |

### Meta Skills (cross-idea or cross-skill synthesis)
| Skill | Status | What it does |
|-------|--------|-------------|
| `/idea-comparison` | **Live** | Side-by-side scoring of 2-4 ideas on 8 weighted dimensions, ranked recommendation, trade-off analysis, sequencing advice |
| `/launch-plan` | **Live** | 30/60/90-day execution roadmap with weekly actions, decision gates, kill criteria, tools/budget, phase exit criteria. Synthesizes all prior skill outputs |

### Filter Skills (lightweight decision filters)
| Skill | Status | What it does |
|-------|--------|-------------|
| `/sanity-check` | **Live** | Applies 6 bootstrapper principles to any founder decision. One-page output: verdict, minimalist version, primary risk, this week's action. No research — fast and opinionated. Can review output of other skills |

## Reference Library

Books live in `references/`. Before reading any PDF, always check `references/INDEX.md` first to find which book is relevant and which pages to read.

**Progressive disclosure protocol:**
1. Check INDEX.md for topic → book mapping
2. Read only the relevant section summary from the index
3. Only open the actual PDF when specific detail is needed
4. Never load entire books into context

## Philosophy

**Bootstrapped, revenue-first, contrarian.** We do not build for sale. We build for long-term profitability, self-funded from customer revenue. When everybody is trying to hunt for the next unicorn, the wise option is to farm cash cows.

- No VC mindset, no exit-first thinking, no valuation theater
- Revenue, cash flow, and profitability are the metrics that matter
- Build things people pay for, then compound over decades
- The best moment to sell a good business is never

### The Bottleneck Shift (AI-Native Reality)

The cost of building code has dropped to near zero. AI coding tools (Claude Code, Cursor, etc.) mean a solo founder can ship what used to take a funded team of engineers. **The old SaaS playbook — raise capital → hire developers → build → pray — is dead for bootstrappers.**

The bottleneck has moved. The new scarce resources are:

1. **Clarity** — Do you actually know what's worth building? You can now build faster than you can think. The ones who make money are the ones with clarity about what customers will pay for.
2. **Distribution** — When everybody can build, product is not the moat. Getting your product into people's hands is the moat. Channels, relationships, and audience ownership matter more than features.
3. **Ambition** — When shipping was expensive, small bets made sense. Now you can take 50 swings per year. The risk is timidity, not building the wrong thing.
4. **Relationships** — You can't vibe-code a relationship. Trust, reputation, and being known in your market are durable advantages when technical skills are commoditized.

See `.claude/skills/_shared/philosophy.md` for the operational framework that skills consume. Key points:
- "Can we build it?" is no longer a meaningful filter
- CAC and time-to-clarity are the dominant variables
- Many reference books were written when code was expensive — apply frameworks but discount dev cost assumptions

### Structured Output Is for Founders, Not VCs

The pitch-deck-style output from our skills is NOT for pitching VCs or angels. Bootstrapped companies don't pitch anyone. The structured format exists to **force clarity of thinking** — for founders validating ideas with their own money and time. Every section is a question the founder must answer honestly before risking their resources. The audience is the founder, their co-founders, and reality.

See: `references/ai-native-bottleneck-shift.md` for the full framework.

## Conventions

- Never reference book titles or quote material directly when giving advice — distill as original counsel
- Tone: authoritative, insightful, occasionally blunt. Never robotic or polished.
- Always ask for context when a question is vague rather than giving generic advice
- When evaluating business ideas, always consider founder fit, unit economics, and real market evidence
- When Oracle scoring contradicts dimension skill evidence, explain why — don't smooth over the mismatch

## Origin

Created by [Alex Diaz](https://www.linkedin.com/in/revenuehunt/), co-founder of [RevenueHunt](https://www.revenuehunt.com/). RevenueHunt is a 7-figure bootstrapped SaaS platform that powers product recommendation quizzes for ecommerce stores — helping brands increase conversions and collect zero-party customer data. Built without venture capital, grown through revenue.

The Oracle scoring skill was inspired by a framework from [Andrew Shackleford](https://www.linkedin.com/in/andrew-s-a175623/), a fellow [Dynamite Circle](https://dynamitecircle.com/) member.

This toolkit distills the frameworks, mental models, and hard-won lessons from building RevenueHunt into a set of reusable Claude Code skills — so other bootstrapped founders can pressure-test their ideas with the same rigor.

