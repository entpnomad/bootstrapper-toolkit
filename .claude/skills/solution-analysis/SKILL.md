---
name: solution-analysis
description: Product fitness and solution validation for bootstrapped founders. Assesses whether THIS specific solution is the right way to address a validated problem — value proposition clarity, solution-problem fit, minimum product achievability, differentiation reality, switching motivation, time-to-value, retention potential, and substitute vulnerability. Use when user runs `/solution-analysis`, asks about "is this the right solution", "product-market fit", "differentiation", "MVP scope", "time to value", "substitute threat", "should I build this", "solution validation", or needs to evaluate whether a specific product approach is worth building.
---

# Solution Analysis — Product Fitness for Bootstrappers

When code is cheap, the question is never "can we build it?" — it's "is this the right thing to build?"

## Philosophy

**Building is easy. Knowing WHAT to build is scarce.** AI tools collapsed dev cost to near zero. Any founder can ship a functional product in a weekend. This creates a dangerous new failure mode: building the wrong thing, fast. The clarity bottleneck means founders ship features nobody asked for, solve problems from the wrong angle, and mistake "I can build it" for "I should build it."

Read `.claude/skills/_shared/philosophy.md` for the full bottleneck shift and bootstrapper framework. For solution analysis specifically:

**Solution ≠ problem.** This skill assumes the problem exists (problem-analysis validates that). The question here is: given a real problem, is THIS specific approach — this product, this feature set, this user experience — the right way to address it? A real problem with the wrong solution is still a dead business.

**AI-native reality check — false confidence traps:**
- "We can build it, therefore we should" — build cost approaching zero makes this the most dangerous sentence in startups
- "Our feature list is longer" — features are commoditized; a competitor can match them in days
- "It's like X but better" — cosmetic differentiation is not differentiation; if "better" means "same thing, slightly nicer," you have nothing
- "We'll figure out the value prop later" — if you can't articulate why someone switches to your product in one sentence, you don't have a product
- "AI can't do this" — verify explicitly; AI capabilities expand monthly and free AI tools are the most dangerous substitute

**What IS a strong solution:**
- Value proposition statable in one sentence a user cares about (not a founder cares about)
- Direct hit on the #1 pain point — not a tangential attack on a secondary annoyance
- Meaningful first version shippable within weeks, not quarters
- Differentiation based on structural trade-offs competitors can't copy without cannibalizing their own position
- Time-to-value fast enough that users experience the payoff before they forget why they signed up
- Retention designed into the product — usage creates value that compounds

## Reference Books

Check `references/INDEX.md` for relevant frameworks. Key topics for solution validation: habit-forming product design and stored value loops, build-less philosophy and scope control, shaping and appetite-based scoping, lean experimentation and validated learning, opportunity trees and assumption mapping, product-led growth and activation, product-market fit methodology, product positioning and differentiation.

## Research-First Protocol

Research autonomously before outputting anything. See `_shared/philosophy.md` for the full protocol. Key searches:

- "[problem domain] solutions" / "[problem domain] tools" / "[problem domain] approaches"
- "[competitor category] reviews" / "[competitor category] onboarding experience" / "[competitor category] time to value"
- "[product category] Product Hunt" / "[product category] alternatives" / "[product category] vs"
- "[problem domain] workflow" / "[problem domain] how people currently do this"
- "[competitor] demo" / "[competitor] first experience" / "[competitor] getting started"
- "AI [problem domain]" / "ChatGPT [problem domain]" / "free AI [problem domain]" (substitute threat)
- If problem-analysis has already been run, pull pain severity, workaround data, and customer language from it instead of re-researching
- If competitor-analysis has already been run, pull product comparisons, pricing, and feature data from it
- If moat-analysis has already been run, pull switching cost and lock-in data from it
- If gtm-strategy has already been run, pull positioning, ICP, and message-market fit data from it

## Sub-Skill Mode

See `_shared/philosophy.md` Sub-Skill Mode Protocol.

## End-to-End Flow

### STEP 0 — CONTEXT GATHERING

