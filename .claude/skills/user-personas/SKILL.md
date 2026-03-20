---
name: user-personas
description: ICP and buyer persona card generator for bootstrapped founders. Produces 2-3 detailed persona cards (primary buyer, secondary buyer, anti-persona) with demographics, psychographics, behavior patterns, pain story, buying triggers, objections, and targeting criteria. Includes beachhead drift check. Use when user runs `/user-personas`, asks about "who is my customer", "buyer persona", "ICP", "ideal customer profile", "target audience", "customer avatar", or needs detailed persona cards for marketing, sales, or product decisions.
---

# User Personas — ICP & Buyer Persona Card Generator

Produces detailed, research-backed persona cards that founders can use immediately for marketing copy, ad targeting, sales conversations, and product decisions. Not theoretical personas — actionable profiles built from evidence.

## Philosophy

**Personas are targeting instruments, not creative writing exercises.** A persona is useful if it tells you exactly where to find this person, what words to use, and what triggers their purchase. A persona is useless if it reads like a character sheet for a novel.

Read `.claude/skills/_shared/philosophy.md` for the full bottleneck shift and bootstrapper framework. For personas specifically:

**The bootstrapper persona standard:**
- Can you find this person in 5 minutes? (If not, the persona is too vague)
- Can you write a cold email opener that would make them stop scrolling? (If not, you don't understand their pain)
- Can you name 10 specific companies where this person works? (If not, your targeting is too broad)
- Is this the person who PAYS, or just the person who USES? (If they're different, you need both)

**Common persona failures:**
- "Small business owners" — this is an audience, not a persona. Which business? What size? What stage? What industry?
- Demographics without psychographics — age and location don't predict buying behavior. Pain, workflow, and trigger events do.
- Aspirational personas — describing who you WISH your customer was, not who the evidence says they are
- Too many personas — for a bootstrapped launch, you need 1 primary buyer. Not 5 segments. Focus.

**Beachhead drift risk:** Founders often build personas around the customer they WANT, not the customer who actually has the most pain and willingness to pay. This skill checks for drift.

## Reference Books

Check `references/INDEX.md` for relevant frameworks. Key books for persona development:

- **startup-owners-manual** (Blank & Dorf) — Customer development methodology and earlyvangelists; how to identify and characterize the first buyers who will pay before the product is polished
- **mom-test** (Fitzpatrick) — How to interview customers to discover real pain; avoiding false positives and compliments; the language and behavior patterns that feed persona pain stories
- **crossing-the-chasm** (Moore) — Pragmatist vs. visionary buyer archetypes; beachhead segment selection; whole product concept that shapes what different personas need
- **continuous-discovery** (Torres) — Opportunity solution trees and experience maps for structuring persona research; weekly customer touchpoints as a habit
- **disciplined-entrepreneurship** (Aulet) — Persona development templates; market segmentation matrix for identifying which persona to target first; end-user profile construction
- **obviously-awesome** (Dunford) — Best-fit customer identification; the positioning question "who cares the most?" directly shapes the primary buyer persona

## Research-First Protocol

Research autonomously before generating personas. See `_shared/philosophy.md` for the full protocol.

**Key searches:**
- "[target role] day in the life" / "[target role] workflow" / "[target role] challenges"
- "[target role] job posting" (reveals actual responsibilities, tools used, reporting structure)
- "[competitor] customer reviews" / "[competitor] case studies" (reveals who actually buys)
- "[target industry] salary" / "[target role] buying authority" (reveals budget access)
- "[problem domain] reddit" / "[problem domain] community" (reveals language, frustrations, congregating points)
- "[target role] influencers" / "[target industry] thought leaders" / "[target industry] podcast" (reveals trusted voices)
- LinkedIn search for the target role (reveals company sizes, industries, seniority)

**Consume prior intelligence:** If dimension skills have been run in this session, pull heavily from:
- **problem-analysis**: Pain language, buyer persona clarity, trigger events, workarounds
- **gtm-strategy**: ICP definition, beachhead segment, congregation points, buying process
- **competitor-analysis**: Customer segments, review mining (who complains and what about), case study targets
- **market-size**: Beachhead market, customer segments, demand signals

## End-to-End Flow

### STEP 0 — CONTEXT GATHERING

Extract from the user's input:
- The business idea or product (what it does, who it's for)
- The founder's stated target customer (if any)
- Current stage (idea, MVP, live product with customers)
- Any existing customer data or interview insights
- Prior skill outputs available in session

If the idea description is too vague to identify buyer personas, ask ONE clarifying question. Otherwise, proceed to research.

### STEP 1 — BUYER RESEARCH

Research who actually buys in this market. Don't start from the founder's assumptions — start from evidence.

**Evidence sources (prioritized):**
1. Competitor customer reviews and case studies (who's already buying?)
2. Job postings for the target role (what do they actually do?)
3. Community discussions (how do they describe their pain?)
4. LinkedIn profiles of likely buyers (company size, industry, seniority)
5. Prior dimension skill outputs (if available)

**Key questions to answer through research:**
- Who has this problem most acutely? (Not who has it — who has it WORST)
- Who has budget authority to solve it? (User vs. buyer split)
- Where do they congregate? (Communities, events, publications, platforms)
- What tools do they already use? (Tech stack context)
- What triggers their search for a solution? (Buying trigger)
- What would stop them from buying? (Objections)

### STEP 2 — PERSONA CONSTRUCTION

Build 2-3 persona cards:

1. **Primary Buyer** — The person most likely to find you, pay you, and stay. This is your beachhead customer. Build everything for this person first.
2. **Secondary Buyer** — A viable adjacent segment. Not your launch target, but your expansion path. Different enough to need different messaging.
3. **Anti-Persona** — The person who looks like your customer but ISN'T. They'll waste your time, request features you shouldn't build, and churn. Know them so you can avoid them.

**For each persona card, develop:**
- Identity (role, company context, seniority)
- Demographics (age range, location patterns, income/budget)
- Psychographics (values, fears, motivations, decision-making style)
- Behavior patterns (daily workflow, tools used, information diet)
- Pain story (the specific problem moment — when, where, how it hurts)
- Buying trigger (what event makes them search for a solution NOW)
- Objections (what stops them from buying — price, trust, switching cost, inertia)
- Targeting criteria (how to find them — platforms, communities, search terms, ad targeting)
- Influencers (who do they listen to? whose recommendation matters?)

### STEP 3 — BEACHHEAD DRIFT CHECK

Compare the founder's stated target customer against the research-backed primary buyer:
- **ALIGNED** — founder's target matches the evidence
- **DRIFTED** — evidence points to a different primary buyer

If DRIFTED, explain:
- Who the evidence says the primary buyer is
- Why they're different from the founder's assumption
- What this means for GTM strategy
- Whether to pivot targeting or gather more evidence

### STEP 4 — OUTPUT

Produce the full report using the template below.

## Output Template

```
# USER PERSONAS: [Product/Idea Name]

Research date: [date]
Stage: [Idea / MVP / Live Product]
Founder's stated target: "[Who the founder thinks the customer is]"
Prior analysis consumed: [List skills run in session, or "Standalone"]

---

## PERSONA 1: PRIMARY BUYER — [Persona Name]

**The archetype:** [One sentence — who this person is and why they buy]

### Identity
- **Role:** [Job title(s)]
- **Company:** [Type, size, industry, stage]
- **Seniority:** [IC / Manager / Director / VP / C-level]
- **Reports to:** [Who their boss is — matters for buying authority]
- **Budget authority:** [Can they swipe a credit card? Or need approval?]

### Demographics
- **Age range:** [Typical range]
- **Location patterns:** [Geographic clusters, remote/in-office]
- **Income/compensation range:** [If relevant to pricing]
- **Education/background:** [Common paths to this role]

### Psychographics
- **Core motivation:** [What drives them professionally]
- **Biggest fear:** [What keeps them up at night re: this problem domain]
- **Decision style:** [Data-driven / intuition-led / consensus-seeker / authority-driven]
- **Risk tolerance:** [Early adopter / pragmatist / conservative]
- **Values:** [What they optimize for — efficiency, quality, cost, innovation, simplicity]

### Behavior Patterns
- **Daily workflow:** [What their day looks like, where the pain shows up]
- **Tools they already use:** [Software stack — this is your integration map]
- **Information diet:** [Where they learn — newsletters, podcasts, communities, conferences]
- **How they find new tools:** [Peer recommendation, Google search, marketplace browse, social media, industry events]

### Pain Story
> [Write a 3-4 sentence narrative of the pain moment. First person. Use the language real customers use. This should feel like a direct quote from a customer interview.]

### Buying Trigger
- **Primary trigger:** [The specific event that moves them from "aware" to "actively searching"]
- **Trigger frequency:** [How often this trigger occurs — daily/monthly/yearly/once]
- **Trigger detectability:** [Can you detect this trigger externally? How? Job postings, funding announcements, regulatory deadlines, seasonal patterns]

### Objections
| # | Objection | Response Strategy |
|---|-----------|-------------------|
| 1 | [Most common objection] | [How to address it] |
| 2 | [Second objection] | [How to address it] |
| 3 | [Third objection] | [How to address it] |
| 4 | [Fourth objection — if applicable] | [How to address it] |

### Targeting Criteria
- **LinkedIn targeting:** [Job titles, company sizes, industries, seniority levels]
- **Community targeting:** [Specific subreddits, Slack groups, Discord servers, forums, Facebook groups]
- **Content targeting:** [Keywords they search, topics they engage with, hashtags they follow]
- **Event targeting:** [Conferences, meetups, webinars they attend]
- **Ad targeting:** [Platform-specific criteria — Facebook interests, Google keywords, LinkedIn filters]
- **Outbound signals:** [Job postings, funding announcements, tool reviews — signals that someone is in-market]

### Influencers & Trust Sources
- **People they listen to:** [Name specific people only if found through research. If no specific influencers were identified, describe the type of voice they trust (e.g., "peer practitioners who share results, not gurus")]
- **Publications they trust:** [Newsletters, blogs, media outlets]
- **Proof they need:** [Case studies, ROI data, peer testimonials, free trial, demo]

---

## PERSONA 2: SECONDARY BUYER — [Persona Name]

**The archetype:** [One sentence — who this person is and why they might buy]
**Relationship to Primary:** [How they differ — different company size? Different industry? Different role?]
**When to target:** [Not now — when expansion makes sense, what signal to watch for]

### Identity
[Same structure as Primary, but abbreviated — focus on how they DIFFER from Primary]

### Pain Story
> [3-4 sentence narrative — different pain angle from Primary]

### Buying Trigger
- **Primary trigger:** [Different trigger than Primary]
- **Key difference from Primary:** [What makes selling to them different]

### Targeting Criteria
[Abbreviated — focus on channels and criteria DIFFERENT from Primary]

---

## PERSONA 3: ANTI-PERSONA — [Persona Name]

**The archetype:** [One sentence — who this person is and why they're NOT your customer]
**Why they seem like a fit:** [What makes them look like your target at first glance]
**Why they're NOT:** [The critical difference that makes them a bad customer]

### Warning Signs
| # | Signal | What It Means |
|---|--------|---------------|
| 1 | [Behavior or attribute] | [Why this indicates a bad fit] |
| 2 | [Behavior or attribute] | [Why this indicates a bad fit] |
| 3 | [Behavior or attribute] | [Why this indicates a bad fit] |

### What Happens If You Sell to Them
[2-3 sentences on the consequences — feature requests that derail your roadmap, high support costs, churn, price sensitivity, etc.]

### How to Filter Them Out
[Specific qualification criteria or pricing/positioning decisions that naturally repel the anti-persona]

---

## BEACHHEAD DRIFT CHECK

**Founder's stated target:** [Who the founder said they're building for]
**Research-backed primary buyer:** [Who the evidence points to]
**Drift status:** ALIGNED / DRIFTED

[If DRIFTED:]
- **Where evidence points:** [The research-backed segment]
- **Why it differs:** [Key evidence that contradicts the founder's assumption]
- **Recommendation:** [Pivot targeting / Gather more evidence / Acknowledge and test both]
- **Impact on strategy:** [What changes if the founder targets the research-backed segment instead]

[If ALIGNED:]
- **Confirming evidence:** [What validates the founder's targeting instinct]

---

## PERSONA-TO-ACTION MAP

| Action | Primary Buyer Specifics |
|--------|------------------------|
| **Homepage headline should say:** | [Draft headline speaking to Primary's pain] |
| **First email subject line:** | [Draft subject line that would get opened] |
| **Ideal first content piece:** | [Topic and format that Primary would engage with] |
| **Best channel for first 10 customers:** | [Specific channel with rationale] |
| **Demo/trial should show:** | [The aha moment that matches Primary's pain story] |

---

## BOTTOM LINE

**Your primary buyer is:** [One sentence — the single most important person to build for]

**The honest answer about your customer:** [One sentence — what the evidence says about who actually needs this, which may or may not match who the founder imagined]

**Top 3 actions for the next 7 days:**
1. [Specific persona validation action — e.g., "Post in r/[subreddit] asking about [pain point] and note which job titles respond"]
2. [Specific targeting action — e.g., "Create a LinkedIn Sales Navigator search for [criteria] and save the list"]
3. [Specific messaging action — e.g., "Write 3 cold email openers using the pain language from the Primary persona card and test which gets replies"]
```

## Important Rules

See `_shared/philosophy.md` Universal Skill Rules.

**Skill-specific rules:**
- **Research before inventing** — personas must be built from market evidence, not imagination. Every attribute should trace back to research (competitor reviews, community posts, job listings, prior skill outputs). If evidence is thin, say so.
- **Use real language** — the pain story must use words real customers use, not marketing jargon. Pull exact phrases from forums, reviews, and community discussions.
- **One primary, not three equals** — the primary buyer must be clearly identified. If you can't choose, the research isn't deep enough. Force the choice.
- **Anti-persona is not optional** — knowing who to avoid saves more time than knowing who to pursue. Every founding team builds for the wrong customer at some point. The anti-persona prevents that.
- **Targeting criteria must be specific** — "small businesses" fails. "Operations managers at DTC ecommerce brands doing $1M-$10M revenue who use Shopify Plus and have 3+ fulfillment locations" passes. Specificity enables action.
- **Buying trigger is the unlock** — without a trigger event, personas describe a static population. With a trigger, they describe an in-market buyer. Always identify what creates urgency.
- **This is a Generator skill** — the output is a deliverable artifact. No validation gates, no digest mode. Produce complete, usable persona cards that can be referenced in marketing, sales, and product conversations.
- **Persona-to-action map is required** — personas sitting in a document are worthless. The action map ensures the founder walks away with something to DO, not just something to READ.
