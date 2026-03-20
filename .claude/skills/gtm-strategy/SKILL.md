---
name: gtm-strategy
description: Go-to-market strategy for bootstrapped founders — beachhead selection, GTM motion, channel strategy, message-market fit, funnel design, distribution economics, and concrete launch plan. Use when user runs `/gtm-strategy`, asks about "go to market", "how to reach customers", "distribution strategy", "first customers", "launch plan", "GTM", "channels", "message-market fit", or needs a distribution strategy for a bootstrapped product.
---

# GTM Strategy — Go-to-Market for Bootstrappers

Distribution strategy for founders who fund from customers, not VCs. No SDR army, no $50K/month ad budget, no "growth team." This is GTM for operators: find the buyers, reach them profitably, convert them repeatedly, compound over time.

## Philosophy

**Distribution is the bottleneck.** Read `.claude/skills/_shared/philosophy.md` for the full framework. Code is cheap — the question is never "can we build it?" but "can we reach the people who'll pay for it?"

**Bootstrapped GTM is different from funded GTM:**
- No burning $200K/month on ads to "figure out" channels. Every dollar of CAC must pay back.
- No hiring 5 SDRs and "seeing what sticks." Distribution must be founder-driven early.
- No buying growth with VC money. Revenue funds everything.
- Channels must compound — avoid channels that scale linearly with spend unless the unit economics are rock-solid.
- Speed of iteration > quality of planning. Run the test, don't write the strategy doc about the test. The meeting to discuss a channel takes longer than testing the channel.
- **Action bias always**: Build the landing page, don't write the deck. Send the cold email, don't plan the outreach sequence. The permission loop, the polish cycle, and the planning phase all cost more than the prototype. Default to doing.

**Competition validates distribution paths.** If competitors are acquiring customers, they've already proven which channels work. Study them. Use their playbook. Then out-execute with better economics (lean ops, no bloat, profitable pricing).

## Reference Books

Check `references/INDEX.md` for relevant frameworks. Key topics for GTM: Bullseye framework and traction channels, sales funnels and conversion mechanics, outbound sales and B2B pipeline, stair-step approach, SaaS channel selection, PLG strategy, beachhead segments and chasm crossing, product positioning and differentiation.

## Research-First Protocol

Research autonomously before outputting anything. See `_shared/philosophy.md` for the full protocol.

1. **Use WebSearch** to understand how customers in this market discover and buy products:
   - "[category] how companies choose [product type]"
   - "[category] customer acquisition channels"
   - "[competitor name] marketing strategy" / "[competitor name] how they got first customers"
   - "[category] community forums" / "[category] subreddit"
   - "[category] conferences events"
   - "best [product type] [current year]" (see which channels surface results)
2. **Use WebFetch** to analyze landing pages, ad libraries, and content strategies of relevant players
3. **Check if competitor-analysis has already been run** — if so, pull channel/marketing intelligence from it instead of re-researching
4. **Only ask the user** when information is truly unknowable (budget, time commitment, existing audience, personal network, domain expertise)
5. State research findings and assumptions so the user can correct errors

## Sub-Skill Mode

See `_shared/philosophy.md` Sub-Skill Mode Protocol.

## End-to-End Flow

### STEP 0 — CONTEXT GATHERING

