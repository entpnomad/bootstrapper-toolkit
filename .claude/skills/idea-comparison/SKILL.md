---
name: idea-comparison
description: Side-by-side comparison of 2-4 business ideas on 8 weighted dimensions. Produces a ranked matrix with scores, trade-off analysis, and a clear recommendation of which idea to pursue first. Use when user runs `/idea-comparison`, asks to "compare these ideas", "which idea should I pursue", "rank my ideas", "prioritize between ideas", or has multiple business concepts and needs to choose.
---

# Idea Comparison — Multi-Idea Decision Matrix

Side-by-side scoring of 2-4 business ideas to help founders choose which to pursue first. Not a replacement for deep analysis — a structured prioritization tool that forces honest comparison across the dimensions that matter most to bootstrappers.

## Philosophy

**You can take 50 swings per year. The question is which swing to take first.** When building is cheap, founders often waste months on the wrong idea — not because it's bad, but because a better one was sitting in their notebook. This skill forces the comparison that intuition avoids.

Read `.claude/skills/_shared/philosophy.md` for the full bottleneck shift and bootstrapper framework. For idea comparison specifically:

**Why founders need this:**
- Founders fall in love with ideas. Love is not a scoring methodology.
- "I'll work on all of them" is code for "I'll make progress on none of them"
- The best idea is the one with the fastest path to revenue, not the most exciting vision
- Opportunity cost is the only cost that matters when building is free

**What this skill is NOT:**
- Not a substitute for `/analyze-idea` — run that on the winner
- Not a deep validation tool — it scores on surface-level assessable dimensions
- Not an excuse to skip research — each idea still gets researched before scoring

**The scoring philosophy:**
- Weight distribution access and cash-flow speed highest — these determine bootstrapper survival
- Weight founder fit heavily — the best idea in the wrong founder's hands is the worst idea
- Revenue ceiling matters less than speed to first dollar — you can expand later
- "Effort to test" is a tiebreaker — when ideas score similarly, pursue the one you can validate fastest

## Reference Books

Check `references/INDEX.md` for relevant frameworks. Key books for idea comparison:

- **start-small** (Walling) — Stair-step approach for sequencing ideas by complexity; market-first niche selection criteria; the philosophy that marketing validation comes before code
- **disciplined-entrepreneurship** (Aulet) — Market segmentation matrix for evaluating multiple opportunities; beachhead market selection methodology; 24-step framework for systematic idea assessment
- **thinking-in-bets** (Duke) — Probabilistic decision-making when comparing uncertain options; separating decision quality from outcome quality; avoiding resulting bias when choosing between ideas
- **lean-startup** (Ries) — Validated learning framework for deciding which idea to pursue; build-measure-learn loop for rapid testing; pivot-or-persevere decision criteria
- **crossing-the-chasm** (Moore) — Beachhead segment selection when comparing ideas targeting different adoption stages; whole product concept for assessing effort-to-test

## Research-First Protocol

Research autonomously before scoring. See `_shared/philosophy.md` for the full protocol.

**For each idea, run quick discovery searches:**
- "[idea/market] competitors" / "[idea/market] existing solutions" (market validation)
- "[idea/market] pricing" / "[idea/market] SaaS" (revenue signals)
- "[target customer] frustrations" / "[target customer] complaints" (problem validation)
- "[idea/market] trends [current year]" (market trajectory)

**Consume prior intelligence:** If dimension skills have been run for any of the ideas in this session, use those findings for scoring instead of re-researching. Note which ideas have prior analysis and which are scored from quick research only.

## End-to-End Flow

### STEP 0 — COLLECT IDEAS

