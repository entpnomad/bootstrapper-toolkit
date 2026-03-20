---
name: moat-analysis
description: Defensibility and switching cost analysis for bootstrapped founders. Assesses real vs. fake moats, user-investment lock-in, network effects, data advantages, distribution moats, and long-term defensibility. Use when user runs `/moat-analysis`, asks about "defensibility", "switching costs", "moat", "competitive advantage", "lock-in", "barriers to entry", or needs to understand what makes a business defensible in an AI-native world.
---

# Moat Analysis — Defensibility for Bootstrappers

What keeps customers from leaving and competitors from copying. Calibrated to AI-native reality where code is cheap and product moats are mostly fake.

## Philosophy

**Most moats are bullshit.** When code is cheap and AI can replicate features in a weekend, "technology advantage" and "first mover" are not moats. They're stories founders tell themselves. A real moat is something that gets stronger the longer you operate and that a well-funded competitor cannot buy or build overnight.

Read `.claude/skills/_shared/philosophy.md` for the full bottleneck shift and user-investment lock-in framework. For moat analysis specifically:

**The grab-them-by-the-balls principle.** Design products where usage creates investment, and investment creates lock-in. This isn't evil — it's good product design. A product people invest in is a product people value. See the shared philosophy for the lock-in checklist.

**Distribution is the real moat when code is cheap.** A mediocre product with great distribution beats a great product with no distribution. Owned audience, brand trust, channel dominance, community presence — durable advantages that can't be cloned with AI tools.

**AI-native reality check — fake moats:**
- "We built it first" / "Our technology is superior" / "We have more features" / "Our team is great" — NOT moats when code is cheap.
- What IS a moat: things that take time to accumulate and can't be fast-forwarded — data, relationships, trust, community, user investment, regulatory position, distribution leverage.

## Reference Books

Check `references/INDEX.md` for relevant frameworks. Key topics for moat analysis: durable competitive advantage sources, barriers to entry and captive customers, intangible economy dynamics, monopoly thinking, Five Forces and industry structure, habit-forming products and stored value, installed base profit models, chain-link systems and resource leverage.

## Research-First Protocol

Research autonomously before outputting anything. See `_shared/philosophy.md` for the full protocol. Key searches:
- "[category] switching costs" / "[category] vendor lock-in"
- "[competitor] customer retention" / "[competitor] churn rate"
- "[category] network effects" / "[category] data advantage"
- "[category] barriers to entry"
- Competitor lock-in mechanisms (onboarding flows, data portability, export tools)
- If competitor-analysis has already been run, pull switching cost data from it instead of re-researching

## Sub-Skill Mode

See `_shared/philosophy.md` Sub-Skill Mode Protocol.

## End-to-End Flow

### STEP 0 — CONTEXT GATHERING

