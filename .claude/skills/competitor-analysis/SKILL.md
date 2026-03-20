---
name: competitor-analysis
description: Deep competitive intelligence skill that analyzes competitors across 16 dimensions — funding, team, pricing, SEO, ads, reviews, tech stack, product, and more. Use when user runs `/competitor-analysis`, asks to "analyze the competition", "who are the competitors", "competitive landscape", "competitor research", or needs deep intelligence on who they're up against. Red ocean philosophy — competition is validation.
---

# Competitor Analysis — Deep Competitive Intelligence

Comprehensive competitor intelligence for bootstrapped founders entering established markets. We are sharks — we compete, we welcome competition, and we outperform. No competitors = red flag (unvalidated market). VC-backed competitors = advantage (they overspend, we compete on price).

## Philosophy

**Red ocean, not blue ocean.** Blue oceans are unvalidated — that's for unicorn hunters. We thrive in proven markets with paying customers. Competition proves demand exists. Our job is to find where competitors are weak, where they over-serve, where they bleed money, and where we can win.

**VC-backed competitors are a gift:**
- They overhire and overspend (bloated cost structure)
- They can't sustain low prices forever (burn rate catches up)
- They chase growth metrics, not profitability (misaligned incentives)
- They move slowly (board approvals, consensus culture)
- They can't compete with freemium models (unit economics don't work at their burn rate)
- We can undercut them and still be profitable

**When code is cheap, competitive advantages shift.** Read `.claude/skills/_shared/philosophy.md` for the full bottleneck shift framework. For competitor analysis specifically:
- **Engineering team size is a dissolving advantage** — headcount signals burn rate, not capability
- **Technical moats are temporary** — any feature can be replicated in days. Distribution, data, relationships, and user-investment lock-in are what matter.

**No competitors is the real danger.** If nobody is solving this problem, either:
1. The problem isn't painful enough to pay for
2. The market is too small to sustain a business
3. Everyone who tried has failed (find out why)

## Reference Books

Check `references/INDEX.md` for relevant frameworks. Key topics for competitive intelligence: Five Forces and industry structural analysis, competitive positioning and differentiation, value curve analysis and strategic canvas, barriers to entry and moat assessment, good strategy vs. bad strategy, intangible economy dynamics, product positioning and value mapping.

## Research-First Protocol

Research autonomously before outputting anything. See `_shared/philosophy.md` for the full protocol.

1. **Use WebSearch** to find competitors, funding data, pricing, reviews, news, team info
2. **Use WebFetch** to analyze competitor websites, pricing pages, ad libraries, job postings
3. **Form hypotheses** about competitive dynamics, then validate with data
4. **Only ask the user** when information is truly unknowable (e.g., which competitors they already know about, their specific geographic advantage, their cost structure)
5. State research findings and assumptions so the user can correct errors

## Sub-Skill Mode

See `_shared/philosophy.md` Sub-Skill Mode Protocol.

## End-to-End Flow

### STEP 0 — CONTEXT GATHERING

Extract from the user's input:
- The business idea or market being entered
- Any known competitors
- The user's geographic location and cost advantage (if stated)
- Specific competitive questions they want answered

If the market description is too vague to identify competitors, ask ONE clarifying question. Otherwise, proceed to research.

### STEP 1 — COMPETITOR DISCOVERY (research phase)

Use WebSearch to build a comprehensive competitor roster:

**Search queries to run (adapt to the specific market):**
- "[market/category] software companies"
- "[market/category] SaaS alternatives"
- "best [product type] tools [current year]"
- "[market/category] competitors comparison"
- "[known competitor] alternatives"
- "G2 [market category] grid"
- "Capterra [market category] top rated"
- Crunchbase search for funded companies in the space

**Categorize every competitor found:**
- **Direct competitors** — Same product, same market, same customer
- **Indirect competitors** — Different product, same job-to-be-done
- **Adjacent competitors** — Same product, different market (could expand)

**Aim for 5-10 direct competitors minimum.** If fewer exist, expand to indirect and adjacent.

### STEP 2 — PER-COMPETITOR DEEP DIVE (16 dimensions)

For each major competitor (top 5-7), analyze across all 16 dimensions. Use WebSearch and WebFetch actively throughout.

---

