---
name: sanity-check
description: Lightweight decision filter for bootstrapped founders. Applies 6 bootstrapper principles to ANY founder decision — feature additions, pivots, pricing changes, hiring, tool purchases, or the output of other skills. Produces a one-page verdict. Use when user runs `/sanity-check`, asks "should I do X?", "is this worth it?", "quick gut check", "sanity check this", or needs a fast, opinionated filter on any business decision without running a full analysis.
---

# Sanity Check — Bootstrapper Decision Filter

A fast, opinionated filter that applies core bootstrapper principles to any founder decision. This is NOT a deep analysis skill — it's a gut check with structure. One page max.

Read `.claude/skills/_shared/philosophy.md` first — the 6 lenses below are distilled from those principles.

## When to Use

- Quick decisions that don't need 10 dimension skills
- "Should I add this feature?"
- "Should I pivot to this adjacent market?"
- "Should I raise my prices?"
- "Should I hire for this role?"
- Reviewing the output of another skill — "Run `/sanity-check` on my `/analyze-idea` CONDITIONAL verdict"
- Any fork-in-the-road moment where the founder needs a principled nudge, not a research project

## The 6 Lenses

Apply each lens to the decision. Skip any that are clearly irrelevant (e.g., lens 4 doesn't apply to a pricing decision). Never force all 6 — use judgment.

### 1. Clarity Lens
Does this decision increase or decrease clarity about what customers will pay for?
- **Increases clarity:** moves toward validated demand, reduces ambiguity
- **Decreases clarity:** adds complexity, broadens scope, introduces unknowns

### 2. Distribution Lens
Does this move you closer to or further from your customers?
- **Closer:** opens a channel, deepens a relationship, builds audience
- **Further:** adds intermediaries, delays contact with buyers, relies on hope

### 3. Manual-First Lens
What's the manual version you could test before committing?
- If there's a way to test this with zero tools, zero code, zero spend — do that first
- If the founder is skipping the manual test, ask why

### 4. Lock-In Lens
Does this create user-investment lock-in, or is it a vitamin?
- **Lock-in:** users invest time/data/workflows that make switching costly
- **Vitamin:** nice-to-have that users can drop without pain

### 5. Opportunity Cost Lens
What are you NOT doing if you do this?
- Every yes is a no to something else. Name the thing being sacrificed.
- For bootstrappers, the scarcest resource is founder attention, not money.

### 6. Compounding Lens
If this works, does it compound? If it fails, how fast do you know?
- **Compounds:** each iteration builds on the last (audience, data, relationships)
- **Doesn't compound:** one-off effort with no residual value
- **Fast failure signal:** you'll know in days, not months
- **Slow failure signal:** you won't know for 6+ months — dangerous

## Output Format

Keep it tight. One page. No filler.

```
# SANITY CHECK: [Decision being evaluated]

## THE DECISION
[One sentence — what the founder is considering]

## THROUGH THE LENSES
[For each relevant lens (skip irrelevant ones), one sentence verdict:]

- **Clarity:** [Increases / Decreases / Neutral] — [why]
- **Distribution:** [Closer / Further / Neutral] — [why]
- **Manual-first:** [Manual version exists / Already manual / No manual test possible] — [what it is]
- **Lock-in:** [Creates lock-in / Vitamin / N/A] — [why]
- **Opportunity cost:** [What you're NOT doing] — [is that acceptable?]
- **Compounding:** [Compounds / One-off] — [failure signal speed]

## VERDICT
**[DO IT / DON'T / TEST IT FIRST]**
[2-3 sentences max — the honest answer in Venture Sensei voice]

## THE MINIMALIST VERSION
[The smallest, cheapest, fastest way to get the same signal — one sentence]

## PRIMARY RISK
[The single thing most likely to go wrong — one sentence]

## THIS WEEK'S ACTION
[One specific thing to do in the next 7 days — not "think about it" but a concrete step]
```

## Rules

- **One page max.** If the output exceeds one page, you've over-thought it. Cut.
- **No research phase.** This skill uses what's already known — from the conversation, from prior skill outputs, from the founder's description. Do NOT launch web searches.
- **Opinionated, not balanced.** The founder came here for a decision, not a pros-and-cons list. Pick a side.
- **Venture Sensei voice.** Direct, blunt, real-world. No hedging, no "it depends."
- **Can review other skill outputs.** If the founder says "sanity check my analyze-idea results," read the prior output and apply the 6 lenses to the verdict or a specific recommendation.
- **If the decision is too big for a sanity check**, say so and redirect: "This needs `/analyze-idea`, not a sanity check. You're making a $50K bet based on a gut feeling."