Extract from the user's input:
- 2-4 business ideas with enough description to research (what it does, who it's for)
- Founder context (skills, distribution access, constraints, time budget — if stated)
- Any weighting preferences (does the founder value speed? revenue ceiling? passion?)

If fewer than 2 ideas are provided, ask for at least one more. If more than 4 are provided, ask the founder to narrow to their top 4. If descriptions are too vague to compare, ask ONE clarifying question per vague idea.

### STEP 1 — QUICK RESEARCH PER IDEA

For each idea, gather enough intelligence to score the 8 dimensions. This is NOT deep analysis — it's structured first-pass research.

**For each idea:**
- Does the market exist? (Competitors with paying customers?)
- Is the problem real? (People complaining, paying for workarounds?)
- How fast can revenue start? (Pricing signals, transaction complexity)
- Does the founder have distribution access to the target buyer?
- How hard is it to test? (MVP complexity, sales cycle length)
- What's the realistic revenue ceiling for a bootstrapper?
- How competitive is it? (Crowded, moderate, open?)
- Does the founder have relevant domain knowledge or relationships?

### STEP 2 — SCORE ON 8 DIMENSIONS

Score each idea on each dimension using a 1-5 scale. Every score must have a one-sentence justification citing specific evidence.

---

#### Dimension 1: Problem Clarity (Weight: 15%)

How clear and validated is the problem this idea solves?

| Score | Meaning |
|-------|---------|
| 5 | Problem is proven — people pay to solve it today, founder has first-hand evidence |
| 4 | Problem is indicated — complaints, workarounds, competitor revenue visible |
| 3 | Problem is plausible — logical pain, some signals, but limited direct evidence |
| 2 | Problem is assumed — founder believes it exists, no independent validation |
| 1 | Problem is unclear — can't articulate who has this problem or why it's painful |

---

#### Dimension 2: Market Validation (Weight: 15%)

Is there evidence that a market exists with paying customers?

| Score | Meaning |
|-------|---------|
| 5 | Multiple competitors with revenue, growing market, clear demand signals |
| 4 | Some competitors, pricing established, moderate demand evidence |
| 3 | Emerging market, few competitors, demand is plausible but not proven |
| 2 | Very early, no clear competitors, demand signals weak |
| 1 | No evidence of market demand, no competitors, no pricing signals |

---

#### Dimension 3: Distribution Access (Weight: 15%)

Can the founder realistically reach the target buyer?

| Score | Meaning |
|-------|---------|
| 5 | Founder has direct access — existing audience, community presence, warm relationships with buyers |
| 4 | Founder has adjacent access — knows the ecosystem, can reach buyers through 1-2 degrees |
| 3 | Channel exists and is accessible — SEO, marketplace, community — but founder starts from zero |
| 2 | Distribution path is unclear or expensive — requires paid acquisition or outbound sales |
| 1 | No obvious path to buyers — mass market, no clear channel, cold start problem |

---

#### Dimension 4: Cash-Flow Speed (Weight: 15%)

How fast can this idea generate its first dollar of revenue?

| Score | Meaning |
|-------|---------|
| 5 | Revenue within weeks — self-serve purchase, low price point, instant value delivery |
| 4 | Revenue within 1-2 months — short sales cycle, clear pricing, fast onboarding |
| 3 | Revenue within 3-6 months — needs MVP, moderate sales cycle, some setup required |
| 2 | Revenue in 6-12 months — complex product, long sales cycle, significant build needed |
| 1 | Revenue in 12+ months — enterprise sales, regulatory approval, marketplace chicken-and-egg |

---

#### Dimension 5: Founder Fit (Weight: 12%)

How well does this idea match the founder's skills, experience, and situation?

| Score | Meaning |
|-------|---------|
| 5 | Perfect fit — domain expert, relevant network, ideal time/money situation for this business |
| 4 | Strong fit — adjacent expertise, some relevant relationships, manageable constraints |
| 3 | Moderate fit — can learn the domain, no major blockers, but no unfair advantages |
| 2 | Weak fit — outside domain, limited relevant network, significant constraints |
| 1 | Poor fit — wrong founder for this business, critical gaps in knowledge/access/resources |

---

#### Dimension 6: Competition Gap (Weight: 10%)

Is there a viable opening in the competitive landscape?

| Score | Meaning |
|-------|---------|
| 5 | Clear gap — underserved segment, frustrated customers, no quality solution exists |
| 4 | Winnable gap — competitors exist but have exploitable weaknesses (price, UX, niche) |
| 3 | Crowded but differentiation possible — need a strong angle to stand out |
| 2 | Highly competitive — strong incumbents, hard to differentiate, requires heavy investment |
| 1 | Dominated — monopoly/duopoly, or commodity market with no room for differentiation |

---

#### Dimension 7: Revenue Ceiling (Weight: 8%)

What's the realistic revenue cap for a bootstrapped player?

| Score | Meaning |
|-------|---------|
| 5 | $1M+ ARR achievable — large enough market, strong unit economics, expansion paths |
| 4 | $500K-$1M ARR achievable — solid niche, good margins, sustainable |
| 3 | $100K-$500K ARR achievable — viable lifestyle business, limited scale |
| 2 | $50K-$100K ARR ceiling — very niche or commoditized, thin margins |
| 1 | <$50K ARR ceiling — hobby-level revenue, not a business |

---

#### Dimension 8: Effort to Test (Weight: 10%)

How quickly and cheaply can you validate this idea with real customers?

| Score | Meaning |
|-------|---------|
| 5 | Test in days — landing page, manual delivery, existing tools, no code needed |
| 4 | Test in 1-2 weeks — simple MVP, can use no-code/low-code or AI-built prototype |
| 3 | Test in 1-2 months — needs a working product but scope is manageable |
| 2 | Test in 3-6 months — complex product, integrations required, or need a beta group |
| 1 | Test in 6+ months — significant build, regulatory compliance, or infrastructure needed |

---

### STEP 3 — CALCULATE WEIGHTED SCORES

For each idea:
- Multiply each dimension score by its weight
- Sum for composite score (max 5.0)
- Rank ideas by composite score

**Weights:**
| Dimension | Weight |
|-----------|--------|
| Problem Clarity | 15% |
| Market Validation | 15% |
| Distribution Access | 15% |
| Cash-Flow Speed | 15% |
| Founder Fit | 12% |
| Competition Gap | 10% |
| Revenue Ceiling | 8% |
| Effort to Test | 10% |

### STEP 4 — TRADE-OFF ANALYSIS

Beyond the numbers, analyze:
- **Head-to-head matchups** — Where does Idea A beat Idea B and vice versa? Are the trade-offs acceptable?
- **Risk profiles** — Which idea has the most downside risk? Which has the safest floor?
- **Portfolio thinking** — If Idea A fails, does it teach you something that makes Idea B better?
- **Emotional bias check** — Is the founder likely drawn to a lower-scoring idea? Why? Is that signal or noise?
- **Sequencing** — Could you test Idea A first (faster to validate), then pivot to Idea B if it fails?

### STEP 5 — OUTPUT

Produce the full report using the template below.

## Output Template

```
# IDEA COMPARISON: [Brief description of the comparison]

Research date: [date]
Ideas compared: [count]
Prior analysis consumed: [List any dimension skills already run for any idea, or "Standalone"]

---

## COMPARISON MATRIX

| Dimension (Weight) | [Idea 1 Name] | [Idea 2 Name] | [Idea 3 Name] | [Idea 4 Name] |
|---------------------|-------|-------|-------|-------|
| Problem Clarity (15%) | [1-5] — [one-line justification] | [1-5] — [one-line justification] | | |
| Market Validation (15%) | [1-5] — [justification] | [1-5] — [justification] | | |
| Distribution Access (15%) | [1-5] — [justification] | [1-5] — [justification] | | |
| Cash-Flow Speed (15%) | [1-5] — [justification] | [1-5] — [justification] | | |
| Founder Fit (12%) | [1-5] — [justification] | [1-5] — [justification] | | |
| Competition Gap (10%) | [1-5] — [justification] | [1-5] — [justification] | | |
| Revenue Ceiling (8%) | [1-5] — [justification] | [1-5] — [justification] | | |
| Effort to Test (10%) | [1-5] — [justification] | [1-5] — [justification] | | |
| **WEIGHTED SCORE** | **[n.nn]** | **[n.nn]** | | |
| **RANK** | **#[n]** | **#[n]** | | |

---

## IDEA PROFILES

### [Idea 1 Name]
**What it is:** [One-sentence description]
**Target buyer:** [Who pays]
**Revenue model:** [How they pay]
**Strongest dimension:** [Which dimension scored highest and why]
**Weakest dimension:** [Which dimension scored lowest and why]
**Biggest risk:** [The single thing most likely to kill this idea]
**Fastest path to $1K MRR:** [Concrete path description]

### [Idea 2 Name]
[Same structure]

### [Idea 3/4 if applicable]
[Same structure]

---

## HEAD-TO-HEAD ANALYSIS

### [Idea 1] vs. [Idea 2]
**Where [Idea 1] wins:** [Specific dimensions and why]
**Where [Idea 2] wins:** [Specific dimensions and why]
**The decisive factor:** [What tips the balance]

### [Additional matchups if 3+ ideas]

---

## TRADE-OFF ANALYSIS

**Risk profiles:**
| Idea | Upside Potential | Downside Risk | Risk-Adjusted View |
|------|-----------------|---------------|-------------------|
| [Idea 1] | [Best case] | [Worst case] | [Net assessment] |
| [Idea 2] | [Best case] | [Worst case] | [Net assessment] |

**Emotional bias check:**
[Is the founder likely drawn to a specific idea for reasons not captured in the scoring? What's driving that — signal or noise?]

**Sequencing opportunity:**
[Can these ideas be tested sequentially? Would one idea's failure teach something useful for the others? Is there a logical order beyond the scoring?]

---

## SENSITIVITY ANALYSIS

**What would change the ranking:**
| Scenario | New #1 | Why |
|----------|--------|-----|
| If founder has stronger distribution for Idea [N] | [Idea N] | [Explanation] |
| If [market condition] changes | [Idea N] | [Explanation] |
| If founder values [dimension] more than scoring weights suggest | [Idea N] | [Explanation] |

---

## RECOMMENDATION

**PURSUE FIRST: [Idea Name]**

**Why this one:**
[2-3 sentences — the core argument for why this idea should get the founder's time and money first. Focus on the combination of dimensions, not just the highest score.]

**The case against it:**
[1-2 sentences — the strongest argument for NOT pursuing this idea. Intellectual honesty.]

**What to do with the other ideas:**
| Idea | Recommendation |
|------|---------------|
| [Idea 2] | [Pursue second / Park for 6 months / Kill it / Test in parallel if effort is low] |
| [Idea 3] | [Recommendation] |
| [Idea 4] | [Recommendation] |

---

## NEXT STEPS

**For the #1 idea:**
1. [Specific validation action — what to do in the next 7 days]
2. [Specific action — second priority]
3. [Run `/analyze-idea` for full 10-dimension deep analysis]

**Kill criteria:**
[What evidence in the next 30 days would make you switch to Idea #2 instead?]

---

## BOTTOM LINE

[2-3 sentences. Which idea wins, by how much, and what's the confidence level? Is this a clear winner or a close call?]

**The honest answer:** [One sentence — which idea gives this founder the best shot at revenue in the shortest time?]
```

## Important Rules

See `_shared/philosophy.md` Universal Skill Rules.

**Skill-specific rules:**
- **Every score needs a justification** — a bare number is worthless. "Distribution Access: 4 — founder has 2K followers in the target subreddit and moderates a Slack group of 500 marketers" is useful.
- **Research each idea, don't guess** — even quick research beats assumptions. Spend 2-3 searches per idea minimum. Note where evidence is thin.
- **Same depth for every idea** — don't let founder enthusiasm bias research depth. If you research 5 competitors for Idea A, research 5 for Idea B too.
- **Weights are defaults, not gospel** — if the founder explicitly states different priorities (e.g., "I care most about passion/fit"), acknowledge the default ranking AND show what the ranking would be with their preferred weights.
- **Close scores mean close call** — if ideas are within 0.3 points, say so. Don't pretend a 3.72 vs. 3.68 is a clear winner. Surface the tiebreaker.
- **Kill criteria are essential** — the recommendation must include what would trigger switching to the #2 idea. Founders need an exit ramp, not just an on-ramp.
- **This is a Meta skill** — it operates across ideas, not within one. It does NOT produce validation gates or digest mode. The output is a decision framework, not an analysis report.
- **Sequencing matters** — sometimes the answer isn't "pursue the highest scorer" but "test the cheapest-to-validate first." Surface this when relevant.
