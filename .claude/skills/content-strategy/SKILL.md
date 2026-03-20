---
name: content-strategy
description: Content and distribution strategy generator for bootstrapped founders. Produces content pillars, 15 specific content ideas with titles, 20 SEO keywords, a 90-day content calendar, channel-specific tactics, and a distribution checklist. Use when user runs `/content-strategy`, asks about "content strategy", "what should I write about", "blog topics", "SEO keywords", "content calendar", "content marketing plan", or needs a concrete content and distribution plan for their product.
---

# Content Strategy — Content & Distribution Plan for Bootstrappers

Produces a complete, actionable content and distribution strategy. Not "you should do content marketing" — specific titles, keywords, calendars, and distribution checklists that a founder can execute starting tomorrow.

## Philosophy

**Content is distribution you own.** Every blog post, every guide, every video is an asset that compounds. Paid ads stop when you stop paying. Content keeps working. For bootstrappers with limited budgets, content is the highest-leverage marketing investment — but only if it's strategic.

Read `.claude/skills/_shared/philosophy.md` for the full bottleneck shift and bootstrapper framework. For content strategy specifically:

**The bootstrapper content reality:**
- You don't have a content team. Every piece must justify the founder's time.
- Quality beats quantity when you're publishing 2-4 pieces per month, not 20.
- Distribution matters more than creation. A great post nobody sees is worthless.
- Content should sell without selling — answer the questions buyers ask before they buy.
- SEO is a compounding channel. The posts you write today pay dividends for years — if you target the right keywords.

**Content strategy for the AI age:**
- AI tools can help create content, but AI-generated generic content is noise. The signal is original insight, proprietary data, and founder perspective.
- Answer engines (Perplexity, ChatGPT, Google AI Overviews) are changing how people find information. Content must be structured for AI extraction AND human reading.
- Bottom-of-funnel content (comparisons, alternatives, tutorials, templates) converts better than top-of-funnel thought leadership for bootstrappers.
- Your content should make your product the obvious answer to the problem it discusses.

## Reference Books

Check `references/INDEX.md` for relevant frameworks. Key books for content strategy:

- **traction-weinberg** (Weinberg & Mares) — 19 traction channels and the Bullseye framework for channel selection; content marketing as one of the channels with testing methodology; the 50% rule (spend half your time on distribution)
- **dotcom-secrets** (Brunson) — Traffic temperature model (hot/warm/cold) maps to TOFU/MOFU/BOFU content; value ladder concept for sequencing content toward conversion; funnel structure informs content calendar priorities
- **make-handbook** (Levels) — Build-in-public content strategy; SEO as primary bootstrapper channel; community-driven distribution; practical solo-founder content production cadence
- **start-small** (Walling) — SEO-first content strategy for developer-founders; marketing-before-code philosophy applied to content planning; niche keyword targeting for bootstrappers
- **product-led-growth** (Bush) — Product-qualified leads through content; time-to-value concept applied to content experience; how content drives self-serve acquisition
- **saas-playbook** (Walling) — SaaS-specific content and channel strategies; funnel optimization; how to choose between content, community, and paid channels based on market type

## Research-First Protocol

Research autonomously before generating the strategy. See `_shared/philosophy.md` for the full protocol.

**Key research:**
- Competitor blogs and content (WebFetch) — what are they writing about? What ranks?
- "[market/category] blog" / "[market/category] guide" — what content exists?
- Keyword research: "[problem] how to" / "[product category] best" / "[competitor] alternative" / "[competitor] vs"
- Community questions: What does the target audience ask on Reddit, Quora, forums?
- "[target buyer role] newsletter" / "[target buyer role] podcast" — where do they consume content?

**Consume prior intelligence:** If dimension skills have been run in this session, pull heavily from:
- **gtm-strategy**: Channels, beachhead, distribution strategy, congregation points
- **problem-analysis**: Customer language, pain points, trigger events, buyer questions
- **competitor-analysis**: Competitor content strategy, SEO gaps, messaging gaps
- **user-personas**: Primary buyer's information diet, pain story, search behavior (if run)
- **positioning**: Language bank, customer pain phrases, messaging hierarchy (if run)

