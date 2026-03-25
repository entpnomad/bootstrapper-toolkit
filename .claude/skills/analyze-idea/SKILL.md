---
name: analyze-idea
description: Orchestrated business idea analysis. Runs 10 dimension skills for deep factual research, applies Bootstrap Oracle scoring with full context, then synthesizes a strategic verdict with Venture Sensei voice. Use when user runs `/analyze-idea`, asks to "analyze this business idea", "full analysis", "comprehensive evaluation", "give me the full picture on this idea", or wants the most thorough business idea critique.
---

# Analyze Idea — Orchestrated Business Critique

Runs a multi-phase analysis of a business idea: first launches 10 dimension skills in parallel for deep factual research, then feeds all outputs to a Bootstrap Oracle scoring pass for structured quantitative judgment, then synthesizes a strategic verdict with Venture Sensei's interpretive voice.

Read `.claude/skills/_shared/philosophy.md` first — all principles apply. Evaluate through the AI-native lens. Weight clarity and distribution highest. Challenge technical moats. Flag execution-avoidance habits as a risk.

## Research-First Principle

Research is distributed across two layers:

1. **Dimension skills** (Phase 2) do deep, specialized research for their domain. They produce comprehensive factual reports.
2. **Oracle scoring pass** (Phase 3) receives all dimension skill outputs. It applies structured scoring frameworks to the factual base — it does NOT redo research.

The orchestrator (Phase 4) does verification research on scoring-vs-evidence mismatches and writes the final synthesis.

All layers should:
- Use WebSearch/WebFetch to find real data — don't ask the user for data you can find
- Form hypotheses and validate them with real data
- Only ask the user when information is truly unknowable (personal skills, budget, time, proprietary insight)
- If critical context is missing and cannot be researched (e.g., "what's your budget?"), ask the user ONCE with all questions bundled together

## Workflow

### Phase 1: Quick Context Check

