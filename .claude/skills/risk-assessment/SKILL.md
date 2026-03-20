---
name: risk-assessment
description: Risk matrix and pre-mortem analysis for bootstrapped founders. Produces a pre-mortem exercise, ranked risk matrix (10-15 risks), blind spot detection, and 7-dimension risk assessment with 5 validation gates. Surfaces the risks founders aren't thinking about. Use when user runs `/risk-assessment`, asks about "risks", "what could go wrong", "blind spots", "pre-mortem", "risk analysis", "failure modes", or needs to identify and prioritize threats before committing resources.
---

# Risk Assessment — Risk Matrix & Pre-Mortem for Bootstrappers

Surfaces the risks founders aren't thinking about. Produces a pre-mortem exercise, ranked risk matrix, blind spot analysis, and 7-dimension risk assessment. Designed to be the uncomfortable conversation the founder needs to have with themselves before committing real time and money.

## Philosophy

**Founders are optimists. Optimism builds businesses. Unchecked optimism kills them.** This skill exists to inject structured pessimism into the founder's planning process — not to discourage, but to prepare. The founder who knows their top 3 failure modes and has a mitigation plan is 10x more likely to survive than the one who "figured they'd deal with problems when they come up."

Read `.claude/skills/_shared/philosophy.md` for the full bottleneck shift and bootstrapper framework. For risk assessment specifically:

**The bootstrapper risk profile is different:**
- No safety net. When a VC-backed startup hits a risk, they have 18 months of runway to recover. A bootstrapper has weeks or months.
- Founder risk IS business risk. If the founder burns out, gets sick, or runs out of savings, the business dies. Personal risk is existential.
- Platform risk is amplified. A bootstrapper building on someone else's platform (Shopify, Apple, Google) has no leverage if the rules change.
- Revenue concentration is lethal. Two or three large customers leaving can end a bootstrapped business overnight.
- Speed of kill matters. The best risk mitigation is knowing WHEN to kill the idea, not just what might go wrong.

**What this skill does that founder intuition doesn't:**
- Forces the pre-mortem: "Imagine it's 12 months from now and this business has failed. What happened?"
- Surfaces blind spots: risks the founder literally hasn't considered
- Prioritizes by severity x likelihood: not all risks are equal
- Provides mitigation actions: not just "this could happen" but "here's what to do about it"
- Includes the uncomfortable risks: founder burnout, relationship strain, opportunity cost

## Reference Books

Check `references/INDEX.md` for relevant frameworks. Key books for risk assessment:

- **thinking-in-bets** (Duke) — Probabilistic thinking for risk severity × likelihood scoring; separating decision quality from outcome quality; scenario planning and mental time travel for the pre-mortem exercise; Ulysses contracts for kill criteria
- **only-paranoid-survive** (Grove) — Strategic inflection points as a risk framework; 10x forces that fundamentally change industry dynamics; signal vs. noise for early warning detection; when to let chaos reign vs. rein it in
- **hard-thing** (Horowitz) — Managing through crises when risks materialize; wartime vs. peacetime CEO mindset; the psychology of leadership under pressure; founder team risk patterns
- **innovators-dilemma** (Christensen) — Disruption risk from below; why incumbents fail (resource dependence, value network blindness); technology S-curves for assessing platform and technology risk
- **competitive-strategy** (Porter) — Five Forces as a risk scan framework; industry structure risks (new entrants, substitutes, buyer/supplier power); competitive response patterns for anticipating competitor threats
- **reboot** (Colonna) — Founder psychological risk; burnout patterns; radical self-inquiry for the founder/team risk dimension; the emotional cost of entrepreneurship that doesn't show up in spreadsheets

## Research-First Protocol

Research autonomously before producing the risk assessment. See `_shared/philosophy.md` for the full protocol.

**Key research:**
- "[market/category] startup failures" / "[market/category] business failures" (historical failure patterns)
- "[market/category] regulations" / "[market/category] legal requirements" (regulatory risk)
- "[platform name] policy changes" / "[platform name] developer restrictions" (platform risk)
- "[market/category] trends [current year]" (market trajectory risks)
- "[competitor names] layoffs" / "[competitor names] shutdown" (competitive landscape risks)

