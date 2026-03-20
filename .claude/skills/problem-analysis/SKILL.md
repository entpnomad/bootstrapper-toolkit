---
name: problem-analysis
description: Problem existence and pain validation for bootstrapped founders. Assesses whether the problem is real, how severe the pain is, willingness to pay, buyer persona clarity, and urgency triggers — separating founder assumptions from market evidence. Use when user runs `/problem-analysis`, asks about "is this a real problem", "pain severity", "willingness to pay", "buyer persona", "customer pain", "problem validation", "does anyone actually need this", or needs to validate that a problem exists before building anything.
---

# Problem Analysis — Pain Validation for Bootstrappers

If the problem isn't real, nothing else matters. This skill forces founders to separate assumptions from evidence before building anything.

## Philosophy

**Assumption is the enemy. Evidence is the standard.** Every founder believes their problem is real. Most are wrong. The difference between a business and a hobby project is whether real people experience real pain frequently enough to pay real money. This skill exists to find out before you build.

Read `.claude/skills/_shared/philosophy.md` for the full bottleneck shift and bootstrapper framework. For problem analysis specifically:

**The clarity bottleneck.** When code is cheap, the question is never "can we build it?" — it's "do we know what's worth building?" Problem analysis is the clarity engine. A founder who deeply understands customer pain — in the customer's own words — has the most valuable asset in the AI age: knowing exactly what to build.

**Founder assumption vs. market reality.** Founders project their own pain onto the market. They build what they'd want, not what customers will pay for. The gap between "I think this is a problem" and "real people describe this pain and pay to solve it" is where most startups die. This skill measures that gap.

**AI-native reality check — false confidence traps:**
- "I experienced this problem myself" — sample size of one is not validation
- "People say they'd use this" — compliments are not commitments; past behavior beats stated intent
- "There's nothing good out there" — if nobody's paying to solve it, maybe the pain isn't severe enough
- "Everyone has this problem" — vague problems attract nobody; specific problems attract buyers

**What IS evidence:**
- Real people describing this pain unprompted (forums, reviews, social media)
- Money already being spent on workarounds (agencies, spreadsheets, manual processes, competing tools)
- Buyer identifiable by job title, company type, and trigger event
- Customer language that matches — or contradicts — the founder's framing

## Reference Books

Check `references/INDEX.md` for relevant frameworks. Key topics for problem validation: customer interview methodology, customer development and earlyvangelists, opportunity trees and assumption mapping, validated learning, persona development, importance-vs-satisfaction frameworks, buyer archetypes.

## Research-First Protocol

Research autonomously before outputting anything. See `_shared/philosophy.md` for the full protocol. Key searches:

- "[problem domain] complaints" / "[problem domain] frustrations" / "[problem domain] pain points"
- "[problem domain] reddit" / "[problem domain] forum" / "[problem domain] reviews"
- "[competitor category] reviews negative" / "[competitor category] switching from"
- "[buyer role] biggest challenge" / "[buyer role] workflow problems"
- "[problem domain] agency pricing" / "[problem domain] consultant rates" (willingness-to-pay signals)
- "[problem domain] spreadsheet workaround" / "[problem domain] manual process" (active workaround signals)
- If competitor-analysis has already been run, pull review mining and customer segment data from it instead of re-researching
- If gtm-strategy has already been run, pull ICP and message-market fit data from it

## Sub-Skill Mode

See `_shared/philosophy.md` Sub-Skill Mode Protocol.

## End-to-End Flow

### STEP 0 — CONTEXT GATHERING

Extract from the user's input:
- The business idea or product (what it does, who it's for)
- The problem the founder believes they're solving (in the founder's words)
- Current stage (idea, MVP, live product with customers)
- Any existing customer evidence (interviews, reviews, usage data)
- Whether the founder has personally experienced this problem

If the idea description is too vague to assess the problem, ask ONE clarifying question. Otherwise, proceed to research.

### STEP 1 — PROBLEM DISCOVERY RESEARCH

Research whether real people actually experience this problem. Not what the founder thinks — what the market says.

