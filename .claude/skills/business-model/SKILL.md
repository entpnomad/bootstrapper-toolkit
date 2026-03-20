---
name: business-model
description: Revenue model and unit economics analysis for bootstrapped founders. Evaluates pricing architecture, margin structure, cash flow dynamics, offer design, and revenue quality — forcing founders to examine whether the way they make money is optimal, sustainable, and designed to compound before scaling acquisition. Use when user runs `/business-model`, asks about "revenue model", "pricing strategy", "unit economics", "margins", "business model", "how to monetize", "pricing", "cash flow", "offer design", or needs to understand whether their revenue engine can sustain a self-funded business.
---

# Business Model Analysis — Revenue Engine for Bootstrappers

How the business makes money, keeps money, and compounds money. Calibrated to bootstrapped reality where revenue funds everything and the model must work at low volume before it works at scale.

## Philosophy

**Revenue model is not an afterthought — it's the engine.** Most founders obsess over product and treat the business model as a dropdown menu (SaaS? Marketplace? Agency?). But how you charge, what you charge for, and how cash flows through the business determines whether you eat or starve. The revenue model IS the business.

Read `.claude/skills/_shared/philosophy.md` for the full bottleneck shift and bootstrapper framework. For business model analysis specifically:

**AI-native reality — COGS collapses but CAC dominates.** When dev cost is near zero, software COGS approaches hosting + API calls. Gross margins look incredible on paper. But the money you saved on development moves to customer acquisition. A model that looks profitable in a spreadsheet but requires expensive distribution is not a good model for a bootstrapper. The question isn't "what's the gross margin?" — it's "can you acquire customers profitably with YOUR resources?"

**The cash-flow timing trap.** Revenue ≠ cash. A model with 80% gross margins but 12-month sales cycles and annual billing in arrears will kill a bootstrapper before the margins matter. Cash flow timing is more important than margin percentage for self-funded businesses. Money in the bank today beats money on the invoice net-60.

**Bootstrapped model constraints:**
- Must be profitable at low volume — can't "grow into profitability"
- Must have short CAC payback — can't wait 18 months to recoup acquisition cost
- Must generate cash upfront or at least monthly — can't float on VC runway
- Must not require a sales team to close — self-serve or founder-sold early
- Must compound over time — retention and expansion beat perpetual new-customer acquisition

## Reference Books

Check `references/INDEX.md` for relevant frameworks. Key topics for business model analysis: profit model archetypes, pricing psychology and value stacking, grand slam offer design, financial statements and margin analysis, SaaS pricing optimization, B2B revenue structure, profit-first behavioral cash flow, labor efficiency and owner compensation, value ladder and conversion economics.

## Research-First Protocol

Research autonomously before outputting anything. See `_shared/philosophy.md` for the full protocol. Key searches:

- "[category] pricing models" / "[category] how companies charge"
- "[competitor] pricing page" / "[competitor] plans" / "[competitor] pricing changes"
- "[category] average revenue per user" / "[category] LTV benchmarks"
- "[category] churn rate" / "[category] retention benchmarks"
- "[category] gross margin benchmarks" / "[category] unit economics"
- "[category] freemium vs paid" / "[category] free trial conversion rate"
- "[category] annual vs monthly billing" / "[category] pricing strategy"
- If competitor-analysis has already been run, pull pricing, revenue models, and funding data from it instead of re-researching
- If market-size has already been run, pull demand signals, beachhead size, and revenue ceiling from it
- If problem-analysis has already been run, pull willingness-to-pay ratings and pain severity from it
- If moat-analysis has already been run, pull switching cost and counter-positioning data from it
- If gtm-strategy has already been run, pull CAC estimates and channel costs from it

## Sub-Skill Mode

See `_shared/philosophy.md` Sub-Skill Mode Protocol.

## End-to-End Flow

### STEP 0 — CONTEXT GATHERING

