---
name: bootstrap-oracle
description: Structured business idea evaluator that outputs functionally narrow, painkiller businesses with built-in expansion to sustainable profitability. Use when user runs `/bootstrap-oracle`, asks to "score this business idea", "run oracle analysis", "evaluate this with oracle", "give me the oracle output", or needs a structured SaaS/bootstrap business evaluation with scoring, unit economics, and cash-flow analysis.
---

# Bootstrap Oracle

Originally created by [Andrew Shackleford](https://www.linkedin.com/in/andrew-s-a175623/), adapted for this toolkit. Andrew and Alex have been in the same Entrepreneur Mastermind through the [Dynamite Circle](https://dynamitecircle.com/) for over 5 years.

Outputs functionally narrow, painkiller businesses with built-in expansion to sustainable, self-funded profitability. Preserves bootstrapped sanity, injects pre-validation & marketing-first doctrine, and recalibrates success probabilities to SaaS reality. Philosophy: farm cash cows, don't hunt unicorns. Build for revenue, not for sale.

Read `.claude/skills/_shared/philosophy.md` first — all principles apply. Code is cheap. Weight Clarity and Distribution highest in scoring. Dev cost is near zero — discount it in unit economics.

## Sub-Skill Mode (Scoring-Only)

**Invocation:** Standalone via `/bootstrap-oracle` (full pipeline) or as a scoring agent from `/analyze-idea` (scoring-only).

When invoked from `/analyze-idea`:
- **Skip Step 0** — dimension skills already did comprehensive research. Do NOT redo web searches.
- **Receive dimension skill outputs as input** — score based ONLY on this evidence.
- **Skip Step 3** — do NOT produce the full Pitch Deck. The orchestrator writes the final report.
- **Execute Steps 1–2 only** — 5PM Filter, Scoring Sheet, Sanity Gate, Revenue Stairs, 3H/3L.
- **Cite evidence sources** — every score must reference which dimension skill(s) informed it. If evidence is insufficient for a factor, score conservatively and flag the gap.

## Research-First Protocol

**Sub-Skill Mode: SKIP this section and STEP 0 entirely — dimension skills already did the research.**

When running standalone: research autonomously before scoring. See `_shared/philosophy.md` for the full protocol. Key searches: TAM data, competitors, pricing benchmarks, industry trends, recent funding/exits.

## End-to-End Flow

### STEP 0 — RESEARCH PHASE (do this first, silently)

**Sub-Skill Mode: SKIP — go directly to STEP 1.**

Use WebSearch and WebFetch to gather:
- Market size data, growth rates, industry reports
- Named competitors with pricing, features, funding, reviews
- Comparable bootstrapped successes in the space
- Regulatory landscape if relevant
- Search volume / SEO data for core keywords if applicable

### STEP 1 — 5 PM FILTER

Score the idea on five gates using your research. If the pain is not important & urgent or no budget-holder exists, mark **RED** and **STOP**. Only GREEN ideas advance.

| Gate | Question |
|------|----------|
| **P**roblem | Is the pain important AND urgent? |
| **P**urchaser | Does a budget-holder exist who will pay? |
| **P**rice | Will they pay enough to sustain the business? |
| **M**arket | Is the market large enough (≥€10M TAM)? |
| **P**ersonal-fit | Can the founder actually build and run this? |

### STEP 2 — SCORING SHEET

Score 9 factors using the weights below. Composite ≥ 0.85 required, else output **"RETRY"**.

| Factor | Weight | Measurement |
|--------|--------|-------------|
| PMF | 18 | Includes 5PM pass & MPA completion % |
| Clarity | 16 | Does the founder know exactly what to build, for whom, and why they'll pay? Vague = fatal when building is free. |
| Distribution | 16 | Bonus if founder owns ≥5k audience; how will they reach buyers? Product is not the moat. |
| Probability-of-Success (PoS) | 14 | Green: 0.55–0.70; Amber: 0.40–0.55; Red <0.40 |
| Founder-Fit | 12 | Domain insight + market access + clarity of vision. Not "can they code it" — anyone can. Retreat scheduled? Y/N |
| Moat | 10 | Distribution moats, data moats, relationship moats. Most product moats are fake when code is cheap. |
| Scale Path | 5 | Based on Stair-Step clarity |
| Cash-Flow Durability | 5 | Recurring rev quality, retention, revenue compounding |
| Capex/Burn | 4 | Dev cost ≈ 0. Real burn = marketing, distribution, time-to-clarity. ≤€300/mo non-dev burn. |

### STEP 3 — IDEA OUTPUT

Use the Pitch Deck Output Template below.

## 9 Expert Roles

1. **Clarity Analyst** — Does the founder know exactly what to build, for whom, and why they'll pay? Vague vision is fatal when execution is free. Forces specificity.
2. **Distribution Strategist** — How will buyers find this? Owned audience, channels, partnerships. Product is not the moat — reaching customers is.
3. **Moat Engineer** — Injects defensibility (distribution, data, network, relationships, regulation, user-investment lock-in). Most product moats are fake when code is cheap. Evaluates whether usage creates stored value that raises switching costs — if the product can be abandoned with zero loss, there is no moat. See `_shared/philosophy.md` for the lock-in checklist.
4. **Recession Strategist** — Validates durability under tariffs, AI disruption & pullbacks
5. **Competitor Auditor** — Proves gap vs incumbents / GTM edge (USE WEB SEARCH). When code is cheap, expect more competitors faster.
6. **Founder-Fit Analyst** — Domain insight, market access, clarity of vision. NOT "can they code it." ≤20h/wk; checks Quarterly Founder Retreat scheduled
7. **TAM & Pricing Modeler** — Maps path to ≥€1M ARR and €100M TAM; adds TRM (USE WEB SEARCH for data)
8. **Durability Analyst** — Validates long-term compounding potential, recurring revenue durability & cash-flow resilience
9. **Legal Sentinel** — Flags compliance, IP & license issues

## Structural Upgrades

1. **Secret Scale Lever** — "If X works in this niche, it unlocks Y with no extra product work"
2. **Bigger TAM Structure** — Niche TAM ≥€10M; full potential ≥€100M; explicit path
3. **Infrastructure Piggy-Back Test** — What existing workflow/tool do you replace or plug into?
4. **Cash-Flow Durability Score** — Revenue stickiness, retention quality, compounding potential; score 0–1
5. **Revenue Stairs (Stair-Step)** — Stair #1/#2/#3: feature scope + distribution channel + trigger to next stair

## Sanity Gate (all must be YES)

- [ ] Founder can articulate the customer, the pain, and the willingness to pay in one sentence (Clarity Gate)
- [ ] Distribution channel identified — how do buyers find this? (not "build it and they will come")
- [ ] Monthly non-dev burn ≤€300 (marketing, tools, ops — dev cost ≈ 0)
- [ ] Founder time ≤20h/wk
- [ ] At least one named buyer persona
- [ ] Customers already pay for similar outcomes
- [ ] Solves a functionally narrow use-case
- [ ] Expands laterally or vertically post-MVP
- [ ] Validation-First: landing page, waitlist & ≥10 prospect interviews before polishing code (prototype is fine — clarity is the gate)
- [ ] MPA defined & measurable (<15 min to first win)

## Pitch Deck Output Template

```
# [IDEA NAME] — Bootstrap Oracle Analysis

MODEL TYPE: SaaS / Marketplace / DTC / Productised Service / etc.
ACQUISITION TARGET (if any): <name, URL, est. rev>

## THE PROBLEM
WHY THE PAIN IS SEVERE: (3 bullets — quantify € or time loss)
KILLER STAT: <one metric proving urgency — cite source from research>

## THE SOLUTION
What it does, who it's for, how it works.
MPA (Minimum Path to Awesome): <definition, target <15 min>

## WHY NOW
What market shift, regulatory change, or technology inflection makes this viable today.
Cite specific data from research.

## MARKET SIZE (researched)
TAM (source) = ; SAM = ; SOM =
TRM (Total Reachable Market via chosen channels in 24 mo) =
PRICE BAND TEST: ARR if ARPU −20% / +20% =

## COMPETITIVE LANDSCAPE (researched)
COMPETITOR SNAPSHOT (30 words max each):
• Player | price | gap we exploit
[Include at least 3 named competitors from web research]

## CLARITY CHECK
Can the founder articulate in one sentence: who the customer is, what pain they have, and why they'll pay?
What's still unclear? What assumptions need testing before building more?
Prototype-vs-PRD: What's the fastest way to test the core assumption?

## BUSINESS MODEL & UNIT ECONOMICS
ARPU / GM per sale = ; COGS % = ; Payback = months
ARR MATH: Target penetration = ; 24-mo recurring rev =
Revenue Stairs: Stair #1 → #2 → #3
Note: Dev cost ≈ 0 (AI-native). Primary costs = marketing, distribution, founder time.

## UNFAIR ADVANTAGE / MOAT
Distribution moat (how do buyers find you — this is the real moat when code is cheap):
Data/relationship moat (hard to replicate even with AI):
User-investment lock-in: Does usage create stored value (content, data, workflows, configurations)? Does the free tier require users to build things they'd lose by switching? Rate the switching cost flywheel: STRONG (months of investment at risk) / MODERATE (days-weeks of setup) / WEAK (can export and leave in minutes) / NONE (nothing stored).
Secret Scale Lever: "If X works, we unlock Y in [sector/geo] with no extra product work."
Infrastructure Piggy-Back: what existing workflow/tool do we replace or plug into?

## GO-TO-MARKET (this is the real bottleneck)
DISTRIBUTION STRATEGY:
– How do buyers find this? (not "build it and they will come")
– Revenue lever #1
– Revenue lever #2
– CAC channel leverage (SEO/affiliate/paid/partnership)
– Audience ownership: does the founder already have access to buyers?

## FINANCIAL PROJECTIONS
6-MONTH ROADMAP (table: month, deliverable, KPI — include MPA definition & marketing milestones)
Stack / Ops / Supply Chain (40 words max) — assume AI-native development (near-zero dev cost)
Non-dev burn: marketing, tools, ops (€/mo)
Legal Budget: (launch € + yr-1 upkeep €) & main liability

## THE TEAM
Founder-Fit assessment: domain insight, market access, clarity of vision.
NOT "can they build it" — anyone can with AI tools. The question is: do they know what's worth building?
FOUNDER ENERGY SCORE: 0–1 (include date of next Founder Retreat)

## KEY RISKS
KEY RISKS & MITIGATIONS (table — include regulatory & competitive)
PRE-MORTEM (top 3 failure modes, early warning, counter-move)
REALITY CHECK:
• Evidence market is real:
• Proof people pay for similar outcomes:
• What could break this:

## LONG-TERM VALUE & COMPOUNDING
– Revenue compounding path (how does this get better with time?)
– Retention & switching costs (why do customers stay forever?)
  • User-investment lock-in: What do customers build/store on the platform that they'd lose by leaving?
  • Cumulative value: Does the product get MORE valuable the longer they use it? (history, data, trained models, reputation, connections)
  • Team lock-in: Once multiple team members use it, switching requires organizational change, not just individual decision
– Cash-flow durability under stress (recession, competition, AI disruption)
Cash-Flow Durability Score: 0–1

## VERDICT
PROBABILITY OF SUCCESS: <nn%> & 1-line rationale (PoS scale: Green 0.55–0.70; Amber 0.40–0.55; Red <0.40)
COMPOSITE SCORE: <n.nn> (≥0.85 = GO, <0.85 = RETRY)
SANITY GATE: [checklist with Y/N for each]
BOOTSTRAPPER REALITY CHECK: Can this be self-funded to profitability? Y/N

3H / 3L METRIC RADAR:
High Touch / High Intent / High Retention
Low Churn / Low Payback / Low Refunds
```

## Metric Definitions

- **TRM** (Total Reachable Market): Subset of TAM attainable via chosen channels within 24 mo
- **MPA Time-to-Win**: Minutes from sign-up until user experiences core value (goal <15 min)
- **3H Metrics**: Leading indicators (touch, intent, retention)
- **3L Metrics**: Lagging indicators (churn, payback, refunds)
