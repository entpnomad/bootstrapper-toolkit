---
name: positioning
description: Positioning and pitch copy generator for bootstrapped founders. Produces ready-to-paste copy — positioning canvas, one-liner, elevator pitch, homepage hero copy, value propositions, taglines, cold email opener, and language bank. NOT analysis — usable marketing artifacts. Use when user runs `/positioning`, asks about "positioning", "value proposition", "elevator pitch", "tagline", "homepage copy", "pitch", "messaging", "how to describe my product", or needs actual marketing copy for their product.
---

# Positioning & Pitch Copy Generator

Produces actual usable marketing copy for bootstrapped products. Not analysis, not frameworks, not "considerations" — ready-to-paste words. Every output is a deliverable the founder can use today: on their homepage, in cold emails, on social media, in sales conversations.

## Philosophy

**Words are the product's first interface.** Before anyone uses your product, they read your copy. If the copy doesn't land, nobody clicks. If nobody clicks, nothing else matters. Positioning is not a strategy exercise — it's the bridge between what you built and the person who needs it.

Read `.claude/skills/_shared/philosophy.md` for the full bottleneck shift and bootstrapper framework. For positioning specifically:

**The bootstrapper positioning reality:**
- You don't have brand awareness. Your copy has to do ALL the work.
- You can't A/B test across millions of visitors. Your first version needs to be good enough to convert the first 100.
- You compete with "do nothing" more than with competitors. Your copy must make inaction feel costly.
- The founder is usually the copywriter. These outputs should be usable directly — not "inspiration."

**Five-component positioning framework:**
The positioning canvas structures how a product should be understood:
1. **Competitive alternatives** — What would customers do if your product didn't exist?
2. **Unique attributes** — What do you have that alternatives don't?
3. **Value** — What does that enable for the customer? (In their words, not yours)
4. **Target customer** — Who cares the most about the value you deliver?
5. **Market category** — What context makes your value obvious?

**Copy principles:**
- Specificity beats cleverness — "Save 5 hours per week on inventory reconciliation" beats "Streamline your operations"
- Customer language beats founder language — use the words your customers use, not the words you wish they used
- Pain first, solution second — lead with what hurts, then offer the remedy
- One message per surface — the homepage says one thing. The email says one thing. Don't try to say everything everywhere.
- Proof beats promise — "Used by 500 Shopify stores" beats "The best quiz app"

## Reference Books

Check `references/INDEX.md` for relevant frameworks. Key books for positioning and copy:

- **obviously-awesome** (Dunford) — The five-component positioning canvas this skill uses: competitive alternatives, unique attributes, value, target customers, market category. The primary framework for the positioning section.
- **hormozi-100m** (Hormozi) — Value equation (dream outcome × perceived likelihood / time delay × effort & sacrifice) for structuring value propositions; Grand Slam Offer framing for the elevator pitch and hero copy
- **dotcom-secrets** (Brunson) — Attractive character framework for founder-led positioning; hook-story-offer structure for cold emails; traffic temperature (hot/warm/cold) for the messaging hierarchy
- **blue-ocean-strategy** (Kim & Mauborgne) — Four actions framework (eliminate/reduce/raise/create) for differentiation positioning; strategy canvas for visualizing where your positioning diverges from competitors
- **getting-real** (37signals) — "Have an enemy" and opinionated positioning; the philosophy that products should stand for something; counter-positioning language for the words-to-use/avoid bank

## Research-First Protocol

Research autonomously before generating copy. See `_shared/philosophy.md` for the full protocol.

**Key research:**
- Competitor homepages (WebFetch) — what language do they use? Where are they generic?
- Customer reviews and forums — what words do real customers use to describe the problem and solution?
- Search terms and keywords — what phrases do buyers type when looking for a solution?
- The founder's own description — capture their raw explanation for authenticity

**Consume prior intelligence:** If dimension skills have been run in this session, pull heavily from:
- **problem-analysis**: Customer language, pain story, severity framing, buyer persona
- **gtm-strategy**: ICP, message-market fit assessment, beachhead segment, value proposition draft
- **competitor-analysis**: Competitor positioning, messaging gaps, value curve, white space
- **solution-analysis**: Value prop clarity, differentiation, time-to-value, unique attributes
- **user-personas**: Primary buyer's pain story, language, triggers, objections (if run)

## End-to-End Flow

### STEP 0 — CONTEXT GATHERING

