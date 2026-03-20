---
name: market-size
description: Evidence-backed market sizing for bootstrapped founders. Use when user runs `/market-size`, asks to "size the market", "how big is the market", "TAM SAM SOM", "market opportunity", "is the market big enough", or needs bottom-up market research with demand validation and revenue ceiling analysis.
---

# Market Size — Evidence-Backed Market Intelligence

Bottom-up market sizing calibrated for bootstrapped reality. We don't need billion-dollar TAMs. We need a niche we can dominate, customers we can reach, and revenue that compounds.

## Philosophy

Read `.claude/skills/_shared/philosophy.md` for the full bottleneck shift and bootstrapper framework. For market sizing specifically:

**Small is beautiful, not a bug.**

A $10M niche you can dominate > a $10B market where you're noise. Bootstrappers don't raise Series A to chase total addressable markets. They find a beachhead, own it, and expand from strength.

**Bottom-up over top-down.** Analyst reports project fantasy numbers for investor decks. We count real customers × real willingness to pay. Top-down is context. Bottom-up is truth.

**TRM (Total Reachable Market) is the key metric.** Not TAM. Not SAM. TRM: the revenue you can actually capture through your channels, with your resources, in 24 months. Everything else is decoration.

**Demand signals outrank analyst projections.** People already paying > people actively searching > analysts predicting. If nobody is paying for alternatives, the market is theoretical. If competitors have revenue, the market is validated.

**AI-native lens: when code is cheap, more competitors enter fast.** Every niche that looks attractive will have 10 new entrants within a year. Speed to beachhead dominance matters more than TAM precision. The market window is the time between when you spot the niche and when it gets crowded.

## Reference Books

Check `references/INDEX.md` for relevant frameworks. Key topics for market sizing: TAM/SAM/SOM methodology and beachhead selection, market sizing exercises and validation frameworks, customer development for bottom-up sizing, adoption lifecycle and chasm crossing, niche selection and stair-step approach, demand validation and willingness-to-pay research.

## Research-First Protocol

Research autonomously before outputting anything. See `_shared/philosophy.md` for the full protocol. Key searches: industry data, competitor pricing, market reports, census data, job postings, community sizes, directories, marketplace listings.

## Sub-Skill Mode

See `_shared/philosophy.md` Sub-Skill Mode Protocol.

## End-to-End Flow

### STEP 0 — CONTEXT GATHERING

Extract from the user's input:
- The business idea (what product/service, who it serves)
- Geographic scope (local, national, global, specific regions)
- Pricing expectations or range (if stated)
- Any known competitors or existing alternatives
- Target customer segment (if stated)

If the idea description is too vague to begin sizing (e.g., just "a SaaS tool"), ask ONE clarifying question. Otherwise, proceed to research.

### STEP 1 — TOP-DOWN RESEARCH (macro context)

Use WebSearch to find industry-level numbers. This provides context, NOT the answer.

**Search queries to run (adapt to the specific market):**
- "[industry/category] market size [current year]"
- "[industry/category] market growth rate CAGR"
- "[industry/category] industry report"
- "[product category] spending trends"
- "[industry] number of businesses/companies/practitioners"

**What to capture:**
- Total industry market size (global, then relevant geography)
- Growth rate (CAGR) and maturity stage
- Key market segments and their relative sizes
- Analyst projections and their assumptions

**Bootstrapper discount:** Apply a 5-10x discount to analyst TAM numbers. Analyst TAMs are built for VC pitch decks — they include adjacent markets, aspirational segments, and enterprise budgets a bootstrapper will never touch. A $5B "market" may have a $50-100M segment relevant to a bootstrapper.

### STEP 2 — BOTTOM-UP ESTIMATION (the real number)

This is the step that matters. Count real things.

**Customer count estimation — find the denominator:**
- Business directories (industry associations, professional directories)
- LinkedIn company/people searches (job titles, industries)
- Government data (census, BLS, SBA, Companies House)
- Job posting volumes for target roles
- Industry association membership numbers
- Marketplace/app store install counts
- Community sizes (subreddits, forums, Slack/Discord groups)
- Conference/event attendance numbers

