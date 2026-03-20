---
name: launch-plan
description: 30/60/90-day execution roadmap for bootstrapped founders. Synthesizes all prior analysis into a chronological plan with weekly action items, deliverables, decision gates, kill criteria, tools/budget, and phase exit criteria. Best after running dimension skills. Use when user runs `/launch-plan`, asks about "launch plan", "execution roadmap", "what do I do first", "90-day plan", "action plan", "next steps", "how to launch", or needs a concrete step-by-step execution plan.
---

# Launch Plan — 30/60/90-Day Execution Roadmap

Converts analysis into action. Produces a chronological execution plan that tells the founder exactly what to do each week for the next 90 days — from validation through launch and early growth. Most powerful after running dimension skills; works standalone too.

## Philosophy

**Plans without deadlines are daydreams. Actions without sequence are chaos.** Founders don't fail because they lack analysis — they fail because they can't convert analysis into a sequenced, time-bound execution plan. This skill is the bridge between "I know what to build" and "I built it and people are paying."

Read `.claude/skills/_shared/philosophy.md` for the full bottleneck shift and bootstrapper framework. For launch planning specifically:

**The bootstrapper launch reality:**
- You don't have a team. Every action item must be doable by 1-2 people.
- Cash is finite. Every spend must be justified against timeline to revenue.
- Speed is the advantage. The plan should be aggressive — 90 days, not 12 months.
- Validation before building. The plan front-loads customer evidence, not product development.
- Kill criteria are essential. A good plan includes when to STOP, not just what to START.

**Phase philosophy:**
- **Days 1-30 (Validate)**: Prove the problem, customer, and willingness to pay are real. NO product building.
- **Days 31-60 (Build & Test)**: Build the minimum product that tests the core value proposition. Ship to early users.
- **Days 61-90 (Launch & Grow)**: Public launch, first paying customers, initial distribution. Revenue or a clear kill decision.

**What makes this different from generic roadmaps:**
- Every action has a concrete deliverable (not "research the market" but "interview 10 target buyers and document their top 3 pain points")
- Decision gates force go/no-go choices at key moments
- Kill criteria prevent founders from pouring 6 months into a dead idea
- Budget is explicit — founders know what they'll spend before they start
- The plan adapts to prior analysis — if `/problem-analysis` found weak evidence, Week 1 focuses on validation

## Reference Books

Check `references/INDEX.md` for relevant frameworks. Key books for launch planning:

- **lean-startup** (Ries) — Build-measure-learn loop structures the validation phase; MVP definition for Phase 2 scoping; innovation accounting for decision gates; pivot-or-persevere framework for kill criteria
- **startup-owners-manual** (Blank & Dorf) — Customer development methodology for Phase 1 (discovery before building); earlyvangelists as the first customers to target; channel strategy for Phase 3 launch
- **shape-up** (Singer) — Fixed-time, variable-scope approach for the build phase; 6-week cycle concept adapted to 30-day phases; appetite setting before building; circuit breaker principle for kill decisions
- **getting-real** (37signals) — "Launch fast" philosophy; Hollywood launch technique for Phase 3; build less and ship sooner; epicenter design for deciding what to build first in the MVP sprint
- **traction-weinberg** (Weinberg & Mares) — Bullseye framework for channel testing in Phase 3; the 50% rule (spend half effort on distribution); 19 channels as the menu for launch distribution tactics
- **mom-test** (Fitzpatrick) — Customer interview methodology for Phase 1 validation activities; how to structure the customer conversations that decision gates depend on
- **profit-first** (Michalowicz) — Budget allocation framework for the 90-day budget section; Profit First formula for making the financial plan sustainable from day one

## Research-First Protocol

This skill is primarily a synthesis skill — it consumes prior analysis more than it generates new research. However, when run standalone:

**Quick research tasks:**
- "[product category] launch strategy" / "how to launch [product type]"
- "[product category] tools and costs" (for budget estimation)
- "[target market] communities" / "[target market] events" (for launch channels)
- Check competitor launch stories on Product Hunt, IndieHackers, Hacker News