**Search queries to run (adapt to the specific problem domain):**
- Do real people complain about this problem online? (Reddit, forums, Quora, review sites)
- How do people currently describe this pain? (Capture exact language — phrases, words, emotional tone)
- What are the existing workarounds? (Spreadsheets, manual processes, duct-tape solutions, hiring agencies)
- Is this pain trending up or down? (Google Trends, new regulations, industry shifts)
- Are there adjacent communities discussing this problem? (Subreddits, Slack groups, Facebook groups, forums)
- What trigger events create this problem? (New hire, scaling, compliance change, seasonal event)

**From competitor intelligence (if available):**
- What do negative reviews say about existing solutions? (Unmet needs = problem evidence)
- What customer segments are most vocal about the pain?
- What pricing do competitors charge? (High prices = high pain tolerance)

### STEP 2 — WILLINGNESS-TO-PAY RESEARCH

Evidence that people spend money (or significant time) to address this problem. Stated intent is weak. Revealed preference is strong.

**Search queries to run:**
- What do competitors charge for solutions in this space? (Pricing pages, review sites)
- What do agencies/consultants charge for doing this manually? (Hourly rates, project fees)
- Are there premium tools in this category? What do they cost?
- Do companies have budget line items for this category? (Job postings mentioning tools, procurement data)
- Are there free alternatives? If so, why do paid versions still exist? (What do paid users get that free users don't?)
- What's the cost of NOT solving this problem? (Lost revenue, wasted time, compliance fines, opportunity cost)

**From prior intelligence (if available):**
- competitor-analysis: pricing tiers, revenue estimates, customer willingness-to-pay signals
- market-size: demand signals, beachhead spending patterns
- gtm-strategy: distribution economics, LTV benchmarks

### STEP 3 — BUYER PERSONA RESEARCH

Who exactly has this problem, and can you find them?

**Search queries to run:**
- What job titles deal with this problem daily? (LinkedIn search, job postings)
- What company types/sizes experience this most acutely? (SMB, mid-market, enterprise, solo operators)
- Where do these buyers congregate online? (Communities, events, publications, podcasts)
- What's their buying process? (Self-serve, committee, procurement, credit card on the spot)
- Are they the user AND the buyer, or is there a split? (End user vs. budget holder)
- What other tools do they already use? (Stack context — what ecosystem are they in?)

**From prior intelligence (if available):**
- competitor-analysis: customer segments, company sizes, geographic clusters
- gtm-strategy: ICP definition, beachhead segment, congregation points

### STEP 4 — NINE-DIMENSION PROBLEM ASSESSMENT

Work through all nine dimensions. For each, assess based on research evidence, rate categorically, and note the specific evidence that supports the rating.

---

#### Dimension 1: Problem Existence & Evidence

Does this problem actually exist outside the founder's head? What's the evidence quality?

**Evidence hierarchy (strongest to weakest):**

| Evidence Type | Strength | Example |
|--------------|----------|---------|
| **People paying to solve it** | Strongest | Competitor revenue, agency fees, tool spend |
| **People spending significant time on workarounds** | Strong | Spreadsheet processes, manual workflows, hiring for it |
| **People complaining unprompted** | Moderate | Forum posts, review complaints, social media rants |
| **People confirming when asked** | Weak | Survey responses, interview answers (prone to false positives) |
| **Founder's intuition** | Weakest | "I think people need this" with no external validation |

**What to evaluate:**
- Can you find real people describing this problem in their own words? (Not prompted, not hypothetical)
- How many independent sources confirm the problem exists?
- Is the evidence from potential buyers or just observers?
- Does the evidence come from the target segment or a different population?
- Is the founder's description of the problem the same as the customer's?

**Rate: PROVEN / INDICATED / ASSUMED / CONTRADICTED**
- PROVEN: Multiple independent evidence sources, money already changing hands
- INDICATED: Some evidence exists but limited in scope or recency
- ASSUMED: Founder believes it exists, but no independent evidence found
- CONTRADICTED: Evidence suggests the problem is not significant or is already well-solved

---

#### Dimension 2: Pain Severity

How bad is this problem? Annoyances don't generate revenue. Hair-on-fire problems do.

**Pain severity spectrum:**

| Level | What It Looks Like | Buying Behavior |
|-------|--------------------|-----------------|
| **Hair-on-fire** | Actively disrupting operations, costing real money, people desperate for a fix | Will buy immediately, pay premium, tolerate imperfect product |
| **Significant** | Causes real friction, people actively complain, but can function without a fix | Will evaluate options, compare alternatives, buy if value is clear |
| **Moderate** | Noticeable inconvenience, people acknowledge it but aren't losing sleep | Will try free solutions, slow to pay, need convincing |
| **Mild** | Nice-to-solve, people shrug when asked about it | Won't pay, won't switch, won't prioritize |

**What to evaluate:**
- What happens if the problem goes unsolved? (Nothing = mild. Revenue loss = severe.)
- How much time/money do people currently waste on this? (Quantifiable pain = real pain)
- Is the language emotional or clinical? ("This is killing me" vs. "It would be nice if...")
- Would people pay to make this problem go away TODAY? Or would they put it on "someday"?
- Is there a compliance or legal consequence to not solving it?

**Rate: HAIR-ON-FIRE / SIGNIFICANT / MODERATE / MILD**

---

#### Dimension 3: Pain Frequency & Predictability

How often does this problem occur? One-time problems rarely support recurring revenue.

**What to evaluate:**
- Is this a daily/weekly/monthly/yearly/one-time problem?
- Is the frequency predictable? (Recurring on a schedule vs. random occurrence)
- Does frequency increase with scale? (More customers = more instances of the problem)
- Is the problem tied to a specific lifecycle stage? (Onboarding, scaling, compliance audit)
- Can the problem support a subscription model? (Recurring pain = recurring revenue)

**Bootstrapper lens:** Recurring problems justify SaaS subscriptions. One-time problems fit one-time purchases or services. Seasonal problems need enough market size to sustain revenue year-round. If the pain only strikes once per company lifetime, you need an enormous addressable market to sustain growth.

**Rate: HIGH / MODERATE / LOW / ONE-TIME**
- HIGH: Daily or weekly occurrence, predictable, scales with business
- MODERATE: Monthly or quarterly, somewhat predictable
- LOW: A few times per year, unpredictable
- ONE-TIME: Happens once per company or per lifecycle stage

---

#### Dimension 4: Current Solutions & Workarounds

What are people doing about this problem today? Active workarounds are the strongest evidence that the problem is real.

**Workaround types (from most to least promising):**

| Type | What It Means | Opportunity |
|------|--------------|-------------|
| **Active workarounds** | People built spreadsheets, hired VAs, cobbled together tools | Strong — they'll pay for something better |
| **Passive coping** | People know the problem exists but just live with the friction | Moderate — need to prove the cost of inaction |
| **Unaddressed** | People don't realize they have the problem or don't think it's solvable | Risky — requires education-heavy GTM |
| **Well-served** | Good solutions already exist and people are satisfied | Weak — need a 10x better or fundamentally different approach |

**What to evaluate:**
- What specific tools, processes, or hacks do people currently use?
- How much do current workarounds cost in time and money?
- What's broken about current workarounds? (The gap between what they have and what they need)
- Are people switching between solutions? (Churn from existing tools = unmet needs)
- Is anyone paying agencies or consultants for what could be automated?

**Rate: ACTIVE WORKAROUNDS / PASSIVE COPING / UNADDRESSED / WELL-SERVED**

---

#### Dimension 5: Willingness to Pay

Is there evidence that people will actually open their wallets? This is the dimension where most founder assumptions shatter.

**Evidence hierarchy (strongest to weakest):**

| Evidence | Strength |
|----------|----------|
| People already paying for similar solutions | Strongest |
| Budget exists in adjacent category (agency spend, consultant fees) | Strong |
| People state they'd pay (interviews, surveys) | Weak — people lie |
| No evidence of spending in this category | Weakest |

**What to evaluate:**
- Are competitors generating revenue? (Revenue = proven WTP)
- What price range do existing solutions command? (Market-established pricing)
- Is there agency or consultant spend that could be displaced? (Budget already allocated)
- Do target buyers have purchasing authority? (Can they swipe a credit card or need procurement?)
- What's the switching cost FROM current workarounds? (Low switching cost = easier sale but also easier churn)
- Is the value quantifiable in dollars? ("Save X hours/week" or "reduce Y% errors" — can they calculate ROI?)

**Rate: PROVEN BUDGET / ADJACENT BUDGET / STATED INTENT / NO EVIDENCE**
- PROVEN BUDGET: Competitors have revenue, customers pay for this category
- ADJACENT BUDGET: Money spent on agencies, consultants, or adjacent tools
- STATED INTENT: People say they'd pay but no revealed preference
- NO EVIDENCE: No pricing signals, no budget, no spending in this category

---

#### Dimension 6: Urgency & Trigger Events

What makes someone go from "this is a problem" to "I need to solve this NOW"? Without triggers, problems stay on the backlog forever.

**Trigger types:**

| Type | Example | Sales Implication |
|------|---------|-------------------|
| **Regulatory** | New compliance deadline, audit notification | Time-bound — must act |
| **Growth** | Scaling past manual processes, new hire onboarding | Capacity-driven — pain intensifies |
| **Pain spike** | System failure, customer complaint, lost deal | Emotional — ready to buy immediately |
| **Lifecycle** | New role, new company, new market entry | Transition — open to new tools |
| **Seasonal** | Tax season, year-end, holiday rush | Predictable — marketing calendar exists |

**What to evaluate:**
- Is there a specific trigger event that creates urgency to solve this?
- Can you identify when the trigger happens? (Predictable = marketable)
- How long does the urgency window last? (Hours, days, weeks)
- Can you detect the trigger externally? (Job postings, funding announcements, regulatory notices)
- Without a trigger, do people ever prioritize this problem?

**Rate: URGENT / SITUATIONAL / CHRONIC / NO TRIGGER**
- URGENT: Clear trigger events create time pressure, buyer acts within days
- SITUATIONAL: Trigger exists but urgency is moderate, buyer acts within weeks/months
- CHRONIC: Ongoing low-grade pain with no specific trigger, stays on "someday" list
- NO TRIGGER: No identifiable event that moves this from awareness to action

---

#### Dimension 7: Buyer Persona Clarity

Can you describe exactly who has this problem, find them, and reach them?

**Clarity spectrum:**

| Level | What You Know | GTM Implication |
|-------|--------------|-----------------|
| **Razor-sharp** | Job title, company size, industry, trigger event, congregation points, buying process | Can run targeted campaigns from day one |
| **Clear** | Role type and company profile known, but specifics need validation | Can start outreach, need to narrow through testing |
| **Vague** | "Small businesses" or "marketers" — too broad to target efficiently | CAC will be high, messaging will be generic, GTM will struggle |
| **Unknown** | "Everyone" or "people who..." — no concrete buyer identity | Stop. Do customer discovery before building anything. |

**What to evaluate:**
- Can you name the job title of the person who has this problem?
- Can you name the company type (size, industry, stage) where this is most acute?
- Do you know where they congregate? (Online communities, events, publications)
- Do you know their buying process? (Self-serve, team decision, procurement)
- Is the user the buyer? (Or does someone else hold the budget?)
- Can you list 10 specific companies that would be prospects?

**Rate: RAZOR-SHARP / CLEAR / VAGUE / UNKNOWN**

---

#### Dimension 8: Problem Scope & Segmentation

Is the problem focused enough to solve well, or so diffuse that you'd need to be everything to everyone?

**What to evaluate:**
- Is this one problem or a cluster of related but distinct problems?
- Can you solve it for one segment without needing to solve it for all?
- Is there a beachhead segment where the problem is most acute? (Smallest viable market with the most pain)
- Does the problem manifest differently in different segments? (If so, which version do you solve first?)
- Can you define what's OUT of scope? (If you can't draw a boundary, the scope is too diffuse)