**Consume prior intelligence (CRITICAL):** This skill is most powerful after dimension skills have been run. Pull from:
- **problem-analysis**: Weak validation gates, founder-reality gaps, thin evidence
- **competitor-analysis**: Competitive threats, market concentration, funded competitor responses
- **financial-projections**: Cash flow risks, break-even timeline, margin pressure, founder runway
- **gtm-strategy**: Distribution risks, channel dependency, CAC concerns
- **timing-analysis**: Market window risks, regulatory headwinds, too-early/too-late signals
- **moat-analysis**: Defensibility gaps, fake moats, switching cost weaknesses
- **founder-fit**: Execution risks, time constraints, skill gaps, burnout signals
- **business-model**: Revenue model risks, pricing vulnerability, concentration risk
- **solution-analysis**: Substitute threats, AI-substitute test, differentiation reality
- **market-size**: Market shrinkage risks, beachhead viability concerns

## Sub-Skill Mode

See `_shared/philosophy.md` Sub-Skill Mode Protocol. When invoked as a sub-skill, produce both the full report and a digest summary. Note: `/analyze-idea` has its own built-in Risk Synthesis section (Phase 4) that consolidates risk signals from all 10 dimension skills. This skill provides a deeper, standalone risk analysis — it complements the orchestrator's risk synthesis rather than replacing it.

## End-to-End Flow

### STEP 0 — CONTEXT GATHERING