Extract from the user's input:
- The product (what it does, core features)
- The target customer (who it's for)
- The problem it solves (in the founder's words)
- Current positioning (existing homepage, tagline, messaging — if any)
- Competitive landscape (who the alternatives are — if stated)
- Tone preference (professional, conversational, bold, technical — if stated)
- Prior skill outputs available in session

If the product description is too vague to write copy for, ask ONE clarifying question. Otherwise, proceed to research.

### STEP 1 — POSITIONING RESEARCH

Before writing a single word, understand the positioning landscape.

**Research tasks:**
1. Fetch and analyze 3-5 competitor homepages — capture their headlines, value props, and language
2. Find customer language — pull exact phrases from reviews, forums, community posts
3. Identify what competitors DON'T say — the gaps in messaging are your opportunities
4. Check keyword language — what do buyers search for? (These are the words that should appear in your copy)

**Build the language bank first:**
- Customer pain phrases (how they describe the problem)
- Customer desire phrases (how they describe the ideal outcome)
- Competitor positioning phrases (how alternatives frame themselves)
- Category language (the standard vocabulary in this space)

### STEP 2 — POSITIONING CANVAS

Apply the five-step positioning framework:

1. **Competitive alternatives**: List 3-5 things customers would do instead
2. **Unique attributes**: What does this product have that alternatives lack?
3. **Value (so what?)**: What does each attribute enable? Translate features to outcomes.
4. **Target customer**: Who cares most? (Use research-backed primary buyer, not wishful thinking)
5. **Market category**: What frame makes the value obvious?

### STEP 3 — COPY GENERATION

Produce all copy artifacts. Every piece should be ready to paste.

### STEP 4 — OUTPUT

Produce the full report using the template below.

## Output Template

```
# POSITIONING & COPY: [Product Name]

Research date: [date]
Stage: [Idea / MVP / Live Product]
Target buyer: [Primary buyer in one line]
Prior analysis consumed: [List skills run in session, or "Standalone"]

---

## POSITIONING CANVAS

| Element | Finding |
|---------|---------|
| **Competitive alternatives** | [What customers do today if this product doesn't exist — list 3-5] |
| **Unique attributes** | [What this product has that alternatives lack — list 3-5] |
| **Value (so what?)** | [What those attributes enable for the customer — in their words] |
| **Target customer** | [Who cares most about this value — specific segment] |
| **Market category** | [The frame that makes the value obvious] |

---

## ONE-LINER

**The formula:** [Product name] helps [target customer] [achieve outcome] by [unique mechanism].

> [The one-liner — one sentence, under 20 words]

**When to use it:** LinkedIn bio, Twitter bio, email signature, conference intro, directory listing.

---

## ELEVATOR PITCH

> [3-4 sentences. Problem → Agitation → Solution → Proof. Under 60 seconds spoken.]

**When to use it:** Networking events, cold introductions, investor small talk (not pitch meetings — bootstrappers don't pitch), podcast guest intros.

---

## HOMEPAGE HERO COPY

### Option A — Pain-led
**Headline:** [8-12 words — leads with the problem]
**Subheadline:** [15-25 words — introduces the solution and outcome]
**CTA button:** [2-4 words]

### Option B — Outcome-led
**Headline:** [8-12 words — leads with the outcome]
**Subheadline:** [15-25 words — addresses how it works]
**CTA button:** [2-4 words]

### Option C — Category-defining
**Headline:** [8-12 words — creates a new category or reframes the market]
**Subheadline:** [15-25 words — explains what you mean]
**CTA button:** [2-4 words]

**Recommendation:** [Which option to test first and why]

---

## VALUE PROPOSITIONS (x3)

Three distinct value props, each addressing a different dimension of value. These go below the hero on the homepage, in sales decks, and in feature marketing.

### Value Prop 1: [Title — 3-5 words]
**For the buyer who cares about:** [Which pain/desire this addresses]
**Statement:** [2 sentences — the value claim with specificity]
**Proof point:** [Evidence — numbers, customer quote, comparison]

### Value Prop 2: [Title — 3-5 words]
**For the buyer who cares about:** [Different pain/desire]
**Statement:** [2 sentences]
**Proof point:** [Evidence]

### Value Prop 3: [Title — 3-5 words]
**For the buyer who cares about:** [Different pain/desire]
**Statement:** [2 sentences]
**Proof point:** [Evidence]

---

## POSITIONING STATEMENT

**For** [target customer segment]
**who** [have this specific problem/need],
**[Product Name]** is a [market category]
**that** [key benefit/outcome].
**Unlike** [primary competitive alternative],
**we** [key differentiator].

---

## TAGLINE OPTIONS (x5)

| # | Tagline | Style | Best For |
|---|---------|-------|----------|
| 1 | [Tagline] | [Descriptive / Aspirational / Problem-focused / Clever / Direct] | [Where to use it] |
| 2 | [Tagline] | | |
| 3 | [Tagline] | | |
| 4 | [Tagline] | | |
| 5 | [Tagline] | | |

**Recommendation:** [Which to lead with and why]

---

## COLD EMAIL OPENER

**Subject line options:**
1. [Subject line — question-based]
2. [Subject line — value-based]
3. [Subject line — curiosity-based]

**Opening paragraph:**
> [3-4 sentences. Personalized hook → pain identification → bridge to product → soft CTA. Written as a template with [brackets] for personalization fields.]

**When to use:** Outbound to Primary buyer persona. Pair with LinkedIn connection request.

---

## LANGUAGE BANK

### Words & Phrases to USE
| Phrase | Why It Works | Where to Use |
|--------|-------------|-------------|
| [Customer pain phrase] | [Resonates with how they describe the problem] | [Homepage, emails, ads] |
| [Outcome phrase] | [Matches their desired state] | [CTAs, value props] |
| [Category language] | [Establishes credibility in the space] | [SEO, content, directory listings] |
| [Specificity phrase] | [Concrete, believable claim] | [Landing pages, case studies] |
| [Urgency phrase] | [Triggers action] | [Emails, ads, CTAs] |

### Words & Phrases to AVOID
| Phrase | Why It Fails | Use Instead |
|--------|-------------|-------------|
| [Generic/jargon term] | [Why it doesn't land with this audience] | [Better alternative] |
| [Overused buzzword] | [Why it's noise] | [Better alternative] |
| [Competitor's language] | [Why using their frame hurts you] | [Better alternative] |
| [Vague claim] | [Why it's unbelievable] | [Specific version] |

### Customer Pain Phrases (from research)
[5-10 exact phrases pulled from forums, reviews, and communities — the raw language customers use to describe this problem. These are gold for copy, ads, and content.]

1. "[Exact phrase]" — Source: [Where found]
2. "[Exact phrase]" — Source: [Where found]
3. "[Exact phrase]" — Source: [Where found]
4. "[Exact phrase]" — Source: [Where found]
5. "[Exact phrase]" — Source: [Where found]

---

## MESSAGING HIERARCHY

**Primary message** (the ONE thing to communicate): [One sentence — the core positioning]
**Secondary messages** (support the primary):
1. [Supporting message — addresses a key objection or adds credibility]
2. [Supporting message — different dimension of value]
3. [Supporting message — social proof or urgency]

**Message-to-surface map:**
| Surface | Message | Copy |
|---------|---------|------|
| Homepage hero | Primary | [The headline] |
| Homepage below fold | Secondary 1-3 | [The value props] |
| Google ad | Primary | [Headline + description fit] |
| LinkedIn ad | Primary + proof | [Headline + social proof] |
| Email subject | Primary pain | [Subject line] |
| Marketplace listing | Primary + category | [Title and short description] |

---

## BOTTOM LINE

**Your positioning in one sentence:** [The positioning statement, distilled]

**The honest answer about your messaging:** [One sentence — is the positioning clear and differentiated, or does it need more customer evidence to sharpen?]

**Top 3 actions for the next 7 days:**
1. [Specific action — e.g., "Update homepage with Option A hero copy and measure click-through rate"]
2. [Specific action — e.g., "Send cold email opener to 20 prospects from Primary persona list and track reply rate"]
3. [Specific action — e.g., "Run `/user-personas` to deepen buyer understanding if not yet run"]
```

## Important Rules

See `_shared/philosophy.md` Universal Skill Rules.

**Skill-specific rules:**
- **Ready to paste, not ready to discuss** — every copy artifact must be usable as-is. Not "consider something like..." but the actual words. The founder should be able to copy-paste the homepage hero onto their site.
- **Customer language over clever language** — if research reveals customers say "inventory is a nightmare," don't upgrade it to "streamline your inventory management." Use their words.
- **Multiple options for key pieces** — homepage hero gets 3 options (pain-led, outcome-led, category-defining). Taglines get 5. Subject lines get 3. Founders need to test, not commit blindly.
- **Specificity is everything** — "Save time on reporting" fails. "Cut your monthly reporting from 8 hours to 20 minutes" works. Every claim should have a number, a timeframe, or a concrete outcome. For idea-stage products without usage data, frame specificity around the problem ("You're spending 8 hours a month on reporting. There's a better way.") rather than fabricating solution metrics.
- **Don't write copy for imaginary products** — if the product doesn't exist yet, the copy should frame the problem and outcome, not specific features. Copy evolves as the product solidifies.
- **Language bank is the hidden gem** — the words-to-use and words-to-avoid lists are often more valuable than the headlines. They shape every piece of copy the founder writes from this point forward.
- **This is a Generator skill** — the output is a deliverable. No validation gates, no digest mode. Produce complete, ready-to-use copy artifacts.
- **Source the language** — every customer pain phrase in the language bank must cite where it was found. Fabricated "customer quotes" are worse than useless.