**Bootstrapper lens:** Diffuse problems require broad solutions that compete with everyone. Focused problems let you build deep, win a niche, then expand. The ideal problem is narrow enough to dominate but large enough to sustain a business. If you're trying to solve "communication" or "productivity" or "data management" — scope is too diffuse. If you're solving "inventory reconciliation for Shopify merchants with 3+ warehouses" — that's focused.

**Rate: FOCUSED / SEGMENTABLE / DIFFUSE / UNCLEAR**
- FOCUSED: One clear problem for one clear segment, boundaries well-defined
- SEGMENTABLE: Multiple segments have this problem, can be addressed one at a time
- DIFFUSE: Problem is broad, hard to scope, different for everyone
- UNCLEAR: Can't define the boundary of the problem

---

#### Dimension 9: Hair-on-Fire Test

The ultimate synthesis. If you walked into a room of your target buyers and described this problem, how many would lean forward?

**The test:**
- ON FIRE: "Yes! I've been looking for a solution. Can I try it today?" — active demand exists
- WARM: "That's a real problem for me. Tell me more." — interest but not urgency
- LUKEWARM: "Yeah, I guess that's annoying sometimes." — acknowledged but low priority
- COLD: "I don't really think about that." — not a problem they recognize

**What to synthesize:**
- Combine all evidence from dimensions 1-8
- Weight revealed preference (spending, workarounds) over stated preference (surveys, interviews)
- Consider: if you built this product tomorrow and put it in front of the target buyer, would they pull out their credit card? Or would they say "interesting, send me updates"?
- The gap between "interesting" and "take my money" is where most ideas die