Extract from the user's input:
- The business idea or product (what it does, who it's for)
- Current stage (idea, MVP, live product with customers)
- Founder context (constraints, dependencies, personal situation — if stated)
- Prior skill outputs available in session
- Any risks the founder has already identified

If the idea is too vague to assess risks, ask ONE clarifying question. Otherwise, proceed.

### STEP 1 — PRE-MORTEM EXERCISE

Before structured analysis, run the pre-mortem. This surfaces failure modes that structured frameworks miss.

**Three failure stories:**

1. **Most likely failure** — Given everything you know, what's the most probable way this business dies in 12 months? Write a 3-4 sentence narrative.
2. **Second failure mode** — A different path to failure. Maybe the product succeeds but the business model doesn't. Or distribution works but retention fails. Another 3-4 sentence narrative.
3. **Black swan** — The low-probability, high-impact event. Regulatory change, platform shutdown, market collapse, personal crisis. 2-3 sentences.

### STEP 2 — RISK RESEARCH

Research specific risks for this market and business model:

- Regulatory and legal risks in this category
- Platform dependency risks (if applicable)
- Historical failure patterns in similar businesses
- Competitive response patterns from incumbents
- Technology and infrastructure risks
- Market-level risks (demand shifts, category changes)

### STEP 3 — SEVEN-DIMENSION RISK ASSESSMENT

Assess risk across seven dimensions. For each, identify specific risks, rate severity and likelihood, and provide mitigation strategies.

---

#### Dimension 1: Market Risk

Can the market sustain this business? Could the market change in ways that kill it?

**What to assess:**
- Is demand growing, stable, or shrinking?
- Is this a trend or a fad? What's the evidence?
- Could a technology shift eliminate the need for this product?
- Is the market large enough to sustain a bootstrapped business after competition?
- Could buyer behavior shift away from this solution category?

**Rate: CRITICAL / HIGH / MEDIUM / LOW**

---

#### Dimension 2: Competitive Risk

What happens when competitors notice you and respond?

**What to assess:**
- Can well-funded competitors copy your differentiator in weeks?
- Is there a dominant player who could crush you with a free feature?
- Could a competitor acquire the channel you depend on?
- Are new entrants flooding the market? (Especially AI-built competitors)
- Could competitors engage in predatory pricing you can't match?

**Rate: CRITICAL / HIGH / MEDIUM / LOW**

---

#### Dimension 3: Execution Risk

Can this specific founder/team actually pull this off?

**What to assess:**
- Does the founder have the skills to build AND sell?
- Is the timeline realistic given the founder's availability?
- Are there critical dependencies on other people or partners?
- Is the technical complexity manageable? (AI tools help, but not infinitely)
- Is the founder's execution tempo fast enough for this market?
- Are there signs of common execution anti-patterns? (Polish-as-procrastination, consensus-seeking, feature creep)

**Rate: CRITICAL / HIGH / MEDIUM / LOW**

---

#### Dimension 4: Financial Risk

Can the founder survive long enough for the business to become self-sustaining?

**What to assess:**
- How long can the founder survive with zero revenue? (Runway)
- What's the minimum viable revenue to sustain the founder? (Not the business — the person)
- Are the unit economics healthy or thin? (Margin pressure from day one?)
- Is the cash flow profile dangerous? (Long sales cycles, upfront costs, delayed revenue)
- What happens if growth is 50% slower than planned?
- Is there customer concentration risk? (Revenue from a few large accounts)

**Rate: CRITICAL / HIGH / MEDIUM / LOW**

---

#### Dimension 5: Platform & Technology Risk

Are you building on someone else's foundation that could shift?

**What to assess:**
- Dependency on a platform (Shopify, Apple, Google, Amazon, etc.) — what happens if they change rules, raise fees, or launch a competing feature?
- Dependency on an API or third-party service — what happens if pricing changes or the service shuts down?
- AI model dependency — what happens if the AI model you depend on changes capabilities, pricing, or availability?
- Data risk — could you lose access to data you depend on?
- Infrastructure risk — is your tech stack stable and maintainable?

**Rate: CRITICAL / HIGH / MEDIUM / LOW**

---

#### Dimension 6: Regulatory & Legal Risk

Could regulations help or hurt this business?

**What to assess:**
- Is this industry regulated? Are you compliant?
- Are new regulations coming that could affect operations?
- Are there licensing or certification requirements?
- Data privacy implications (GDPR, CCPA, etc.)?
- Intellectual property risks (patents, trademarks, trade secrets)?
- Could regulatory changes create opportunity OR destroy the market?

**Rate: CRITICAL / HIGH / MEDIUM / LOW**

---

#### Dimension 7: Founder & Team Risk

The most underrated risk category. The founder IS the business.

**What to assess:**
- Burnout risk — is the founder's workload sustainable for 2+ years?
- Key person risk — if the founder can't work for a month, does the business survive?
- Relationship risk — is this business straining personal relationships?
- Opportunity cost — what is the founder giving up to pursue this? Is it worth it?
- Psychological resilience — can the founder handle months of slow growth, rejection, and uncertainty?
- Co-founder risk (if applicable) — is the partnership solid? What happens if it dissolves?

**Rate: CRITICAL / HIGH / MEDIUM / LOW**

---

### STEP 4 — BLIND SPOT DETECTION

Identify 3-5 risks the founder probably isn't thinking about. These are risks that:
- Don't appear in the founder's stated concerns
- Are specific to THIS business/market (not generic startup risks)
- Have real potential to derail the business
- Are often invisible until they hit

Common blind spot categories:
- **Second-order effects**: "If this works, what bad thing happens?" (e.g., success attracts competitors, growth strains support, scaling breaks the model)
- **Dependency chains**: Hidden dependencies that aren't obvious (e.g., your product depends on a free API that could monetize)
- **Personal blind spots**: Risks the founder's personality makes them unlikely to see (e.g., an introvert underestimating the need for sales calls)
- **Market timing risks**: The market could be right but the timing wrong in non-obvious ways
- **Success risks**: What breaks when you succeed? (e.g., support costs spike, infrastructure doesn't scale, the founder becomes the bottleneck)

### STEP 5 — VALIDATION GATES

Five binary checks specific to risk readiness.

| # | Gate | Pass/Fail |
|---|------|-----------|
| 1 | No CRITICAL-severity risks without a mitigation plan | |
| 2 | Founder runway covers at least 6 months of zero revenue | |
| 3 | No single-point-of-failure dependency (platform, customer, or partner) | |
| 4 | Kill criteria defined (founder knows when to stop) | |
| 5 | Top 3 risks have been discussed with someone outside the founder's head (advisor, co-founder, peer) | |

### STEP 6 — OUTPUT

Produce the full report using the template below.

## Output Template

```
# RISK ASSESSMENT: [Product/Idea Name]

Research date: [date]
Stage: [Idea / MVP / Live Product]
Prior analysis consumed: [List skills run in session, or "Standalone"]

---

## PRE-MORTEM

### Most Likely Failure Story
> [3-4 sentences. Write in past tense as if looking back on the failure. "The business failed because..." Make it specific, not generic. This should feel uncomfortable to read because it's plausible.]

### Second Failure Mode
> [3-4 sentences. A different path to failure — maybe the product works but distribution doesn't, or customers come but don't stay, or the market shifts.]

### Black Swan
> [2-3 sentences. The low-probability, high-impact event. Platform shutdown, regulatory ban, personal crisis, market collapse. Unlikely but devastating.]

---

## RISK MATRIX

| # | Risk | Dimension | Severity | Likelihood | Risk Score | Mitigation |
|---|------|-----------|----------|------------|------------|------------|
| 1 | [Specific risk] | [Market/Competitive/Execution/Financial/Platform/Regulatory/Founder] | Critical/High/Medium/Low | High/Medium/Low | [S×L rating] | [Specific action] |
| 2 | | | | | | |
| 3 | | | | | | |
| ... | | | | | | |
| 10-15 | | | | | | |

**Risk scoring:** Critical×High = RED, High×High or Critical×Medium = ORANGE, everything else = YELLOW or GREEN.

**Top 3 risks by risk score:**
1. **[Risk]** — [Why this is #1 and what makes it dangerous]
2. **[Risk]** — [Why this is #2]
3. **[Risk]** — [Why this is #3]

---

## SEVEN-DIMENSION ASSESSMENT

### Dimension 1: Market Risk — [CRITICAL / HIGH / MEDIUM / LOW]

**Key risks identified:**
- [Risk 1 with evidence]
- [Risk 2 with evidence]

**Mitigation strategy:** [Specific actions]

### Dimension 2: Competitive Risk — [CRITICAL / HIGH / MEDIUM / LOW]

**Key risks identified:**
- [Risk 1 with evidence]
- [Risk 2 with evidence]

**Mitigation strategy:** [Specific actions]

### Dimension 3: Execution Risk — [CRITICAL / HIGH / MEDIUM / LOW]

**Key risks identified:**
- [Risk 1 with evidence]
- [Risk 2 with evidence]

**Mitigation strategy:** [Specific actions]

### Dimension 4: Financial Risk — [CRITICAL / HIGH / MEDIUM / LOW]

**Key risks identified:**
- [Risk 1 with evidence]
- [Risk 2 with evidence]

**Mitigation strategy:** [Specific actions]

### Dimension 5: Platform & Technology Risk — [CRITICAL / HIGH / MEDIUM / LOW]

**Key risks identified:**
- [Risk 1 with evidence]
- [Risk 2 with evidence]

**Mitigation strategy:** [Specific actions]

### Dimension 6: Regulatory & Legal Risk — [CRITICAL / HIGH / MEDIUM / LOW]

**Key risks identified:**
- [Risk 1 with evidence]
- [Risk 2 with evidence]

**Mitigation strategy:** [Specific actions]

### Dimension 7: Founder & Team Risk — [CRITICAL / HIGH / MEDIUM / LOW]

**Key risks identified:**
- [Risk 1 with evidence]
- [Risk 2 with evidence]

**Mitigation strategy:** [Specific actions]

**Dimension risk summary:**

| Dimension | Rating | Biggest Risk |
|-----------|--------|-------------|
| Market | [rating] | [one-line] |
| Competitive | [rating] | [one-line] |
| Execution | [rating] | [one-line] |
| Financial | [rating] | [one-line] |
| Platform & Tech | [rating] | [one-line] |
| Regulatory & Legal | [rating] | [one-line] |
| Founder & Team | [rating] | [one-line] |

---

## BLIND SPOTS

Risks the founder probably isn't thinking about:

### Blind Spot 1: [Title]
**The risk:** [2-3 sentences — what could happen and why the founder isn't seeing it]
**Why it's a blind spot:** [What makes this easy to miss]
**Early warning signal:** [What to watch for — the canary in the coal mine]
**Mitigation:** [What to do about it]

### Blind Spot 2: [Title]
[Same structure]

### Blind Spot 3: [Title]
[Same structure]

### Blind Spot 4: [Title — if applicable]
[Same structure]

### Blind Spot 5: [Title — if applicable]
[Same structure]

---

## VALIDATION GATES

| # | Gate | Result | Evidence |
|---|------|--------|---------|
| 1 | No CRITICAL risks without mitigation plan | PASS / FAIL | [Explanation] |
| 2 | Founder runway covers 6+ months of zero revenue | PASS / FAIL / UNKNOWN | [Explanation] |
| 3 | No single-point-of-failure dependency | PASS / FAIL | [What the dependency is] |
| 4 | Kill criteria defined | PASS / FAIL | [Whether founder has clear stop conditions] |
| 5 | Top risks discussed with external advisor | PASS / FAIL / UNKNOWN | [Whether founder has sought outside perspective] |

**Gates passed: X/5**

- **5/5**: Risk-aware and prepared — proceed with confidence
- **3-4/5**: Risks acknowledged but gaps exist — address failing gates before scaling
- **< 3/5**: RED FLAG — significant blind spots or unmitigated risks exist
- **Gate 1 FAIL**: STOP — do not proceed with unmitigated CRITICAL risks

---

## RISK MITIGATION ROADMAP

**Immediate actions (next 7 days):**
1. [Specific action to address the #1 risk]
2. [Specific action to address a blind spot]
3. [Specific action to close a failing validation gate]

**Short-term actions (next 30 days):**
1. [Risk mitigation action with timeline]
2. [Risk mitigation action with timeline]

**Ongoing monitoring:**
| Risk | Early Warning Signal | Check Frequency | Action Trigger |
|------|---------------------|-----------------|----------------|
| [Risk 1] | [What to watch] | [Weekly / Monthly / Quarterly] | [What happens if signal fires] |
| [Risk 2] | [What to watch] | [Frequency] | [Action trigger] |
| [Risk 3] | [What to watch] | [Frequency] | [Action trigger] |

---

## KILL CRITERIA

**Kill this business if:**
1. [Specific, measurable kill signal with timeline — e.g., "Zero paying customers after 90 days of active selling"]
2. [Specific kill signal — e.g., "Primary platform changes policy making this product category impossible"]
3. [Specific kill signal — e.g., "Founder runway drops below 2 months with no revenue trajectory"]
4. [Specific kill signal — e.g., "Three direct competitors launch with better distribution in the same quarter"]

**Remember:** Killing quickly is the bootstrapper's superpower. The VC-backed startup is stuck — they have investors to answer to. You can pivot tomorrow.

---

## BOTTOM LINE

**Overall risk profile:** [LOW / MODERATE / HIGH / CRITICAL]

**What kills this business:** [One sentence — the single most likely failure mode]

**What saves it:** [One sentence — the single most important risk mitigation action]

**The honest answer about risk:** [One sentence — is this founder walking into this with eyes open or wearing rose-colored glasses?]

---
[If invoked as sub-skill: produce DIGEST summary per `_shared/philosophy.md` Digest Mode format]
```

## Important Rules

See `_shared/philosophy.md` Universal Skill Rules.

**Skill-specific rules:**
- **No generic risks** — "The market could change" is not a risk assessment. "Google could add a native quiz feature to Shopify, eliminating the need for third-party quiz apps (similar to how they integrated Google Analytics into Search Console)" is.
- **Every risk needs a mitigation** — identifying a risk without a mitigation is incomplete. If there's no mitigation, say "Accept and monitor" — but be explicit about it.
- **The pre-mortem must be uncomfortable** — if the failure stories feel generic or comfortable, they're not honest enough. The best pre-mortems make the founder say "oh shit, that could actually happen."
- **Blind spots are the value** — the risks the founder already knows about are less dangerous than the ones they don't. Spend extra effort on blind spot detection.
- **Severity × Likelihood, not just severity** — a catastrophic but nearly impossible risk is less important than a moderate but highly likely one. Rank by composite risk score.
- **Founder risk is real risk** — don't skip or soft-pedal Dimension 7. Burnout, relationship strain, and opportunity cost kill more bootstrapped businesses than market forces do.
- **Kill criteria are mandatory** — the plan to STOP is as important as the plan to START. If the founder can't articulate when they'd quit, they're not thinking clearly about risk.
- **This is a Dimension skill** — it follows the dimension skill pattern with 7 assessment dimensions, 5 validation gates, sub-skill mode, and digest mode. It runs standalone or as a post-analysis deep dive. Unlike other dimension skills that use 1-5 numeric ratings, this skill uses CRITICAL/HIGH/MEDIUM/LOW severity ratings — appropriate for risk assessment where relative severity matters more than linear scoring.
- **Consume prior analysis aggressively** — when other skills have been run, every risk they surfaced should appear in the risk matrix. This skill consolidates, doesn't duplicate.
