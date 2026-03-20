---
name: financial-projections
description: Financial projections and viability analysis for bootstrapped founders. Assesses revenue model clarity, unit economics, cash-flow profile, break-even path, revenue stairs, AI-native cost structure, pricing power, stress resilience, and founder sustainability. Use when user runs `/financial-projections`, asks about "unit economics", "break-even", "cash flow", "revenue projections", "pricing power", "can I afford this", "runway", "financial viability", "revenue stairs", "cost structure", "profit first", or needs to validate the financial foundation of a business idea.
---

# Financial Projections — Viability for Bootstrappers

Cash is oxygen. This skill forces founders to confront whether the numbers actually work before they build — not VC runway math, but real bootstrapper survival math.

## Philosophy

**Revenue is the only funding round.** There is no Series A safety net. Every dollar the business spends comes from customers or the founder's savings. This changes everything about how you model financials. Bootstrapped financial projections are not about impressing investors with hockey-stick growth curves — they're about answering one question: "Can this business sustain itself and its founder?"

Read `.claude/skills/_shared/philosophy.md` for the full bottleneck shift and bootstrapper framework. For financial projections specifically:

**AI-native cost structure.** When code costs near zero, the traditional SaaS cost stack collapses. No engineering headcount. No $15K/month dev team. The real costs are marketing (CAC), tools & SaaS subscriptions, hosting & infrastructure, API costs (especially AI APIs), and the founder's time. Any financial model that includes "hire 3 developers" in year one is running old math. Recalibrate everything.

**Founder sustainability is the hidden variable.** Every financial model projects the business. Almost none project the founder. How long can the founder personally survive without income from this business? Do they have a partner's salary as a safety net? Do they have dependents? A mortgage? Student loans? The founder's personal financial runway IS the business's runway when there's no outside funding. This skill makes founder sustainability a first-class dimension, not an afterthought.

## Reference Books

Check `references/INDEX.md` for relevant frameworks. Key topics for financial projections: financial keys and profit targets, financial statements and ratio analysis, behavioral cash flow system, margin of safety principles, profit model archetypes, capital allocation, stair-step approach to revenue.

## Research-First Protocol

Research autonomously before outputting anything. See `_shared/philosophy.md` for the full protocol. Key searches:

- "[competitor name] pricing" / "[category] pricing page" / "[category] pricing benchmarks"
- "[category] gross margins" / "[category] SaaS margins" / "[category] COGS"
- "[category] churn rate" / "[category] retention benchmarks"
- "[category] ARPU" / "[category] LTV" / "[category] unit economics"
- "[category] hosting costs" / "[category] infrastructure costs" / "[category] API costs"
- "[category] average contract value" / "[category] pricing trends"
- "SaaS benchmarks [year]" / "bootstrapped SaaS profitability benchmarks"
- If competitor-analysis has already been run, pull pricing tiers and revenue estimates from it
- If market-size has already been run, pull TRM, revenue ceiling, and demand signals from it
- If gtm-strategy has already been run, pull CAC, LTV:CAC, payback period, and distribution economics from it
- If problem-analysis has already been run, pull WTP evidence and pricing signals from it

## Sub-Skill Mode

See `_shared/philosophy.md` Sub-Skill Mode Protocol.

## End-to-End Flow

### STEP 0 — CONTEXT GATHERING

