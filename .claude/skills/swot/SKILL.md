---
name: swot
description: Quick SWOT analysis with bootstrapper lens. Produces a structured strengths/weaknesses/opportunities/threats matrix with evidence, strategic implications, and action priorities. Use when user runs `/swot`, asks for "SWOT analysis", "strengths and weaknesses", "strategic overview", "quick business assessment", or needs a fast strategic snapshot before deeper analysis.
---

# SWOT Analysis — Strategic Snapshot for Bootstrappers

Fast, structured strategic assessment. Produces a usable SWOT matrix with evidence and bootstrapper-specific implications. Gateway tool — run this first for a quick read, then go deep with dimension skills where it matters.

## Philosophy

**SWOT is a lens, not a verdict.** It organizes thinking, surfaces blind spots, and prioritizes where to dig deeper. It does NOT replace the rigor of dimension skills — it's the 20-minute version that tells you where to spend the next 20 hours.

Read `.claude/skills/_shared/philosophy.md` for the full bottleneck shift and bootstrapper framework. For SWOT specifically:

**Bootstrapper SWOT is different from corporate SWOT:**
- Strengths aren't "great team" — they're founder distribution access, domain clarity, cost structure, and speed
- Weaknesses aren't "limited budget" (every bootstrapper has that) — they're specific gaps that block THIS idea
- Opportunities aren't "large TAM" — they're specific market windows, competitor vulnerabilities, and channel openings
- Threats aren't "competition" (competition is validation) — they're platform risk, regulatory change, and market timing

**AI-native reality check:**
- "We can build it" is not a strength (anyone can build it)
- "AI-powered" is not a differentiator (everyone is AI-powered)
- The real strengths are clarity, distribution, relationships, and unfair cost advantages

## Reference Books

Check `references/INDEX.md` for relevant frameworks. Key books for SWOT analysis:

- **competitive-strategy** (Porter) — Five Forces framework for assessing industry threats and opportunities; competitive positioning for strengths/weaknesses assessment
- **good-strategy-bad-strategy** (Rumelt) — Kernel of strategy (diagnosis, guiding policy, coherent action) maps directly to SWOT → strategic implications; distinguishes real strategic insight from buzzword-filled weakness lists
- **blue-ocean-strategy** (Kim & Mauborgne) — Four actions framework (eliminate/reduce/raise/create) for the value curve; useful for identifying opportunities in the strategic implications cross-reference
- **7-powers** (Helmer) — Seven sources of competitive advantage for assessing real strengths vs. claimed strengths; helps classify moat-related items in the S and W quadrants
- **understanding-porter** (Magretta) — Accessible Five Forces reference; competitive advantage (cost vs. differentiation) for quick strength classification

## Research-First Protocol

Research autonomously before producing the SWOT. See `_shared/philosophy.md` for the full protocol.

**Key searches (adapt to the specific idea/market):**
- "[market/category] trends [current year]" (opportunities)
- "[market/category] challenges" / "[market/category] risks" (threats)
- "[competitor names] weaknesses" / "[competitor names] reviews" (competitive landscape)
- "[market/category] regulatory changes" (threat/opportunity signals)
- "[market/category] demand signals" / "[market/category] growth" (market trajectory)

**Consume prior intelligence:** If dimension skills have already been run in this session (competitor-analysis, market-size, problem-analysis, etc.), pull findings from them instead of re-researching. SWOT should synthesize existing intelligence, not duplicate it.

## End-to-End Flow

### STEP 0 — CONTEXT GATHERING