**Consume prior intelligence (CRITICAL):** This skill is designed to run AFTER dimension skills. Pull from:
- **problem-analysis**: Validation status, customer discovery recommendations, weak gates to address
- **gtm-strategy**: Channel strategy, first 100 customers plan, distribution economics
- **competitor-analysis**: Competitive wedge, customers to steal, positioning strategy
- **solution-analysis**: MPA (Minimum Product Achievability), time-to-value, differentiation
- **financial-projections**: Break-even timeline, startup costs, founder sustainability
- **business-model**: Revenue model, pricing strategy, monetization approach
- **market-size**: Beachhead market, demand signals
- **founder-fit**: Time budget, financial runway, execution tempo, critical gaps
- **timing-analysis**: Market window, entry timing urgency
- **moat-analysis**: What to invest in for long-term defensibility
- **user-personas**: Primary buyer targeting criteria, buying triggers (if run)
- **positioning**: Homepage copy, messaging, language bank (if run)
- **content-strategy**: Content calendar, keyword targets, distribution checklist (if run)
- **risk-assessment**: Top risks and mitigations (if run)
- **bootstrap-oracle / analyze-idea**: Overall verdict, scoring, recommended actions

**Adaptation rules:**
- If problem-analysis gates < 4/6 → Phase 1 extends to 45 days, heavy on customer discovery
- If financial-projections shows founder runway < 6 months → Compress to 60-day plan, cut non-essential actions
- If timing-analysis rated market window as CLOSING (< 3 months) or CLOSED → Compress Phase 1 to 2 weeks, accelerate everything
- If founder-fit shows time budget < 15 hrs/week → Reduce weekly actions to 3-4, extend timeline to 120 days

## End-to-End Flow

### STEP 0 — CONTEXT GATHERING