Extract from the user's input:
- The business idea or product (what it does, who it's for)
- Current stage (idea, MVP, live product with revenue)
- Any known pricing (planned or actual)
- Revenue model (subscription, one-time, usage-based, marketplace, etc.)
- Founder's personal financial situation (if shared — savings, dependents, alternative income)
- Any existing financial data (MRR, costs, margins, customer count)

If the idea description is too vague to model financially, ask ONE clarifying question focused on pricing model or revenue structure. Otherwise, proceed to research.

### STEP 1 — FINANCIAL LANDSCAPE RESEARCH

Research the financial benchmarks and competitive pricing for this specific market.

**Search queries to run (adapt to the specific market):**
- What do competitors charge? (Pricing pages, review sites, comparison articles)
- What are industry-standard gross margins for this category?
- What are typical churn rates and customer lifetimes?
- What does hosting/infrastructure cost for this type of product?
- What are API costs if the product relies on third-party APIs (especially AI)?
- What ARPU and LTV benchmarks exist for this category?
- What pricing trends are emerging? (Race to bottom? Premium positioning? Usage-based?)
- What do bootstrapped SaaS companies in this category report for profitability?

**From prior intelligence (if available):**
- competitor-analysis: pricing tiers, funding status, revenue estimates, competitive pricing pressure
- market-size: TRM (Total Realistic Market), revenue ceiling, beachhead size, demand signals
- gtm-strategy: CAC estimates, LTV:CAC ratio, payback period, distribution economics, channel costs
- problem-analysis: WTP evidence, pricing signals, agency/consultant rates, budget holder identity
- moat-analysis: pricing power assessment, switching costs, lock-in potential

### STEP 2 — NINE-DIMENSION FINANCIAL ASSESSMENT

Work through all nine dimensions. For each, assess based on research evidence, rate categorically, and note the specific evidence that supports the rating.

---

#### Dimension 1: Revenue Model Clarity

Is the pricing model defined, testable, and benchmarked against the market?

**What to evaluate:**
- Is there a specific pricing model? (Subscription, per-seat, usage-based, one-time, freemium + paid, marketplace commission)
- Are price points defined? (Not "we'll figure it out" — actual numbers)
- Is the pricing benchmarked against competitors? (Higher, lower, or differently structured — and why?)
- Is the pricing testable? (Can you put up a pricing page and see if people click "buy"?)
- Does the pricing model align with how customers get value? (Per-seat for team tools, usage-based for infrastructure, flat-rate for simplicity)
- Are there expansion revenue paths? (Upsell tiers, add-ons, usage growth, seat growth)

**Revenue model red flags:**
- "We'll monetize later" — no clear path to revenue
- "We'll charge what the market bears" — no pricing research done
- Pricing copied from a funded competitor without considering their subsidy economics
- Usage-based pricing without understanding usage patterns
- Freemium with no clear upgrade trigger

**Rate: DEFINED / SKETCHED / VAGUE / ABSENT**
- DEFINED: Specific pricing tiers, benchmarked against competitors, testable
- SKETCHED: General pricing approach but specifics not finalized
- VAGUE: "We'll charge a subscription" with no numbers
- ABSENT: No revenue model articulated

---

#### Dimension 2: Unit Economics & Margins

Are the per-customer economics sustainable?

**Key metrics to assess:**

| Metric | What It Measures | Healthy (Bootstrapped) |
|--------|-----------------|----------------------|
| **ARPU** | Average revenue per user/month | Depends on market — but must cover CAC |
| **COGS** | Direct cost to serve one customer | Hosting, API calls, support time, third-party tools |
| **Gross margin** | (Revenue - COGS) / Revenue | > 70% for SaaS, > 60% minimum |
| **LTV** | ARPU x gross margin x avg lifetime (months) | > 3x CAC |
| **LTV:CAC** | Lifetime value / acquisition cost | > 3:1 healthy, > 5:1 excellent |
| **Payback period** | CAC / (monthly ARPU x gross margin) | < 6 months for bootstrapped |

**COGS breakdown (AI-native):**
- Hosting/infrastructure per customer
- API costs per customer (AI APIs can be expensive — model this carefully)
- Third-party tool costs per customer
- Support time per customer (founder time has a cost)
- Payment processing fees (2.9% + $0.30 typical)

**What to evaluate:**
- Can you estimate COGS per customer with reasonable confidence?
- Does gross margin exceed 60%? (Below this, SaaS economics don't work for bootstrappers)
- Is LTV:CAC above 3:1? (Below this, growth consumes all profit)
- Is payback period under 6 months? (Bootstrappers can't fund long payback cycles)
- Do unit economics improve with scale? (Hosting gets cheaper per-user, support can be automated)
- Are there hidden costs that increase with usage? (AI API costs, bandwidth, storage)

**Rate: STRONG / VIABLE / THIN / UNSUSTAINABLE**
- STRONG: Gross margin > 70%, LTV:CAC > 5:1, payback < 3 months
- VIABLE: Gross margin > 60%, LTV:CAC > 3:1, payback < 6 months
- THIN: Gross margin 40-60%, LTV:CAC 1-3:1, payback 6-12 months
- UNSUSTAINABLE: Gross margin < 40%, LTV:CAC < 1:1, or payback > 12 months

---

#### Dimension 3: Cash-Flow Profile

When does cash come in vs. when does cash go out? Cash flow timing kills more bootstrapped businesses than lack of profit.

**What to evaluate:**
- Is revenue collected before or after delivering the service?
- Monthly vs. annual billing? (Annual = cash up front, but harder to sell; monthly = steady but slower accumulation)
- Are there upfront costs before first revenue? (Product build time, marketing spend, certifications)
- What's the payment collection cycle? (Credit card = instant; invoicing = 30-90 days)
- Are there seasonal variations in revenue?
- Does the billing model create natural cash reserves?

**Cash-flow patterns:**

| Pattern | Description | Bootstrapper Impact |
|---------|-------------|-------------------|
| **Pre-paid** | Annual contracts, lifetime deals, prepaid credits | Cash-positive early, but creates future delivery obligation |
| **Monthly recurring** | Monthly subscriptions | Predictable but slow to accumulate; cash cushion takes time |
| **Usage-based** | Pay per use, metered billing | Variable and unpredictable; hard to forecast |
| **Transaction-based** | Marketplace commission, per-transaction fee | Scales with volume but volatile |
| **Hybrid** | Monthly base + usage overage | Combines predictability with upside |

**Billing strategy analysis:**
- What's the optimal billing cycle? (Annual discount to get cash early vs. monthly for lower barrier)
- Should there be a prepaid credit system? (Locks in revenue, reduces churn)
- Is there an annual plan incentive? (2 months free for annual = cash in hand + lower churn)

**Rate: CASH-POSITIVE / NEUTRAL / CASH-HUNGRY / DANGEROUS**
- CASH-POSITIVE: Revenue collected before delivery, annual billing, positive working capital
- NEUTRAL: Revenue and costs roughly aligned in timing
- CASH-HUNGRY: Significant upfront costs before revenue, long payment cycles
- DANGEROUS: Costs significantly front-loaded, revenue delayed or uncertain

---

#### Dimension 4: Break-Even Path

How many customers at what price to cover all costs? Three-tier analysis for bootstrapper reality.

**Three-tier break-even (the bootstrapper's honest calculation):**

| Tier | What It Covers | Formula |
|------|---------------|---------|
| **Business-only** | Just the business costs — hosting, tools, marketing, APIs | Monthly fixed costs / (ARPU x gross margin) |
| **Minimum-salary** | Business costs + founder's minimum survivable income | (Fixed costs + minimum salary) / (ARPU x gross margin) |
| **Market-rate** | Business costs + what the founder could earn employed elsewhere | (Fixed costs + market salary) / (ARPU x gross margin) |

**Why three tiers:**
- Business-only break-even tells you when the business sustains itself — but the founder is still unpaid
- Minimum-salary break-even tells you when the founder can stop draining savings — survival mode
- Market-rate break-even tells you when this business is actually worth doing vs. getting a job — opportunity cost threshold

**What to evaluate:**
- What are the monthly fixed costs? (Be exhaustive — hosting, domains, tools, APIs, email, accounting, legal, insurance)
- What's the founder's minimum monthly income requirement? (Rent, food, insurance, loan payments, dependents)
- What could the founder earn as an employee? (This is the opportunity cost baseline)
- How many customers are needed at each tier?
- Is each tier achievable within a reasonable timeframe?
- How does break-even change with pricing changes? (Sensitivity analysis)

**Rate: FAST / REASONABLE / SLOW / UNREACHABLE**
- FAST: Business-only break-even under 50 customers; market-rate under 200
- REASONABLE: Business-only under 200 customers; market-rate under 500
- SLOW: Business-only under 500 customers; market-rate under 1,000
- UNREACHABLE: Business-only requires 500+ customers; market-rate requires 1,000+

---

#### Dimension 5: Revenue Stairs

The stair-step path from $0 to meaningful revenue. Not a hockey stick — a series of deliberate plateaus with specific triggers.

**Revenue stair framework:**

| Stage | MRR Target | What Changes | Trigger to Next Stage |
|-------|-----------|-------------|---------------------|
| **Step 0** | $0 | Pre-revenue — building, validating | First paying customer |
| **Step 1** | $0 → $1K | First customers, manual everything, founder-led sales | Repeatable acquisition channel found |
| **Step 2** | $1K → $5K | Channel producing reliably, product-market fit signals | Expansion revenue or second channel |
| **Step 3** | $5K → $10K | Process maturing, some automation, possible first hire consideration | Operational capacity for growth |
| **Step 4** | $10K → $25K | Multiple channels, compounding growth, operational maturity | Self-sustaining growth engine |
| **Step 5** | $25K → $100K | Scale mode — team growth, infrastructure, expansion | Market expansion or product expansion |

**What to evaluate:**
- For each stair, what specifically needs to happen to climb it?
- What's the expected timeline for each stair?
- What are the bottlenecks at each stair? (Capacity, channel, product, support)
- Where is the "danger zone"? (A stair that requires significant investment to climb without guaranteed return)
- Is the $0 → $1K MRR path concrete? (This is the most important stair — and the least certain)

**Rate: CLEAR STAIRS / SOME STAIRS / FLAT / BLOCKED**
- CLEAR STAIRS: Each step has a defined trigger, realistic timeline, and identified bottleneck
- SOME STAIRS: Some steps are clear but gaps exist (especially $0 → $1K)
- FLAT: Revenue growth model is vague or depends on "things just working"
- BLOCKED: A clear obstacle exists that prevents climbing to the next stair without solving a hard problem first

---

#### Dimension 6: Cost Structure (AI-Native)

What does this business actually cost to run when development cost is near zero?

**AI-native cost stack:**

| Category | Typical Costs | Notes |
|----------|-------------|-------|
| **Marketing & CAC** | Ads, content creation, tools, outreach | Usually the #1 cost for bootstrappers |
| **Hosting & Infrastructure** | Cloud hosting, CDN, database, storage | Scale with usage; model per-customer |
| **API & Third-Party** | AI APIs (OpenAI, Anthropic), payment processing, email, SMS | Can be surprisingly expensive at scale |
| **SaaS Tools** | Analytics, monitoring, support desk, CRM, email marketing | Death by 1,000 subscriptions |
| **Operations** | Accounting, legal, insurance, domain, compliance | Fixed overhead — often underestimated |
| **Founder Time** | Opportunity cost of the founder's hours | The real cost that never shows up on P&L |
| **Contractor/Freelance** | Design, copywriting, specialized tasks | Variable — should be project-based early |

**What NOT in the cost stack (AI-native reality):**
- Full-time developers (code is cheap — founder + AI tools)
- CTO/engineering manager (no engineering team to manage)
- QA team (automated testing + AI-assisted QA)
- DevOps team (managed cloud services)
- Office space (remote by default)

**What to evaluate:**
- What are the actual monthly operating costs? (Be specific, not vague)
- Which costs are fixed vs. variable? (Fixed costs are the survival threshold)
- Which costs scale with customers? (At what rate?)
- Are there any cost cliffs? (e.g., AI API costs that spike with usage)
- Is the cost structure lean enough for a bootstrapper? (Under $500/month fixed is ideal pre-revenue)
- Where is there fat to cut if revenue is slow?

**Rate: LEAN / MODERATE / HEAVY / BLOATED**
- LEAN: Under $500/month fixed costs pre-revenue; variable costs well-understood
- MODERATE: $500-$2,000/month fixed; some variable cost uncertainty
- HEAVY: $2,000-$5,000/month fixed; significant upfront investment required
- BLOATED: Over $5,000/month fixed; cost structure assumes funded company

---

#### Dimension 7: Pricing Power

Can you raise prices? Or are you in a race to the bottom?

**Pricing power sources:**

| Source | What It Means | Strength |
|--------|-------------|----------|
| **Switching costs** | Customers invested too much to leave for a cheaper option | Very high |
| **Unique value** | You solve a problem no one else solves well | High |
| **Brand/trust** | Customers pay for the brand, not just the product | High |
| **Complexity** | Product is complex enough that price comparison is difficult | Moderate |
| **Integration depth** | Product is embedded in workflows, hard to rip out | High |
| **Vertical specialization** | Domain-specific product with no generic substitute | High |
| **Commodity** | Multiple identical alternatives compete on price | None |

**What to evaluate:**
- If you raised prices 20%, how many customers would leave? (Low churn = pricing power)
- Are competitors competing on price? (Price war = no pricing power)
- Is the product differentiated enough to justify premium pricing?
- Do customers compare prices before buying? (Comparison shopping = price-sensitive market)
- Is there willingness-to-pay headroom above current pricing? (Are you leaving money on the table?)
- Can you segment pricing by customer value? (Enterprise pays more than SMB for the same product)

**Rate: HIGH / MODERATE / LOW / COMMODITY**
- HIGH: Product is differentiated, switching costs exist, price is not the primary buying factor
- MODERATE: Some differentiation, but price is a significant factor in buying decision
- LOW: Competitors compete on price, product is not differentiated enough to justify premium
- COMMODITY: Multiple identical alternatives, price is the only differentiator

---

#### Dimension 8: Stress Resilience

What happens when things go wrong? Every financial model looks great in the base case. The real test is the downside scenarios.

**Stress scenarios to model:**

| Scenario | What Happens | Impact |
|----------|-------------|--------|
| **Churn spike** | Monthly churn doubles for 3 months | Revenue contracts, growth stalls |
| **Competitor goes free** | A funded competitor offers a free tier or drops prices 50% | Price pressure, customer loss |
| **Recession** | Customers cut discretionary spend by 30% | Revenue drop, longer sales cycles |
| **Platform change** | Key platform changes API/pricing/rules | Cost increase or feature loss |
| **AI cost spike** | AI API costs increase 3x due to model changes | COGS explodes, margins compress |
| **CAC inflation** | Acquisition costs increase 50% due to competition | Growth slows, unit economics weaken |
| **Key customer loss** | Largest customer churns | Revenue concentration risk |

**What to evaluate:**
- How concentrated is revenue? (If top customer = >20% of revenue, it's fragile)
- What happens to cash flow if growth stops for 3 months? (Can the business survive on existing revenue?)
- What's the minimum revenue to sustain operations? (Below this, the business dies)
- How quickly can costs be cut in a downturn? (Fixed vs. variable cost ratio matters)
- Is there a "survival mode" configuration? (Cut to the bone and keep the lights on)
- What single event would kill this business? (The existential risk)

**Rate: RESILIENT / ADAPTABLE / FRAGILE / BRITTLE**
- RESILIENT: Survives multiple stress scenarios; low fixed costs; diversified revenue
- ADAPTABLE: Survives most scenarios with adjustments; can cut costs quickly
- FRAGILE: One or two scenarios could be fatal; high fixed costs or concentrated revenue
- BRITTLE: Any stress event threatens survival; no margin for error

---

#### Dimension 9: Founder Sustainability

Can the founder survive long enough for the business to work? This is the dimension nobody models — and the one that kills most bootstrapped startups.

**What to evaluate:**
- How many months can the founder live without any business income? (Savings runway)
- Does the founder have alternative income? (Partner's salary, freelance work, investment income)
- What are the founder's monthly personal expenses? (Rent, food, insurance, loans, dependents)
- Does the founder have dependents? (Children, elderly parents, partner without income)
- What's the founder's opportunity cost? (What could they earn employed? This is the real cost of starting up)
- Is the founder's current lifestyle sustainable during the building phase? (Can they cut expenses if needed?)
- Does the founder have a "Plan B" if the business fails? (Employability, savings, safety net)

**Sustainability levels:**

| Level | What It Means | Implication |
|-------|-------------|-------------|
| **FUNDED** | 18+ months of personal runway or alternative income covers expenses | Full focus on the business, no desperation decisions |
| **MANAGEABLE** | 9-18 months of runway or partial alternative income | Must be disciplined about timeline; set clear milestones |
| **TIGHT** | 3-9 months of runway, no alternative income | High pressure; must validate quickly or find interim income |
| **UNSUSTAINABLE** | < 3 months of runway, dependents, no safety net | STOP — do not start a bootstrapped business from this position |

**Rate: FUNDED / MANAGEABLE / TIGHT / UNSUSTAINABLE**

---

### STEP 3 — VALIDATION GATES

Six binary checks. Pass/fail. No nuance.

| # | Gate | Pass/Fail |
|---|------|-----------|
| 1 | Revenue model defined with specific price points | |
| 2 | Gross margin exceeds 60% | |
| 3 | Monthly fixed costs known and documented | |
| 4 | Break-even point is calculable | |
| 5 | Founder can sustain 9+ months without business income | |
| 6 | Path from $0 to $1K MRR is concrete and specific | |

**Gates passed: X/6**

- **6/6**: Financially grounded — proceed with confidence
- **4-5/6**: Viable with blind spots — address the failing gates before committing
- **< 4/6**: RED FLAG — significant financial unknowns
- **< 3/6**: STOP — do the financial homework before building

### STEP 4 — PROFIT-FIRST ALLOCATION PLAN

Apply the behavioral finance principle: Sales - Profit = Expenses. Not Sales - Expenses = Profit. Set aside profit first, then operate on what's left.

**Allocation framework (adapt to stage):**

| Stage | Revenue | Profit | Owner's Pay | Tax | Operating |
|-------|---------|--------|-------------|-----|-----------|
| **Pre-revenue** | $0 | 0% | 0% | 0% | All from savings |
| **$0-$5K MRR** | 100% | 5% | 50% | 15% | 30% |
| **$5K-$25K MRR** | 100% | 10% | 35% | 15% | 40% |
| **$25K-$100K MRR** | 100% | 15% | 25% | 15% | 45% |
| **$100K+ MRR** | 100% | 20% | 20% | 15% | 45% |

**Why this works:** Forces discipline. If operating expenses must fit within the allocation, you naturally keep costs lean. The profit allocation creates a war chest for downturns. The tax allocation prevents the "surprise tax bill" that kills many founders.

### STEP 5 — OUTPUT

Produce the full report using the template below.

## Output Template

```
# FINANCIAL PROJECTIONS: [Product/Idea Name]

Research date: [date]
Stage: [Idea / MVP / Live Product]

---

## FINANCIAL VIABILITY SCORE

Overall verdict: [FINANCIALLY GROUNDED / VIABLE WITH GAPS / RED FLAG / NOT VIABLE]

| Dimension | Rating | Evidence Summary |
|-----------|--------|-----------------|
| Revenue Model Clarity | DEFINED/SKETCHED/VAGUE/ABSENT | |
| Unit Economics & Margins | STRONG/VIABLE/THIN/UNSUSTAINABLE | |
| Cash-Flow Profile | CASH-POSITIVE/NEUTRAL/CASH-HUNGRY/DANGEROUS | |
| Break-Even Path | FAST/REASONABLE/SLOW/UNREACHABLE | |
| Revenue Stairs | CLEAR STAIRS/SOME STAIRS/FLAT/BLOCKED | |
| Cost Structure | LEAN/MODERATE/HEAVY/BLOATED | |
| Pricing Power | HIGH/MODERATE/LOW/COMMODITY | |
| Stress Resilience | RESILIENT/ADAPTABLE/FRAGILE/BRITTLE | |
| Founder Sustainability | FUNDED/MANAGEABLE/TIGHT/UNSUSTAINABLE | |

---

## VALIDATION GATES

| # | Gate | Result |
|---|------|--------|
| 1 | Revenue model defined with specific price points | PASS / FAIL |
| 2 | Gross margin exceeds 60% | PASS / FAIL |
| 3 | Monthly fixed costs known and documented | PASS / FAIL |
| 4 | Break-even point is calculable | PASS / FAIL |
| 5 | Founder can sustain 9+ months without business income | PASS / FAIL |
| 6 | Path from $0 to $1K MRR is concrete and specific | PASS / FAIL |

**Gates passed: X/6** — [Assessment: Financially grounded / Viable with gaps / RED FLAG / STOP]

---

## REVENUE MODEL ASSESSMENT

**Pricing model**: [subscription / per-seat / usage-based / one-time / freemium + paid / marketplace / hybrid]

**Pricing structure:**

| Tier | Price | What's Included | Target Segment |
|------|-------|----------------|----------------|
| [Free / Starter] | $X/mo | [features] | [who] |
| [Pro / Growth] | $X/mo | [features] | [who] |
| [Enterprise / Scale] | $X/mo | [features] | [who] |

**Competitor pricing comparison:**

| Competitor | Pricing Model | Price Range | Positioning |
|-----------|--------------|-------------|-------------|
| [Competitor 1] | [model] | [range] | [premium/mid/budget] |
| [Competitor 2] | | | |
| [Competitor 3] | | | |

**Revenue model verdict**: [DEFINED / SKETCHED / VAGUE / ABSENT]
[2-3 sentences on whether the pricing model is testable and benchmarked]

**Expansion revenue paths**: [Upsell triggers, add-ons, usage growth, seat expansion — or none identified]

---

## UNIT ECONOMICS

**Per-customer economics:**

| Metric | Estimate | Benchmark | Verdict |
|--------|---------|-----------|---------|
| ARPU (monthly) | $X | $X (industry) | |
| COGS per customer | $X | | |
| Gross margin | X% | X% (industry) | |
| Estimated CAC | $X | | |
| LTV (12-month) | $X | | |
| LTV:CAC | X:1 | 3:1 (minimum) | Healthy / Warning / Red flag |
| Payback period | X months | < 6 months | Healthy / Warning / Red flag |

**COGS breakdown:**

| Cost Component | $/Customer/Month | % of ARPU | Notes |
|---------------|-----------------|-----------|-------|
| Hosting/infrastructure | | | |
| API costs (AI, etc.) | | | |
| Third-party tools | | | |
| Payment processing | | | |
| Support (founder time) | | | |
| **Total COGS** | | | |

**Unit economics verdict**: [STRONG / VIABLE / THIN / UNSUSTAINABLE]
[2-3 sentences on the sustainability of per-customer economics]

---

## CASH-FLOW PROFILE

**Billing strategy:**
- Primary billing cycle: [monthly / annual / usage-based]
- Annual discount offered: [Y/N — X months free for annual]
- Payment collection: [credit card / invoice / prepaid credits]
- Cash-flow timing: [cash before delivery / cash at delivery / cash after delivery]

**Cash-flow analysis:**
- When does cash come in relative to when costs are incurred?
- What's the working capital requirement? (Cash needed to operate before revenue covers costs)
- Is there a seasonal pattern to revenue?
- What's the billing model's impact on churn? (Annual = lower churn, monthly = higher but more flexible)

**Cash-flow verdict**: [CASH-POSITIVE / NEUTRAL / CASH-HUNGRY / DANGEROUS]
[2-3 sentences on cash flow timing and working capital needs]

---

## BREAK-EVEN ANALYSIS

**Monthly fixed costs:**

| Category | Monthly Cost |
|----------|-------------|
| Hosting & infrastructure | $X |
| SaaS tools & subscriptions | $X |
| Marketing / CAC budget | $X |
| Domain, email, misc. | $X |
| Accounting / legal | $X |
| Insurance | $X |
| **Total fixed costs** | $X |

**Three-tier break-even:**

| Tier | Monthly Target | Customers Needed | Timeline Estimate |
|------|---------------|-----------------|-------------------|
| **Business-only** | $X (covers fixed costs) | X customers | X months |
| **Minimum-salary** | $X (fixed + $X founder min.) | X customers | X months |
| **Market-rate** | $X (fixed + $X market salary) | X customers | X months |

**Sensitivity analysis:**
- If ARPU is 20% lower: business-only break-even = X customers
- If ARPU is 20% higher: business-only break-even = X customers
- If churn is 2x expected: monthly net growth = X customers/month

**Break-even verdict**: [FAST / REASONABLE / SLOW / UNREACHABLE]
[2-3 sentences on the realism of the break-even path]

---

## REVENUE STAIRS

| Stage | MRR Range | Key Challenge | Trigger to Next | Timeline |
|-------|-----------|--------------|-----------------|----------|
| Step 0 → 1 | $0 → $1K | [challenge] | [trigger] | [estimate] |
| Step 1 → 2 | $1K → $5K | [challenge] | [trigger] | [estimate] |
| Step 2 → 3 | $5K → $10K | [challenge] | [trigger] | [estimate] |
| Step 3 → 4 | $10K → $25K | [challenge] | [trigger] | [estimate] |
| Step 4 → 5 | $25K → $100K | [challenge] | [trigger] | [estimate] |

**The $0 → $1K MRR plan:**
[Specific, concrete tactics. This is the most critical stair and must be detailed:
- How will you get the first 10 customers?
- At what price point?
- Through which channel?
- In what timeframe?]

**Revenue stairs verdict**: [CLEAR STAIRS / SOME STAIRS / FLAT / BLOCKED]
[2-3 sentences on the credibility of the growth path]

---

## AI-NATIVE COST STACK

**Monthly operating costs (pre-revenue / early stage):**

| Category | Monthly Cost | Fixed/Variable | Notes |
|----------|-------------|---------------|-------|
| Hosting & infrastructure | $X | Variable | [scales how?] |
| AI API costs | $X | Variable | [per-request pricing, expected volume] |
| SaaS tools | $X | Fixed | [list key tools] |
| Marketing / CAC | $X | Variable | [budget allocation] |
| Domain, DNS, email | $X | Fixed | |
| Payment processing | $X | Variable | [% of revenue] |
| Accounting / bookkeeping | $X | Fixed | |
| Legal / compliance | $X | Fixed/One-time | |
| Insurance | $X | Fixed | |
| **Total monthly burn** | **$X** | | |

**What's NOT in this cost stack** (AI-native):
- Full-time developers: [N/A — founder + AI tools]
- Office space: [N/A — remote]
- [Other traditional costs eliminated by AI-native approach]

**Cost trajectory:**
- Pre-revenue monthly burn: $X
- At 100 customers: $X/month
- At 500 customers: $X/month
- At 1,000 customers: $X/month

**Cost structure verdict**: [LEAN / MODERATE / HEAVY / BLOATED]

---

## PRICING POWER ASSESSMENT

**Pricing power sources:**

| Source | Present? | Strength | Evidence |
|--------|---------|----------|---------|
| Switching costs | Y/N | Strong/Moderate/Weak | |
| Unique value | Y/N | | |
| Brand/trust | Y/N | | |
| Integration depth | Y/N | | |
| Vertical specialization | Y/N | | |
| Complexity barrier | Y/N | | |

**Price sensitivity indicators:**
- Do customers compare prices before buying? [Y/N — evidence]
- Are competitors competing on price? [Y/N — evidence]
- Is there WTP headroom above current/planned pricing? [Y/N — how much?]
- Can you segment pricing? (Different prices for different customer types)

**Pricing power verdict**: [HIGH / MODERATE / LOW / COMMODITY]
[2-3 sentences on ability to maintain or raise prices over time]

---

## STRESS TEST RESULTS

| Scenario | Revenue Impact | Cash Survival | Recovery Plan |
|----------|---------------|---------------|---------------|
| Churn doubles (3 months) | -X% revenue | X months | |
| Competitor goes free | -X% customers | X months | |
| Recession (-30% spend) | -X% revenue | X months | |
| Platform change | +$X/mo costs | X months | |
| AI API costs 3x | +$X/mo COGS | X months | |
| CAC increases 50% | -X% growth | X months | |

**Survival mode configuration:**
- Minimum revenue to keep lights on: $X/month
- Costs that can be cut immediately: $X/month
- Costs that are truly fixed (can't cut without shutting down): $X/month

**Stress resilience verdict**: [RESILIENT / ADAPTABLE / FRAGILE / BRITTLE]
[2-3 sentences on the business's ability to survive downside scenarios]

---

## FOUNDER SUSTAINABILITY

**Personal financial assessment:**

| Factor | Status | Notes |
|--------|--------|-------|
| Monthly personal expenses | $X | [rent, food, insurance, loans, dependents] |
| Savings runway | X months | [total savings / monthly expenses] |
| Alternative income | $X/month | [partner salary, freelance, investments, none] |
| Dependents | X | [children, elderly parents, partner] |
| Opportunity cost (market salary) | $X/year | [what they'd earn employed] |
| Health insurance | [covered / uncovered] | [employer plan, ACA, partner's plan, none] |

**Founder runway calculation:**
- Monthly burn (personal): $X
- Alternative income offset: $X
- Net monthly drain on savings: $X
- Months until must earn from business: X months

**Founder sustainability verdict**: [FUNDED / MANAGEABLE / TIGHT / UNSUSTAINABLE]
[2-3 sentences on the founder's ability to sustain through the building phase]

---

## PROFIT-FIRST ALLOCATION PLAN

**Current/target stage allocation:**

| Category | % of Revenue | Monthly Amount (at $X MRR) |
|----------|-------------|---------------------------|
| Profit (set aside first) | X% | $X |
| Owner's pay | X% | $X |
| Tax reserve | X% | $X |
| Operating expenses | X% | $X |

**When does the business start paying the founder?**
[Specific MRR milestone where owner's pay becomes meaningful]

**When does profit allocation become meaningful?**
[Specific MRR milestone where the profit reserve creates a real buffer]

---

## 24-MONTH PROJECTION

**For idea-stage businesses:** This projection is directional, not predictive. Flag every cell as assumption-based. The value is in stress-testing the assumptions, not in the specific numbers. Projection confidence should default to LOW unless the founder has prior data from a related business.

**Assumptions (state explicitly):**
- Monthly customer growth rate: X% (conservative) / X% (base) / X% (optimistic)
- Monthly churn rate: X%
- ARPU: $X (assumed flat / growing X% annually)
- Monthly operating costs: $X growing to $X

| Month | Customers (C/B/O) | MRR (C/B/O) | Costs | Net (C/B/O) |
|-------|-------------------|-------------|-------|-------------|
| 3 | X / X / X | $X / $X / $X | $X | $X / $X / $X |
| 6 | | | | |
| 9 | | | | |
| 12 | | | | |
| 18 | | | | |
| 24 | | | | |

*(C = Conservative, B = Base, O = Optimistic)*

**Key milestones in the projection:**
- Business-only break-even: Month X (conservative) / Month X (base)
- Founder minimum salary: Month X (conservative) / Month X (base)
- Market-rate salary: Month X (conservative) / Month X (base)
- $10K MRR: Month X (conservative) / Month X (base)

**Assumption sensitivity:**
- If churn is 2x assumed: break-even pushed to Month X
- If ARPU is 20% lower: break-even pushed to Month X
- If growth is 50% slower: break-even pushed to Month X

**Projection confidence**: [HIGH / MODERATE / LOW]
[One sentence on what makes these projections credible or speculative]

---

## BOTTOM LINE

**Financial verdict**: [FINANCIALLY GROUNDED / VIABLE WITH GAPS / RED FLAG / NOT VIABLE]

[2-3 sentences. Do the numbers work for a bootstrapped business? What's the strongest financial signal? What's the biggest financial risk? If the numbers don't work, what would need to change to make them work?]

**The honest answers:**

- **"Can this business sustain itself?"** [One sentence — based on unit economics and break-even]
- **"Can this business sustain its founder?"** [One sentence — based on founder sustainability and revenue stairs]
- **"What kills this financially?"** [One sentence — the single most likely financial failure mode]

**Top 3 actions for the next 30 days:**
1. [Specific, concrete, actionable — focused on the weakest financial dimension]
2. [Specific, concrete, actionable]
3. [Specific, concrete, actionable]

---
[If invoked as sub-skill: produce DIGEST summary per `_shared/philosophy.md` Digest Mode format]
```

## Important Rules

See `_shared/philosophy.md` Universal Skill Rules.

**Skill-specific rules:**
- **AI-native cost structure** — never include engineering headcount, office space, or traditional dev team costs. The real costs are marketing, tools, hosting, APIs, and founder time. If you catch yourself writing "hire a developer," stop.
- **Founder sustainability is non-negotiable** — always assess the founder's personal financial position. If the founder can't survive 9 months without income, that's a red flag regardless of how good the business economics look.
- **Cash flow > profitability** — a profitable business with bad cash flow timing dies. Assess when cash comes in vs. when it goes out. Annual billing, prepaid credits, and collected-before-delivered models are survival mechanisms.
- **No vanity projections** — hockey-stick growth curves are for VC pitch decks. Use conservative, base, and optimistic scenarios. State all assumptions explicitly. If a projection requires >10% MoM growth sustained for 24 months, flag it as unrealistic.
- **Stress test everything** — every financial model looks great in the base case. Model what happens when churn doubles, a competitor goes free, or AI API costs spike.
- **Gross margin floor** — if gross margin is below 60%, say so clearly. AI API costs are the new killer — model them per-customer carefully.
- **Profit First discipline** — always include a Profit-First allocation plan. The formula is Sales - Profit = Expenses, not Sales - Expenses = Profit.
- **Three-tier break-even** — always calculate all three tiers (business-only, minimum-salary, market-rate). Founders who only calculate business-only break-even are lying to themselves.
- **Revenue stairs are required** — not a smooth growth curve. Stair-step with specific triggers at each stage. The $0 → $1K MRR stair must be concrete and specific.
- **Scenario projections** — always provide conservative, base, and optimistic projections with stated assumptions.