Extract from the user's input:
- The business idea or product (what it does, who it's for)
- Current stage (idea, MVP, live product with customers)
- Founder context (skills, distribution access, constraints — if stated)
- Any specific strategic questions

If the idea description is too vague to assess, ask ONE clarifying question. Otherwise, proceed to research.

### STEP 1 — RESEARCH & INTELLIGENCE GATHERING

Research the market, competitors, and external forces. If prior skill outputs exist in the session, synthesize those instead of re-researching.

**For each SWOT quadrant, gather evidence:**
- **Strengths**: Founder advantages, cost structure, distribution access, domain expertise, speed, existing assets
- **Weaknesses**: Founder gaps, resource constraints, distribution gaps, credibility deficits, execution risks
- **Opportunities**: Market windows, competitor vulnerabilities, technology shifts, regulation changes, underserved segments, channel openings
- **Threats**: Platform dependencies, funded competitor responses, market timing risks, regulatory headwinds, substitute products, AI commoditization

### STEP 2 — SWOT MATRIX CONSTRUCTION

For each quadrant, produce 4-6 items with:
- Specific, evidence-backed finding (not generic)
- Source or basis for the claim
- Relevance to bootstrapper context

**Quality gates per item:**
- Is this specific to THIS idea (not generic to all startups)?
- Is there evidence or reasoning behind it (not just intuition)?
- Would a bootstrapper find this actionable?

### STEP 3 — STRATEGIC IMPLICATIONS

Cross-reference quadrants to derive strategy:
- **Leverage (S+O)**: Strengths that can exploit opportunities — attack here
- **Defend (S+T)**: Strengths that can neutralize threats — protect here
- **Improve (W+O)**: Weaknesses that, if fixed, unlock opportunities — invest here
- **Avoid (W+T)**: Weaknesses exposed to threats — danger zone, mitigate or pivot

### STEP 4 — OUTPUT

Produce the full report using the template below.

## Output Template

```
# SWOT ANALYSIS: [Product/Idea Name]

Research date: [date]
Stage: [Idea / MVP / Live Product]
Prior analysis consumed: [List skills run in session, or "Standalone"]

---

## SWOT MATRIX

### STRENGTHS (Internal — what you have)

| # | Strength | Evidence / Basis | Bootstrapper Relevance |
|---|----------|-----------------|----------------------|
| S1 | [Specific strength] | [Source or reasoning] | [Why this matters for a self-funded business] |
| S2 | | | |
| S3 | | | |
| S4 | | | |
| ... | (add more only if evidence supports — do not pad to fill rows) | | |

### WEAKNESSES (Internal — what you lack)

| # | Weakness | Evidence / Basis | Risk Level |
|---|----------|-----------------|------------|
| W1 | [Specific weakness] | [Source or reasoning] | Critical / High / Medium / Low |
| W2 | | | |
| W3 | | | |
| W4 | | | |
| ... | (add more only if evidence supports — do not pad to fill rows) | | |

### OPPORTUNITIES (External — what's opening up)

| # | Opportunity | Evidence / Basis | Time Window |
|---|------------|-----------------|-------------|
| O1 | [Specific opportunity] | [Source or reasoning] | [Now / 3-6 mo / 6-12 mo / Ongoing] |
| O2 | | | |
| O3 | | | |
| O4 | | | |
| ... | (add more only if evidence supports — do not pad to fill rows) | | |

### THREATS (External — what could hurt you)

| # | Threat | Evidence / Basis | Severity |
|---|--------|-----------------|----------|
| T1 | [Specific threat] | [Source or reasoning] | Critical / High / Medium / Low |
| T2 | | | |
| T3 | | | |
| T4 | | | |
| ... | (add more only if evidence supports — do not pad to fill rows) | | |

---

## STRATEGIC IMPLICATIONS

### LEVERAGE (S + O) — Attack here
[Which strengths let you exploit which opportunities? These are your highest-leverage moves.]

| Strength | Opportunity | Strategic Move |
|----------|------------|----------------|
| S_ | O_ | [Specific action] |
| S_ | O_ | [Specific action] |
| S_ | O_ | [Specific action] |

### DEFEND (S + T) — Protect here
[Which strengths can neutralize which threats? These are your defensive priorities.]

| Strength | Threat | Defense Strategy |
|----------|--------|-----------------|
| S_ | T_ | [Specific action] |
| S_ | T_ | [Specific action] |

### IMPROVE (W + O) — Invest here
[Which weaknesses, if addressed, would unlock which opportunities? These are your development priorities.]

| Weakness | Opportunity | Investment Needed |
|----------|------------|-------------------|
| W_ | O_ | [What to do and estimated effort] |
| W_ | O_ | [What to do and estimated effort] |

### AVOID (W + T) — Danger zone
[Which weaknesses are exposed to which threats? These are existential risks.]

| Weakness | Threat | Mitigation or Pivot |
|----------|--------|---------------------|
| W_ | T_ | [How to mitigate, or whether to avoid entirely] |
| W_ | T_ | [How to mitigate, or whether to avoid entirely] |

---

## PRIORITY ACTIONS

**Top 3 strategic moves (in order of impact):**

1. **[Action]** — [Which S+O or W+O combination this exploits] — [Expected outcome]
2. **[Action]** — [Which combination this addresses] — [Expected outcome]
3. **[Action]** — [Which combination this addresses] — [Expected outcome]

**Top risk to monitor:**
[The single W+T combination that could kill this business, and the early warning signal to watch for]

---

## GO DEEPER

Based on this SWOT, the most valuable deep-dive skills to run next:

| Priority | Skill | Why |
|----------|-------|-----|
| 1 | [/skill-name] | [What this SWOT surfaced that needs deeper investigation] |
| 2 | [/skill-name] | [What this SWOT surfaced that needs deeper investigation] |
| 3 | [/skill-name] | [What this SWOT surfaced that needs deeper investigation] |

Or run `/analyze-idea` for the full 10-dimension analysis.

---

## BOTTOM LINE

[2-3 sentences. What does this SWOT reveal about the strategic position? Is the balance favorable? What's the single most important thing the founder should do next?]

**The honest snapshot:** [One sentence — the real strategic position, unvarnished]
```

## Important Rules

See `_shared/philosophy.md` Universal Skill Rules.

**Skill-specific rules:**
- **Specificity over generality** — "We have a fast development cycle" is useless. "Solo founder can ship MVP in 2 weeks using AI tools, vs. competitor's 50-person engineering team shipping quarterly" is useful. Every item must be specific to THIS idea.
- **Evidence over intuition** — every SWOT item should cite a source, a data point, or a clear reasoning chain. "Large market" is not a strength. "Shopify has 4.6M stores and only 3 quiz apps have >100 reviews" is an opportunity.
- **Bootstrapper lens always** — filter everything through self-funded reality. "Limited budget" is not a weakness worth listing (it's universal). "No existing audience in the target community" is a real weakness.
- **Cross-reference is the value** — the SWOT matrix itself is basic. The strategic implications (S+O, S+T, W+O, W+T) are where the insight lives. Spend more effort on implications than on the matrix.
- **Gateway, not endpoint** — always recommend which dimension skills to run next based on what the SWOT reveals. This skill is most valuable as a starting point.
- **No padding** — if a quadrant only has 3 strong items, don't pad to 6. Quality over quantity. Mark thin quadrants as having limited evidence.
- **This is a Generator skill** — the output is the deliverable. No validation gates, no digest mode. Produce a complete, usable artifact.