**Willingness to pay (WTP) — find the numerator:**
- Competitor pricing as primary proxy (what people already pay)
- Adjacent product pricing (what they pay for similar tools)
- Survey data or market research (if available via web search)
- Price elasticity signals (competitor tier distribution, review complaints about pricing)

**Calculate the stack:**

| Metric | How to Calculate |
|--------|-----------------|
| **TAM** | Total potential customers in the category × average annual spend |
| **SAM** | TAM filtered by geography, segment, and product fit |
| **SOM** | SAM filtered by realistic penetration rate (1-5% year 1 for bootstrapper) |
| **TRM** | Customers reachable through YOUR specific channels × YOUR price point × conversion estimate |

**TRM by channel** — break down reachable customers by distribution channel:
- Organic search (keyword volume × CTR × conversion)
- Marketplace (category traffic × listing conversion)
- Content/community (audience size × conversion)
- Outbound (reachable contacts × response rate × close rate)
- Referral (existing customer base × referral rate)
- Paid (budget ÷ CAC)

**Confidence assessment:**
- **High confidence**: Multiple data sources converge, competitor revenue visible, customer count verifiable
- **Medium confidence**: Some data sources available, estimates required for key variables
- **Low confidence**: Mostly estimates, few verifiable data points, novel market

### STEP 3 — BEACHHEAD IDENTIFICATION

Find the single segment to win first. A beachhead must be specific enough to dominate with limited resources.

**Score candidate segments on:**

| Factor | What to Evaluate | Weight |
|--------|-----------------|--------|
| **Pain intensity** | How badly does this segment need a solution? | High |
| **Willingness to pay** | Evidence they already pay for alternatives | High |
| **Reachability** | Can you reach them through channels you have/can build? | High |
| **Word-of-mouth** | Do they talk to each other? (conferences, communities, associations) | Medium |
| **Competition gap** | Are they underserved by current solutions? | Medium |
| **Expansion path** | Does winning here open adjacent segments? | Medium |

**Beachhead must be specific.** Not "small businesses" — "Shopify store owners doing $500K-$2M annual revenue selling physical products in the US." Specific enough to write targeted copy, find them in a directory, and count them.

### STEP 4 — DEMAND SIGNAL VALIDATION

Prove that people already pay for solutions to this problem. Demand signals ranked by strength:

| Signal | Strength | How to Find |
|--------|----------|------------|
| **Competitor revenue** | Strongest | Crunchbase, press releases, podcast interviews, SaaS revenue databases |
| **Marketplace install counts** | Strong | App store listings, plugin directories, Chrome Web Store |
| **Job postings** | Strong | LinkedIn Jobs, Indeed — roles that exist because the problem exists |
| **Search volume** | Medium | Google Trends, keyword research tools |
| **Community complaints** | Medium | Reddit threads, forum posts, review site complaints |
| **Adjacent spending** | Medium | What they currently spend on workarounds (Excel, agencies, manual processes) |
| **Analyst predictions** | Weakest | Market research reports (backward-looking, inflated) |

**Verdict:**
- **VALIDATED** — Multiple strong demand signals, competitors with revenue, customers paying
- **PARTIALLY VALIDATED** — Some signals present but incomplete, or only weak signals
- **UNVALIDATED** — No evidence of paying customers, theoretical demand only

### STEP 5 — MARKET DYNAMICS

Assess the structural characteristics that determine whether this market is good for a bootstrapper.

**Growth trajectory:**
- Emerging (pre-chasm, few competitors, educating market)
- Growing (post-chasm, expanding demand, new entrants)
- Mature (stable, consolidated, growth from share gains)
- Declining (shrinking demand, commoditization)

**Concentration:**
- Fragmented (no player > 10% share) → niche dominance play
- Moderately concentrated (top 3 hold 30-50%) → find underserved edges
- Concentrated (top 3 hold > 60%) → dangerous, need clear differentiation