**Rate: ON FIRE / WARM / LUKEWARM / COLD**

---

### STEP 4b — VALIDATION GATES

Six binary checks. Pass/fail. No nuance.

| # | Gate | Pass/Fail |
|---|------|-----------|
| 1 | Real people describe this pain in their own words (not prompted by the founder) | |
| 2 | Someone is already paying to solve this (money or significant time on workarounds) | |
| 3 | Buyer is identifiable by job title and company type | |
| 4 | A trigger event exists that creates urgency | |
| 5 | Problem recurs frequently enough to support ongoing payment | |
| 6 | Founder's framing matches customer language (or the gap is identified) | |

**Gates passed: X/6**

- **6/6**: Strong foundation — proceed with confidence
- **4-5/6**: Viable but has gaps — address the failing gates before scaling
- **< 4/6**: RED FLAG — significant validation gaps exist
- **< 3/6**: STOP — do customer discovery before building anything

### STEP 5 — OUTPUT

Produce the full report using the template below.

## Output Template

```
# PROBLEM ANALYSIS: [Product/Idea Name]

Research date: [date]
Stage: [Idea / MVP / Live Product]
Founder's problem statement: "[The problem as the founder described it]"

---

## PROBLEM VALIDITY SCORE

Overall verdict: [PROBLEM WORTH SOLVING / NEEDS MORE EVIDENCE / PROBLEM IS WEAK / NO PROBLEM FOUND]

| Dimension | Rating | Evidence Summary |
|-----------|--------|-----------------|
| Problem Existence & Evidence | PROVEN/INDICATED/ASSUMED/CONTRADICTED | |
| Pain Severity | HAIR-ON-FIRE/SIGNIFICANT/MODERATE/MILD | |
| Pain Frequency | HIGH/MODERATE/LOW/ONE-TIME | |
| Current Solutions | ACTIVE WORKAROUNDS/PASSIVE COPING/UNADDRESSED/WELL-SERVED | |
| Willingness to Pay | PROVEN BUDGET/ADJACENT BUDGET/STATED INTENT/NO EVIDENCE | |
| Urgency & Triggers | URGENT/SITUATIONAL/CHRONIC/NO TRIGGER | |
| Buyer Persona Clarity | RAZOR-SHARP/CLEAR/VAGUE/UNKNOWN | |
| Problem Scope | FOCUSED/SEGMENTABLE/DIFFUSE/UNCLEAR | |
| Hair-on-Fire Test | ON FIRE/WARM/LUKEWARM/COLD | |

---

## VALIDATION GATES

| # | Gate | Result |
|---|------|--------|
| 1 | Real people describe this pain in their own words | PASS / FAIL |
| 2 | Someone is already paying to solve this | PASS / FAIL |
| 3 | Buyer identifiable by job title and company type | PASS / FAIL |
| 4 | Trigger event exists that creates urgency | PASS / FAIL |
| 5 | Problem recurs frequently enough for ongoing payment | PASS / FAIL |
| 6 | Founder's framing matches customer language | PASS / FAIL |

**Gates passed: X/6** — [Assessment: Strong foundation / Viable with gaps / RED FLAG / STOP]

---

## PROBLEM EXISTENCE DEEP DIVE

**Evidence found:**

| Source | What People Say | Strength |
|--------|----------------|----------|
| [Forum/review/social post] | "[Exact quote or close paraphrase]" | Strong/Moderate/Weak |
| [Source 2] | "[Quote]" | |
| [Source 3] | "[Quote]" | |

**Customer language captured:**
- How customers describe the problem: "[their words]"
- How the founder describes the problem: "[founder's words]"
- **Language gap**: [Match / Minor gap / Significant gap — explain]

**Evidence quality**: [Strong / Moderate / Thin — explain what's missing]

---

## PAIN SEVERITY ASSESSMENT

**Current cost of the problem:**
- Time wasted: [hours/week or month, if quantifiable]
- Money spent on workarounds: [dollar amount or range]
- Opportunity cost: [revenue lost, deals missed, customers churned]
- Compliance/legal risk: [if applicable]

**Pain trajectory**: [Getting worse / Stable / Getting better — and why]

**Severity verdict**: [HAIR-ON-FIRE / SIGNIFICANT / MODERATE / MILD]
[2-3 sentences explaining why this level, with specific evidence]

---

## CURRENT SOLUTIONS & WORKAROUND MAP

| Solution/Workaround | Type | Cost | What's Broken |
|---------------------|------|------|---------------|
| [Competitor tool] | Direct competitor | $X/mo | [Specific gap] |
| [Spreadsheet/manual process] | DIY workaround | X hours/week | [Limitations] |
| [Agency/consultant] | Outsourced | $X/project | [Why it's not ideal] |
| [Do nothing] | Passive coping | [Hidden cost] | [Consequences] |

**Workaround intensity**: [How much effort are people expending? More effort = more pain = more willingness to pay for a real solution]

---

## WILLINGNESS-TO-PAY ASSESSMENT

**Pricing signals from the market:**
- Competitor pricing: [range]
- Agency/consultant rates: [range]
- Adjacent tool pricing: [range]
- Budget holder: [who controls the spend — self-serve buyer vs. procurement]

**WTP verdict**: [PROVEN BUDGET / ADJACENT BUDGET / STATED INTENT / NO EVIDENCE]
[2-3 sentences on the revenue potential based on pricing signals]

---

## BUYER PERSONA

**Primary buyer:**
- Job title(s): [specific titles]
- Company type: [size, industry, stage]
- Trigger event: [what makes them buy NOW]
- Where they congregate: [communities, events, publications]
- Buying process: [self-serve / team / procurement]
- User = Buyer? [Yes / No — if no, describe the split]

**Persona clarity**: [RAZOR-SHARP / CLEAR / VAGUE / UNKNOWN]

**Beachhead drift**: [ALIGNED / DRIFTED — if drifted, who does evidence point to as the real beachhead? See _shared/philosophy.md Beachhead Drift section for drift patterns.]

**Can you list 10 prospect companies?** [Yes — list them / No — explain what's missing]

---

## URGENCY & TRIGGER MAP

| Trigger Event | Frequency | Detectability | Urgency Level |
|--------------|-----------|---------------|---------------|
| [Trigger 1] | [How often] | [Can you detect it externally?] | [High/Medium/Low] |
| [Trigger 2] | | | |
| [Trigger 3] | | | |

**Without triggers, does this problem ever get prioritized?** [Yes/No — explain]

---

## FOUNDER ASSUMPTION vs. MARKET REALITY

| What the Founder Believes | What the Evidence Shows | Gap |
|--------------------------|------------------------|-----|
| [Founder's problem framing] | [Market evidence] | [Match / Minor / Significant] |
| [Founder's target customer] | [Actual sufferers] | |
| [Founder's severity estimate] | [Evidence-based severity] | |
| [Founder's WTP assumption] | [Market WTP signals] | |
| [Founder's urgency belief] | [Actual trigger evidence] | |

**Biggest assumption gap**: [The single most dangerous assumption — where the founder's belief diverges most from evidence]

---

## CUSTOMER DISCOVERY RECOMMENDATIONS

[Only include this section if validation gates < 5/6 or evidence quality is thin]

**What you still don't know:**
1. [Specific unknown that matters]
2. [Specific unknown that matters]
3. [Specific unknown that matters]

**Recommended discovery actions:**

| Action | What It Validates | How to Do It | Minimum Sample |
|--------|-------------------|-------------|----------------|
| [Interview target buyers] | [Problem existence, severity, language] | [Where to find them, what to ask] | [5-10 conversations] |
| [Analyze competitor reviews] | [Unmet needs, pain language] | [Which review sites, what to look for] | [50+ reviews] |
| [Run a smoke test] | [WTP, urgency] | [Landing page, waitlist, prototype] | [100+ visitors] |
| [Monitor community] | [Frequency, trigger events] | [Which communities, what keywords] | [2-4 weeks observation] |

**Do NOT build until**: [Specific validation milestone — e.g., "5 potential buyers describe this pain without prompting and state current workaround costs"]

---

## BOTTOM LINE

**Problem verdict**: [PROBLEM WORTH SOLVING / NEEDS MORE EVIDENCE / PROBLEM IS WEAK / NO PROBLEM FOUND]

[2-3 sentences. Is this problem real enough to build a business around? What's the strongest evidence? What's the biggest risk? If evidence is thin, how long would discovery take to get confidence?]

**The honest answer to "is this problem real?":**
[One sentence. The real answer, not the comfortable one.]

**Founder-vs-reality gap:**
[One sentence. The single most important place where the founder's assumptions don't match market evidence. If they match, say so.]

**Top 3 actions for the next 7 days:**
1. [Specific, concrete, actionable — related to validating the weakest dimension]
2. [Specific, concrete, actionable]
3. [Specific, concrete, actionable]

---
[If invoked as sub-skill: produce DIGEST summary per `_shared/philosophy.md` Digest Mode format]
```