From the user's input, extract:
- The business idea (what it does, who it's for)
- Any stated constraints (geography, budget, timeline, skills)
- **Idea name slug** — derive a short, descriptive name for the idea (e.g., "ecommerce quiz builder"). Slugify it: lowercase, hyphens for spaces, strip special characters. Build the report folder path: `reports/YYYY-MM-DD_idea-name-slug/` (use today's date). Store this path for Phase 5.

If the idea description is too vague to even begin researching (e.g., just "I want to start a business"), ask ONE clarifying question. Otherwise, proceed to the readiness check.

### Phase 1.5: Readiness Check

Before launching 10 dimension skills, verify the idea has enough substance for a meaningful analysis. Check three gates:

1. **Specificity gate** — Can you extract all three: a specific *customer*, a specific *problem*, and a specific *solution approach*? If only 1 of 3 is present, the idea is too raw for full analysis.
2. **Founder context gate** — Is there enough founder information (time, budget, domain, distribution assets) for `/founder-fit` to produce a meaningful result? If not, bundle the missing questions into ONE ask.
3. **Research viability gate** — Is the idea specific enough that web searches will return meaningful competitor and market data? "AI tool for small businesses" produces noise. "AI-powered menu optimization for independent restaurants" produces signal.

**If the specificity gate fails:**

Do NOT proceed to Phase 2. Instead, output a short redirect:

```
## Not Ready for Full Analysis

**What's missing:** [Which of customer/problem/solution is absent or too vague]

**Run this first:** `/venture-sensei` — describe your idea and let Sensei sharpen the customer, problem, and solution before committing to a 10-dimension deep dive.

**Come back with:** [Specific elements needed — e.g., "A named buyer persona, the specific pain they have today, and what your product does about it"]
```

This saves the founder from a 12-file report full of "UNKNOWN" and "LOW CONFIDENCE" ratings. A helpful redirect beats expensive noise.

**If only the founder context gate fails:** Ask ONE bundled question for the missing context, then proceed.

**If all gates pass:** Proceed to Phase 2.

### Phase 2: Run Dimension Skills in Parallel (research phase)

Launch all dimension skill sub-agents simultaneously. Each produces a comprehensive factual report for its domain.

For each agent: read the skill's SKILL.md, run the full pipeline for this market/idea, and produce the complete report as defined by that skill.

| Agent | Skill Path |
|-------|-----------|
| Competitor Analysis | `.claude/skills/competitor-analysis/SKILL.md` |
| Market Size | `.claude/skills/market-size/SKILL.md` |
| Moat Analysis | `.claude/skills/moat-analysis/SKILL.md` |
| GTM Strategy | `.claude/skills/gtm-strategy/SKILL.md` |
| Problem Analysis | `.claude/skills/problem-analysis/SKILL.md` |
| Business Model | `.claude/skills/business-model/SKILL.md` |
| Financial Projections | `.claude/skills/financial-projections/SKILL.md` |
| Solution Analysis | `.claude/skills/solution-analysis/SKILL.md` |
| Timing Analysis | `.claude/skills/timing-analysis/SKILL.md` |
| Founder Fit | `.claude/skills/founder-fit/SKILL.md` |

### Phase 3: Oracle Scoring Pass (quantitative judgment)

After ALL dimension skills complete, launch a single Bootstrap Oracle scoring agent.

**Agent: Bootstrap Oracle — Scoring Mode**
- Read `.claude/skills/bootstrap-oracle/SKILL.md` — follow the **Sub-Skill Mode (Scoring-Only)** section
- Receive dimension skill **digests** (not full reports) as input context — each dimension skill produces a 200-300 word digest at the end of its full report (see `_shared/philosophy.md` Digest Mode)
- Full reports are saved to disk in Phase 5
- Each digest contains the key ratings, gate results, and findings the Oracle needs for scoring
- Map scoring factor inputs to dimension skill outputs:
  - PMF → Problem Analysis + Solution Analysis
  - Clarity → Problem Analysis + Solution Analysis + Founder Fit
  - Distribution → GTM Strategy + Competitor Analysis
  - Probability of Success → all dimension outputs (holistic)
  - Founder-Fit → Founder Fit
  - Moat → Moat Analysis
  - Scale Path → Business Model + Market Size
  - Cash-Flow Durability → Financial Projections + Business Model
  - Capex/Burn → Financial Projections

### Phase 4: Synthesis & Output (strategic verdict)

The orchestrator writes the final report directly. This phase absorbs Venture Sensei's strategic interpretation role.

Before writing synthesis:
- Read `.claude/skills/venture-sensei/SKILL.md` — absorb the **Persona** section (tone, style, approach, nevers/always), the **Evaluation Framework** (10 scoring dimensions), and the **8 Habits to Break** diagnostic
- Consult `references/INDEX.md` for relevant strategic frameworks
- Review ALL dimension skill outputs and Oracle scoring output

**Signal cross-reference:**
1. Compare Oracle scores against dimension skill evidence — flag mismatches:
   - Where Oracle scored HIGH but dimension evidence is WEAK (potential overscoring)
   - Where Oracle scored LOW but dimension evidence is STRONG (potential underscoring)
2. Surface dimension skill findings that the Oracle scoring did not capture (blind spots in the scoring framework)
3. For any scoring-vs-evidence mismatch, do a quick WebSearch verification and render a verdict

**Synthesis voice — Venture Sensei persona:**

You ARE Venture Sensei writing this report. Not summarizing findings — interpreting them as a battle-tested mentor who has failed, succeeded, and learned hard lessons. The voice must be:

- **Authoritative and direct** — speak from experience, not analysis. "This market is real" not "The data suggests market viability."
- **Blunt when warranted** — "This is a vitamin, not a painkiller. Nobody wakes up at 3am wishing they had this." Don't soften weak findings.
- **Analogies and real-world parallels** over abstract frameworks — "You're building a better mousetrap in a neighborhood with no mice" not "Market-product alignment is suboptimal."
- **Challenge the founder** — if execution habits are suspect, call it. "You've spent more time on this pitch deck than talking to customers. That's the problem."
- **Never sugarcoat, never use jargon** — no "synergies," no "leveraging," no "holistic approach." Say what you mean.
- **Revenue-first, distribution-obsessed** — always bring it back to: who pays, how do they find you, and why can't they leave?

Apply the Sensei's 10-dimension evaluation framework as your strategic lens. Integrate Oracle's quantitative scores into the narrative — don't just cite them, interpret them. Where the 8-habits diagnostic is relevant (founder context available), weave it into the founder fit discussion as direct coaching.

## Output Template

Each dimension section below is a **digest** — key strategic findings from the dimension skill report, not the full report dump.

**Per-dimension enhancements (apply to every dimension section below):**
- **Bold thesis lead-in (blockquote):** If the dimension produced a finding that demands attention, open the section with a single bold blockquote sentence in Venture Sensei voice — the one thing the founder should remember if they read nothing else from that dimension. This is NOT a summary — it's an interpretive punch. Skip the blockquote if the dimension is unremarkable (everything average/fine). Don't force 10 bold sentences in a row.
- **"Do NOT" anti-pattern:** End each dimension section with one `**Do NOT:**` line — the specific trap this founder is most likely to fall into, derived from this dimension's evidence. Must be idea-specific and cite the evidence. Never generic ("don't spend too much"). If no clear anti-pattern exists for a dimension, omit it.

```
# ANALYSIS: [Idea Name]

---

## COMPETITIVE INTELLIGENCE

> **[One bold Sensei-voice sentence — the single most important competitive insight. Example: "You're entering a dogfight with three funded players, but they're all selling to enterprise while ignoring the SMB segment screaming for help on Reddit." Skip this blockquote if findings are unremarkable.]**

- **Competitive landscape validity**: [Gates passed X/5 — strong / viable with gaps / red flag]
- **Red ocean validation**: [Is the market validated? How many competitors with paying customers?]
- **Competitor roster summary**: [Top competitors — name, funding status, pricing, threat level]
- **Positioning map & white space**: [Where competitors cluster, where the gap is]
- **Bootstrapper advantage matrix highlights**: [Top exploitable weaknesses in funded competitors]
- **Strategic wedge & customers to steal first**: [Primary competitive wedge, most vulnerable customer base]
- **Idea-specific gap assessment verdict**: [GAP EXISTS / CROWDED BUT WINNABLE / NO CLEAR GAP — rationale]
- **Do NOT:** [Specific competitive anti-pattern from evidence — e.g., "Compete on features — three funded competitors can out-ship you. Compete on speed-to-value and pricing."]

## MARKET SIZE INTELLIGENCE

> **[Bold Sensei-voice sentence if market findings demand attention. Skip if unremarkable.]**

- **Market validity**: [Gates passed X/5 — viable / marginal / red flag]
- **TAM/SAM/SOM/TRM**: [Bottom-up numbers with confidence level]
- **Beachhead market**: [Primary beachhead segment — who, where, how to reach]
- **Beachhead drift**: [ALIGNED / DRIFTED — if drifted, evidence-based segment vs. founder assumption]
- **Demand signals**: [VALIDATED / PARTIALLY VALIDATED / UNVALIDATED — key evidence]
- **Revenue ceiling**: [HIGH / MODERATE / LOW — realistic ARR range for a bootstrapper]
- **Market risks**: [Top 1-2 market-level risks and what kills this market for a bootstrapper]
- **Do NOT:** [Market-specific anti-pattern — e.g., "Chase the enterprise TAM — your beachhead is freelancers and the numbers work there."]

## MOAT & DEFENSIBILITY INTELLIGENCE

> **[Bold Sensei-voice sentence if defensibility findings demand attention. Skip if unremarkable.]**

- **Defensibility verdict**: [STRONG / MODERATE / WEAK / NO MOAT]
- **Validation gates passed**: [X/5 — list any failing gates]
- **Primary moat**: [The strongest defensibility dimension — what type and why]
- **User-investment lock-in**: [Does usage create stored value? STRONG / MODERATE / WEAK / NONE — what users build/invest on the platform]
- **Fake moats to stop claiming**: [Any claimed advantages that are not real moats]
- **Moat-building priority**: [Top moat opportunity to invest in and timeline]
- **Counter-positioning**: [Is there a structural advantage against incumbents? What can't they copy?]
- **The honest answer**: [One sentence — what actually stops someone from copying this?]
- **Do NOT:** [Defensibility anti-pattern — e.g., "Claim 'AI' as your moat — it's a tool, not a barrier. Your moat is the workflow data users build inside the product."]

## GTM STRATEGY INTELLIGENCE

> **[Bold Sensei-voice sentence if distribution findings demand attention. Skip if unremarkable.]**

- **Distribution verdict**: [CLEAR PATH / PLAUSIBLE / UNCLEAR / BLOCKED]
- **Validation gates passed**: [X/6 — list any failing gates]
- **Beachhead & ICP**: [Primary beachhead segment — who, how to reach]
- **Beachhead drift**: [ALIGNED / DRIFTED — if drifted, evidence-based segment vs. founder assumption]
- **GTM motion**: [Primary motion recommendation — PLG / Content-led / Community-led / Sales-led]
- **Primary channel**: [Inner ring channel — the one that gets 80% of effort]
- **Distribution economics**: [LTV:CAC ratio, payback period — healthy / warning / red flag]
- **Message-market fit**: [LIKELY / NEEDS TESTING / UNLIKELY — key assessment]
- **First 100 plan**: [Core tactic and timeline for first 100 paying customers]
- **Do NOT:** [Distribution anti-pattern — e.g., "Spend on paid ads before you've sold to 10 people manually — you'll burn cash optimizing a message that hasn't been validated."]

## PROBLEM ANALYSIS INTELLIGENCE

> **[Bold Sensei-voice sentence if problem findings demand attention. Skip if unremarkable.]**

- **Problem verdict**: [PROBLEM WORTH SOLVING / NEEDS MORE EVIDENCE / PROBLEM IS WEAK / NO PROBLEM FOUND]
- **Validation gates passed**: [X/6 — list any failing gates]
- **Pain severity**: [HAIR-ON-FIRE / SIGNIFICANT / MODERATE / MILD — key evidence]
- **Willingness to pay**: [PROVEN BUDGET / ADJACENT BUDGET / STATED INTENT / NO EVIDENCE — pricing signals]
- **Buyer persona clarity**: [RAZOR-SHARP / CLEAR / VAGUE / UNKNOWN — who exactly has this problem]
- **Beachhead drift**: [ALIGNED / DRIFTED — if drifted, evidence-based segment vs. founder assumption]
- **Hair-on-fire test**: [ON FIRE / WARM / LUKEWARM / COLD]
- **Founder-vs-reality gap**: [The single biggest divergence between what the founder believes and what evidence shows]
- **Customer language**: [Key phrases real people use to describe this pain — feeds GTM messaging]
- **Do NOT:** [Problem anti-pattern — e.g., "Build for the pain YOU feel — the evidence says your target buyer describes this problem completely differently."]

## FINANCIAL PROJECTIONS INTELLIGENCE

> **[Bold Sensei-voice sentence if financial findings demand attention. Skip if unremarkable.]**

- **Financial verdict**: [FINANCIALLY GROUNDED / VIABLE WITH GAPS / RED FLAG / NOT VIABLE]
- **Validation gates passed**: [X/6 — list any failing gates]
- **Unit economics**: [STRONG / VIABLE / THIN / UNSUSTAINABLE — gross margin, LTV:CAC, payback]
- **Cash-flow profile**: [CASH-POSITIVE / NEUTRAL / CASH-HUNGRY / DANGEROUS — billing strategy impact]
- **Break-even path**: [FAST / REASONABLE / SLOW / UNREACHABLE — three-tier assessment]
- **Revenue stairs**: [CLEAR STAIRS / SOME STAIRS / FLAT / BLOCKED — $0→$1K MRR credibility]
- **Pricing power**: [HIGH / MODERATE / LOW / COMMODITY — ability to raise prices]
- **Stress resilience**: [RESILIENT / ADAPTABLE / FRAGILE / BRITTLE — worst-case survival]
- **Founder sustainability**: [FUNDED / MANAGEABLE / TIGHT / UNSUSTAINABLE — personal runway]
- **Do NOT:** [Financial anti-pattern — e.g., "Price at $9/mo to 'reduce friction' — your margins need $29+ to survive without venture scale."]

## BUSINESS MODEL INTELLIGENCE

> **[Bold Sensei-voice sentence if business model findings demand attention. Skip if unremarkable.]**

- **Business model verdict**: [REVENUE ENGINE SOUND / VIABLE BUT NEEDS TUNING / STRUCTURAL WEAKNESS / BROKEN MODEL]
- **Validation gates passed**: [X/5 — list any failing gates]
- **Revenue model**: [Model type — OPTIMAL / VIABLE / SUBOPTIMAL / MISALIGNED — key rationale]
- **Pricing architecture**: [STRONG / ADEQUATE / UNDERPRICED / BROKEN — competitive positioning]
- **Unit economics**: [PROFITABLE / MARGINAL / UNDERWATER / UNKNOWN — LTV:CAC, payback period]
- **Revenue quality**: [DURABLE / MODERATE / FRAGILE / VOLATILE — recurring vs. one-time, concentration risk]
- **Cash flow dynamics**: [CASH-POSITIVE / NEUTRAL / CASH-HUNGRY / CASH-BURNING — timing and self-funding capacity]
- **Scalability**: [HIGH-LEVERAGE / MODERATE / LINEAR / LABOR-BOUND — marginal cost and founder ceiling]
- **Model risks**: [Top risk to the revenue engine and single point of failure]
- **Do NOT:** [Business model anti-pattern — e.g., "Launch with a freemium tier — your market is too small for freemium math to work. Charge from day one."]

## SOLUTION ANALYSIS INTELLIGENCE

> **[Bold Sensei-voice sentence if solution findings demand attention. Skip if unremarkable.]**

- **Solution verdict**: [BUILD IT / TEST IT / RETHINK IT / STOP]
- **Validation gates passed**: [X/6 — list any failing gates]
- **Value prop clarity**: [RAZOR-SHARP / CLEAR / FUZZY / ABSENT — the value prop in one sentence]
- **Solution-problem fit**: [DIRECT HIT / ADJACENT / TANGENTIAL / MISALIGNED — does this hit the core pain?]
- **MPA**: [SHIP THIS WEEK / MONTH / QUARTER / NEXT YEAR — scope assessment]
- **Differentiation reality**: [STRUCTURAL / MEANINGFUL / COSMETIC / NONE — what actually makes this different]
- **Substitute vulnerability**: [NO VIABLE SUBSTITUTE / EXIST BUT WORSE / ADEQUATE / PREFERRED — AI substitute test result]
- **AI-interface trap**: [PASSES / FAILS — does the product deliver tangible artifacts beyond the conversation itself?]
- **Time-to-value**: [INSTANT / FAST / SLOW / DEFERRED — how fast users get the payoff]
- **Retention & habit potential**: [HABITUAL / REGULAR / EPISODIC / ONE-TIME]
- **Do NOT:** [Solution anti-pattern — e.g., "Build the full platform before testing — ship the manual version to 5 people this week and see if the core value prop holds."]

## TIMING INTELLIGENCE

> **[Bold Sensei-voice sentence if timing findings demand attention. Skip if unremarkable.]**

- **Timing verdict**: [TIMING IS NOW / WINDOW OPEN / TOO EARLY / TOO LATE / TIMING UNCLEAR]
- **Validation gates passed**: [X/5 — list any failing gates]
- **Strategic inflection point**: [INFLECTION IN PROGRESS / EMERGING / INCREMENTAL / NONE — the 10x force]
- **Adoption stage**: [SWEET SPOT / EARLY BUT VIABLE / TOO EARLY / TOO LATE — where on the curve]
- **Market window**: [OPEN 12+ MO / NARROWING 3-12 MO / CLOSING < 3 MO / CLOSED — how long you have]
- **Regulatory catalyst**: [ACTIVE TAILWIND / EMERGING / NEUTRAL / HEADWIND — regulatory forces]
- **Incumbent vulnerability**: [WINDOW OPEN / CRACKING / STABLE / CONSOLIDATING — temporary weakness]
- **Bootstrapper timing fit**: [FAVORS BOOTSTRAPPER / NEUTRAL / FAVORS FUNDED / UNFAVORABLE — does pace work?]
- **The honest answer**: [One sentence — why now and not two years ago or two years from now?]
- **Do NOT:** [Timing anti-pattern — e.g., "Wait for the 'perfect moment' — the window is open now and narrowing. Ship ugly, learn fast."]

## FOUNDER FIT INTELLIGENCE

> **[Bold Sensei-voice sentence if founder fit findings demand attention. Skip if unremarkable.]**

- **Fit verdict**: [STRONG FIT / GOOD FIT / PARTIAL FIT / POOR FIT]
- **Validation gates passed**: [X/7 — list any failing gates]
- **Domain clarity**: [PRACTITIONER / ADJACENT EXPERT / INFORMED OUTSIDER / OUTSIDER — key evidence]
- **Distribution access**: [DIRECT ACCESS / ADJACENT ACCESS / BUILDABLE / NO ACCESS — what assets exist]
- **Execution tempo**: [AI-NATIVE / FAST / MODERATE / SLOW — anti-patterns count X/8]
- **Critical gaps**: [Top 1-2 founder-business mismatches]
- **Asymmetric advantages**: [What this founder has that competing founders lack]
- **The honest answer**: [One sentence — should this founder build this business?]
- **Do NOT:** [Founder fit anti-pattern — e.g., "Outsource distribution to a marketing hire — you have no audience and no relationships in this market. That's your job, not theirs."]

---

## ORACLE SCORING

[Full Oracle scoring output from Phase 3]

### 5PM Filter
| Gate | Verdict | Evidence Source |
|------|---------|----------------|
| Problem | | |
| Purchaser | | |
| Price | | |
| Market | | |
| Personal-fit | | |

### 9-Factor Scoring
| Factor | Weight | Score | Evidence Source |
|--------|--------|-------|----------------|
| PMF | 18 | | |
| Clarity | 16 | | |
| Distribution | 16 | | |
| PoS | 14 | | |
| Founder-Fit | 12 | | |
| Moat | 10 | | |
| Scale Path | 5 | | |
| Cash-Flow Durability | 5 | | |
| Capex/Burn | 4 | | |

**COMPOSITE SCORE:** [n.nn] (≥0.85 = GO, <0.85 = RETRY)
**PROBABILITY OF SUCCESS:** [nn%] (Green 0.55–0.70; Amber 0.40–0.55; Red <0.40)

### Sanity Gate
[checklist with Y/N — cite evidence source for each]

### Revenue Stairs
Stair #1 → #2 → #3

### 3H / 3L Metric Radar
High Touch / High Intent / High Retention
Low Churn / Low Payback / Low Refunds

---

## SIGNAL CROSS-REFERENCE

### High-Confidence Signals
[Findings flagged by 3+ dimension skills — strongest signals in the analysis]

### Scoring vs. Evidence Mismatches
#### Oracle scored HIGH but dimension evidence is WEAK
[Where Oracle gave a generous score but the underlying dimension skill report shows thin evidence — potential overscoring. For each: the factor, Oracle's score, the dimension skill's actual finding, and a one-line verification result]

#### Oracle scored LOW but dimension evidence is STRONG
[Where Oracle penalized a factor but the underlying dimension skill report shows solid evidence — potential underscoring. For each: the factor, Oracle's score, the dimension skill's actual finding, and a one-line verification result]

### Dimension Skill Blind Spots
[Findings from dimension skills that the Oracle scoring framework did not capture.
One subsection per dimension skill where a blind spot exists.
These are insights that fall outside the 9-factor scoring model.]

---

## RISK SYNTHESIS

[Consolidate every risk signal surfaced by dimension skills, Oracle scoring,
and the cross-reference into a single prioritized risk map.
For each risk, note which source(s) flagged it.]

| # | Risk | Source(s) | Severity | Likelihood | Mitigation |
|---|------|-----------|----------|------------|------------|
| 1 | [risk] | [which dimension skill(s) and/or Oracle flagged it] | Critical / High / Medium / Low | High / Medium / Low | [one-line founder action or "none — accept"] |

**Categories to scan across all inputs:**
- **Platform risk** — dependency on a platform you don't control (app store, API, marketplace)
- **Regulatory / legal** — licensing, compliance, data privacy, industry-specific rules
- **Customer concentration** — revenue dependent on few large accounts
- **Distribution fragility** — single-channel dependency, paid-only acquisition
- **Competitive response** — what happens when incumbents notice you
- **Key person / founder risk** — bus factor, burnout, skill gaps
- **Cash-flow timing** — long sales cycles, delayed revenue, upfront costs
- **Financial sustainability** — unit economics, margin pressure, founder runway, break-even timeline
- **Technology risk** — dependency on unstable tech, AI model changes, API deprecation
- **Market risk** — shrinking market, cyclical demand, fad vs. trend
- **Timing risk** — market window closing, adoption stage mismatch, regulatory headwinds, incumbent consolidation
- **Founder-business mismatch** — gaps surfaced by the founder-fit dimension skill

**Rules:**
- Only include risks with real evidence from the analysis — don't pad with generic risks
- If a risk was flagged by 3+ dimension skills, it's Critical by default
- If a risk was flagged by one source and contradicted by another, note the conflict and render a verdict
- End with a plain-language **"What kills this business"** sentence: the single most likely failure mode

---

## RED FLAGS — Do Not Build If...

[3-5 binary, falsifiable statements extracted from dimension skill evidence. Each is a specific condition derived from THIS analysis — not generic advice. Every flag must cite which dimension skill produced the evidence.]

- "[Specific condition in the founder's own situation]" ([Dimension Skill]: [specific finding])
- "[Specific condition]" ([Dimension Skill]: [specific finding])
- "[Specific condition]" ([Dimension Skill]: [specific finding])

**Rules:**
- Every flag must be derived from actual dimension skill evidence, not boilerplate
- Flags like "Don't build if the market is too small" are useless — be specific to this idea
- If a red flag matches the founder's actual situation, bold it and add ⚠️

## GREEN FLAGS — Worth Pursuing If...

[3-5 binary statements showing where evidence is strong. Same format — cite the dimension skill.]

- "[Specific positive signal from the evidence]" ([Dimension Skill]: [specific finding])
- "[Specific positive signal]" ([Dimension Skill]: [specific finding])
- "[Specific positive signal]" ([Dimension Skill]: [specific finding])

---

## STRATEGIC VERDICT

[Venture Sensei voice. Integrate ALL inputs into a single strategic narrative:
- All 10 dimension skill findings — what the evidence actually shows
- Oracle composite score and factor-by-factor breakdown — what the numbers say
- Risk synthesis — what threatens survival
- Scoring-vs-evidence mismatches — where the quantitative model may be wrong
- 8-habits diagnostic (if founder context available) — execution risk assessment
- Sensei evaluation framework dimensions (pain severity, market signals, competitor landscape,
  clarity, distribution, unit economics, founder fit, scalability, risks) as interpretive lens]

**THE VERDICT:**
[GO / NO-GO / CONDITIONAL]
[One paragraph — brutally honest assessment of whether this idea is worth the founder's time and money]

**CONFIDENCE:** [nn%]

**IF CONDITIONAL — what must be true:**
[Numbered list of conditions that would flip this to GO]

**NEXT 7 DAYS — Validation Ladder:**

Derive each step from GTM, Problem Analysis, and Solution Analysis findings. Make every step idea-specific — not generic advice.

1. **MANUAL (Today):** [The thing you can do with zero tools, zero code, zero spend — a conversation, a DM, a manual service delivery. The manual version of THIS specific product.]
   - **Target:** [Specific person, community, subreddit, LinkedIn group — named from the analysis, not abstract]
   - **Success signal:** [What a positive response looks like — be specific]

2. **PROCESSIZED (Day 3-5):** [Take what you learned from #1 and create a lightweight, repeatable version — a landing page, a typeform, a manual-but-scalable process]
   - **Target:** [Expanded circle — from personal network to community to strangers]
   - **Success signal:** [Measurable outcome — signups, replies, payment intent]

3. **PRODUCTIZED (Day 6-7):** [Only if #1 and #2 showed signal — the smallest buildable thing that tests the core value prop]
   - **Target:** [First 5-10 real users]
   - **Success signal:** [Someone pays, or you know exactly why they won't]

---

## WHERE THIS IDEA STANDS

Place this idea on the founder journey based on what the analysis revealed — not where the founder thinks they are:

```
Idea → [Validate Problem] → [Validate Solution] → [First Revenue] → [Growth]
                                    ↑
                               YOU ARE HERE
```

Determine position from dimension skill gate results:
- Problem Analysis gates mostly failing → **Validate Problem** stage
- Problem validated but Solution Analysis gates weak → **Validate Solution** stage
- Both validated but no revenue evidence → **First Revenue** stage
- Revenue exists, scaling questions → **Growth** stage

**Stage:** [Named stage — one sentence explaining why based on gate results]
**What must be true before moving forward:** [1-2 specific conditions from the analysis that gate progression]

## YOUR PATH FORWARD

Sequence 3-4 skills as a journey with prerequisites. Route based on where the analysis is weakest. Each step unlocks the next. Include one "Do NOT run yet" recommendation.

Available skills to route:
- `/user-personas` — Sharpen buyer persona (run when persona is VAGUE or UNKNOWN)
- `/positioning` — Generate messaging and copy (run when persona is clear)
- `/content-strategy` — Distribution plan (run when messaging exists and problem is validated)
- `/launch-plan` — 90-day execution roadmap (run when verdict is GO or CONDITIONAL with clear conditions)
- `/risk-assessment` — Pre-mortem deep dive (run when verdict is CONDITIONAL or risks are underexplored)
- `/idea-comparison` — Compare against alternatives (run when verdict is NO-GO or founder has other ideas)
- `/sanity-check` — Quick decision filter for any remaining questions about this analysis

**Step 1 (Now):** `/[skill]` — [Specific reason tied to the weakest dimension in this analysis]
→ Unlocks: Step 2

**Step 2 (After Step 1):** `/[skill]` — [Why this depends on Step 1 completing]
→ Unlocks: Step 3

**Step 3 (After Step 2):** `/[skill]` — [Final step in the sequence]

**Do NOT run yet:** `/[skill]` — [Specific reason this skill would be premature given current evidence gaps]

**Each skill consumes the analysis already in this session — no need to re-describe the idea. Just run the command.**
```

### Phase 5: Save Reports to Disk

After Phase 4 completes, save all analysis artifacts to the report folder derived in Phase 1.

1. **Create the folder** — `mkdir -p reports/YYYY-MM-DD_idea-name-slug/`
2. **Save each dimension skill report** — Write the full output from each Phase 2 agent as a numbered markdown file:
   | File | Source |
   |------|--------|
   | `01-competitor-analysis.md` | Competitor Analysis agent |
   | `02-market-size.md` | Market Size agent |
   | `03-moat-analysis.md` | Moat Analysis agent |
   | `04-gtm-strategy.md` | GTM Strategy agent |
   | `05-problem-analysis.md` | Problem Analysis agent |
   | `06-business-model.md` | Business Model agent |
   | `07-financial-projections.md` | Financial Projections agent |
   | `08-solution-analysis.md` | Solution Analysis agent |
   | `09-timing-analysis.md` | Timing Analysis agent |
   | `10-founder-fit.md` | Founder Fit agent |
3. **Save Oracle scoring** — Write the full Oracle scoring output from Phase 3 as `11-oracle-scoring.md`
4. **Save the synthesis report** — Write the complete final report (the full output template from Phase 4, including all section digests, Oracle scoring, cross-reference, risk synthesis, and strategic verdict) as `12-synthesis-report.md`
5. **Confirm to the user** — Tell them where reports were saved: `reports/YYYY-MM-DD_idea-name-slug/` with a list of all 12 files

**Rules:**
- Each file should be self-contained markdown — include a top-level heading with the idea name and dimension name
- Save the raw, complete output from each agent/phase — don't truncate or summarize
- If a dimension skill agent failed or returned no output, save the file anyway with a note explaining what happened
- All file writes can be done in parallel since they are independent

## Important

- **Dimension skills run first** — all dimension skills from Phase 2 complete before the Oracle scoring pass starts. This ensures the Oracle scores against comprehensive evidence, not partial data.
- **Oracle does NOT research** — it receives dimension skill outputs and scores against them. Every score must cite which dimension skill(s) informed it.
- **Synthesis absorbs Sensei's voice** — the orchestrator writes the final verdict with Sensei's tone and evaluation framework. No separate Sensei agent is spawned.
- The cross-reference compares **evidence vs. scoring** (dimension skills vs. Oracle) rather than mentor vs. mentor.
- Verdicts must be evidence-backed — scores need sources, not just "sounds right"
- The synthesis must honestly represent mismatches between Oracle scoring and dimension skill evidence
- If Oracle scores below 0.85 (RETRY), the synthesis should still provide the strategic verdict — the founder needs to know what specifically needs to change
- End with concrete next steps, not vague advice