**Buyer dynamics:**
- Who decides? (individual contributor, manager, executive, committee)
- Sales cycle length (self-serve minutes, days, weeks, quarters)
- Budget source (discretionary, allocated, must-have)
- Switching costs (low = easier to acquire, harder to retain)

**Adoption stage (Technology Adoption Lifecycle):**
- Innovators / early adopters (2.5-16%) — evangelist sales, high tolerance
- Early majority (34%) — pragmatist buyers, need references and whole product
- Late majority (34%) — conservative, need standards and simplicity
- Laggards (16%) — forced adoption only

**Pricing trends:**
- Rising (demand > supply, or increasing value capture)
- Stable (mature, well-understood pricing)
- Declining (commoditization, race to bottom, new free alternatives)

### STEP 6 — REVENUE CEILING ANALYSIS

What's the realistic revenue ceiling for a bootstrapped entrant in this market?

**Three scenarios:**

| Scenario | Assumption | Revenue Model |
|----------|-----------|---------------|
| **Conservative** | Beachhead only, organic channels, slow growth | TRM × low conversion × low price |
| **Base** | Beachhead + 1 adjacent segment, mixed channels | TRM × moderate conversion × mid price |
| **Optimistic** | Multiple segments, strong distribution, premium positioning | SAM × higher penetration × premium price |

**Stair-step compatibility:**
- Can this start as a smaller product (plugin, template, one-time tool) and grow into recurring SaaS?
- Does the market support a stair-step approach? (start simple → add features → expand scope)
- Is there a $1K-$10K MRR product hiding inside a bigger vision?

**Revenue benchmarks for bootstrapped SaaS:**
| Stage | Monthly Revenue | What It Means |
|-------|----------------|---------------|
| Ramen profitable | $3-5K MRR | Covers founder living costs |
| Sustainable solo | $10-20K MRR | Comfortable solo operation |
| Small team viable | $30-80K MRR | Can hire 1-3 people |
| Established | $100-250K MRR | Real business, $1-3M ARR |
| Scale-up ready | $250K+ MRR | Expansion optionality |

**Ceiling verdict:**
- **HIGH CEILING** — Realistic path to $1M+ ARR with bootstrapped resources
- **MODERATE CEILING** — $100K-$1M ARR achievable, good lifestyle or stair-step business
- **LOW CEILING** — <$100K ARR likely, may not justify the effort unless very low maintenance
- **UNCERTAIN** — Not enough data to project with confidence

### STEP 7 — MARKET RISK ASSESSMENT

What can go wrong with this market specifically?

| Risk Category | What to Evaluate |
|--------------|-----------------|
| **Market shrinkage** | Is the market growing or contracting? Could it shrink in 3-5 years? |
| **Commoditization** | Is the product becoming a commodity? Race to free/zero? |
| **Platform dependency** | Does the market depend on a platform you don't control? (Shopify, Google, Apple, AWS) |
| **Regulation** | Are there regulatory changes that could kill or reshape the market? |
| **Cyclicality** | Is demand stable or tied to economic cycles? (recession-proof vs. discretionary) |
| **Winner-take-all dynamics** | Do network effects or data moats favor consolidation? Will one player own 80%? |
| **AI disruption** | Could an AI tool replace the need for this product entirely? |
| **Customer concentration** | Is the market dominated by a few large buyers? (dangerous for bootstrappers) |

### STEP 8 — OUTPUT

Produce the full report using the template below.

## Output Template