Extract from the user's input:
- The business idea or product (what it does, who it's for)
- Current or planned revenue model (if stated)
- Current stage (idea, MVP, live product with revenue)
- Pricing (if set) or pricing assumptions
- Any existing revenue, customer, or conversion data

If the idea description is too vague to assess the business model, ask ONE clarifying question. Otherwise, proceed to research.

### STEP 1 — REVENUE MODEL RESEARCH

Research how money flows in this market. Not how the founder wants to charge — how the market actually pays.

**Search queries to run (adapt to the specific market):**
- How do competitors in this space charge? (Subscription, usage-based, per-seat, flat-rate, freemium, one-time)
- What pricing tiers exist in this market? (Entry, mid, enterprise — price points and packaging)
- What's the typical ARPU in this category? (Revenue per customer benchmarks)
- What pricing changes have competitors made recently? (Price increases, model shifts, packaging changes)
- Are there successful alternative models in adjacent markets? (e.g., usage-based in a historically per-seat market)
- What's the dominant billing cadence? (Monthly, annual, usage-based, one-time)

**From prior intelligence (if available):**
- competitor-analysis: pricing tiers, revenue estimates, funding status, business model details
- market-size: WTP evidence, demand signals, beachhead spending patterns
- problem-analysis: willingness-to-pay assessment, pain severity (pricing power indicator)
- moat-analysis: switching costs (pricing sustainability), counter-positioning (pricing asymmetry)
- gtm-strategy: CAC estimates, channel costs, distribution economics, LTV:CAC ratio

### STEP 2 — NINE-DIMENSION BUSINESS MODEL ASSESSMENT

Work through all nine dimensions. For each, assess based on research evidence, rate categorically, and note the specific evidence that supports the rating.

---

#### Dimension 1: Revenue Model Architecture

How the business generates revenue. The structural blueprint of how money enters.

**Revenue model types:**

| Model | How It Works | Bootstrapper Fit |
|-------|-------------|-----------------|
| **Subscription (SaaS)** | Recurring monthly/annual fee | Excellent — predictable, compounds |
| **Usage-based** | Pay per unit of consumption (API calls, transactions, storage) | Good — aligns cost with value, but unpredictable |
| **Per-seat** | Price per user | Good — scales with adoption, but easy to game |
| **Flat-rate** | Single price, unlimited usage | Good for simplicity — but leaves money on table at scale |
| **Freemium** | Free tier + paid upgrade | High CAC efficiency if conversion works — expensive charity if it doesn't |
| **One-time purchase** | Single payment, lifetime access | Cash upfront — but no recurring revenue, no compounding |
| **Marketplace / take-rate** | Percentage of transactions facilitated | Powerful at scale — chicken-and-egg at start |
| **Productized service** | Fixed-scope service at fixed price | Bootstrapper-friendly — trades time for predictability |
| **Hybrid** | Multiple models combined (e.g., subscription + usage) | Flexible — but complexity adds friction |

**What to evaluate:**
- Does the revenue model match how customers in this market expect to buy?
- Does the model align value delivered with price charged? (Or is there a disconnect?)
- Does the model create predictable, recurring revenue? (The gold standard for bootstrappers)
- Can the model work at low volume? (Or does it need scale to function?)
- Does the model encourage expansion revenue? (Customers paying more over time without new acquisition)
- Is there a proven analog? (At least one company using a similar model successfully in this or an adjacent market)

**Rate: OPTIMAL / VIABLE / SUBOPTIMAL / MISALIGNED**
- OPTIMAL: Model matches market expectations, creates recurring revenue, works at low volume, has proven analogs
- VIABLE: Model works but isn't the strongest fit — some friction or missed opportunity
- SUBOPTIMAL: Model has structural issues that limit growth or create revenue fragility
- MISALIGNED: Model doesn't match how customers buy or how value is delivered

---

#### Dimension 2: Pricing Architecture

How prices are set, structured, and communicated. Not just the number — the psychology and structure.

**Pricing dimensions to evaluate:**

| Element | What to Assess |
|---------|---------------|
| **Value metric** | What are you charging per? (Seat, usage, feature, outcome) Does it align with the value customers perceive? |
| **Price point** | Is the price anchored to value delivered or cost of alternatives? Is it within the market's willingness-to-pay range? |
| **Tier structure** | Are there clear upgrade paths? Does each tier justify its price increase with proportional value? |
| **Anchoring** | Is there a high-value anchor that makes mid-tier pricing feel reasonable? |
| **Packaging** | Are features bundled logically? Or is the packaging confusing, with critical features gated behind expensive tiers? |
| **Transparency** | Is pricing public and clear? Or hidden behind "contact sales" (acceptable for enterprise, death for self-serve)? |
| **Discounting** | Is there a strategic discount structure (annual billing), or is discounting reactive and margin-eroding? |

**What to evaluate:**
- Is the price anchored to value, not cost? (Customers don't care what it costs you — they care what it's worth to them)
- Is the value metric clear and fair? (Customers should feel they pay more only when they get more)
- Does the tier structure encourage upgrades? (Clear value gap between tiers without punishing the lower tier)
- Is pricing competitive with alternatives? (Not necessarily cheaper — but clearly justified)
- Does annual billing improve cash flow? (Monthly flexibility vs. annual commitment discount)
- Can the price increase over time? (Expansion revenue path via usage growth, more seats, or tier upgrades)

**Rate: STRONG / ADEQUATE / UNDERPRICED / BROKEN**
- STRONG: Value-anchored pricing with clear upgrade paths, expansion revenue built in, competitive positioning
- ADEQUATE: Pricing works but leaves money on table or has minor structural issues
- UNDERPRICED: Charging too little relative to value delivered — typical founder error
- BROKEN: Pricing doesn't align with value, confuses buyers, or makes the business unviable

---

#### Dimension 3: Unit Economics

Revenue and cost per customer. The math that determines whether each customer makes or loses money.

**Core metrics to evaluate:**

| Metric | What It Means | Healthy Range (Software) |
|--------|--------------|------------------------|
| **ARPU** (Avg Revenue Per User) | Monthly revenue per customer | Market-dependent — compare to competitors |
| **Gross margin** | Revenue minus direct costs (hosting, API, support) | > 70% for SaaS, > 40% for services |
| **CAC** (Customer Acquisition Cost) | Total cost to acquire one customer | Must be < LTV / 3 |
| **LTV** (Lifetime Value) | Total revenue from a customer over their lifetime | Must be > 3x CAC |
| **LTV:CAC ratio** | Efficiency of the growth engine | > 3:1 healthy, > 5:1 excellent |
| **Payback period** | Months to recoup CAC | < 6 months for bootstrappers |
| **Churn** | % of customers leaving per month | < 3% monthly for SMB, < 1% for enterprise |
| **Net revenue retention** | Revenue from existing customers vs. prior period (including expansion) | > 100% = customers growing faster than churning |

**What to evaluate:**
- Can you acquire customers profitably from day one? (Not "at scale" — at current volume)
- What's the realistic CAC given your distribution channels? (Not the best case — the average case)
- What's the realistic churn rate for this market? (Not your hope — the industry benchmark)
- Is there expansion revenue? (Do customers naturally upgrade, add seats, or consume more?)
- What's the gross margin at current and projected scale?
- Is the unit economics math based on real data or founder projections?

**Rate: PROFITABLE / MARGINAL / UNDERWATER / UNKNOWN**
- PROFITABLE: LTV:CAC > 3:1, payback < 6 months, positive gross margin, based on real or well-evidenced data
- MARGINAL: Numbers work on paper but tight — small changes in churn or CAC tip to unprofitable
- UNDERWATER: CAC exceeds LTV, or payback period exceeds 12 months, or negative gross margin
- UNKNOWN: Insufficient data to calculate — no revenue, no benchmarks, pure projection

---

#### Dimension 4: Offer Design

How the product is packaged and presented as a purchasable offer. Not the product itself — the wrapper around it that makes people buy.

**Offer components:**

| Component | What It Does | Example |
|-----------|-------------|---------|
| **Core deliverable** | What the customer gets | The software, the service, the outcome |
| **Bonuses** | Extra value that tips the decision | Templates, onboarding help, community access |
| **Guarantee** | Risk reversal — what happens if it doesn't work | Money-back guarantee, free trial, performance guarantee |
| **Scarcity / urgency** | Why buy now instead of later | Limited-time pricing, capacity constraints, seasonal relevance |
| **Social proof** | Evidence that others have bought and succeeded | Case studies, testimonials, user count, logos |
| **Naming / framing** | How the offer is positioned and described | "Growth Plan" vs. "Enterprise Solution" vs. "Starter Kit" |

**What to evaluate:**
- Is the offer designed to reduce buyer risk? (Free trial, money-back guarantee, low commitment entry)
- Does the value equation favor the buyer? (Dream outcome x perceived likelihood > time delay x effort)
- Are there bonuses or extras that increase perceived value without increasing cost?
- Is there a clear reason to buy now rather than later?
- Is the offer differentiated from competitor offers? (Or is it the same features at the same price with a different logo?)
- Does the offer match the buyer's sophistication? (SMBs want simplicity; enterprise wants configurability)

**Rate: COMPELLING / ADEQUATE / WEAK / COMMODITY**
- COMPELLING: Clear value, low risk, differentiated, strong reasons to buy now
- ADEQUATE: Works but doesn't stand out — price-competitive but not remarkable
- WEAK: Unclear value proposition, high buyer risk, no differentiation
- COMMODITY: Interchangeable with competitors — buying decision comes down to price alone

---

#### Dimension 5: Revenue Quality

How durable, predictable, and resilient the revenue stream is.

**Revenue quality spectrum:**

| Quality Indicator | Strong | Weak |
|-------------------|--------|------|
| **Predictability** | Recurring subscriptions, contracts, committed spend | One-time purchases, project-based, seasonal |
| **Concentration** | Diverse customer base, no single customer > 10% of revenue | Few large customers, top customer > 25% of revenue |
| **Retention** | High retention, low churn, net revenue retention > 100% | High churn, no expansion, constant need for new customers |
| **Dependency** | Revenue from own product, own channels | Revenue dependent on platform, partner, or algorithm |
| **Contractual** | Locked-in contracts, annual commitments | Month-to-month, cancel anytime, no switching cost |

**What to evaluate:**
- Is the revenue recurring and predictable? (Or does the founder start each month at zero?)
- Is the customer base diversified? (Or is revenue concentrated in a few large accounts?)
- Is revenue growing through expansion of existing customers? (Or only through new acquisition?)
- Is there platform dependency risk? (Revenue dependent on App Store, Google algorithm, Amazon, etc.)
- Does the revenue survive economic downturns? (Nice-to-have tools get cut first in a recession)
- Can revenue be forecast with reasonable accuracy for 3-6 months out?

**Rate: DURABLE / MODERATE / FRAGILE / VOLATILE**
- DURABLE: Recurring, diversified, retained, independent — can plan confidently
- MODERATE: Mostly recurring but some concentration or churn risk
- FRAGILE: High churn, concentrated, or platform-dependent — one event can crater revenue
- VOLATILE: Unpredictable, seasonal, project-based, or dependent on external factors

---

#### Dimension 6: Margin Structure

Where the money goes after it comes in. What's left after real costs, not just COGS.

**Margin layers:**

| Margin | What It Includes | Healthy (Software) | Healthy (Services) |
|--------|-----------------|-------------------|-------------------|
| **Gross margin** | Revenue - COGS (hosting, API, direct support) | > 70% | > 40% |
| **Operating margin** | Gross profit - OpEx (marketing, R&D, G&A) | > 20% | > 15% |
| **Net margin** | Operating profit - taxes, interest, etc. | > 15% | > 10% |
| **Owner margin** | What the founder actually takes home (after market-rate salary) | Positive from year 1-2 | Positive from year 1 |

**What to evaluate:**
- What are the real COGS? (Hosting, API costs, third-party tools, direct labor for service delivery)
- How do COGS scale with customers? (Linear = bad for margin. Sublinear = leverage.)
- What's the biggest cost center after COGS? (Customer acquisition? R&D? Support?)
- Does the margin structure improve with scale? (Economies of scale in costs?)
- Is the founder paying themselves a market-rate salary in the projections? (If not, the margins are fake)
- What happens to margins if a key input cost increases 2x? (API pricing changes, hosting costs, contractor rates)

**Rate: HIGH-LEVERAGE / HEALTHY / THIN / NEGATIVE**
- HIGH-LEVERAGE: Gross > 80%, costs scale sublinearly, significant operating margin after real expenses
- HEALTHY: Gross > 60%, sustainable operating margin, founder taking market-rate salary
- THIN: Gross 40-60%, operating margin tight, vulnerable to cost increases
- NEGATIVE: Spending more than earning, or margins only work by underpaying the founder

---

#### Dimension 7: Cash Flow Dynamics

When money arrives vs. when money leaves. The timing matters more than the amount for bootstrappers.

**Cash flow patterns:**

| Pattern | How It Works | Bootstrapper Impact |
|---------|-------------|-------------------|
| **Cash-positive cycle** | Customers pay upfront (annual billing, prepaid), costs come later | Excellent — self-funding growth |
| **Cash-neutral cycle** | Revenue and costs roughly aligned in timing | Manageable — steady state |
| **Cash-hungry cycle** | Costs come before revenue (long sales cycles, deferred billing) | Dangerous — requires capital or reserves |
| **Cash-burning cycle** | Sustained negative cash flow requiring external funding | Fatal for bootstrappers without reserves |

**What to evaluate:**
- When does the customer pay? (Upfront, monthly, on delivery, net-30, net-60?)
- What are the upfront costs before first revenue? (Development, inventory, licensing, certifications)
- Is there an annual billing option? (And how much discount is offered — should be 15-20% for 2 months free)
- What's the sales cycle length? (Days for self-serve, weeks for SMB, months for enterprise)
- Are there seasonal cash flow patterns? (Revenue spikes followed by dry periods)
- What's the minimum cash reserve needed to operate for 3 months with zero new revenue?
- Can the business self-fund growth from operations? (Or does every growth dollar require external capital?)

**Rate: CASH-POSITIVE / NEUTRAL / CASH-HUNGRY / CASH-BURNING**
- CASH-POSITIVE: Customers pay upfront or quickly, costs lag revenue, business self-funds growth
- NEUTRAL: Cash in and cash out are roughly balanced, adequate for steady-state
- CASH-HUNGRY: Significant upfront costs or long collection cycles, needs reserves or credit
- CASH-BURNING: Sustained negative cash flow — not viable without external funding

---

#### Dimension 8: Scalability & Leverage

Can this business grow revenue faster than it grows costs? Or does every dollar of revenue require a proportional dollar of cost?

**Leverage spectrum:**

| Type | How It Scales | Example |
|------|--------------|---------|
| **Code leverage** | Build once, sell infinitely | SaaS, digital products, templates |
| **Content leverage** | Create once, distribute infinitely | Courses, media, documentation |
| **Network leverage** | Users create value for other users | Marketplaces, platforms, communities |
| **Capital leverage** | Money works instead of time | Investments, lending, treasury |
| **People leverage** | Team multiplies founder output | Agencies, consulting firms (linear, not true leverage) |
| **No leverage** | Revenue = founder's time x hourly rate | Solo consulting, custom dev, done-for-you |

**What to evaluate:**
- Does revenue scale without proportional headcount? (The key test of leverage)
- Can 10x customers be served with less than 10x cost? (Sublinear cost scaling = leverage)
- Is there a ceiling on the founder's time? (If every customer needs founder attention, growth is capped)
- Can the delivery be automated or productized? (Manual delivery today, automated delivery tomorrow?)
- Does the product have near-zero marginal cost per additional customer? (Software typically yes; services typically no)
- Is there a natural expansion path within accounts? (Upsell, cross-sell, usage growth)

**Rate: HIGH-LEVERAGE / MODERATE / LINEAR / LABOR-BOUND**
- HIGH-LEVERAGE: Near-zero marginal cost, revenue scales without headcount, automated delivery
- MODERATE: Some leverage (software + services), costs grow slower than revenue
- LINEAR: Every dollar of revenue requires proportional effort or cost
- LABOR-BOUND: Revenue is directly tied to hours worked — growth requires more people

---

#### Dimension 9: Business Model Risks

What can break the revenue engine? Structural risks specific to how this business makes money.

**Risk categories:**

| Risk Type | What It Means | Example |
|-----------|--------------|---------|
| **Pricing pressure** | Competitors or market force prices down | Race to bottom, free alternatives, commoditization |
| **COGS inflation** | Input costs increase faster than pricing power | API costs up, hosting costs up, supplier pricing changes |
| **Channel dependency** | Revenue dependent on a platform or algorithm | App Store takes 30%, Google changes algorithm, marketplace changes rules |
| **Customer concentration** | Too much revenue from too few customers | Top 3 customers = 60% of revenue |
| **Model obsolescence** | Market shifts away from this business model type | One-time purchase market moves to subscription (or vice versa) |
| **Regulatory** | Laws or regulations change the economics | New privacy laws, industry-specific compliance, tax changes |
| **Margin compression** | Competitive or market forces erode margins over time | More competitors, buyer power increases, switching costs decrease |

**What to evaluate:**
- What's the single most likely event that breaks this model?
- If the dominant distribution channel disappears, does the business survive?
- If a well-funded competitor undercuts pricing by 50%, what happens?
- If churn doubles from the projected rate, is the business still viable?
- Are there regulatory risks that could change the model's economics?
- Is there technology risk? (Dependency on third-party APIs, AI model access, platform features)
- What's the concentration risk? (Single customer, single channel, single product)

**Rate: LOW / MANAGEABLE / SIGNIFICANT / CRITICAL**
- LOW: No single point of failure, diversified revenue, strong pricing power
- MANAGEABLE: Known risks with clear mitigations, acceptable for a bootstrapper
- SIGNIFICANT: Material risks that could impair the business model without active management
- CRITICAL: Structural vulnerability that could kill the business — must be addressed before scaling

---

### STEP 3 — VALIDATION GATES

Five binary checks. Pass/fail. No nuance.

| # | Gate | Pass/Fail |
|---|------|-----------|
| 1 | Revenue model has at least one real-world analog (someone using a similar model successfully in this or adjacent market) | |
| 2 | Unit economics positive at low volume (profitable per customer without needing scale) | |
| 3 | CAC payback < 6 months at realistic channel assumptions (not best-case, average-case) | |
| 4 | Gross margin > 60% (software) or > 40% (physical/services) | |
| 5 | Revenue not 100% dependent on single customer, platform, or channel | |

**Gates passed: X/5**

- **5/5**: Revenue engine is sound — scale with confidence
- **3-4/5**: Viable but has gaps — address the failing gates before scaling acquisition
- **< 3/5**: RED FLAG — fix the business model before spending on growth
- **< 2/5**: STOP — the model is broken. More customers won't fix a broken engine.

### STEP 4 — OUTPUT

Produce the full report using the template below.

## Output Template

```
# BUSINESS MODEL ANALYSIS: [Product/Idea Name]

Research date: [date]
Stage: [Idea / MVP / Live Product]
Stated revenue model: [What the founder described, or "not specified"]

---

## BUSINESS MODEL SCORECARD

Overall verdict: [REVENUE ENGINE SOUND / VIABLE BUT NEEDS TUNING / STRUCTURAL WEAKNESS / BROKEN MODEL]

| Dimension | Rating | Key Finding |
|-----------|--------|-------------|
| Revenue Model Architecture | OPTIMAL/VIABLE/SUBOPTIMAL/MISALIGNED | |
| Pricing Architecture | STRONG/ADEQUATE/UNDERPRICED/BROKEN | |
| Unit Economics | PROFITABLE/MARGINAL/UNDERWATER/UNKNOWN | |
| Offer Design | COMPELLING/ADEQUATE/WEAK/COMMODITY | |
| Revenue Quality | DURABLE/MODERATE/FRAGILE/VOLATILE | |
| Margin Structure | HIGH-LEVERAGE/HEALTHY/THIN/NEGATIVE | |
| Cash Flow Dynamics | CASH-POSITIVE/NEUTRAL/CASH-HUNGRY/CASH-BURNING | |
| Scalability & Leverage | HIGH-LEVERAGE/MODERATE/LINEAR/LABOR-BOUND | |
| Business Model Risks | LOW/MANAGEABLE/SIGNIFICANT/CRITICAL | |

---

## VALIDATION GATES

| # | Gate | Result |
|---|------|--------|
| 1 | Revenue model has real-world analog | PASS / FAIL |
| 2 | Unit economics positive at low volume | PASS / FAIL |
| 3 | CAC payback < 6 months at realistic assumptions | PASS / FAIL |
| 4 | Gross margin > 60% (software) or > 40% (services) | PASS / FAIL |
| 5 | Revenue not dependent on single customer/platform/channel | PASS / FAIL |

**Gates passed: X/5** — [Assessment: Sound / Viable with gaps / RED FLAG / STOP]

---

## REVENUE MODEL DEEP DIVE

**Current/proposed model**: [Model type and how it works for this specific business]
**Market standard**: [How competitors in this space charge]
**Model-market fit**: [Does the model match how customers expect to buy?]
**Proven analogs**: [Companies using similar models successfully — name them]

**Revenue model alternatives considered:**

| Alternative | Pros | Cons | Why / Why Not |
|-------------|------|------|---------------|
| [Model 1] | | | |
| [Model 2] | | | |
| [Model 3] | | | |

**Recommendation**: [Stick with current model / Switch to X / Hybrid approach — with rationale]

---

## PRICING ARCHITECTURE

**Current/proposed pricing**: [Price points, tiers, billing cadence]
**Competitor pricing range**: [Low to high, with named competitors]
**Value metric**: [What are you charging per? Is it aligned with perceived value?]

**Pricing analysis:**
- Price vs. value delivered: [Aligned / Underpriced / Overpriced — evidence]
- Tier structure: [Clear upgrade path? / Missing tiers? / Too complex?]
- Expansion revenue built in: [Yes — how / No — what's missing]
- Annual billing opportunity: [Available / Not offered — cash flow impact]

**Pricing recommendation**: [Specific pricing changes if any, with rationale]

---

## UNIT ECONOMICS

**Core metrics (current or projected):**

| Metric | Value | Benchmark | Assessment |
|--------|-------|-----------|------------|
| ARPU (monthly) | | [Category benchmark] | |
| Gross margin | | > 70% SaaS / > 40% services | |
| CAC | | [Realistic for channels used] | |
| LTV | | Must be > 3x CAC | |
| LTV:CAC | | > 3:1 healthy | |
| Payback period | | < 6 months | |
| Monthly churn | | < 3% SMB / < 1% enterprise | |
| Net revenue retention | | > 100% target | |

**Data quality**: [Based on real data / Reasonable projections / Founder guesses — flag which]

**Unit economics verdict**: [PROFITABLE / MARGINAL / UNDERWATER / UNKNOWN]
[2-3 sentences on whether each customer makes or loses money and why]

---

## OFFER DESIGN

**Current offer assessment:**
- Core deliverable: [What the customer gets]
- Risk reversal: [Guarantee, free trial, refund policy — or none]
- Differentiation: [What makes this offer different from competitor offers]
- Perceived value vs. price: [Value equation assessment]

**Offer gaps:**
- [Missing component 1 and why it matters]
- [Missing component 2 and why it matters]

**Offer improvement recommendations:**
1. [Specific, actionable improvement]
2. [Specific, actionable improvement]

---

## REVENUE QUALITY

**Revenue characteristics:**
- Recurring vs. one-time: [% breakdown or projected structure]
- Customer concentration: [Diversified / Moderate concentration / High concentration]
- Retention rate: [Known / Projected / Unknown — with evidence]
- Platform dependency: [None / Moderate / High — name the platform]
- Expansion revenue: [Present / Potential / Absent]

**Revenue quality verdict**: [DURABLE / MODERATE / FRAGILE / VOLATILE]
[2-3 sentences on how predictable and resilient the revenue is]

---

## MARGIN STRUCTURE

**Margin breakdown:**

| Layer | Current/Projected | Target | Gap |
|-------|-------------------|--------|-----|
| Gross margin | | > 70% SaaS / > 40% services | |
| Operating margin | | > 20% | |
| Net margin | | > 15% | |
| Owner margin (after market-rate salary) | | Positive | |

**Biggest cost centers**: [What eats the margin — and is it fixable?]
**Margin scalability**: [Do margins improve with scale? Or stay flat / compress?]
**Cost risks**: [What input costs could change and impact margins?]

---

## CASH FLOW DYNAMICS

**Cash flow pattern**: [CASH-POSITIVE / NEUTRAL / CASH-HUNGRY / CASH-BURNING]

**Cash flow analysis:**
- When customers pay: [Upfront / Monthly / Delayed — specific terms]
- Upfront investment required: [Before first dollar of revenue]
- Sales cycle length: [Days / Weeks / Months]
- Annual billing adoption: [Available? Take rate? Cash flow impact?]
- Seasonal patterns: [Any revenue seasonality?]
- Minimum cash reserve: [What's needed to survive 3 months of zero new revenue?]

**Self-funding capacity**: [Can the business fund its own growth from operations? At what growth rate?]

---

## SCALABILITY & LEVERAGE

**Leverage assessment:**
- Primary leverage type: [Code / Content / Network / None]
- Marginal cost per customer: [Near-zero / Low / Moderate / High]
- Revenue per employee potential: [High / Moderate / Low]
- Automation opportunity: [What's manual today that could be automated?]
- Founder time ceiling: [At what customer count does the founder become the bottleneck?]
- Expansion revenue path: [How do existing customers generate more revenue over time?]

**Scalability verdict**: [HIGH-LEVERAGE / MODERATE / LINEAR / LABOR-BOUND]

---

## BUSINESS MODEL RISKS

| # | Risk | Severity | Likelihood | Mitigation |
|---|------|----------|------------|------------|
| 1 | [Specific risk] | Critical/High/Medium/Low | High/Medium/Low | [Mitigation action] |
| 2 | | | | |
| 3 | | | | |
| 4 | | | | |

**Single point of failure**: [Is there one thing that, if it changed, would break the entire model? Name it.]
**What kills this business model**: [One sentence — the most likely model failure mode]

---

## BOTTOM LINE

**Business model verdict**: [REVENUE ENGINE SOUND / VIABLE BUT NEEDS TUNING / STRUCTURAL WEAKNESS / BROKEN MODEL]

[2-3 sentences. Can this business sustain itself from revenue alone? What's the primary strength of the model? What's the biggest structural risk? If the model is weak, what's the fastest fix?]

**The honest answer to "can this business sustain itself from revenue alone?":**
[One sentence. The real answer, not the comfortable one.]

**Top 3 actions for the next 7 days:**
1. [Specific, concrete, actionable — related to the weakest dimension]
2. [Specific, concrete, actionable]
3. [Specific, concrete, actionable]

---
[If invoked as sub-skill: produce DIGEST summary per `_shared/philosophy.md` Digest Mode format]
```

## Important Rules

See `_shared/philosophy.md` Universal Skill Rules.

**Skill-specific rules:**
- **Unit economics must use real numbers** — if real data isn't available, use industry benchmarks with explicit assumptions. Flag every number that's a projection vs. observed data.
- **Pricing psychology matters more than pricing math** — a price that's "correct" by the numbers but feels wrong to buyers will fail. Assess perceived value, not just cost-plus margin.
- **Cash flow timing kills more bootstrappers than bad margins** — a 70% gross margin business with 90-day payment terms and 30-day cost cycles will run out of cash. Always assess when money arrives vs. when it leaves.
- **The model must work at low volume** — "it gets profitable at 10,000 customers" is not a bootstrapper-viable model. If the unit economics don't work at 50-100 customers, the model needs fixing.
- **Challenge fake profitability** — margins that only work because the founder isn't paying themselves a market-rate salary are fake. Margins that depend on zero support costs are temporary. Flag both.
- **Name specific competitors** when analyzing pricing — "competitors charge $20-50/mo" is weak. "[Competitor A] charges $29/mo for X features, [Competitor B] charges $49/mo with Y included" is useful.
- **Revenue model analogs reduce risk** — if no one in this market or adjacent markets uses the proposed model, that's a signal. Not necessarily a deal-breaker, but a risk to acknowledge.