Extract from the user's input:
- The business idea or product (what it does, who it's for)
- Any known target customers or segments
- Founder's distribution assets (existing audience, network, domain expertise, partnerships)
- Budget and time constraints for GTM
- Any existing traction or channels already tested

If the idea description is too vague to identify a buyer, ask ONE clarifying question. Otherwise, proceed to research.

### STEP 1 — MARKET DISTRIBUTION RESEARCH

Research how customers in this market discover, evaluate, and buy products. This informs every section downstream.

**Search queries to run (adapt to the specific market):**
- How do [target buyers] find and choose [product type]?
- What channels do competitors use to acquire customers?
- What communities, forums, events serve this market?
- What content/keywords does this audience search for?
- What does the buying process look like (self-serve vs. sales)?

**From competitor intelligence (if available):**
- Which channels are competitors investing in? (ads, content, outbound, PLG)
- What's their pricing model and entry point? (indicates sales motion)
- Where do they show up? (review sites, directories, marketplaces)

### STEP 2 — EIGHT-DIMENSION GTM ANALYSIS

Work through all eight dimensions sequentially. Each one builds on the previous.

---

#### Dimension 1: Beachhead & ICP

The narrowest viable segment you'll dominate before expanding. One type of buyer, one acute pain, one distribution channel. Trying to serve "everyone" means reaching no one.

**What to research:**
- Who specifically has this problem? (Job title, company size, industry, geography)
- How acute is their pain? (Do they search for solutions? Do they pay for alternatives?)
- How reachable are they? (Do they congregate somewhere? Are there lists, communities, events?)
- How many are there? (Big enough to build a real business, small enough to dominate)
- What's their buying behavior? (Self-serve? Need demos? Budget authority? Procurement process?)

**Beachhead selection criteria:**
- **Urgency**: They need a solution now, not "someday"
- **Reachability**: You can get in front of them through 1-2 specific channels
- **Willingness to pay**: They already pay for alternatives or workarounds
- **Word of mouth**: They talk to each other (industry events, communities, Slack groups)
- **Simplicity**: You can serve them without building enterprise complexity

**What to produce:**
- ICP definition (demographics + psychographics + buying behavior)
- Beachhead segment (the first 100 customers — who exactly)
- Expansion path (beachhead → adjacent segments → broader market)
- Buyer vs. user distinction (if different — who pays, who uses, who champions)

**Bootstrapper lens:**
- Pick the segment you can reach with founder effort, not paid channels
- Prefer segments where the founder has domain credibility or network access
- Prefer segments with short sales cycles (under 30 days from discovery to payment)
- Avoid enterprise initially unless the founder has existing enterprise relationships

---

#### Dimension 2: GTM Motion

The strategic architecture of how you sell. This determines your hiring, pricing, product, and everything downstream.

**Four motions (pick ONE primary, maybe one secondary):**

| Motion | How it works | Bootstrapper fit | When to use |
|--------|-------------|-----------------|-------------|
| **Product-led (PLG)** | Product drives acquisition, activation, expansion. Free tier or trial → self-serve upgrade | Excellent — scales without humans | Product delivers value fast, low-touch, buyers can evaluate alone |
| **Content-led** | SEO, education, and thought leadership drive inbound leads → self-serve or light-touch sales | Excellent — compounds over time, near-zero marginal cost | Buyer researches before buying, searchable pain, long content lifecycle |
| **Community-led** | Build or embed in community → trust → organic adoption | Good — but slow to build, hard to manufacture | Buyer values peer recommendations, strong community exists, founder has credibility |
| **Sales-led** | Outbound or inbound leads → demos → close | Harder bootstrapped — founder must be the salesperson | High ACV ($5K+/yr), complex buying process, relationship-driven market |

**What to research:**
- How do competitors sell? (Self-serve signup? Demo request? Sales team?)
- What does the buyer expect? (Enterprise buyers expect sales calls; developers expect self-serve)
- What's the ACV range? (Under $1K/yr = must be PLG; $1K-$10K = hybrid; $10K+ = sales-led viable)
- Does the product deliver value without configuration? (If yes → PLG. If needs setup → sales-assisted)

**PLG as dual-purpose flywheel (acquisition + lock-in):**

The best freemium strategies serve dual purpose: acquisition (free beats paid) AND retention (user investment creates switching costs). Evaluate PLG viability using the user-investment lock-in checklist in `_shared/philosophy.md`. The key question: does product usage create stored value that makes leaving painful? If the answer is "no," freemium is a cost center, not a weapon.

**Hybrid motions:**
- PLG + content-led is the bootstrapper sweet spot (product converts, content drives awareness)
- PLG + sales-assisted works when ACV justifies occasional human touch (expansion deals, annual contracts)
- Content-led + community-led works in technical/developer markets

**What to produce:**
- Primary motion recommendation with rationale
- Secondary motion (if applicable)
- Why other motions don't fit (or fit later at scale)
- Implications for product (free tier? trial? onboarding investment?)
- Implications for founder time allocation

---

#### Dimension 3: Channel Strategy

Which specific channels reach your ICP? Not all 19 — the 2-3 that matter now.

**Apply the Bullseye framework:**

**Outer ring** (brainstorm — what's plausible?):
Run through all 19 traction channels and quickly assess relevance:

| # | Channel | Relevant? | Notes |
|---|---------|-----------|-------|
| 1 | Viral marketing | | |
| 2 | PR / media | | |
| 3 | Unconventional PR | | |
| 4 | SEO / content marketing | | |
| 5 | Social & display ads | | |
| 6 | Offline ads | | |
| 7 | Search ads (SEM) | | |
| 8 | Affiliate programs | | |
| 9 | Existing platforms (marketplaces, app stores) | | |
| 10 | Trade shows / events | | |
| 11 | Speaking engagements | | |
| 12 | Community building | | |
| 13 | Targeting blogs / publications | | |
| 14 | Sales (outbound) | | |
| 15 | Business development / partnerships | | |
| 16 | Email marketing | | |
| 17 | Engineering as marketing (free tools) | | |
| 18 | Direct outreach (cold email, DMs) | | |
| 19 | Referral programs | | |

**Middle ring** (test candidates — top 5-6 most promising):
For each, estimate:
- **Cost to test**: $0-100 (free), $100-1K (cheap), $1K-5K (moderate), $5K+ (expensive)
- **Time to signal**: Days, weeks, or months before you know if it works
- **Scalability**: Does it compound, or does it require linear spend?
- **Bootstrapper sustainability**: Can a solo/small team run this channel?
- **Competitor presence**: Are competitors already winning here? (Validated but crowded) or absent? (Opportunity or dead end)

**Inner ring** (primary channel — THE ONE that gets most of your energy):
- One channel gets 80% of your distribution effort initially
- Second channel gets 15% as a hedge
- Everything else gets 5% or zero

**What to research:**
- WebSearch for where competitors drive traffic and leads
- WebSearch for "[category] marketing strategy" articles and case studies
- Check if existing platforms/marketplaces exist for this category
- Research community presence (Reddit, Slack groups, Discord, forums, Facebook groups)
- Check SEO landscape (search volume for core keywords, content competition)

**Bootstrapper channel preferences (ranked by sustainability):**
1. SEO / content (compounds, near-zero marginal cost, builds moat)
2. Existing platforms / marketplaces (built-in audience, but platform risk)
3. Community (organic trust, word-of-mouth, but slow)
4. Engineering as marketing (free tools drive leads, compounds)
5. Direct outreach (free but doesn't scale, good for first 20 customers)
6. Referral programs (only works once you have customers)
7. Partnerships / BD (free but relationship-intensive)
8. Paid ads (scales immediately but costs money every month — only if unit economics are proven)

---

#### Dimension 4: Positioning & Message-Market Fit

Positioning is the strategic frame. Message-market fit is the proof that the frame works. You need both.

**Positioning (strategic):**

Apply the positioning framework — five components:

1. **Competitive alternatives**: What would customers use if you didn't exist? (Not just direct competitors — spreadsheets, manual processes, hiring someone, doing nothing)
2. **Unique attributes**: What do you have that alternatives lack? (Not "features" — capabilities, approach, architecture, constraints removed)
3. **Value**: What do those unique attributes enable for the customer? (Outcomes, not features. Time saved, money made, risk reduced, pain eliminated)
4. **Best-fit customers**: Who cares most about this value? (The segment where your unique value matters most — this should align with Dimension 1)
5. **Market category**: What frame helps customers understand what you are? (Existing category, sub-category, or new category — each has trade-offs)

**What to research:**
- How do competitors position themselves? (Headlines, taglines, value props on their websites)
- What language do customers use to describe this problem? (Review sites, Reddit, forums, support tickets)
- What are the most common objections and questions? (FAQ pages, sales call patterns, review complaints)
- What messaging has changed over time? (Wayback Machine — competitors who've shifted positioning are still searching for fit)

**Message-Market Fit (tactical):**

Message-market fit is the alignment between your value proposition and how your target audience thinks, speaks, and decides. When it clicks, prospects understand instantly. When it doesn't, you get blank stares, "interesting, let me think about it," and silent churn.

**Five components of message-market fit:**

| Component | Test | Red Flag |
|-----------|------|----------|
| **Clarity** | Can a buyer understand what you do in 8 seconds? | "So... what exactly does this do?" |
| **Relevance** | Does the buyer immediately see themselves in the message? | "That's cool but not really for us" |
| **Urgency** | Does the message trigger action now, not later? | "I'll check it out sometime" |
| **Differentiation** | Can the buyer tell you apart from alternatives? | "How is this different from [competitor]?" |
| **Credibility** | Does the buyer believe the claim? | "Sounds too good to be true" |

**How to assess message-market fit (research-based):**
- **Landing page test**: If the competitor's homepage headline were your headline, would YOUR buyers care? If yes, you're not differentiated.
- **Review language mining**: Pull exact phrases from G2/Capterra reviews, Reddit posts, and forum complaints. The customer's own words are your best messaging.
- **Objection analysis**: The most common objections reveal where your message fails. Research what questions buyers ask before purchasing in this category.
- **Search intent analysis**: What queries do people type? High search volume for "[category] for [segment]" means the segment is self-identifying. Use their language, not yours.
- **Competitor messaging drift**: Competitors who've changed their homepage headline 3 times in 2 years haven't found message-market fit. That's your opening.

**What to produce:**
- Positioning canvas (five components filled in)
- Primary headline / value prop (one sentence that passes the 8-second test)
- Key messages for the beachhead segment (3-5 supporting points, in the customer's language)
- Differentiation statement (how you're different from the top 2-3 alternatives, not just competitors)
- Message-market fit assessment: Likely / Needs Testing / Unlikely — with rationale
- If "Needs Testing": specific message tests to run (landing page variants, ad copy tests, outreach scripts)

**Bootstrapper lens:**
- Your message must work without a sales team to explain it. If it needs a demo to make sense, the messaging isn't right yet.
- Borrow language directly from customer reviews and complaints about competitors. Don't invent marketing speak.
- Position against the real alternative (often "doing nothing" or "spreadsheet"), not just the closest SaaS competitor.
- If you can't articulate the difference in one sentence, you don't have positioning yet — you have a feature list.

---

#### Dimension 5: Funnel & Conversion

The path from "never heard of you" to "paying customer." Every step has friction. Your job is to reduce friction at each stage.

**Map the funnel for your GTM motion:**

**PLG funnel:**
```
Discovery → Landing page → Signup (free) → Onboarding → Aha moment → Upgrade → Expansion
```

**Content-led funnel:**
```
Search/social → Content → Email capture → Nurture → Trial/signup → Activate → Convert
```

**Sales-led funnel:**
```
Outreach/inbound → Qualify → Demo → Proposal → Negotiate → Close → Onboard
```

**For each stage, assess:**
- **Conversion rate benchmark**: What's typical in this market? (Research competitor funnels, industry benchmarks)
- **Key friction points**: What causes drop-off? (Pricing confusion, complex onboarding, credit card required, slow time-to-value)
- **Trust signals needed**: What proof does the buyer need at each stage? (Social proof, case studies, free trial, money-back guarantee)
- **Time in stage**: How long from discovery to payment? (Same day? 14-day trial? 3-month sales cycle?)

**What to research:**
- Competitor signup flows (WebFetch their signup page — credit card required? How many steps?)
- Competitor onboarding (sign up for free trials where possible)
- Pricing presentation (how competitors frame the upgrade decision)
- Reviews mentioning onboarding quality ("easy to set up" vs "took weeks to configure")

**What to produce:**
- Funnel map with estimated conversion rates per stage
- Top 3 friction points and how to address each
- Time-to-value target (how fast should the buyer experience the core benefit?)
- Pricing presentation strategy (freemium, free trial, money-back guarantee — what fits this market?)
- Trust signals plan (what proof do you need to build, and in what order?)

---

#### Dimension 6: Distribution Economics

Can you acquire customers profitably? If not, nothing else matters.

**Key metrics to estimate:**

| Metric | Formula | Target (bootstrapped) |
|--------|---------|----------------------|
| **CAC** | Total acquisition cost / new customers | Varies — but must be < 1/3 of first-year revenue |
| **LTV** | ARPU x gross margin x avg. lifetime (months) | > 3x CAC for sustainability |
| **LTV:CAC** | LTV / CAC | > 3:1 (healthy) / > 5:1 (excellent) |
| **Payback period** | CAC / (monthly ARPU x gross margin) | < 6 months (bootstrapped must-have) |
| **CAC by channel** | Channel spend / customers from that channel | Varies — rank channels by efficiency |

**Per-channel economics:**
For each channel in the inner/middle ring (from Dimension 3), estimate:
- Cost to acquire one customer through this channel
- Expected volume (customers/month at steady state)
- Scalability curve (does CAC increase with volume?)
- Time to payback through this channel

**What to research:**
- Competitor pricing (informs ARPU assumptions)
- Ad costs for this category (CPC for search ads, CPM for social)
- Content marketing benchmarks (cost per article, typical organic traffic per article)
- Sales cycle length for this buyer (informs payback period)
- Churn benchmarks for this category (informs LTV)

**What to produce:**
- Unit economics table with estimated CAC, LTV, LTV:CAC, payback period
- Per-channel CAC estimates for top 3 channels
- Break-even analysis: How many customers at what price to cover operating costs?
- Cash flow timing: When does revenue from a customer cohort cover acquisition cost?
- Red flags: Any channel where CAC > first-year revenue (unsustainable without funding)

**Bootstrapper lens:**
- Payback period matters more than LTV:CAC. You can't fund 12-month payback periods from cash flow.
- Free channels (SEO, community, referrals) have time cost, not dollar cost. Account for founder hours.
- If CAC is high, the pricing must be high. Don't try to sell $19/month products through sales calls.
- The #1 way to reduce CAC: make the product good enough that customers refer others. Word of mouth is the ultimate bootstrapper channel.

---

#### Dimension 7: First 100 Customers

The first 100 are the hardest. Nothing scales yet. Everything is manual. That's fine.

**Pre-launch (before the product exists or is ready):**
- **Waitlist / landing page**: Validate demand. Collect emails. Test messaging.
- **Founder interviews**: Talk to 20-30 potential buyers. Use their language in your messaging.
- **Content seeding**: Start publishing in the channels you'll use. Build organic presence before launch.
- **Community presence**: Join and contribute to communities where your buyers hang out. Don't sell. Help.

**Launch (first 1-20 customers):**
- **Direct outreach**: Personal emails/DMs to people you've talked to, who have the problem. Not cold spam — warm outreach to people who already told you about their pain.
- **Founder network**: Everyone you know who might know someone who has this problem. Ask for introductions, not purchases.
- **Early adopter deals**: Lifetime deals, steep discounts, or extended trials in exchange for feedback and case studies.
- **Platform launches**: Product Hunt, Hacker News, relevant subreddits, Indie Hackers — one-time bursts of attention.

**Growth (20-100 customers):**
- **Case studies from first 20**: Turn early wins into proof. Specific numbers, specific outcomes.
- **Referral triggers**: Ask happy customers to introduce you to peers. Make it easy (pre-written email, one-click share).
- **Content from customer conversations**: Every customer call is a content idea. Write about the problems they describe.
- **Channel validation**: By customer 50, you should know which 1-2 channels work. Double down.

**What to produce:**
- Week-by-week launch plan (pre-launch → launch → first 100)
- Specific non-scalable tactics (with effort estimates)
- Communities and platforms to target (with URLs where possible)
- Outreach templates or messaging frameworks
- Milestones and decision points (when to double down, when to pivot channels)

---

#### Dimension 8: Compounding & Scale

How distribution grows from 100 to 10,000 customers. The goal: build channels that compound without proportional increase in spend or effort.

**Compounding channels (invest early, harvest later):**
- **SEO / content**: Every article is a permanent asset. Traffic grows monthly. CAC approaches zero for organic visitors.
- **Word of mouth / referral**: Every happy customer is a potential channel. Net promoter flywheel.
- **Community moat**: As your community grows, it becomes harder for competitors to replicate.
- **Data/network effects**: If applicable — more users = more value = more users.
- **Engineering as marketing**: Free tools that drive traffic and leads indefinitely.

**Linear channels (scale with spend):**
- Paid ads (more spend = more leads, but CAC stays flat or rises)
- Outbound sales (more reps = more pipeline, but cost per deal stays constant)
- Events/conferences (each event is a one-time effort)

**Channel stacking strategy:**
- **Phase 1 (0-100)**: One primary channel + founder hustle
- **Phase 2 (100-500)**: Primary channel optimized + one compounding channel started
- **Phase 3 (500-2K)**: Two channels producing reliably + testing a third
- **Phase 4 (2K-10K)**: Three channels, at least two compounding + paid as accelerant

**What to produce:**
- Channel stacking roadmap (which channels when)
- Investment timeline (when each channel starts producing)
- Compounding projections (what organic traffic / referral volume looks like at 12/24 months)
- Scale risks (channel concentration, platform dependency, diminishing returns)
- When to hire (at what revenue level does each channel need a dedicated person?)

---

### STEP 2b — GTM VALIDATION GATES

Run these binary checks before producing output. Each gate is PASS or FAIL.

| # | Gate | Pass/Fail |
|---|------|-----------|
| 1 | **Beachhead specificity** — The beachhead segment is specific enough to find and target individually (not "SMBs", "marketers", or "small businesses") | |
| 2 | **Organic channel exists** — At least one distribution channel can reach the ICP without paid spend | |
| 3 | **CAC payback viable** — Estimated CAC payback period is under 6 months | |
| 4 | **First 100 plan is concrete** — The first 100 customer plan names specific tactics, communities, or channels — not generic advice like "do content marketing" | |
| 5 | **No single-platform dependency** — The primary distribution path does not depend on a single platform the founder does not control | |
| 6 | **Message-market fit is plausible** — Message-market fit verdict is LIKELY or NEEDS TESTING (not UNLIKELY) | |

**Gates passed: X/6**

- **6/6**: Strong GTM foundation — clear path to first customers
- **4-5/6**: Viable with gaps — address failing gates before scaling
- **< 4/6**: RED FLAG — significant distribution risks exist. Discuss explicitly in the Bottom Line.

### STEP 3 — OUTPUT

Produce the full report using the template below.

## Output Template

```
# GTM STRATEGY: [Product/Idea Name]

Research date: [date]

---

## BEACHHEAD & ICP

**Ideal Customer Profile:**
- Job title / role: [specific]
- Company size: [range]
- Industry / vertical: [specific or horizontal]
- Geography: [if relevant]
- Budget authority: [Y/N, procurement process]
- Current solution: [what they use today — competitor, spreadsheet, manual, nothing]

**Beachhead segment**: [The narrowest viable group — who are the first 100?]

**Beachhead drift**: [ALIGNED / DRIFTED — if drifted, which segment does evidence point to and why? See _shared/philosophy.md Beachhead Drift section for drift patterns.]

**Why this beachhead:**
- Urgency: [why they need this now]
- Reachability: [how you get in front of them]
- Willingness to pay: [evidence they pay for alternatives]
- Word of mouth: [do they talk to each other?]

**Expansion path**: [Beachhead → next segment → next → broader market]

**Buyer vs. User**: [Same person? Different? Who champions internally?]

---

## GTM MOTION

**Primary motion**: [PLG / Content-led / Community-led / Sales-led]
**Secondary motion**: [if applicable]

**Why this motion:**
[2-3 sentences on why this fits the product, buyer, and bootstrapper constraints]

**Why NOT the alternatives:**
[Brief dismissal of motions that don't fit, and when they might become relevant]

**Implications:**
- Product: [free tier needed? trial length? onboarding investment?]
- Pricing: [self-serve pricing page? "contact us"? usage-based?]
- Founder time: [% of time on product vs. distribution vs. sales?]

---

## CHANNEL STRATEGY

### Bullseye Assessment

**Inner ring (primary — 80% of effort):**
| Channel | Why | Cost to Test | Time to Signal | Scalability |
|---------|-----|-------------|---------------|-------------|
| [channel] | [rationale] | [estimate] | [estimate] | [compound/linear] |

**Middle ring (test candidates — 15% of effort):**
| Channel | Why | Cost to Test | Time to Signal | Scalability |
|---------|-----|-------------|---------------|-------------|
| [channel] | | | | |
| [channel] | | | | |

**Outer ring (not now — but plausible later):**
[List with brief rationale for deferral]

**Dismissed channels:**
[Channels that don't fit and why — not every channel is relevant]

**Competitor channel intelligence:**
[How are competitors acquiring customers? What channels are validated? What's underutilized?]

---

## POSITIONING & MESSAGE-MARKET FIT

### Positioning Canvas

| Component | Assessment |
|-----------|-----------|
| **Competitive alternatives** | [What buyers use if you don't exist] |
| **Unique attributes** | [What you do that alternatives can't/don't] |
| **Value** | [What those attributes enable — outcomes, not features] |
| **Best-fit customers** | [Who cares most — should align with beachhead] |
| **Market category** | [How buyers should think about what you are] |

### Message-Market Fit Assessment

**Primary value prop**: [One sentence. 8-second test.]

**Supporting messages** (in the customer's language):
1. [Message — tied to a specific pain point]
2. [Message — tied to a specific outcome]
3. [Message — differentiation from alternatives]

**Differentiation statement**: [How you're different from the top alternatives — one sentence]

| MMF Component | Status | Evidence |
|---------------|--------|----------|
| Clarity | Strong / Weak / Unknown | [Can buyer understand in 8 sec?] |
| Relevance | Strong / Weak / Unknown | [Does buyer see themselves?] |
| Urgency | Strong / Weak / Unknown | [Does it trigger action now?] |
| Differentiation | Strong / Weak / Unknown | [Can buyer tell you apart?] |
| Credibility | Strong / Weak / Unknown | [Does buyer believe the claim?] |

**Message-market fit verdict**: LIKELY / NEEDS TESTING / UNLIKELY

**If NEEDS TESTING — test plan:**
[Specific message tests: landing page variants, ad copy A/B, outreach script variants, what metrics to watch]

---

## FUNNEL & CONVERSION

**Funnel map:**
```
[Stage 1] → [Stage 2] → [Stage 3] → [Stage 4] → [Stage 5]
  est. X%      est. X%      est. X%      est. X%
```

**Top 3 friction points:**
| # | Friction Point | Impact | Mitigation |
|---|---------------|--------|-----------|
| 1 | | | |
| 2 | | | |
| 3 | | | |

**Time-to-value target**: [How fast should buyer experience the core benefit?]

**Pricing presentation**: [Freemium / free trial / money-back / paid-only — what fits and why]

**Trust signals needed** (in priority order):
1. [Most important proof point to build first]
2. [Second]
3. [Third]

---

## DISTRIBUTION ECONOMICS

| Metric | Estimate | Benchmark | Verdict |
|--------|---------|-----------|---------|
| ARPU (monthly) | | | |
| Estimated CAC | | | |
| LTV (12-month) | | | |
| LTV:CAC | | | Healthy / Warning / Red flag |
| Payback period | | | Healthy / Warning / Red flag |

**Per-channel economics:**
| Channel | Est. CAC | Volume potential | Scalability | Verdict |
|---------|---------|----------------|-------------|---------|
| [channel 1] | | | | |
| [channel 2] | | | | |
| [channel 3] | | | | |

**Break-even**: [X customers at $Y/month to cover operating costs of $Z/month]

**Cash flow timing**: [When does a customer cohort pay back its acquisition cost?]

**Red flags**: [Any unsustainable economics identified]

---

## FIRST 100 CUSTOMERS

### Pre-Launch (Weeks 1-4)
| Tactic | Effort | Expected Result |
|--------|--------|----------------|
| | | |

### Launch (Weeks 5-8)
| Tactic | Effort | Expected Result |
|--------|--------|----------------|
| | | |

### Growth to 100 (Weeks 9-20)
| Tactic | Effort | Expected Result |
|--------|--------|----------------|
| | | |

**Communities & platforms to target:**
[Specific URLs, groups, forums — not generic "social media"]

**Key milestones:**
- [ ] First 10 customers by [week]
- [ ] First paying customer by [week]
- [ ] Channel validation signal by [week]
- [ ] 100 customers by [week]

**Decision points:**
- If [primary channel] hasn't produced [X] by [week Y]: [pivot to what]
- If CAC exceeds [threshold]: [action]

---

## COMPOUNDING & SCALE

**Channel stacking roadmap:**
| Phase | Customer Range | Primary Channel | Secondary | Investment |
|-------|---------------|----------------|-----------|------------|
| 1 | 0-100 | | Founder hustle | $[X]/month + [Y] hrs/week |
| 2 | 100-500 | | | |
| 3 | 500-2K | | | |
| 4 | 2K-10K | | | |

**Compounding projections:**
- 6 months: [expected organic/referral volume]
- 12 months: [expected organic/referral volume]
- 24 months: [expected organic/referral volume]

**Scale risks:**
| Risk | Likelihood | Impact | Mitigation |
|------|-----------|--------|-----------|
| Channel concentration | | | |
| Platform dependency | | | |
| Diminishing returns | | | |

**Hiring triggers:**
| Role | When to hire | Revenue trigger | What they own |
|------|------------|----------------|--------------|
| | | | |

---

## BOTTOM LINE

**Distribution verdict**: [CLEAR PATH / PLAUSIBLE / UNCLEAR / BLOCKED]

**Validation gates passed**: [X/6 — list any failing gates]

[2-3 sentences. Is there a viable path to 100 paying customers with bootstrapper resources? What's the primary distribution advantage? What's the biggest distribution risk?]

**The honest answer to "can we reach paying customers?":** [One sentence]

**Top 3 actions for the next 30 days:**
1. [Specific, concrete, actionable]
2. [Specific, concrete, actionable]
3. [Specific, concrete, actionable]

---
[If invoked as sub-skill: produce DIGEST summary per `_shared/philosophy.md` Digest Mode format]
```

## Important Rules

See `_shared/philosophy.md` Universal Skill Rules.

**Skill-specific rules:**
- **Be specific** — "join the Shopify Partners Slack community" not "engage with relevant communities"
- **Name real channels, real platforms, real communities** — no abstract "leverage social media"
- **Bootstrapper economics always** — if a channel requires $10K/month to test, say so and flag it as expensive
- **Honest assessments** — if distribution looks hard, say so. Don't invent easy paths that don't exist.
- **Message in the customer's language** — mine reviews, forums, and Reddit for exact phrases. Don't write marketing copy from imagination.
- **First 100 > first 10,000** — the launch plan must be concrete and achievable with founder effort alone. Scale comes later.
- **One channel first** — resist the urge to recommend 5 channels simultaneously. Bootstrappers don't have the bandwidth. Pick one, prove it, then stack.
- **No vanity metrics** — followers, impressions, and traffic don't matter. Paying customers matter. Frame everything in terms of revenue impact.