```
# MARKET SIZE INTELLIGENCE: [Market/Idea Name]

Research date: [date]
Geography: [scope]
Confidence level: [High / Medium / Low]

---

## BOOTSTRAPPER MARKET VALIDITY

Is this market viable for a bootstrapped entrant?

- [ ] Bottom-up TAM exceeds $10M (enough room for a niche player — if the founder's stated ARR target is under $1M AND the TRM gate passes, this gate can pass at $5M)
- [ ] TRM exceeds $500K ARR (enough reachable revenue to sustain a business)
- [ ] Demand is validated (competitors have revenue, customers are paying)
- [ ] Beachhead segment is identifiable and reachable
- [ ] Revenue ceiling exceeds founder's minimum threshold

Gates passed: [X/5]
If fewer than 3 gates pass: **RED FLAG — market may not support a bootstrapped business.**

---

## MARKET SIZE ESTIMATES

### Top-Down Context

| Metric | Value | Source | Notes |
|--------|-------|--------|-------|
| Global market size | | | |
| Relevant geography | | | |
| CAGR | | | |
| Maturity stage | | | |
| Bootstrapper-adjusted TAM | | | [Global TAM ÷ 5-10x discount] |

⚠️ Top-down numbers are context, not targets. See bottom-up for actionable numbers.

### Bottom-Up Calculation

**Customer count:**
- [Source 1]: [number] potential customers — [how derived]
- [Source 2]: [number] potential customers — [how derived]
- **Estimated total addressable customers**: [number]

**Willingness to pay:**
- Competitor pricing range: $[low]-$[high]/mo
- Median price point: $[X]/mo
- Price band: $[low] (entry) → $[mid] (typical) → $[high] (premium)

**Market size stack:**

| Metric | Customers | × Price | = Annual Revenue |
|--------|-----------|---------|-----------------|
| **TAM** | [total addressable] | $[avg annual] | $[TAM] |
| **SAM** | [serviceable] | $[avg annual] | $[SAM] |
| **SOM** (Year 1) | [obtainable] | $[your price] | $[SOM] |
| **TRM** (24 months) | [reachable] | $[your price] | $[TRM] |

### TRM by Channel

| Channel | Reachable Customers | Conversion Est. | Revenue Potential | Confidence |
|---------|-------------------|----------------|-------------------|------------|
| Organic search | | | | |
| Marketplace | | | | |
| Content/community | | | | |
| Outbound | | | | |
| Referral | | | | |
| Paid | | | | |
| **Total TRM** | | | **$[total]** | |

### Confidence Assessment

**Overall confidence**: [High / Medium / Low]
- What we know: [verified data points]
- What we estimated: [assumptions made]
- What we don't know: [gaps that would change the numbers]

---

## BEACHHEAD MARKET

### Primary Beachhead

**Segment**: [Specific description — not "small businesses" but "US-based Shopify stores doing $500K-$2M in physical product revenue"]

**Beachhead drift**: [ALIGNED / DRIFTED — if drifted, evidence-based segment vs. founder assumption. See _shared/philosophy.md Beachhead Drift section for drift patterns.]

**Why this beachhead:**
- Pain: [specific pain this segment feels]
- WTP: [evidence they pay for solutions]
- Reachability: [how you reach them — channels, communities, directories]
- Size: [count of customers in this specific segment]
- Expansion path: [adjacent segments this opens]

### Segment Evaluation Matrix

| Segment | Pain Intensity | WTP | Reachability | Word-of-Mouth | Competition Gap | Expansion Path | Score |
|---------|---------------|-----|-------------|---------------|----------------|----------------|-------|
| [Beachhead] | | | | | | | |
| [Alternative 1] | | | | | | | |
| [Alternative 2] | | | | | | | |

(Rate each: Strong / Medium / Weak)

### Expansion Path

Beachhead → [Adjacent Segment 1] → [Adjacent Segment 2] → [Broader Market]

[Explain the logic of each expansion step — what you learn, what you build, what credibility you earn]

---

## DEMAND SIGNALS

| Signal | Finding | Strength | Source |
|--------|---------|----------|--------|
| Competitor revenue | | Strongest / Strong / Medium / Weak | |
| Marketplace installs | | | |
| Job postings | | | |
| Search volume | | | |
| Community complaints | | | |
| Adjacent spending | | | |
| Analyst predictions | | | |

**Demand verdict**: VALIDATED / PARTIALLY VALIDATED / UNVALIDATED
[1-2 sentence summary of demand evidence]

---

## MARKET DYNAMICS

**Growth trajectory**: [Emerging / Growing / Mature / Declining] — [evidence]

**Concentration**: [Fragmented / Moderate / Concentrated] — [top players and estimated share]

**Buyer dynamics**:
- Decision maker: [who]
- Sales cycle: [length]
- Budget type: [discretionary / allocated / must-have]
- Switching costs: [low / medium / high]

**Adoption stage**: [Innovators / Early Adopters / Early Majority / Late Majority]
[What this means for GTM approach]

**Pricing trends**: [Rising / Stable / Declining] — [evidence]

---

## REVENUE CEILING ANALYSIS

| Scenario | Customers | Price | MRR | ARR | Assumption |
|----------|-----------|-------|-----|-----|-----------|
| **Conservative** | | | | | |
| **Base** | | | | | |
| **Optimistic** | | | | | |

**Stair-step compatibility**: [Yes / Partial / No]
[Can this start as a simpler product and grow? What's the $5K MRR version?]

**Ceiling verdict**: HIGH CEILING / MODERATE CEILING / LOW CEILING / UNCERTAIN
[1-2 sentence explanation — is this a $100K, $1M, or $10M business for a bootstrapper?]

---

## MARKET RISKS

| # | Risk | Severity | Likelihood | Impact on Bootstrapper |
|---|------|----------|------------|----------------------|
| 1 | | Critical / High / Medium / Low | High / Medium / Low | |
| 2 | | | | |
| 3 | | | | |

**What kills this market for a bootstrapper**: [One sentence — the single most likely market-level failure mode, not execution risk]

---

## PRICE BAND SENSITIVITY TEST

How do the numbers change at different price points?

| Price Point | Addressable Customers | TRM | Competitive Position | Verdict |
|-------------|---------------------|-----|---------------------|---------|
| $[low]/mo | [more customers] | | [undercut everyone] | |
| $[mid]/mo | [baseline] | | [competitive] | |
| $[high]/mo | [fewer customers] | | [premium, needs differentiation] | |

---

## BOTTOM LINE

[2-3 sentence verdict. Is this market viable for a bootstrapper? What's the realistic revenue opportunity? What's the single biggest market risk? What makes this market interesting — or not?]

**Top 3 actions for the next 14 days:**
1. [Specific market validation action with measurable outcome]
2. [Specific market validation action with measurable outcome]
3. [Specific market validation action with measurable outcome]

**The honest answer to "is this market big enough?":** [One sentence]

---
[If invoked as sub-skill: produce DIGEST summary per `_shared/philosophy.md` Digest Mode format]
```

## Important Rules

See `_shared/philosophy.md` Universal Skill Rules.

**Skill-specific rules:**
- **No vanity TAM** — never lead with "This is a $X billion market" without immediately discounting it for bootstrapper reality. Top-down is context, bottom-up is truth.
- **Bottom-up over top-down** — if top-down and bottom-up disagree, trust bottom-up. Explain the gap.
- **TRM is the key metric** — TAM impresses VCs, TRM determines if you eat. Always calculate TRM by channel.
- **Beachhead must be specific** — "SMBs" is not a beachhead. A beachhead has a name, a job title, a company size, a geography, and a channel to reach them.
- **AI-native lens** — when code is cheap, new competitors flood every attractive niche. Factor in market window: how long before 10 copycats appear? Speed to beachhead dominance > TAM precision.
- **Price band sensitivity** — always test the numbers at low/mid/high price points. A market that only works at $99/mo but competitors charge $29/mo is a problem.
- **Demand signals are evidence, not predictions** — "people already pay $X for Y" beats "analysts project $X growth" every time.
- **Cite sources with methodology** — every market number needs a named source: "LinkedIn search shows 45,000 professionals with this title in the US" not "approximately 50K potential customers."