Extract from the user's input:
- The business idea or product (what it does, who it's for)
- The problem it claims to solve (the pain point)
- The proposed solution approach (how it solves the problem — UX, features, delivery mechanism)
- Current stage (idea, prototype, MVP, live product with customers)
- Any stated differentiation claim (why this is better/different)
- Target user (who uses it, what their day looks like)
- Any evidence of product-market fit (usage data, retention, NPS, paying customers)

If the idea description is too vague to assess the solution, ask ONE clarifying question: "Describe what the user does in their first session — what do they see, what do they do, what value do they get?" Otherwise, proceed to research.

### STEP 1 — SOLUTION LANDSCAPE RESEARCH

Research how people currently solve this problem. Not the competitive landscape (competitor-analysis handles that) — the solution approaches and user experiences.

**Search queries to run (adapt to the specific solution domain):**
- How do people currently handle this workflow? (Current tools, manual processes, workarounds)
- What does the user experience look like for existing solutions? (Onboarding, time to first value, friction points)
- What do users praise and complain about in current solutions? (Reviews, forums, social media)
- What's the time-to-value for alternatives? (How fast do users get the payoff?)
- Are there free or AI-powered alternatives emerging? (ChatGPT workflows, free tools, open-source options)
- What does the typical "first session" look like for competing products? (Product Hunt demos, YouTube walkthroughs, getting-started guides)

**From prior intelligence (if available):**
- problem-analysis: pain severity, workaround map, customer language, WTP evidence
- competitor-analysis: product features, pricing, reviews, positioning, gaps
- moat-analysis: switching costs, lock-in mechanisms, user investment patterns
- gtm-strategy: ICP, message-market fit, positioning recommendations

### STEP 2 — NINE-DIMENSION SOLUTION ASSESSMENT

Work through all nine dimensions. For each, assess based on research evidence, rate categorically, and note the specific evidence that supports the rating.

---

#### Dimension 1: Value Proposition Clarity

Can you articulate why someone would use this product — in one sentence a user would care about? Not a founder sentence. A user sentence.

**Clarity spectrum:**

| Level | What It Looks Like | User Reaction |
|-------|--------------------|---------------|
| **RAZOR-SHARP** | One sentence that makes the user lean forward. Specific outcome, specific user, obvious value. | "Where do I sign up?" |
| **CLEAR** | Value is understandable but takes a paragraph to explain. Benefit is real but not instantly graspable. | "Okay, tell me more." |
| **FUZZY** | Value exists somewhere but is buried under features, jargon, or scope creep. Founder can explain it; user can't repeat it. | "I think I get it... what exactly does it do?" |
| **ABSENT** | No articulated value prop. A technology looking for a use case. Features described but not connected to a user outcome. | "So... why would I use this?" |

**What to evaluate:**
- Can you state the value prop in < 15 words? (If not, it's not clear enough)
- Is it stated from the user's perspective? ("You get X" not "We built Y")
- Does it describe an outcome or a feature? (Outcomes sell. Features don't.)
- Would the target user understand it without context? (No jargon, no insider knowledge required)
- Does it pass the "so what?" test? (Every claim should survive "so what?" asked three times)
- Is the value prop the same as the founder's problem description, or has it drifted?

**AI-native lens:** When code is cheap, value props based on "we built a tool that..." are weak. Anyone can build a tool. The value prop must be about the outcome: time saved, money made, pain eliminated, status gained. "We automate X" is a feature. "You stop losing Y hours/week to Z" is a value prop.

**Rate: RAZOR-SHARP / CLEAR / FUZZY / ABSENT**

---

#### Dimension 2: Solution-Problem Fit

Does this solution attack the core of the problem, or does it nibble at the edges?

**Fit spectrum:**

| Level | What It Means | Risk |
|-------|--------------|------|
| **DIRECT HIT** | Solution addresses the #1 pain point head-on. The problem and solution are obviously connected. Users immediately see "this solves my problem." | Low risk — validate execution |
| **ADJACENT** | Solution addresses a related pain point or a secondary aspect of the problem. Useful but not essential. | Moderate risk — may get "nice to have" not "must have" |
| **TANGENTIAL** | Solution touches the problem domain but doesn't solve the core pain. Often happens when founders build what they can, not what's needed. | High risk — users acknowledge the problem but don't see your product as the answer |
| **MISALIGNED** | Solution doesn't actually address the stated problem. Common when the founder's vision diverges from user reality. | Fatal — stop and re-examine |

**What to evaluate:**
- Does the solution address the #1 pain point identified by problem-analysis? (Or a secondary pain?)
- If you removed all features except one, which would remain — and does it hit the core pain?
- Do user reviews of similar products suggest this approach works? (Or do they want something different?)
- Is the founder solving the problem the way USERS want it solved, or the way the FOUNDER thinks it should be solved?
- Would users describe their problem and arrive at this solution independently? (Or is it a leap?)

**AI-native lens:** When founders can build anything fast, they often build what's interesting to build rather than what users need. The gap between "technically elegant solution" and "solution users want" is where products die. If problem-analysis captured customer language, does this solution match those words?

**Rate: DIRECT HIT / ADJACENT / TANGENTIAL / MISALIGNED**

---

#### Dimension 3: Minimum Product Achievability (MPA)

How fast can you ship a version that delivers the core value? Not a demo. Not a landing page. A product someone would pay for (or invest time in, for freemium).

**Achievability spectrum:**

| Level | What It Means | Implication |
|-------|--------------|-------------|
| **SHIP THIS WEEK** | Core value deliverable with existing tools, APIs, and frameworks. No novel technology needed. One founder can ship it. | Do it. Stop planning. Ship. |
| **SHIP THIS MONTH** | Core value clear but requires meaningful integration, data pipeline, or UX work. Still one-founder achievable. | Good scope. Time-box it. Don't expand scope. |
| **SHIP THIS QUARTER** | Requires significant development, multiple integrations, or domain-specific complexity. Risk of scope creep is high. | Dangerous — can you cut scope? What's the one-week version? |
| **SHIP NEXT YEAR** | Requires infrastructure, team, partnerships, regulatory approval, or fundamental R&D. Not a bootstrapper MVP. | RED FLAG — either find a simpler version or question whether this is a bootstrapper opportunity |

**What to evaluate:**
- What's the absolute minimum feature set that delivers the core value prop?
- Can the core value be delivered with a spreadsheet + Zapier? (If yes, why build custom software?)
- What's the single biggest technical risk? (The thing that could block shipping)
- Does the MVP require data that doesn't exist yet? (Cold start problem)
- Is the founder scoping the MPA or the "wouldn't it be cool if" version?
- What can be manual on day one and automated later? (Wizard of Oz approach)

**AI-native lens:** When code is cheap, MPA is rarely about technical difficulty. It's about clarity. Founders who can't ship in a week usually don't have a clarity problem with technology — they have a clarity problem with scope. If you can't define the one-week version, you don't understand the product yet.

**Rate: SHIP THIS WEEK / SHIP THIS MONTH / SHIP THIS QUARTER / SHIP NEXT YEAR**

---

#### Dimension 4: Differentiation Reality

What makes this solution meaningfully different from alternatives? "Better" is not differentiation. "Different in a way that matters to a specific user" is differentiation.

**Differentiation spectrum:**

| Level | What It Means | Durability |
|-------|--------------|------------|
| **STRUCTURAL** | Differentiation comes from a trade-off competitors can't or won't make. Counter-positioned against incumbents. Built into the business model, not the feature set. | Durable — competitors can't copy without hurting themselves |
| **MEANINGFUL** | Clear, user-valued difference. Not just "more features" — a genuinely different approach that some users prefer. Could be copied but requires real effort. | Moderate — defensible for 12-24 months |
| **COSMETIC** | "Like X but with a better UI" / "Same thing but cheaper" / "Same thing but for [segment]." Can be matched by any competitor with a weekend of work. | Weak — erasable in weeks |
| **NONE** | No articulated difference. "We're building [category]." Relies on execution speed or founder belief that they'll figure out differentiation later. | Zero — commodity from day one |

**What to evaluate:**
- What trade-off does this product make that competitors won't? (True differentiation requires sacrifice)
- Can a competitor add your differentiator as a feature without changing their core business? (If yes — cosmetic)
- Is the differentiation valued by users or only by the founder? (User-valued difference vs. founder vanity)
- Is the differentiation in the product, the business model, or the distribution? (All three are valid, but product-only is weakest)
- Does the positioning framework (from competitor-analysis or gtm-strategy) support this claim?

**AI-native lens:** When any feature can be replicated in days, product differentiation is the weakest form. Business model differentiation (freemium vs. paid, self-serve vs. sales-led, simple vs. complex) and distribution differentiation (owned audience, community, partnerships) are more durable. The question is not "what does your product do differently?" but "what about your business is structurally different?"

**Rate: STRUCTURAL / MEANINGFUL / COSMETIC / NONE**

---

#### Dimension 5: Switching Motivation

Why would someone stop using their current solution and switch to yours? Switching has real costs — learning curves, data migration, workflow disruption, team retraining. The benefit must exceed these costs decisively.

**Motivation spectrum:**

| Level | What It Means | Expected Behavior |
|-------|--------------|-------------------|
| **COMPELLING** | Current solution causes active pain. Users are looking for alternatives. Switching cost is justified by immediate, obvious benefit. | Users switch proactively, tolerate setup friction |
| **FAVORABLE** | Current solution is adequate but has known gaps. Switching benefit is real but not urgent. Users will switch if the process is easy. | Users switch when triggered (contract renewal, pain spike, growth event) |
| **MARGINAL** | Current solution works fine. Your product is slightly better in some dimension but not enough to justify switching friction. | Users say "interesting" but don't act. Conversion rate will be painful. |
| **INSUFFICIENT** | Current solution is good enough. No clear reason to switch. Product is a vitamin, not a painkiller. | Users won't switch. New users might try but existing users won't move. |

**What to evaluate:**
- What's the switching cost FROM the current solution? (Data migration, workflow rebuilding, team retraining, contract lock-in)
- What's the immediate benefit of switching? (Time saved, money saved, capability gained — in the first week, not the first year)
- Is the switching benefit large enough to overcome inertia? (Users default to doing nothing)
- Are there natural switching moments? (Contract renewal, tool consolidation, team changes, scaling events)
- Can you offer migration assistance or a gradual transition? (Reducing switching friction)

**AI-native lens:** When users have spent months building workflows, importing data, and training their team on a competitor's product, "slightly better" is not a reason to switch. The bar for switching is not "is your product better?" — it's "is your product SO MUCH better that it's worth the pain of migration?" If the answer is "we're 20% better," that's insufficient for most users.

**Rate: COMPELLING / FAVORABLE / MARGINAL / INSUFFICIENT**

---

#### Dimension 6: Time-to-Value

How fast does a new user experience the product's core value? Not "sees a dashboard" — actually gets the promised benefit.

**Time-to-value spectrum:**

| Level | What It Looks Like | Retention Impact |
|-------|--------------------|-----------------|
| **INSTANT** | User gets value in the first session. < 5 minutes to "aha moment." No setup required. | High activation, high retention — users know why they're here |
| **FAST** | User gets value within the first day. Some setup required but the payoff comes quickly. | Good activation if onboarding is smooth. Drop-off risk during setup. |
| **SLOW** | User needs days or weeks of setup, data import, or configuration before seeing value. | High drop-off. Most users will abandon before reaching value. Requires high-touch onboarding or strong motivation. |
| **DEFERRED** | Value only appears after extended use (months of data, team adoption, workflow maturity). | Very high churn risk. Only works if switching costs are already high or if the problem is hair-on-fire. |

**What to evaluate:**
- What does the user's first 5 minutes look like? (If it's "create an account and stare at an empty dashboard" — that's a problem)
- How many steps between signup and first value? (Every step is a drop-off point)
- Can you show value before requiring input? (Pre-populated demos, sample data, guided tours)
- Does the product require other team members or external data to become useful? (Dependencies delay value)
- What's the "aha moment"? (The specific interaction where the user thinks "this is worth it")
- How does time-to-value compare to competitors? (If a competitor delivers value faster, you lose)

**AI-native lens:** When users can try 10 products in a day, the one that delivers value fastest wins. This is the activation filter. If your product requires a 30-minute setup before the user sees any benefit, you've already lost most potential users to a simpler alternative — or to an AI chatbot that delivers 60% of the value in 30 seconds.

**Rate: INSTANT / FAST / SLOW / DEFERRED**

---

#### Dimension 7: Retention & Habit Potential

Will users come back? Does the product create a usage pattern that becomes habitual, or is it a one-time/occasional tool?

**Retention spectrum:**

| Level | Usage Pattern | Revenue Implication |
|-------|--------------|---------------------|
| **HABITUAL** | Users return daily or multiple times per week without prompting. Product becomes part of their workflow. Stored value accumulates. | Strong SaaS economics. Low churn. High LTV. |
| **REGULAR** | Users return weekly or on a predictable schedule. Consistent utility but not a daily habit. | Solid SaaS foundation. Moderate churn. Retention requires ongoing value delivery. |
| **EPISODIC** | Users return when a specific need arises — seasonal, event-driven, or project-based. | Challenging for SaaS. Consider per-use or project pricing. High dormant-user rate. |
| **ONE-TIME** | Users get the value once and don't need to return. The product solves a one-time problem. | Not SaaS-compatible. Transaction pricing or high one-time price required. |

**What to evaluate:**
- Does the product design include a trigger → action → reward → investment loop?
- Does usage create stored value that makes the product more valuable over time? (Content, data, history, configurations)
- Is there a natural frequency to the problem? (Daily workflow = habitual. Annual audit = episodic.)
- What brings users back after their first session? (Internal trigger or external prompt?)
- Does the product have a "pull" mechanism — or does it rely on push notifications and emails to re-engage?
- How does retention compare to the problem frequency? (If the problem is daily but users visit monthly, something is wrong)

**AI-native lens:** Retention is where moat-analysis and solution-analysis intersect. Products that create user investment (content, data, workflows) have structural retention. Products that deliver a result with no stored value (calculators, generators, one-shot tools) have zero retention moat. In the AI age, if your product's value can be replicated by a single prompt, retention will be near zero.

**Rate: HABITUAL / REGULAR / EPISODIC / ONE-TIME**

---

#### Dimension 8: Substitute Vulnerability

Can the core value of this product be replicated by a free tool, an AI chatbot, a spreadsheet, or a human process that's "good enough"?

**Vulnerability spectrum:**

| Level | Substitute Reality | Pricing Power |
|-------|--------------------|---------------|
| **NO VIABLE SUBSTITUTE** | No free or cheap alternative delivers comparable value. The product's value requires proprietary data, integrations, or workflows that can't be replicated casually. | Strong — can charge premium, users have no free escape hatch |
| **EXIST BUT WORSE** | Substitutes exist but are meaningfully worse — slower, harder, less reliable, require more effort. Users who've tried both choose the paid product. | Moderate — pricing must reflect the gap. If gap narrows, pricing power drops. |
| **ADEQUATE** | Free or cheap substitutes deliver 70-80% of the value. Users who don't need the last 20% won't pay. | Weak — must target the segment that needs the 20% premium. Large market is free-tier only. |
| **PREFERRED** | A free alternative (AI chatbot, spreadsheet, manual process) is actually preferred by most users. The paid product adds complexity without proportional value. | Critical — question whether this product should exist |

**What to evaluate:**
- Can ChatGPT / Claude / free AI tools do 80%+ of what this product does? (Test this explicitly — run the workflow through an AI chatbot and compare)
- Is there a spreadsheet or manual process that's "good enough" for most users?
- Are there free open-source alternatives? How do they compare?
- What does the paid product provide that free alternatives genuinely cannot? (Be specific — "better UX" is usually not enough)
- Is the product's value in the output (replicable) or in the workflow/integration/data layer (harder to replicate)?

**AI-native lens — the AI substitute test:** This is critical. For every product, explicitly test: "Can a user achieve this outcome by spending 5 minutes with a free AI chatbot?" If yes, the product must deliver value BEYOND what AI can do — through integrations, stored data, team collaboration, compliance, or workflow automation that a chatbot can't provide. Products that wrap an AI prompt in a UI are vulnerable to the AI provider building the same feature natively.

**Rate: NO VIABLE SUBSTITUTE / EXIST BUT WORSE / ADEQUATE / PREFERRED**

---

#### Dimension 9: Solution Conviction (Synthesis)

The ultimate synthesis. Given everything above — is this the right solution to build?

**The verdict:**

| Level | What It Means | Action |
|-------|--------------|--------|
| **BUILD IT** | Strong value prop, direct problem fit, achievable scope, real differentiation, users will switch, fast time-to-value, retention built in, no killer substitute. | Ship it. Stop analyzing. Build the MPA and get it in front of users. |
| **TEST IT** | Promising but unproven. Some dimensions are strong, others need validation. The riskiest assumptions should be tested before committing fully. | Design the cheapest experiment that tests the riskiest assumption. Don't build the full product yet. |
| **RETHINK IT** | The solution approach has fundamental issues — wrong angle of attack, cosmetic differentiation, slow time-to-value, vulnerable to substitutes. The problem may be real but this isn't the right solution. | Go back to the problem. What would a solution look like if you started from the user's workflow instead of from the feature list? |
| **STOP** | Multiple fatal dimensions — no value prop, misaligned with the problem, substitutes are preferred, no switching motivation. Building this would waste the founder's scarcest resource: time-to-clarity. | Stop. The problem may be real (see problem-analysis) but this solution is not the answer. Invest time in customer discovery, not code. |

**What to synthesize:**
- Combine all evidence from dimensions 1-8
- Weight value prop clarity and solution-problem fit highest (if these are wrong, nothing else matters)
- Consider MPA in context — if everything else is strong, a quarter-long build might be justified. If anything is uncertain, scope down to a week.
- Flag any dimension rated at the lowest level as a potential deal-breaker
- Consider the AI substitute test result — if AI can replicate 80%+ of the value for free, the bar for everything else goes up dramatically

**Rate: BUILD IT / TEST IT / RETHINK IT / STOP**

---

### STEP 2b — VALIDATION GATES

Six binary checks. Pass/fail. No nuance.

| # | Gate | Pass/Fail |
|---|------|-----------|
| 1 | Value prop statable in one sentence a user cares about | |
| 2 | Solution addresses the #1 pain point directly | |
| 3 | Meaningful first version shippable within 4 weeks | |
| 4 | Real, user-valued differentiation exists | |
| 5 | Target user would switch from current solution | |
| 6 | AI/LLM cannot replicate 80%+ of the value for free | |

**Gates passed: X/6**

- **6/6**: Strong solution foundation — proceed with confidence
- **4-5/6**: Viable but has gaps — address the failing gates before scaling
- **< 4/6**: RED FLAG — significant solution fitness issues
- **< 3/6**: STOP — rethink the solution approach before building anything

### STEP 3 — SOLUTION DESIGN STRATEGY

For the top weaknesses identified in the assessment, produce actionable strategies:

**Riskiest Assumption Test** (for every solution):
- What is the single riskiest assumption about this solution?
- What's the cheapest experiment to test it? (Under $100, under 1 week)
- What result would confirm or kill the assumption?
- What decision does the test inform? (Build / pivot / stop)

**Scope Reduction Exercise** (if MPA is SHIP THIS QUARTER or worse):
- What's the one-week version? What feature delivers the core value with nothing else?
- What can be manual on day one? (Support, onboarding, data entry, integrations)
- What features can be "unlocked" only after the core is validated?
- Is there a Wizard of Oz approach — deliver the outcome manually while building the automation?

**Differentiation Strengthening** (if COSMETIC or NONE):
- What trade-off could you make that competitors can't? (Pricing model, target segment, feature philosophy)
- Where do incumbents overserve? (Complexity, features, pricing) — can you win by building LESS?
- Is there a counter-position available? (Self-serve vs. sales-led, freemium vs. paid-only, simple vs. bloated)
- Can differentiation come from distribution rather than product? (Community, content, partnerships)

### STEP 4 — OUTPUT

Produce the full report using the template below.

## Output Template

```
# SOLUTION ANALYSIS: [Product/Idea Name]

Research date: [date]
Stage: [Idea / Prototype / MVP / Live Product]
Proposed solution: "[The solution approach as the founder described it]"
Problem being solved: "[The problem — from problem-analysis if available, otherwise founder's description]"

---

## SOLUTION FITNESS SCORE

Overall verdict: [BUILD IT / TEST IT / RETHINK IT / STOP]

| Dimension | Rating | Evidence Summary |
|-----------|--------|-----------------|
| Value Proposition Clarity | RAZOR-SHARP/CLEAR/FUZZY/ABSENT | |
| Solution-Problem Fit | DIRECT HIT/ADJACENT/TANGENTIAL/MISALIGNED | |
| Minimum Product Achievability | SHIP THIS WEEK/MONTH/QUARTER/NEXT YEAR | |
| Differentiation Reality | STRUCTURAL/MEANINGFUL/COSMETIC/NONE | |
| Switching Motivation | COMPELLING/FAVORABLE/MARGINAL/INSUFFICIENT | |
| Time-to-Value | INSTANT/FAST/SLOW/DEFERRED | |
| Retention & Habit Potential | HABITUAL/REGULAR/EPISODIC/ONE-TIME | |
| Substitute Vulnerability | NO VIABLE SUBSTITUTE/EXIST BUT WORSE/ADEQUATE/PREFERRED | |
| Solution Conviction | BUILD IT/TEST IT/RETHINK IT/STOP | |

---

## VALIDATION GATES

| # | Gate | Result |
|---|------|--------|
| 1 | Value prop statable in one sentence a user cares about | PASS / FAIL |
| 2 | Solution addresses the #1 pain point directly | PASS / FAIL |
| 3 | Meaningful first version shippable within 4 weeks | PASS / FAIL |
| 4 | Real, user-valued differentiation exists | PASS / FAIL |
| 5 | Target user would switch from current solution | PASS / FAIL |
| 6 | AI/LLM cannot replicate 80%+ of the value for free | PASS / FAIL |

**Gates passed: X/6** — [Assessment: Strong foundation / Viable with gaps / RED FLAG / STOP]

---

## VALUE PROPOSITION ASSESSMENT

**Founder's value prop:** "[How the founder describes the value]"
**User-facing value prop:** "[Restated from the user's perspective — what they actually get]"

**Clarity test:**
- In < 15 words: [attempt to state the value prop in under 15 words]
- "So what?" test: [Does it survive three rounds of "so what?"]
- User language match: [Does it use words the target user would use?]

**Value prop verdict:** [RAZOR-SHARP / CLEAR / FUZZY / ABSENT]
[2-3 sentences explaining why, with specific evidence]

---

## SOLUTION-PROBLEM FIT

**Problem being solved:** [The #1 pain point — from problem-analysis or research]
**How this solution attacks it:** [Direct / indirect / tangential]

**Fit analysis:**
- Does the solution hit the core pain? [Yes/No — explain]
- Would users independently arrive at this solution? [Yes/No — explain]
- Does the solution approach match customer language? [Yes/No — explain]

**Fit verdict:** [DIRECT HIT / ADJACENT / TANGENTIAL / MISALIGNED]
[2-3 sentences with evidence]

---

## MINIMUM PRODUCT DEFINITION

**Proposed scope:** [What the founder wants to build]
**Minimum viable scope:** [What actually needs to exist to deliver the core value]

**Scope analysis:**
- Core value feature(s): [The 1-2 features that deliver 80% of the value]
- Nice-to-have features: [Features that can be cut without losing the value prop]
- Scope risk: [Is the founder building the MPA or the "wouldn't it be cool if" version?]
- Manual-first opportunities: [What can be done manually while validating?]
- Technical risks: [Any blocking technical challenges?]

**MPA verdict:** [SHIP THIS WEEK / SHIP THIS MONTH / SHIP THIS QUARTER / SHIP NEXT YEAR]
[2-3 sentences on achievability and scope recommendations]

---

## DIFFERENTIATION ANALYSIS

**Founder's differentiation claim:** "[What the founder says makes this different]"
**Differentiation reality:** "[What actually makes this different after research]"

**Differentiation test:**
| Claimed Difference | Real? | Could Competitor Copy It? | In How Long? |
|--------------------|-------|--------------------------|-------------|
| [Claim 1] | Yes/No | Yes/No | [Days/Weeks/Months/Never] |
| [Claim 2] | | | |
| [Claim 3] | | | |

**Trade-off analysis:** [What trade-off does this product make that competitors can't or won't?]

**Differentiation verdict:** [STRUCTURAL / MEANINGFUL / COSMETIC / NONE]
[2-3 sentences with evidence]

---

## SWITCHING CALCULUS

**Current solution(s):** [What users use today]
**Switching costs:** [What users lose by switching — data, workflows, learning, team adoption]
**Switching benefits:** [What users gain by switching — immediate, concrete benefits]

**Switching equation:**
- Benefit of switching: [quantified if possible]
- Cost of switching: [quantified if possible]
- Net switching value: [Positive / Negative / Marginal]
- Natural switching moments: [When users are most likely to switch]

**Switching verdict:** [COMPELLING / FAVORABLE / MARGINAL / INSUFFICIENT]
[2-3 sentences]

---

## TIME-TO-VALUE MAP

**First session experience:**
- Minute 0-1: [What happens when user signs up]
- Minute 1-5: [First actions and impressions]
- Minute 5-15: [Where value should appear]
- End of first session: [What value has the user received?]

**"Aha moment":** [The specific interaction where the user thinks "this is worth it"]
**Steps to aha moment:** [How many steps between signup and the aha moment?]
**Competitor comparison:** [How does time-to-value compare to alternatives?]

**Time-to-value verdict:** [INSTANT / FAST / SLOW / DEFERRED]
[2-3 sentences]

---

## RETENTION ASSESSMENT

**Usage frequency prediction:** [How often will users return? Based on what evidence?]
**Stored value analysis:** [Does usage create value that makes the product stickier over time?]

| What Users Build/Store | Accumulation Speed | Switching Cost Created |
|-----------------------|--------------------|----------------------|
| [Content/data type] | [Fast/Moderate/Slow] | [High/Medium/Low] |

**Habit loop analysis:**
- Trigger: [What prompts the user to open the product?]
- Action: [What do they do?]
- Reward: [What value do they get?]
- Investment: [What do they leave behind that makes them come back?]

**Retention verdict:** [HABITUAL / REGULAR / EPISODIC / ONE-TIME]
[2-3 sentences]

---

## SUBSTITUTE THREAT MAP

| Substitute | Type | Cost | Value Delivered | Threat Level |
|-----------|------|------|-----------------|-------------|
| [AI chatbot (ChatGPT/Claude)] | Free AI | $0 | [X% of value] | [Critical/High/Medium/Low] |
| [Spreadsheet/manual process] | DIY | [time cost] | [X% of value] | |
| [Free tool / open source] | Free software | $0 | [X% of value] | |
| [Competitor tool] | Paid alternative | $X/mo | [X% of value] | |
| [Do nothing] | Status quo | $0 | [Current state] | |

**AI substitute test result:**
- Workflow tested: [What specific workflow was tested with a free AI tool?]
- AI result quality: [How well did the AI perform? X% of product value?]
- What the product provides that AI cannot: [Specific, honest assessment]
- **AI-interface trap**: [PASSES / FAILS — if the AI chat disappeared, what tangible artifact does the user walk away with? If "nothing" or "a conversation transcript," the product is an interface, not a solution. See _shared/philosophy.md.]

**Substitute verdict:** [NO VIABLE SUBSTITUTE / EXIST BUT WORSE / ADEQUATE / PREFERRED]
[2-3 sentences]

---

## SOLUTION DESIGN RECOMMENDATIONS

### Riskiest Assumption
- **Assumption:** [The single most dangerous assumption about this solution]
- **Cheapest test:** [Under $100, under 1 week — what experiment validates or kills this?]
- **Success signal:** [What result = proceed?]
- **Failure signal:** [What result = stop or pivot?]

### Scope Recommendations
[If MPA > SHIP THIS MONTH:]
- **One-week version:** [What's the smallest version that delivers core value?]
- **Manual-first approach:** [What can be done by hand while validating?]
- **Feature unlock sequence:** [What gets added only after core is validated?]

### Differentiation Strengthening
[If differentiation < MEANINGFUL:]
- **Available trade-offs:** [What could you sacrifice that competitors can't?]
- **Counter-position opportunity:** [Is there an approach incumbents can't adopt?]
- **Build-less advantage:** [Can you win by doing less, not more?]

---

## BOTTOM LINE

**Solution verdict**: [BUILD IT / TEST IT / RETHINK IT / STOP]

[2-3 sentences. Is this the right solution to this problem? What's the strongest dimension? What's the weakest? If TEST IT or RETHINK IT, what specifically needs to change?]

**The honest answer to "should I build this?":**
[One sentence. The real answer, not the comfortable one.]

**What would make this a BUILD IT:**
[One sentence — the specific change or evidence that would upgrade the conviction to BUILD IT. If already BUILD IT, state what could downgrade it.]

**Top 3 actions for the next 7 days:**
1. [Specific, concrete, actionable — related to the riskiest assumption or weakest dimension]
2. [Specific, concrete, actionable]
3. [Specific, concrete, actionable]

---
[If invoked as sub-skill: produce DIGEST summary per `_shared/philosophy.md` Digest Mode format]
```

## Important Rules

See `_shared/philosophy.md` Universal Skill Rules.

**Skill-specific rules:**
- **Solution, not problem** — this skill assumes the problem is real (problem-analysis validates that). Do NOT re-validate the problem. Focus on whether THIS SOLUTION is the right approach to an already-validated problem.
- **No "can we build it?" analysis** — when code is cheap, buildability is almost never the constraint. The question is "should we build it?" and "is this the right thing to build?" MPA dimension assesses scope, not technical feasibility.
- **Be specific about substitutes** — "there are substitutes" is vague. "ChatGPT with the prompt 'analyze my competitor pricing from these screenshots' delivers 70% of the value in 30 seconds for free" is specific and useful.
- **Test the AI substitute explicitly** — for every product, describe what would happen if a user tried to get the same outcome from a free AI chatbot. Be honest. If the AI can do 80%+ of the job, flag it as critical.
- **Differentiation requires trade-offs** — "we're better" is not differentiation. "We deliberately exclude feature X to keep the product simple, which means we win segment Y but lose segment Z" is differentiation. True differentiation means sacrificing something.