## Important Rules

See `_shared/philosophy.md` Universal Skill Rules.

**Skill-specific rules:**
- **Evidence over intuition** — every rating must cite specific evidence. "This seems like a real problem" is not analysis. "47 Reddit posts in r/ecommerce describe this exact frustration" is analysis.
- **Capture customer language** — exact phrases people use to describe the problem. This is gold for GTM messaging and directly feeds into gtm-strategy if run later.
- **Measure the founder-reality gap** — the signature insight of this skill. Compare what the founder believes vs. what evidence shows for every major dimension. Be honest about the gap.
- **Don't manufacture confidence** — if evidence is thin, say so. Prescribe specific discovery actions instead of producing a confident analysis on insufficient data. "NEEDS MORE EVIDENCE" is a valid and valuable verdict.
- **Willingness to pay requires revealed preference** — people saying "I'd pay for that" is nearly worthless. People already paying competitors, hiring agencies, or spending hours on spreadsheet workarounds is strong evidence.
- **Buyer persona must be specific** — "small businesses" is not a persona. "Operations managers at 20-100 employee e-commerce companies who just opened a second warehouse" is a persona.
- **Name specific communities and sources** — "people complain about this" is vague. "r/shopify, the Shopify Community forums, and TrustPilot reviews for [competitor]" is actionable.
- **Validate trigger events** — without a trigger event, problems stay on the "someday" list. If you can't find a trigger, that's a major risk.