#### Dimension 1: Company Profile & Funding

**What to research:**
- Founded when, by whom, where (Crunchbase, LinkedIn, company website)
- Total funding raised, round history, lead investors, last raise date
- Revenue estimates if available (press, interviews, leaked data)
- Bootstrapped vs. VC-backed vs. PE-backed vs. public

**What to look for:**
- Recent large raise = 18-24 months of aggressive spend coming
- No funding + sustained growth = profitable and dangerous
- Series B+ with no revenue disclosure = burn-heavy, unsustainable
- Down rounds or flat extensions = struggling
- PE ownership = cost-cutting, price hikes coming

**Bootstrapper signal:**
- VC-backed competitor → **PLUS** (we compete on price, they can't sustain low margins)
- Bootstrapped competitor → **NEUTRAL** (respect them, they know the game)
- PE-backed competitor → **WATCH** (they'll optimize ruthlessly)

---

#### Dimension 2: Team & Location Intelligence

**What to research:**
- Founding team backgrounds (Crunchbase, LinkedIn, company website)
- Domain expertise: Do founders have experience in the sector?
- Total headcount (LinkedIn company page)
- Department breakdown: Engineering vs. Sales vs. Marketing ratio
- Hiring patterns: What roles are they posting? (LinkedIn Jobs, company careers page)
- **Geographic location of founders and team** (LinkedIn profiles, company About page, job postings)

**Location cost intelligence:**
| Location Tier | Examples | Signal |
|---------------|----------|--------|
| **Tier 1 ($$$$)** | San Francisco, New York, London, Zurich, Singapore | Extremely high overhead — salaries 2-4x global average |
| **Tier 2 ($$$)** | Berlin, Amsterdam, Sydney, Toronto, Tel Aviv | High overhead — salaries 1.5-2.5x global average |
| **Tier 3 ($$)** | Lisbon, Prague, Warsaw, Buenos Aires, Mexico City | Moderate overhead — competitive salaries at lower cost |
| **Tier 4 ($)** | Thailand, Indonesia, Philippines, India, Ukraine, Vietnam | Lean operations — maximum cost efficiency |

**What this reveals:**
- US-based team of 50 = ~$7-10M/yr payroll overhead minimum
- Same team in SE Asia = ~$1.5-3M/yr — they can operate at 3-5x lower cost
- Location mismatch (VC funding + expensive HQ) = cost vulnerability we can exploit
- Remote-first teams are harder to undercut on cost (they may already be optimized)

**Hiring pattern intelligence:**
- Engineering hiring = new product development
- Sales/AE hiring = scaling revenue (sales-led motion)
- CSM/Support hiring = churn problems or scaling accounts
- Executive hires (CFO, COO) = preparing for raise or exit
- No hiring = plateau, runway conservation, or bootstrapped efficiency

**Bootstrapper signal:**
- Expensive HQ + large team → **PLUS** (high burn, we compete on price)
- Remote-first + lean team → **CAUTION** (cost-efficient competitor, harder to undercut)
- Founders without domain expertise → **OPPORTUNITY** (we can out-execute with deeper knowledge)

---

#### Dimension 3: Website & Messaging

**What to research (WebFetch their homepage, pricing page, about page):**
- Headline messaging: What problem do they claim to solve, and for whom?
- Value proposition: How do they differentiate?
- Customer segmentation: SMB, mid-market, enterprise?
- Feature hierarchy: What gets top billing?
- Changelog/updates cadence: How fast do they ship?
- Historical positioning: Check Wayback Machine (web.archive.org) for messaging drift

**What this reveals:**
- Public pricing = self-serve confidence (product-led growth)
- "Contact sales" pricing = enterprise dependency (high-touch, long cycles)
- Frequent messaging changes = struggling to find positioning
- Changelog velocity = resource allocation and engineering investment

---

#### Dimension 4: Pricing Intelligence

**What to research (WebFetch their pricing page):**
- Public vs. "contact sales"
- Number of tiers and tier names
- Value metric (per seat, per usage, per feature, flat rate)
- Entry price point and "most popular" tier
- Annual vs. monthly pricing and discount depth
- Free tier or trial structure (self-serve vs. gated demo)
- Feature gating: What's in free/starter vs. premium/enterprise?
- Historical pricing: Wayback Machine for price changes over time

**What this reveals:**
- Deep annual discounts (30%+) = cash flow urgency
- Frequent price changes = haven't found pricing-market fit
- Credit card required for trial = low trial-to-paid conversion or revenue urgency
- No free tier = high-touch sales dependency

**Bootstrapper pricing strategy:**
- If they're expensive → undercut and capture price-sensitive segment
- If they have no free tier → offer freemium (we can afford it, VC-backed can't)
- If pricing is opaque → make yours transparent (trust signal)
- If pricing is per-seat → offer flat-rate (simpler, predictable)

---

#### Dimension 5: Product Intelligence

**What to research:** Research the product experience through G2/Capterra walkthrough reviews, YouTube product demos and walkthroughs, Product Hunt launch videos, onboarding teardowns on blogs, and screenshot galleries. Look for:
- Sign-up friction: Email only, or credit card required?
- Onboarding flow: Interactive tour, video walkthrough, or blank dashboard?
- Time to first value: How fast to the "aha moment"?
- Feature depth vs. simplicity
- UX/UI quality: Polished or janky?
- Mobile experience (if applicable)
- Integrations: What tools do they connect with?
- API availability and documentation quality

**What this reveals:**
- Frictionless signup + no credit card = PLG confidence
- Weak onboarding = churn risk (opportunity to win their frustrated users)
- Aggressive sales follow-up after trial = sales-led dependency
- Poor mobile experience = opportunity if mobile matters in your market

---

#### Dimension 6: SEO & Content Strategy

**What to research:**
- Domain authority / domain rating (estimate from web research)
- Content velocity: Blog frequency and quality
- Keyword targeting: Category keywords, long-tail, competitor terms
- Content types: Blog, guides, case studies, comparison pages, glossary/pillar pages
- Backlink profile: Who links to them? (press, partners, directories)
- On-page SEO: Title tags, meta descriptions, schema markup
- International SEO: Multiple languages, regional targeting

**What this reveals:**
- High DA + low traffic = legacy brand coasting (opportunity to out-content)
- Low DA + high traffic = paid acquisition dependent (vulnerable to budget cuts)
- Strong content velocity = inbound focus (lower CAC, sustainable)
- No blog presence = enterprise sales motion (not relying on organic)
- Comparison pages for rivals = sophisticated SEO strategy

---

#### Dimension 7: AI/LLM Discoverability

**How to test:**
- Query ChatGPT, Perplexity, Claude with category searches:
  - "Best [product category] for [target customer]"
  - "Top [product type] tools [current year]"
  - "[Product category] comparison"
- Note which competitors get mentioned, cited, or recommended
- Check if competitors have structured data, FAQ schema, comparison content optimized for AI scraping

**What this reveals:**
- AI citation = the new SEO — if they're mentioned and you're not, you're invisible
- Strong documentation and recent content = Perplexity/Claude visibility
- Wikipedia presence = ChatGPT visibility
- Review site presence (G2, Capterra) influences AI recommendations

---

#### Dimension 8: Ad Spend & Paid Channels

**Check these ad transparency libraries:**
- **Meta Ad Library**: https://www.facebook.com/ads/library (Facebook, Instagram, Messenger ads)
- **Google Ads Transparency Center**: https://adstransparency.google.com (Search, Display, YouTube ads)
- **TikTok Creative Center**: TikTok ad library (primarily EU/UK access)
- **LinkedIn**: Search company pages for active ad campaigns

**What to analyze:**
- Are they running ads at all? On which platforms?
- Ad creative: Pain points, benefits, CTAs used
- Ad consistency: Running for 6+ months = proven unit economics
- Ad volume: 10+ active ads = mature A/B testing operation
- Ad gaps: No ads for months then sudden spikes = seasonal or fundraise-driven
- Geographic targeting: Where are they spending?

**Bootstrapper signal:**
- Sustained ad spend (6+ months) = most reliable indicator of business health
- Heavy paid spend + VC funding = burning cash for growth metrics
- No paid ads + growing = organic/referral engine (harder to compete, but also harder to scale fast)

---

#### Dimension 9: Social Media Presence

**Which platforms to check:**
- **LinkedIn** (B2B primary): Company page, founder personal brand, engagement
- **Twitter/X** (secondary): Product updates, developer community, support
- **YouTube** (content): Product demos, webinars, customer stories
- **Reddit** (community): Mentions in relevant subreddits, sentiment
- **Instagram/TikTok** (B2C/PLG): If relevant to the market

**What to measure:**
- Follower count (directional, not definitive)
- Engagement rate: Likes, comments, shares per post
- Content cadence and consistency
- Founder-led vs. brand-led social (founder-led = earlier stage, more authentic)
- Community engagement: Do they respond to comments?

---

#### Dimension 10: Review Mining

**Platforms to check:**
- **G2** (https://www.g2.com) — Startup/SMB focused, US-heavy
- **Capterra** (https://www.capterra.com) — SMB, global reach
- **Trustpilot** (https://www.trustpilot.com) — Consumer-facing SaaS
- **TrustRadius** (https://www.trustradius.com) — Enterprise, more technical depth
- **Product Hunt** — Launch reception, community sentiment

**What to mine from reviews:**
- **Feature gaps**: "I wish it had X" = roadmap intel for you
- **Pain points**: "Support is slow", "Pricing is confusing" = differentiation opportunities
- **Churn signals**: "We switched because..." = their vulnerability, your opening
- **Customer segments**: Job titles, company sizes, industries of reviewers
- **Sentiment trajectory**: Getting better or worse over time?

**Bootstrapper signal:**
- High review count + low rating = churn problem (steal their frustrated customers)
- Low review count + high rating = niche or early-stage (limited traction)
- Specific complaints that repeat = systemic issues they can't/won't fix

---

#### Dimension 11: Tech Stack

**Tools to use:**
- **BuiltWith** (https://builtwith.com) — Deep infrastructure detection
- **Wappalyzer** (https://www.wappalyzer.com) — Client-side tech, browser extension
- Manual inspection: Check page source, network requests

**What to look for:**
- Hosting: AWS, GCP, Azure, Vercel (scale and burn rate)
- Framework: React, Vue, Rails, Django (hiring pool and velocity)
- Analytics: Segment, Mixpanel, Amplitude (data maturity)
- CRM: Salesforce, HubSpot, Pipedrive (sales motion)
- Support: Intercom, Zendesk, Drift (customer touch model)
- Payment: Stripe, Paddle, Chargebee (monetization infrastructure)

**What this reveals:**
- Expensive tools (Segment, Amplitude, Salesforce) = well-funded or profitable
- Cheap tools (GA, Mailchimp) = bootstrapped or scrappy
- Modern stack = fast iteration; legacy stack = technical debt and slower shipping

---

#### Dimension 12: Community & Developer Presence

**Where to check:**
- **GitHub**: Stars, forks, contributors, commit velocity, issue response time, documentation quality
- **Stack Overflow**: Competitor mentions, troubleshooting volume
- **Discord/Slack**: Community size, activity level, founder presence
- **Product Hunt**: Launch history, upvotes, awards
- **Developer docs**: API documentation quality (if applicable)

**What this reveals:**
- Active community = product-led growth with organic evangelism
- No community = sales-led motion (top-down selling, not grassroots)
- High GitHub issues + slow response = understaffed or deprioritizing developers
- Multiple Product Hunt launches = iterating publicly (or desperate for traction)

---

#### Dimension 13: Customer Intelligence

**What to research:**
- Customer logos on homepage (SMB vs. enterprise, industry verticals)
- Case studies: What outcomes do they claim? What metrics?
- Testimonials: Job titles, company sizes — who are the champions?
- Customer segments: Horizontal (all industries) vs. vertical (specific niche)
- Partnership page: Who do they integrate with? Whose ecosystem are they in?

**What this reveals:**
- Enterprise logos = upmarket positioning (high ACV, long cycles, complex sales)
- SMB testimonials = volume play (low ACV, fast cycles, self-serve)
- Metrics-heavy case studies = ROI-focused buyers (mature market)
- Vague testimonials = early-stage or weak proof

---

#### Dimension 14: Traffic & Distribution

**What to research (use web search for estimates):**
- Monthly traffic estimates
- Traffic source breakdown: Direct, organic, paid, referral, social
- Geographic distribution
- Traffic trend: Growing, flat, declining?

**What this reveals:**
- High traffic + low engagement = SEO spam or weak product
- Organic-dominant = sustainable, compounding growth (harder to disrupt)
- Paid-dominant = CAC-dependent, vulnerable to budget cuts
- Referral traffic = strong partnerships or affiliate program

---

#### Dimension 15: Switching Cost Assessment

**Evaluate for each competitor:**

| Switching Cost Type | What to Check |
|---------------------|---------------|
| **Financial** | Annual contracts, early termination fees, sunk implementation costs |
| **Technical** | Data portability (easy export?), API dependencies, integration depth |
| **Psychological** | Comfort with status quo, learning curve of alternatives, brand trust |

**Strategic implications:**
- Low switching costs = easier to steal their customers (attack here first)
- High switching costs = harder to steal but stickier once you acquire
- Offer migration assistance, data import tools, and risk-reversal to lower perceived switching cost

---

#### Dimension 16: OSINT Signals

**Additional intelligence to gather:**
- **Domain age**: Whois lookup — older = more established
- **Glassdoor reviews**: Employee satisfaction, culture problems, leadership issues
- **Job board monitoring**: Indeed, LinkedIn Jobs — what they're hiring for reveals strategy
- **Patent/trademark filings**: Deep R&D investment, brand expansion plans
- **Podcast appearances**: Search for founder interviews — revenue disclosures, strategy leaks
- **Conference presence**: Which events they sponsor/speak at (industry focus, budget)
- **Status pages**: Uptime transparency = operational maturity
- **Changelog/release notes**: Feature velocity, customer-requested features

---

### STEP 3 — STRATEGIC ANALYSIS

After gathering per-competitor intelligence, apply these frameworks:

#### Competitive Positioning Map
Plot competitors on a 2-axis grid using the two dimensions that matter most in this market (e.g., Price vs. Feature Depth, Ease-of-Use vs. Power, SMB vs. Enterprise focus). Identify:
- Where competitors cluster (crowded, fight-for-scraps zone)
- White space (underserved segments)
- Your target position

#### Value Curve Analysis
For 8-12 factors the industry competes on, rate each competitor's delivery (1-5). Then apply:
- **Eliminate**: What can we remove that the industry takes for granted?
- **Reduce**: What can we offer below industry standard?
- **Raise**: What can we elevate above industry standard?
- **Create**: What can we offer that nobody else does?

#### Moat Assessment
For each competitor, assess moat reality:
- **Real moats**: Network effects, data advantages, switching costs, regulatory barriers, brand with pricing power
- **Fake moats**: "First mover", "great team", "AI/ML" (using the same APIs as everyone), "technology advantage"
- Rate each: Strong / Weak / Fake

#### Marketplace & Directory Opportunity Assessment

**When the idea targets an app marketplace or plugin directory** (Shopify App Store, WooCommerce Extensions, WordPress Plugins, Chrome Web Store, browser extension stores, Slack App Directory, Zapier integrations, etc.), analyze the marketplace itself as a competitive landscape:

**1. Search & Saturation**
- Run the core category search on the marketplace. How many results?
- Filter for actually relevant apps (marketplace search is noisy — many results are unrelated)
- **Sweet spot**: Enough relevant competitors to validate demand (3-15), few enough that a quality entrant can rank. 100+ relevant results = saturated category.
- Zero results = unvalidated demand on this channel — red flag, not opportunity.

**2. Quality Badge & Certification Status**
- Do the top results have the marketplace's quality badge/certification?
  - Shopify: "Built for Shopify" badge
  - WordPress: "Featured" or recommended status
  - Chrome: "Featured" badge
  - Other marketplaces: equivalent quality certifications
- If top competitors LACK the badge: ranking opportunity — earn the badge, get algorithmic boost, signal quality that incumbents don't have.
- If top competitors HAVE the badge: higher bar to compete, but still possible on other dimensions.

**3. Rating & Review Pattern**
- High review count + mediocre/low ratings = **frustrated demand** — people need the solution but hate what exists. This is the ideal entry signal.
- High review count + high ratings = tough incumbents, need strong differentiation to win.
- Low review count = early/unproven category on this marketplace, or low demand.
- Read the negative reviews specifically — they're your product roadmap.

**4. Pricing Gap**
- Do top apps have free tiers or freemium models?
- If all incumbents are paid-only: freemium is an immediate competitive wedge (same playbook as RevenueHunt entering Shopify quiz market).
- If incumbents are overpriced relative to value: undercut and capture the price-sensitive segment.
- Check if pricing is transparent or "contact sales" — transparency wins in marketplaces.

**5. UX & Design Quality**
- Are top apps modern, well-designed, and polished? Or outdated and clunky?
- Poor UX in incumbents = quality wedge. A well-designed app stands out visually in marketplace listings and converts better.
- Check screenshots, demo videos, and if possible trial the top apps.

**6. Marketplace Algorithm Signals**
- What does the marketplace's ranking algorithm reward? (reviews, installs, recency, quality badges, retention, support responsiveness)
- Which signals can you win on from day one vs. which require time to build?

**For non-marketplace competitors** (standalone SaaS, web apps not listed in marketplaces):
- Check rating platforms (Trustpilot, G2, Capterra, Product Hunt) for quality signals
- Poorly rated SaaS with high traffic/usage = demand exists, quality is poor — same opportunity pattern as marketplace apps with bad reviews
- A competitor with a bad Trustpilot score but strong traffic is a customer acquisition opportunity

#### Idea-Specific Gap Assessment

**When analyzing for a specific business idea** (not just a market), assess how the idea fits into the competitive landscape:

- **White space fit**: Does the idea target an identified underserved segment, or does it enter a crowded quadrant on the positioning map?
- **Displacement potential**: Which competitors' customers would realistically switch to this idea, and why? (price, simplicity, feature gap, frustration)
- **Minimum viable differentiation**: What must this idea do differently from existing competitors to survive? What's the minimum bar?
- **Positioning defensibility**: Can the proposed position hold as competitors react? Or is it easily copied/countered?

This assessment bridges competitive intelligence and idea evaluation — it answers "given this competitive landscape, does THIS specific idea have room to win?"

#### Market Concentration
If enough data exists, estimate:
- **CR4** (top 4 competitors' combined market share): <40% fragmented, >60% concentrated
- **Implications**: Fragmented = niche dominance play; concentrated = attack from edges

### STEP 3b — COMPETITIVE LANDSCAPE VALIDATION GATES

Binary pass/fail gates. Check each honestly.

- [ ] **Gate 1 — Market validated**: At least 3 direct competitors exist with paying customers
- [ ] **Gate 2 — Intelligence depth**: Pricing data verified from primary sources (pricing pages, not estimates) for top 3 competitors
- [ ] **Gate 3 — Exploitable weakness**: At least one concrete competitor weakness is actionable (not just "they're expensive")
- [ ] **Gate 4 — Entry not blocked**: No monopoly, duopoly, or regulatory barrier prevents a new entrant
- [ ] **Gate 5 — Bootstrapper wedge exists**: A viable competitive angle exists that doesn't require VC-scale spend (price, niche, UX, channel)

**Threshold:**
- 5/5: Strong competitive landscape for entry
- 3-4/5: Viable with gaps — name the failing gates and what they mean
- < 3/5: **RED FLAG — competitive landscape may not support entry.** Explain which gates fail and whether they're fixable.

### STEP 4 — OUTPUT

Produce the full report using the template below.

## Output Template

```
# COMPETITIVE INTELLIGENCE: [Market/Idea Name]

Research date: [date]
Competitors analyzed: [count]

---

## RED OCEAN VALIDATION

Is this market validated?
- [ ] Multiple competitors exist with paying customers
- [ ] At least one competitor is profitable or well-funded
- [ ] Customers already pay for this type of solution
- [ ] Market is large enough to support another player

If fewer than 2 boxes are checked: **RED FLAG — market may not be validated.**

---

## COMPETITOR ROSTER

| # | Competitor | Founded | HQ / Team Location | Headcount | Funding | Est. Revenue | Pricing Model | Entry Price | Primary Channel |
|---|-----------|---------|-------------------|-----------|---------|-------------|---------------|-------------|----------------|
| 1 | | | | | | | | | |
| 2 | | | | | | | | | |
| ... | | | | | | | | | |

**Cost Structure Signal:**
[Summary of competitor team locations and what this means for their cost overhead. Which are based in expensive locations? Which are lean? What pricing pressure can we apply?]

---

## PER-COMPETITOR DEEP DIVES

### [Competitor 1 Name]

**Profile**: [1-line summary — what they do, who they serve, how they're funded]

**Funding & Corporate**: [Bootstrapped/VC/PE, total raised, last round, key investors]

**Team**: [Headcount, key people, domain expertise, HQ location, cost tier]

**Pricing**: [Model, tiers, entry point, free tier Y/N, value metric]

**Product**: [Core features, UX quality, onboarding experience, key differentiator]

**GTM Motion**: [Sales-led / Product-led / Marketing-led, primary channels]

**SEO & Content**: [Domain strength, content strategy, ranking keywords]

**AI Visibility**: [Mentioned in ChatGPT/Perplexity/Claude? Y/N — for what queries?]

**Ad Spend**: [Active ads? Platforms? Duration? Creative approach?]

**Reviews**: [G2/Capterra rating, review count, top complaints, top praise]

**Tech Stack**: [Key technologies detected]

**Community**: [GitHub, Discord/Slack, developer presence]

**Customers**: [Key logos, segments, case study highlights]

**Moat Assessment**: [Real moat: _____ / Fake moat: _____ / No moat: _____]

**VULNERABILITIES** (where they're weak):
1. [Vulnerability 1]
2. [Vulnerability 2]
3. [Vulnerability 3]

**THREAT LEVEL**: [High / Medium / Low] — [1-line rationale]

[Repeat for each major competitor]

---

## COMPETITIVE POSITIONING MAP

[Describe the 2-axis positioning map]

**X-axis**: [Dimension 1 — e.g., Price (Low → High)]
**Y-axis**: [Dimension 2 — e.g., Feature Depth (Simple → Complex)]

| Quadrant | Competitors | Opportunity |
|----------|------------|-------------|
| Low price, Simple | | |
| Low price, Complex | | |
| High price, Simple | | |
| High price, Complex | | |

**White space identified**: [Where no competitor sits — your entry point]

---

## VALUE CURVE ANALYSIS

| Factor | Competitor 1 | Competitor 2 | Competitor 3 | Industry Avg | OUR STRATEGY |
|--------|-------------|-------------|-------------|-------------|-------------|
| Price | | | | | Eliminate / Reduce / Raise / Create |
| Features | | | | | |
| Ease of Use | | | | | |
| Support | | | | | |
| Integrations | | | | | |
| Onboarding | | | | | |
| Customization | | | | | |
| Brand/Trust | | | | | |
| [Market-specific] | | | | | |

**Strategic divergence**: [How our value curve should look different from the industry]

---

## BOOTSTRAPPER ADVANTAGE MATRIX

| Competitor | Their Weakness | Our Advantage | How to Exploit |
|-----------|---------------|---------------|----------------|
| | VC burn rate / expensive HQ | Lean ops, profitable pricing | Undercut by X%, offer freemium |
| | Slow shipping / complex product | Speed, simplicity | Ship faster, focus on core JTBD |
| | Enterprise-only / no self-serve | SMB self-serve | PLG with transparent pricing |
| | US-based team ($$$) | [Our location] team ($) | Compete on price, reinvest margin |

---

## MARKETPLACE OPPORTUNITY ASSESSMENT

[Only include when the idea targets an app marketplace or plugin directory]

**Marketplace(s) analyzed**: [Shopify App Store / WooCommerce Extensions / WordPress Plugins / etc.]

| Signal | Finding | Opportunity? |
|--------|---------|-------------|
| **Category search results** | [X relevant apps out of Y total results] | Validated / Saturated / Unproven |
| **Quality badge status** | [Do top apps have the badge? Which ones?] | Badge gap exists / No gap |
| **Rating pattern** | [Top apps: avg rating, review count, trend] | Frustrated demand / Well-served / Unproven |
| **Pricing gap** | [Free tiers available? Price range of top apps] | Freemium wedge / Undercut possible / No gap |
| **UX quality** | [Top apps: modern or dated? Design quality?] | Quality wedge / No gap |
| **Ranking signals** | [What the algorithm rewards, what we can win on] | [Key levers] |

**Non-marketplace quality signals** (Trustpilot, G2, Capterra):
[Any competitors with high traffic/usage but poor ratings on review platforms — indicates demand with quality gap]

**Marketplace verdict**: OPPORTUNITY EXISTS / SATURATED / UNVALIDATED — [1-line rationale]

---

## IDEA-SPECIFIC GAP ASSESSMENT

[Only include when analyzing for a specific business idea, not just a market]

**White space fit**: Does the idea target an underserved segment? Y/N — [explain which quadrant on the positioning map, whether it's crowded or open]

**Displacement potential**: Which competitors' customers would switch? Why? [Name specific competitors and the trigger — price, frustration, missing feature, complexity]

**Minimum viable differentiation**: What must this idea do differently to survive? [The minimum bar to not be "just another X"]

**Positioning defensibility**: Can this position hold as competitors react? [Would it take them weeks or years to counter? Why?]

**Verdict**: GAP EXISTS / CROWDED BUT WINNABLE / NO CLEAR GAP — [1-line rationale]

---

## SWITCHING COST MAP

| Competitor | Financial Lock-in | Technical Lock-in | Psychological Lock-in | Overall | Steal Difficulty |
|-----------|------------------|------------------|---------------------|---------|-----------------|
| | Low/Med/High | Low/Med/High | Low/Med/High | | Easy/Medium/Hard |

**Easiest targets** (lowest switching costs): [Competitors whose customers are easiest to steal]
**Migration strategy**: [What tools/assistance to offer to reduce switching friction]

---

## THREAT RANKING

| Rank | Competitor | Threat Level | Why | Watch For |
|------|-----------|-------------|-----|-----------|
| 1 | | High/Med/Low | | |
| 2 | | | | |
| 3 | | | | |

---

## STRATEGIC RECOMMENDATIONS

### Positioning
[Where to position in the competitive landscape and why]

### Pricing Strategy
[How to price relative to competitors — undercut, match, premium — and why]

### Primary Competitive Wedge
[The #1 differentiator to lead with]

### Customers to Steal First
[Which competitor's customers are most vulnerable and how to reach them]

### Channels to Exploit
[Distribution channels competitors underutilize or ignore]

### Moat to Build
[What defensibility to invest in over time]

### What to Watch
[Competitive moves that would change the landscape — funding rounds, acquisitions, pivots, price changes]

---

## COMPETITIVE LANDSCAPE VALIDITY

- [ ] At least 3 direct competitors with paying customers
- [ ] Pricing data verified from primary sources for top 3
- [ ] At least one exploitable competitor weakness identified
- [ ] No monopoly/duopoly/regulatory barrier blocks entry
- [ ] Bootstrapper wedge exists (doesn't require VC-scale spend)

Gates passed: [X/5]
If fewer than 3 gates pass: **RED FLAG — competitive landscape may not support entry.**

---

## BOTTOM LINE

[2-3 sentence verdict. Is the competitive landscape favorable for a bootstrapped entrant? What's the single biggest opportunity? What's the single biggest threat?]

**Top 3 actions for the next 14 days:**
1. [Specific competitive intelligence action with measurable outcome]
2. [Specific competitive intelligence action with measurable outcome]
3. [Specific competitive intelligence action with measurable outcome]

**The honest answer to "how crowded is this market?":** [One sentence]

---
[If invoked as sub-skill: produce DIGEST summary per `_shared/philosophy.md` Digest Mode format]
```

## Important Rules

See `_shared/philosophy.md` Universal Skill Rules.

**Skill-specific rules:**
- **Cite specific intelligence sources** — Crunchbase, G2, LinkedIn, ad libraries, pricing pages, job boards. Generic claims without attribution are not competitive intelligence.
- **Name names** — no "Competitor A/B/C" anonymization. Use real company names, real URLs, real data
- **No blue ocean thinking** — if there are no competitors, say so clearly and flag it as a warning, not an opportunity
- **Location matters** — always check where the team is based and what that means for their cost structure
- **VC = advantage for us** — always frame VC-backed competitors as an opportunity to compete on price and efficiency
- **Be specific** — "their pricing is $49/mo for starter" not "their pricing is competitive"
- **Update the roster** — if the user has run this before, check if competitors have changed (new entrants, exits, pivots)