## End-to-End Flow

### STEP 0 — CONTEXT GATHERING

Extract from the user's input:
- The product (what it does, who it's for)
- Current content assets (existing blog, social presence, email list — if any)
- Founder's content skills and preferences (writing, video, podcast, design)
- Time available for content (hours per week)
- Prior skill outputs available in session

If the product is too vague to build a content strategy for, ask ONE clarifying question. Otherwise, proceed to research.

### STEP 1 — CONTENT LANDSCAPE RESEARCH

Map the content landscape before creating strategy.

**Research tasks:**
1. Analyze 3-5 competitor blogs — topics, frequency, quality, engagement
2. Identify high-intent keywords in the category (bottom-of-funnel first)
3. Mine community questions — Reddit, Quora, forums, Stack Exchange
4. Check what content ranks for category terms (Google search analysis)
5. Identify content gaps — topics the audience asks about that nobody answers well

### STEP 2 — PILLAR & KEYWORD STRATEGY

Define content pillars and map keywords to the buyer journey.

**Content pillars:** 3-4 core themes that everything maps to. Each pillar should:
- Connect directly to a problem the product solves
- Have enough keyword volume to sustain 12+ months of content
- Be defensible — aligned with the founder's domain expertise

**Keyword mapping by intent:**
- **Bottom-of-funnel (BOFU)**: "[competitor] alternative", "[product category] comparison", "[specific problem] solution", pricing pages
- **Middle-of-funnel (MOFU)**: "how to [solve problem]", "best [tools] for [use case]", "[problem] guide"
- **Top-of-funnel (TOFU)**: "[industry] trends", "[role] challenges", educational content

**Bootstrapper priority**: BOFU first, then MOFU. TOFU only after the pipeline converts.

### STEP 3 — CONTENT PLAN GENERATION

Produce specific, titled content pieces with distribution plans.

### STEP 4 — OUTPUT

Produce the full report using the template below.

## Output Template

```
# CONTENT STRATEGY: [Product Name]

Research date: [date]
Stage: [Idea / MVP / Live Product]
Target buyer: [Primary buyer in one line]
Founder content capacity: [Estimated hours/week, if known]
Prior analysis consumed: [List skills run in session, or "Standalone"]

---

## CONTENT PILLARS

| # | Pillar | Connection to Product | Target Keywords (seed) | Content Volume Potential |
|---|--------|----------------------|----------------------|------------------------|
| 1 | [Pillar name] | [How this connects to what you sell] | [2-3 seed keywords] | [High / Medium — estimated monthly search volume range] |
| 2 | [Pillar name] | [Connection] | [Seeds] | [Volume] |
| 3 | [Pillar name] | [Connection] | [Seeds] | [Volume] |
| 4 | [Pillar name — if applicable] | [Connection] | [Seeds] | [Volume] |

---

## SEO KEYWORD MAP (20 keywords)

| # | Keyword | Intent | Relative Demand | Competition | Priority | Content Type |
|---|---------|--------|----------------|-------------|----------|-------------|
| 1 | [keyword] | BOFU / MOFU / TOFU | High / Med / Low | Low / Med / High | P1 / P2 / P3 | [Blog / Guide / Comparison / Landing page / Video] |
| 2 | | | | | | |
| ... | | | | | | |
| 20 | | | | | | |

**Relative Demand** is estimated from search result volume, competitor content investment, and community discussion frequency — NOT from keyword research tools. For precise search volumes, use Google Keyword Planner (free), Ubersuggest (free tier), or Ahrefs.

**Keyword strategy rationale:**
[2-3 sentences on why these keywords were chosen. What's the BOFU-first logic? Where are the competitor gaps?]

---

## CONTENT IDEAS (15 pieces)

### BOFU — Bottom of Funnel (Convert searchers to buyers)

| # | Title | Keyword Target | Format | Pillar | Why This Works |
|---|-------|---------------|--------|--------|---------------|
| 1 | "[Exact title — ready to publish]" | [keyword] | [Blog / Comparison / Landing page] | [#] | [Why this converts] |
| 2 | "[Title]" | [keyword] | | | |
| 3 | "[Title]" | [keyword] | | | |
| 4 | "[Title]" | [keyword] | | | |
| 5 | "[Title]" | [keyword] | | | |

### MOFU — Middle of Funnel (Educate and build trust)

| # | Title | Keyword Target | Format | Pillar | Why This Works |
|---|-------|---------------|--------|--------|---------------|
| 6 | "[Exact title]" | [keyword] | [Guide / How-to / Template / Checklist] | [#] | [Why this builds trust] |
| 7 | "[Title]" | [keyword] | | | |
| 8 | "[Title]" | [keyword] | | | |
| 9 | "[Title]" | [keyword] | | | |
| 10 | "[Title]" | [keyword] | | | |

### TOFU — Top of Funnel (Build awareness and authority)

| # | Title | Keyword Target | Format | Pillar | Why This Works |
|---|-------|---------------|--------|--------|---------------|
| 11 | "[Exact title]" | [keyword] | [Blog / Report / Video / Industry analysis] | [#] | [Why this attracts the right audience] |
| 12 | "[Title]" | [keyword] | | | |
| 13 | "[Title]" | [keyword] | | | |
| 14 | "[Title]" | [keyword] | | | |
| 15 | "[Title]" | [keyword] | | | |

---

## 90-DAY CONTENT CALENDAR

### Month 1: Foundation (Weeks 1-4)

| Week | Content Piece | Type | Keyword | Distribution Plan |
|------|--------------|------|---------|-------------------|
| 1 | [Title from ideas list] | [Format] | [keyword] | [Where to publish and promote] |
| 2 | [Title] | | | |
| 3 | [Title] | | | |
| 4 | [Title] | | | |

**Month 1 goal:** [Specific, measurable goal — e.g., "Publish 4 BOFU pieces targeting comparison keywords"]

### Month 2: Expand (Weeks 5-8)

| Week | Content Piece | Type | Keyword | Distribution Plan |
|------|--------------|------|---------|-------------------|
| 5 | [Title] | | | |
| 6 | [Title] | | | |
| 7 | [Title] | | | |
| 8 | [Title] | | | |

**Month 2 goal:** [Specific goal — e.g., "Add MOFU content, begin email capture, repurpose Month 1 into social"]

### Month 3: Scale (Weeks 9-12)

| Week | Content Piece | Type | Keyword | Distribution Plan |
|------|--------------|------|---------|-------------------|
| 9 | [Title] | | | |
| 10 | [Title] | | | |
| 11 | [Title] | | | |
| 12 | [Title] | | | |

**Month 3 goal:** [Specific goal — e.g., "Begin TOFU content, optimize Month 1-2 pieces for rankings, launch newsletter"]

---

## CHANNEL TACTICS

### SEO / Organic Search
- **Primary strategy:** [Bottom-up keyword targeting approach]
- **Quick wins:** [Low-competition keywords to target first]
- **Long-term plays:** [High-volume keywords to build toward]
- **Technical checklist:** [On-page SEO, schema markup, internal linking, site speed]

### Community & Forums
- **Target communities:** [Specific subreddits, Slack groups, Discord servers, forums — with member counts if available]
- **Engagement approach:** [How to participate without being spammy — answer questions, share insights, be genuinely helpful]
- **Content to share:** [Which content pieces map to community discussions]
- **Rules to follow:** [Community-specific posting guidelines to not get banned]

### Social Media
- **Primary platform:** [The ONE platform where the target buyer is most active]
- **Content format:** [What works on this platform — threads, carousels, short video, screenshots]
- **Posting cadence:** [Realistic for a solo founder — 3x/week, not daily]
- **Repurposing strategy:** [How blog content becomes social content]

### Email / Newsletter
- **Lead magnet idea:** [Specific free resource that attracts the right audience]
- **Email capture placement:** [Where to put the opt-in — blog posts, homepage, tool output]
- **Newsletter cadence:** [Weekly / Biweekly — what's sustainable]
- **Content mix:** [Curated links, original insights, product updates — ratio]

### Partnerships & Guest Content
- **Target publications:** [Specific blogs, newsletters, or podcasts that reach the target buyer]
- **Pitch angle:** [What unique perspective or data you can offer]
- **Co-marketing opportunities:** [Complementary tools or services to partner with]

---

## DISTRIBUTION CHECKLIST (per content piece)

Every piece of content should go through this distribution checklist:

- [ ] **Publish** on your blog/site with proper SEO (title tag, meta description, internal links, schema)
- [ ] **Share** on primary social platform with native-format adaptation
- [ ] **Post** to 1-2 relevant communities (with genuine value, not just a link drop)
- [ ] **Email** to your list (if you have one) with a compelling subject line
- [ ] **Repurpose** into at least one other format (thread, carousel, short video, infographic)
- [ ] **Cross-link** from/to related existing content on your site
- [ ] **Submit** to relevant aggregators or directories (Hacker News, Product Hunt, IndieHackers, etc. — if appropriate)
- [ ] **Monitor** comments and engagement for 48 hours — respond to everything

---

## AI DISCOVERABILITY

**Structure content for answer engines:**
- Use clear H2/H3 headings that match search queries
- Include FAQ sections with structured data markup
- Provide definitive answers in the first paragraph (AI overviews pull from here)
- Use comparison tables (AI models love structured data)
- Include "[Product] vs [Competitor]" pages (heavily cited by AI recommendation engines)

**Monitor AI mentions:**
- Monthly check: ask ChatGPT, Perplexity, Claude "[product category] best tools" — are you mentioned?
- If not mentioned, focus on: increasing citations on review sites, building backlinks from authoritative sources, creating comprehensive comparison content

---

## CONTENT METRICS TO TRACK

| Metric | Tool | Cadence | What It Tells You |
|--------|------|---------|-------------------|
| Organic traffic per post | Google Search Console / Analytics | Weekly | Which content drives discovery |
| Keyword rankings | Google Search Console | Monthly | SEO progress |
| Email signups per post | Your email tool | Weekly | Which content attracts the right audience |
| Conversions per post | Analytics | Monthly | Which content drives revenue |
| Community engagement | Manual check | Weekly | Which topics resonate |
| AI citation checks | ChatGPT / Perplexity | Monthly | AI visibility progress |

**North star metric:** Signups or revenue attributed to content. Everything else is a leading indicator.

---

## BOTTOM LINE

**Your content strategy in one sentence:** [The core approach — e.g., "Win bottom-of-funnel comparison keywords in Month 1, build MOFU educational content in Month 2, scale with TOFU thought leadership in Month 3"]

**The honest answer about content:** [One sentence — is content the right channel for this product and this founder? Or should they focus elsewhere first?]

**Top 3 actions for the next 7 days:**
1. [Specific action — e.g., "Publish the first BOFU comparison post: '[exact title]'"]
2. [Specific action — e.g., "Set up Google Search Console and submit sitemap"]
3. [Specific action — e.g., "Join [specific community] and answer 5 questions related to [pain point]"]
```

## Important Rules

See `_shared/philosophy.md` Universal Skill Rules.

**Skill-specific rules:**
- **Titles must be ready to publish** — not "something about competitor comparisons" but "[Product] vs [Competitor]: Which Is Better for [Use Case] in [Year]?" The founder should be able to use the exact title.
- **Keywords must have evidence** — every keyword should come from actual search research, not imagination. Rate relative demand (High/Med/Low) based on search result density, competitor content investment, and community discussion frequency. These are directional signals, not precise volumes.
- **BOFU first, always** — for bootstrappers, comparison and alternative keywords convert 10x better than thought leadership. The calendar must front-load BOFU content.
- **Distribution > creation** — the distribution checklist and channel tactics should be as detailed as the content ideas. A post without distribution is a tree falling in an empty forest.
- **Realistic cadence** — a solo founder can realistically produce 1-2 quality pieces per week, not 5. The 90-day calendar must be achievable by the person reading it.
- **Community-specific guidance** — don't just say "post on Reddit." Name the specific subreddits, note their rules, and describe how to participate without getting banned.
- **This is a Generator skill** — the output is a deliverable. No validation gates, no digest mode. Produce a complete content plan the founder can execute immediately.
- **Connect content to product** — every content piece should have a natural connection to the product. Content for content's sake is a bootstrapper's luxury they can't afford.