Extract from the user's input:
- The business idea or product (what it does, who it's for)
- Current stage (idea, MVP, live product with customers)
- Any stated moat or defensibility claims
- Known competitors (or use competitor-analysis output if available)

If the idea description is too vague to assess defensibility, ask ONE clarifying question. Otherwise, proceed to research.

### STEP 1 — MOAT LANDSCAPE RESEARCH

Research what defensibility looks like in this specific market. Not all moat types apply to every market.

**Search queries to run (adapt to the specific market):**
- How do incumbents retain customers in this category?
- What are the switching costs for [product category]?
- Do competitors offer data export/portability? (low = higher lock-in)
- Are there network effects in this market? How do they work?
- What regulatory barriers exist in this space?
- What does the customer onboarding process look like? (longer setup = higher switching costs)

**From competitor intelligence (if available):**
- What switching cost dimensions did competitor-analysis identify?
- What moat assessments (Real/Weak/Fake) were assigned?
- What user investment do competitor products require?

### STEP 2 — NINE-DIMENSION MOAT ASSESSMENT

Work through all nine moat dimensions. For each, assess whether it applies, rate its current strength and buildability, and identify specific actions.

---

#### Dimension 1: User-Investment Lock-In (The Core Moat)

The most powerful and achievable moat for bootstrappers. Does usage create stored value that raises switching costs?

**Types of user investment:**

| Investment Type | Examples | Switching Cost Level |
|----------------|---------|---------------------|
| **Content created** | Quizzes built, templates designed, posts written, pages configured | Very High — recreating content is painful |
| **Data imported/accumulated** | Contacts, transactions, history, analytics, customer records | Very High — data migration is expensive and lossy |
| **Workflows configured** | Automations, rules, integrations, custom pipelines | High — workflow rebuilding requires relearning |
| **Integrations connected** | API connections, embedded widgets, third-party hooks | High — re-integrating is technical and time-consuming |
| **Team adoption** | Multiple users trained, roles configured, internal processes built around the tool | Very High — organizational change is harder than individual switching |
| **Reputation/history built** | Seller ratings, review history, transaction track record, community reputation | Extreme — reputation is non-portable |
| **Learning invested** | Time spent learning the UI, keyboard shortcuts, mental models | Medium — annoying but not catastrophic |
| **Customization** | Theme customization, branding, configuration tweaks | Medium — cosmetic but emotionally invested |

**What to evaluate:**
- Does the product require users to create, build, import, or configure things? (If no — weak lock-in potential)
- Is the stored value portable? (Can they export everything and migrate? If yes — weaker lock-in)
- Does the value accumulate over time? (Does it get MORE valuable the longer they use it?)
- Does the free tier require meaningful investment? (If freemium, does the free plan create lock-in, or can they leave with zero loss?)
- How long before switching costs become significant? (Days? Weeks? Months?)
- Does team adoption multiply switching costs? (Individual tool vs. team workflow)

**Design principles for maximizing user investment:**
- Make the free tier require building, not just browsing
- Make onboarding productive — every setup step creates stored value
- Make data import easy, export less obvious (not dishonest — just don't advertise the exit)
- Design features that get better with accumulated history
- Encourage team adoption early (shared workspaces, collaboration features)
- Build integration hooks that embed your product into other workflows

**Rate: STRONG / MODERATE / WEAK / NONE**

---

#### Dimension 2: Network Effects

More users = more value for each user. The strongest moat type, but rare and hard to manufacture.

**Types of network effects:**

| Type | How It Works | Example Pattern |
|------|-------------|-----------------|
| **Direct** | More users on the same side = more value | Communication tools, social platforms |
| **Indirect / cross-side** | More users on one side attract more on the other | Marketplaces, platforms, app ecosystems |
| **Data** | More users = more data = better product for everyone | Search engines, recommendation systems, AI products |
| **Content** | More users = more content = more value for all | Review sites, Q&A platforms, forums |
| **Local** | Network effects within a geography or segment | Delivery networks, local marketplaces |

**What to evaluate:**
- Does the product become more valuable as more people use it? (The acid test)
- Is this a genuine network effect or just "more customers = more revenue"? (The latter is not a network effect)
- What's the minimum viable network? (How many users before the network effect kicks in?)
- Are the network effects local or global? (Local = easier to bootstrap one market at a time)
- Can data from users improve the product for all users? (AI/ML opportunity)
- Is there a marketplace or platform dynamic? (Two-sided market potential)

**Bootstrapper reality check:** True network effects are extremely rare in bootstrapped businesses. Don't claim network effects unless the product genuinely gets better with more users. "We could add a community feature" is not a network effect — it's a feature idea.

**Rate: STRONG / MODERATE / WEAK / NONE / NOT APPLICABLE**

---

#### Dimension 3: Data Moat

Proprietary data that improves the product and that competitors cannot easily replicate.

**What to evaluate:**
- Does the product generate unique data from usage? (Behavioral data, customer inputs, transaction data)
- Does that data make the product better? (Better recommendations, better predictions, better defaults)
- Is the data defensible? (Can it be scraped, bought, or synthesized? If yes — weak moat)
- Does data accumulate over time, creating compounding advantage?
- Could an AI model trained on this data create a genuine advantage?
- Is the data derived from user activity, or publicly available? (User-generated data is more defensible)

**Data moat spectrum:**
- **Weak**: Data that's available to anyone (public datasets, scraped info)
- **Moderate**: Data that requires a user base to collect (usage patterns, preferences)
- **Strong**: Data that's unique, proprietary, and improves the product in ways competitors can't replicate (transaction history, vertical-specific benchmarks, trained models on proprietary data)

**Rate: STRONG / MODERATE / WEAK / NONE**

---

#### Dimension 4: Distribution Moat

Owned channels, audience, and brand presence that competitors cannot replicate quickly. **This is the #1 moat for bootstrappers in the AI age.**

**What to evaluate:**
- Does the founder/company own an audience? (Email list, social following, community, blog traffic)
- Is there an SEO moat? (Ranking for valuable keywords with years of content history)
- Is there a marketplace position? (App store ranking, directory listing, review site presence)
- Are there partnerships or channel relationships? (Resellers, integrators, affiliates)
- Is there a brand that buyers trust? (Brand recall, "default choice" status in a niche)
- Is there community ownership? (Discord, Slack group, forum that competitors can't replicate)
- How long would it take a new competitor to match this distribution? (Months = weak; Years = strong)

**Rate: STRONG / MODERATE / WEAK / NONE**

---

#### Dimension 5: Counter-Positioning

Your business model or approach is something incumbents can't adopt without cannibalizing their own revenue.

**What to evaluate:**
- Are you doing something that incumbents can't copy because it would hurt their existing business?
- Would matching your approach require them to cannibalize revenue? (e.g., offering freemium when they're paid-only)
- Would it require them to abandon their sales motion? (e.g., self-serve when they're sales-led)
- Would it require organizational restructuring? (e.g., going downmarket when they're enterprise)
- Is there a pricing or business model asymmetry? (e.g., flat-rate vs. per-seat when they have 500 enterprise customers on per-seat pricing)

**Classic counter-positions for bootstrappers:**
- Freemium vs. paid-only incumbents (they can't match without losing revenue)
- Self-serve vs. sales-led incumbents (they can't fire the sales team)
- Simple/focused vs. bloated incumbents (they can't remove features their enterprise customers use)
- Transparent pricing vs. "contact sales" incumbents (they can't publish prices without destabilizing existing contracts)
- Bootstrapped cost structure vs. VC-funded overhead (they can't cut costs without cutting team)

**Rate: STRONG / MODERATE / WEAK / NONE / NOT APPLICABLE**

---

#### Dimension 6: Economies of Scale

Cost advantages that come from volume, where a larger operation has structurally lower per-unit costs.

**What to evaluate:**
- Do unit economics improve with scale? (Lower cost per customer as you grow)
- Are there fixed costs that get amortized over more customers? (Infrastructure, content creation, compliance)
- Is there purchasing power at scale? (API costs, hosting, supplier negotiations)
- Does scale improve the product? (More data, better ML models, more content)

**Bootstrapper reality:** Scale economies rarely apply at bootstrapper scale. This moat type is more relevant when evaluating whether incumbents have an advantage over you. If a competitor has 10x your users and meaningfully lower costs because of it, that's a threat. If scale just means "more revenue" without structural cost advantages, it's not a real moat.

**Rate: STRONG / MODERATE / WEAK / NONE / NOT APPLICABLE**

---

#### Dimension 7: Regulatory & Compliance Moat

Legal, regulatory, or compliance requirements that create barriers to entry.

**What to evaluate:**
- Are there licensing requirements to operate in this market?
- Are there compliance certifications needed? (SOC 2, HIPAA, GDPR, PCI-DSS, ISO 27001)
- Do regulations create barriers that slow new entrants?
- Are there data residency or jurisdiction requirements?
- Is there a "compliance moat" — once achieved, it becomes a selling point and barrier to entry?

**Bootstrapper lens:** Compliance can be a moat if you achieve it and competitors don't. SOC 2 certification, HIPAA compliance, or industry-specific certifications take time and money to earn. Once you have them, they're a trust signal AND a barrier. But they're expensive to achieve — evaluate whether the market demands them.

**Rate: STRONG / MODERATE / WEAK / NONE / NOT APPLICABLE**

---

#### Dimension 8: Relationship & Trust Moat

Personal relationships, reputation, and trust that can't be replicated by technology.

**What to evaluate:**
- Does the founder have existing relationships in the target market?
- Is the business in a market where trust and reputation determine vendor selection?
- Do customers buy from people they know? (High-touch markets, consulting-adjacent, enterprise)
- Is there a community of users who advocate for the product?
- Can trust be transferred? (Case studies, testimonials, word-of-mouth)
- How long does it take to build trust in this market? (Long = strong moat once built)

**AI-native lens:** Relationships can't be vibe-coded. In a world where anyone can build a product in a weekend, the founder who has spent 10 years in an industry, knows the buyers personally, and has earned trust through years of delivering value has an advantage that no AI tool can replicate. This is one of the most underrated moats.

**Rate: STRONG / MODERATE / WEAK / NONE**

---

#### Dimension 9: Process & Operational Moat

Organizational processes, operational excellence, or institutional knowledge that's hard to replicate.

**What to evaluate:**
- Are there operational processes that take years to develop and can't be copied?
- Is there institutional knowledge embedded in how the business operates?
- Does operational excellence create a customer experience advantage?
- Is there a "machine" (content engine, support system, onboarding process) that compounds over time?

**Bootstrapper lens:** This is a moat that builds over time, not at launch. A well-oiled content machine that produces 4 high-quality articles/week, a support process that consistently delivers 95+ NPS, or an onboarding flow that's been iterated 200 times — these are hard to replicate even with unlimited money.

**Rate: STRONG / MODERATE / WEAK / NONE / NOT APPLICABLE**

---

### STEP 3 — MOAT REALITY CHECK

After assessing all nine dimensions, apply two critical filters:

#### Filter 1: Real vs. Fake Moat Classification

Classify every claimed or potential moat:

| Category | What It Means | Action |
|----------|--------------|--------|
| **Real** | Structural advantage that strengthens over time and can't be bought or built overnight | Invest here, communicate to customers |
| **Weak** | Some advantage, but could be eroded by a well-funded or persistent competitor | Build on it, but don't depend on it alone |
| **Fake** | Sounds defensible but isn't — will not protect against a competent competitor | Stop telling yourself this story |
| **Buildable** | Not present today, but can be deliberately constructed over time | Design the product and strategy to build this moat |

**Common fake moats to flag:**
- "First mover advantage" — being first means nothing if followers can build faster and better
- "Superior technology" — when code is cheap, technology advantages are measured in weeks, not years
- "Our team" — great teams help, but they're not a structural barrier
- "More features" — feature parity is achievable by any funded competitor
- "Our AI is better" — if you're using the same foundation models as everyone else, you don't have an AI moat
- "We're faster" — speed of execution is temporary; it's not a structural advantage
- "Patents" — useful in some industries, mostly irrelevant in SaaS

#### Filter 2: Moat Timeline Assessment

Moats are not static. Assess the timeline:

- **What moats exist today?** (If the product is live — what's actually keeping customers?)
- **What moats will exist in 6 months?** (What can be built deliberately?)
- **What moats will exist in 24 months?** (What compounds over time?)
- **What moats require scale?** (And what's the minimum scale to activate them?)

### STEP 3b — MOAT VALIDATION GATES

Run these binary checks. Each gate is PASS or FAIL.

| # | Gate | Pass/Fail |
|---|------|-----------|
| 1 | **Real moat exists** — At least one moat dimension is rated "Real" (not all Fake or Buildable) | |
| 2 | **Lock-in mechanism identified** — A specific user-investment lock-in mechanism is identified (not vague "switching costs") | |
| 3 | **Copy protection is real** — The honest answer to "what stops someone from copying this?" is not "nothing", "we move faster", or "first-mover advantage" | |
| 4 | **Buildable within 12 months** — At least one moat is buildable within 12 months of launch | |
| 5 | **Not temporary** — The primary moat does not depend on a temporary advantage (first-mover, feature lead, information asymmetry that erodes) | |

**Gates passed: X/5**

- **5/5**: Strong defensibility foundation
- **3-4/5**: Viable with gaps — address failing gates in the moat-building strategy
- **< 3/5**: RED FLAG — business has no durable defensibility. Discuss explicitly in the Bottom Line.

### STEP 4 — MOAT-BUILDING STRATEGY

For the top 2-3 moat opportunities identified, produce a concrete strategy:

**For each moat opportunity:**
- What specific product decisions strengthen this moat?
- What specific metrics indicate the moat is working?
- What's the investment required (time, money, product changes)?
- When does the moat become significant enough to matter?
- What's the risk if this moat fails to materialize?

### STEP 5 — OUTPUT

Produce the full report using the template below.

## Output Template

```
# MOAT ANALYSIS: [Product/Idea Name]

Research date: [date]
Stage: [Idea / MVP / Live Product]

---

## MOAT REALITY SCORE

Overall defensibility: [STRONG / MODERATE / WEAK / NONE]

| Dimension | Rating | Classification | Notes |
|-----------|--------|---------------|-------|
| User-Investment Lock-In | Strong/Moderate/Weak/None | Real/Weak/Fake/Buildable | |
| Network Effects | | | |
| Data Moat | | | |
| Distribution Moat | | | |
| Counter-Positioning | | | |
| Economies of Scale | | | |
| Regulatory/Compliance | | | |
| Relationship/Trust | | | |
| Process/Operational | | | |

**Real moats (invest here)**: [List dimensions rated Real]
**Buildable moats (design for these)**: [List dimensions rated Buildable]
**Fake moats (stop claiming these)**: [List dimensions rated Fake — be brutal]

---

## USER-INVESTMENT LOCK-IN ASSESSMENT

**Lock-in flywheel present?** YES / PARTIAL / NO

**Stored value analysis:**

| What Users Build/Store | Current State | Switching Cost | Portability |
|-----------------------|---------------|---------------|-------------|
| [Content type] | [exists/planned/absent] | [Very High/High/Medium/Low] | [Locked/Exportable/Portable] |
| [Data type] | | | |
| [Workflow type] | | | |
| [Integration type] | | | |
| [Team adoption] | | | |

**Free-tier lock-in assessment** (if freemium):
- Does the free tier require user investment? [Y/N — what kind?]
- How much time before switching costs become meaningful? [hours/days/weeks/months]
- Does the free plan create enough lock-in to drive upgrades? [Y/N — explain]
- Dual-purpose score: STRONG (free tier is both acquisition AND retention engine) / PARTIAL / WEAK

**Time to lock-in**: [How long before a typical user is meaningfully invested?]
- Day 1: [what they've invested]
- Week 1: [what they've invested]
- Month 1: [what they've invested]
- Month 6+: [what they've invested]

**Lock-in verdict**: [Is this product designed to create user investment that raises switching costs? If not, what product changes would enable it?]

---

## NETWORK EFFECTS ASSESSMENT

**Network effect type**: [Direct / Indirect / Data / Content / Local / None]

[If applicable:]
- Minimum viable network: [how many users before it kicks in]
- Current status: [pre-network / early network / strong network / N/A]
- Bootstrap strategy: [how to seed the initial network]

[If not applicable:]
- Why network effects don't apply to this business
- Whether a data network effect could be engineered

---

## DATA MOAT ASSESSMENT

**Data uniqueness**: [What data does this product generate that competitors can't easily get?]
**Data defensibility**: [Can it be scraped, bought, or synthesized?]
**Data compounding**: [Does more data = better product?]
**Data moat timeline**: [When does the data advantage become meaningful?]

---

## DISTRIBUTION MOAT ASSESSMENT

**Current distribution assets**: [What channels, audience, or brand does the founder/company own?]
**Competitor distribution comparison**: [Who has the strongest distribution moat in this market?]
**Distribution moat buildability**: [What can be built in 6/12/24 months?]
**Channel lock-in**: [Are there marketplace positions, SEO rankings, or partnerships that create distribution barriers?]

---

## COUNTER-POSITIONING ASSESSMENT

**Incumbent vulnerabilities**: [What can't incumbents copy without hurting their own business?]
**Pricing asymmetry**: [Is there a business model that incumbents can't match?]
**Structural advantage**: [What gives a bootstrapper an unfair advantage against funded competitors?]

---

## COMPETITOR MOAT COMPARISON

| Moat Dimension | Our Position | Top Competitor 1 | Top Competitor 2 | Top Competitor 3 |
|---------------|-------------|------------------|------------------|------------------|
| User Investment | | | | |
| Network Effects | | | | |
| Data | | | | |
| Distribution | | | | |
| Counter-Position | | | | |
| Switching Costs | | | | |
| Brand/Trust | | | | |
| Regulatory | | | | |

**Who has the strongest moat in this market?** [Name and why]
**Where are they vulnerable?** [Specific moat gaps we can exploit]

---

## MOAT TIMELINE

| Timeframe | Moat Status | Key Actions |
|-----------|-------------|-------------|
| Today | [What moats exist now?] | [What to protect] |
| 6 months | [What moats should exist?] | [What to build] |
| 12 months | [What moats will compound?] | [What to invest in] |
| 24 months | [Target moat position] | [What should be entrenched] |

---

## MOAT-BUILDING STRATEGY

### Priority 1: [Most important moat to build]
- **Product decisions**: [Specific changes that strengthen this moat]
- **Success metric**: [How to measure if the moat is working]
- **Investment**: [Time, money, product changes required]
- **Timeline**: [When it becomes significant]

### Priority 2: [Second moat to build]
- **Product decisions**: [Specific changes]
- **Success metric**: [How to measure]
- **Investment**: [What it costs]
- **Timeline**: [When it matters]

### Priority 3: [Third moat opportunity]
- **Product decisions**: [Specific changes]
- **Success metric**: [How to measure]
- **Investment**: [What it costs]
- **Timeline**: [When it matters]

---

## MOAT RISKS

| Risk | Impact | Likelihood | Mitigation |
|------|--------|------------|-----------|
| [A competitor replicates our core moat] | | | |
| [Regulatory change eliminates a barrier] | | | |
| [Platform dependency undermines lock-in] | | | |
| [Data becomes commoditized] | | | |
| [AI tools erode our process advantage] | | | |

---

## BOTTOM LINE

**Defensibility verdict**: [STRONG / MODERATE / WEAK / NO MOAT]

**Validation gates passed**: [X/5 — list any failing gates]

[2-3 sentences. Is this business defensible long-term? What's the primary moat? What's the biggest moat risk? If weak, is there a clear path to building defensibility, and how long does it take?]

**The honest answer to "what stops someone from copying this?":**
[One sentence. The real answer, not the comfortable one.]

**Top 3 moat-building actions for the next 90 days:**
1. [Specific, concrete, actionable]
2. [Specific, concrete, actionable]
3. [Specific, concrete, actionable]

---
[If invoked as sub-skill: produce DIGEST summary per `_shared/philosophy.md` Digest Mode format]
```

## Important Rules

See `_shared/philosophy.md` Universal Skill Rules.

**Skill-specific rules:**
- **Be brutally honest about fake moats** — the founder needs truth, not comfort. "Technology advantage" and "first mover" are almost never real moats. Say so.
- **User-investment lock-in is the default focus** — for most bootstrapped SaaS products, this is the most achievable and impactful moat. Assess it deeply.
- **Distribution moat is #1 in the AI age** — when code is cheap, the real question is "can competitors reach YOUR customers?" If they can't, that's a moat.
- **Don't confuse features with moats** — features can be cloned. Moats are structural advantages that compound over time.
- **Name specific competitors** when comparing moats — "competitors have weaker lock-in" is vague. "[Competitor name] allows full data export and has no onboarding investment" is specific.
- **Consider the freemium dual-purpose** — when evaluating products with free tiers, always assess whether the free tier creates lock-in (dual-purpose weapon) or just gives away value with no switching costs (expensive charity).
- **Moat timeline matters** — most bootstrapped businesses start with zero moats. The question is: can you build one in 6-24 months? And will it compound?