Extract from the user's input:
- The business idea (what it does, who it's for)
- Current stage (idea, MVP, live product)
- Available prior analysis (list all skill outputs available in session)
- Founder constraints (time per week, budget, skills, team size)
- Launch urgency (market window, personal timeline)

If critical context is missing (no idea description, no founder constraints), ask ONE clarifying question bundling all gaps. Otherwise, proceed.

### STEP 1 — SYNTHESIS & PLAN ARCHITECTURE

Review all available prior analysis and construct the plan architecture:

1. **Identify validation gaps** — what's unproven that the plan must address?
2. **Identify assets** — what's already validated that the plan can build on?
3. **Determine plan intensity** — based on founder constraints and urgency
4. **Set phase durations** — adjust from default 30/30/30 based on context
5. **Define success metrics** — what does "done" look like for each phase?

### STEP 2 — PLAN GENERATION

Build the week-by-week plan with deliverables, decision gates, and kill criteria.

### STEP 3 — OUTPUT

Produce the full report using the template below.

## Output Template

```
# LAUNCH PLAN: [Product/Idea Name]

Plan date: [date]
Stage: [Idea / MVP / Live Product]
Plan duration: [60 / 90 / 120 days — adjusted for context]
Weekly founder hours: [Estimated — e.g., "20 hrs/week" or "full-time"]
Prior analysis consumed: [List skills run in session, or "Standalone — no prior analysis"]

---

## PLAN OVERVIEW

**What this plan achieves:**
[2-3 sentences — what the founder will have at the end of 90 days. Be concrete: "10 paying customers, validated pricing, functioning product, and a repeatable acquisition channel" not "a launched business"]

**Key assumptions this plan rests on:**
1. [Critical assumption — what must be true for this plan to work]
2. [Critical assumption]
3. [Critical assumption]

**Plan intensity:** [Aggressive / Standard / Conservative — and why]

---

## PHASE 1: VALIDATE (Days 1-30)

**Phase goal:** Prove that real people have this problem, will pay to solve it, and can be reached through a specific channel.

**Phase exit criteria** (must hit before moving to Phase 2):
- [ ] [Specific validation milestone — e.g., "10 target buyers confirm the pain in their own words"]
- [ ] [Specific milestone — e.g., "3 potential customers state willingness to pay $X/month"]
- [ ] [Specific milestone — e.g., "Primary distribution channel identified with access confirmed"]
- [ ] [Specific milestone — e.g., "Landing page live with 100+ visitors and X% email signup rate"]

### Week 1: [Week theme — e.g., "Customer Discovery Sprint"]

| Day(s) | Action | Deliverable | Time Est. |
|--------|--------|-------------|-----------|
| 1-2 | [Specific action] | [Tangible output] | [hours] |
| 3-4 | [Specific action] | [Tangible output] | [hours] |
| 5-7 | [Specific action] | [Tangible output] | [hours] |

**Week 1 checkpoint:** [What you should know by end of week — a specific question answered]

### Week 2: [Week theme]

| Day(s) | Action | Deliverable | Time Est. |
|--------|--------|-------------|-----------|
| 8-9 | [Specific action] | [Tangible output] | [hours] |
| 10-11 | [Specific action] | [Tangible output] | [hours] |
| 12-14 | [Specific action] | [Tangible output] | [hours] |

**Week 2 checkpoint:** [What you should know by end of week]

### Week 3: [Week theme]

| Day(s) | Action | Deliverable | Time Est. |
|--------|--------|-------------|-----------|
| 15-17 | [Specific action] | [Tangible output] | [hours] |
| 18-19 | [Specific action] | [Tangible output] | [hours] |
| 20-21 | [Specific action] | [Tangible output] | [hours] |

**Week 3 checkpoint:** [What you should know by end of week]

### Week 4: [Week theme]

| Day(s) | Action | Deliverable | Time Est. |
|--------|--------|-------------|-----------|
| 22-24 | [Specific action] | [Tangible output] | [hours] |
| 25-26 | [Specific action] | [Tangible output] | [hours] |
| 27-30 | [Specific action] | [Tangible output] | [hours] |

**Week 4 checkpoint:** [What you should know by end of week]

### DECISION GATE 1 (Day 30)

**Question:** Is the problem validated with enough evidence to build?

| Signal | Threshold | Actual | Pass/Fail |
|--------|-----------|--------|-----------|
| Customer conversations completed | ≥10 | [_] | |
| Confirmed pain (unprompted) | ≥7/10 | [_] | |
| Stated willingness to pay | ≥5/10 | [_] | |
| Landing page signup rate | ≥5% | [_] | |
| Distribution channel access | Confirmed | [_] | |

**If PASS:** Proceed to Phase 2.
**If MARGINAL (3-4/5):** Extend Phase 1 by 2 weeks, focus on failing signals.
**If FAIL (<3/5):** KILL or PIVOT. [Specific guidance on what to do]

---

## PHASE 2: BUILD & TEST (Days 31-60)

**Phase goal:** Build the minimum product, get it into real users' hands, and test the core value proposition with actual usage.

**Phase exit criteria:**
- [ ] [Specific milestone — e.g., "MVP live and functional"]
- [ ] [Specific milestone — e.g., "10 beta users actively using the product"]
- [ ] [Specific milestone — e.g., "First payment processed (even if discounted)"]
- [ ] [Specific milestone — e.g., "Core retention metric: X% of users return in Week 2"]

### Week 5: [Week theme — e.g., "MVP Sprint Start"]

| Day(s) | Action | Deliverable | Time Est. |
|--------|--------|-------------|-----------|
| 31-33 | [Specific action] | [Tangible output] | [hours] |
| 34-35 | [Specific action] | [Tangible output] | [hours] |
| 36-37 | [Specific action] | [Tangible output] | [hours] |

**Week 5 checkpoint:** [What you should know by end of week]

### Week 6: [Week theme]
[Same structure]

### Week 7: [Week theme]
[Same structure]

### Week 8: [Week theme]
[Same structure]

### DECISION GATE 2 (Day 60)

**Question:** Does the product deliver value that users will pay for?

| Signal | Threshold | Actual | Pass/Fail |
|--------|-----------|--------|-----------|
| Beta users active | ≥10 | [_] | |
| Users reporting value | ≥7/10 | [_] | |
| Payment conversion (even early) | ≥1 | [_] | |
| Retention (Week 2 return) | ≥40% | [_] | |
| NPS or satisfaction signal | Positive | [_] | |

**If PASS:** Proceed to Phase 3.
**If MARGINAL:** Fix the weakest signal. Extend Phase 2 by 2 weeks.
**If FAIL:** Evaluate pivot options. [Specific guidance]

---

## PHASE 3: LAUNCH & GROW (Days 61-90)

**Phase goal:** Public launch, first paying customers from organic channels, repeatable acquisition motion established.

**Phase exit criteria:**
- [ ] [Specific milestone — e.g., "$1K MRR or 10 paying customers"]
- [ ] [Specific milestone — e.g., "Primary acquisition channel producing consistent leads"]
- [ ] [Specific milestone — e.g., "Customer retention above X% at 30 days"]
- [ ] [Specific milestone — e.g., "Unit economics validated: LTV > 3x CAC"]

### Week 9: [Week theme — e.g., "Launch Preparation"]
[Same structure]

### Week 10: [Week theme — e.g., "Public Launch"]
[Same structure]

### Week 11: [Week theme — e.g., "Post-Launch Optimization"]
[Same structure]

### Week 12: [Week theme — e.g., "Growth Foundation"]
[Same structure]

### DECISION GATE 3 (Day 90)

**Question:** Is this a business worth continuing?

| Signal | Threshold | Actual | Pass/Fail |
|--------|-----------|--------|-----------|
| Paying customers | ≥10 | [_] | |
| MRR | ≥$500 | [_] | |
| Organic acquisition | Repeatable | [_] | |
| Customer satisfaction | Positive | [_] | |
| Founder energy | Sustainable | [_] | |

**If PASS:** Continue — build the 6-month growth plan.
**If MARGINAL:** Identify the bottleneck. Give yourself 30 more days on the weakest signal.
**If FAIL:** Honest evaluation time. [Specific kill/pivot/persist guidance]

---

## KILL CRITERIA

**Kill this idea at any point if:**
1. [Specific kill signal — e.g., "30 customer conversations and <3 confirm the pain unprompted"]
2. [Specific kill signal — e.g., "Nobody converts to paid after 60 days of free usage"]
3. [Specific kill signal — e.g., "Primary distribution channel proves inaccessible or too expensive"]
4. [Specific kill signal — e.g., "Founder runway drops below 3 months with no revenue"]
5. [Specific kill signal — e.g., "A well-funded competitor launches identical product with better distribution"]

**Killing is not failing.** Killing a bad idea in 30 days to pursue a better one is the highest-leverage action a bootstrapper can take. The plan is designed to produce a kill signal FAST — before you've invested months of building.

---

## TOOLS & RESOURCES

| Category | Tool/Resource | Cost | When Needed |
|----------|-------------|------|-------------|
| **Landing page** | [Specific tool] | [$/mo or free] | Week 1 |
| **Email capture** | [Specific tool] | [$/mo or free] | Week 1-2 |
| **MVP building** | [Specific tool/approach] | [$/mo or free] | Week 5-8 |
| **Analytics** | [Specific tool] | [$/mo or free] | Week 1 |
| **Payment processing** | [Specific tool] | [% per transaction] | Week 7-8 |
| **Customer communication** | [Specific tool] | [$/mo or free] | Week 1 |
| **SEO/Content** | [Specific tool] | [$/mo or free] | Week 9+ |
| **Social/Community** | [Specific platforms] | Free | Week 1 |
| **Domain/Hosting** | [Specific service] | [$/mo] | Week 1 |

---

## 90-DAY BUDGET ESTIMATE

| Category | Month 1 | Month 2 | Month 3 | Total |
|----------|---------|---------|---------|-------|
| Tools & subscriptions | $[_] | $[_] | $[_] | $[_] |
| Paid marketing (if any) | $[_] | $[_] | $[_] | $[_] |
| Domain, hosting, infrastructure | $[_] | $[_] | $[_] | $[_] |
| Other (legal, design, etc.) | $[_] | $[_] | $[_] | $[_] |
| **TOTAL** | **$[_]** | **$[_]** | **$[_]** | **$[_]** |

**Budget philosophy:** Spend as little as possible in Month 1 (validation should be nearly free). Increase in Month 2 only if validation passes. Month 3 is the first real marketing spend.

---

## BOTTOM LINE

**Your 90-day mission:** [One sentence — the concrete outcome this plan produces]

**The honest answer about execution:** [One sentence — is this plan achievable given the founder's constraints? What's the biggest execution risk?]

**If you only do 3 things from this entire plan:**
1. [The single most important validation action]
2. [The single most important building action]
3. [The single most important distribution action]
```

## Important Rules

See `_shared/philosophy.md` Universal Skill Rules.

**Skill-specific rules:**
- **Every action must have a deliverable** — "Research the market" is not an action. "Interview 10 target buyers and document their top 3 pain points in a spreadsheet" is. If it doesn't produce a tangible output, it's not a task.
- **Time estimates are mandatory** — founders need to know if this is a 5-hour week or a 40-hour week. Be realistic about time requirements.
- **Decision gates are non-negotiable** — every phase ends with a go/no-go decision. Without gates, founders drift into building mode without validation.
- **Kill criteria save lives** — or at least months. The plan must include specific, measurable signals that mean "stop." This is the hardest part for founders and the most valuable.
- **Adapt to prior analysis** — if dimension skills revealed specific risks, the plan must address them. If validation is already strong (high gate pass rates), Phase 1 can be compressed. If evidence is thin, Phase 1 extends.
- **Budget must be explicit** — founders need to know the cash requirement before they start. Hidden costs kill bootstrapped businesses.
- **This is a Meta skill** — it synthesizes all prior skill outputs into a sequenced execution plan. No validation gates, no digest mode. The output is a complete roadmap.
- **No building in Phase 1** — validation always comes first. If the plan has "build MVP" in Week 1, something is wrong. The exception is when prior analysis already validated the problem and customer (gates passed).
- **Standalone must work** — when run without prior analysis, the plan must include its own validation activities. It will be less precise but still functional.
