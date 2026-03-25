# Shared Philosophy — All Skills

Read this file before executing any skill. These principles apply universally.

## The Bottleneck Shift (AI-Native Reality)

Code is cheap. AI tools collapsed development cost to near zero. The old SaaS playbook (raise → hire devs → build → pray) is dead. The new bottlenecks are:

1. **Clarity** — Do you know what's worth building? You can build faster than you can think. The bottleneck is knowing what customers will pay for.
2. **Distribution** — Product is not the moat. Reaching customers is. Channels, audience, relationships.
3. **Ambition** — You can take 50 swings/year. The risk is timidity, not wasted dev spend.
4. **Relationships** — Trust, reputation, and being known in your market. Can't be vibe-coded.

**What this changes:**
- Development cost is no longer meaningful capex — the real spend is marketing, distribution, and time-to-clarity
- "Can we build it?" is never the question — "Do we know what to build?" and "Can we reach buyers?" are
- Founder technical skills matter less than domain insight, market access, and clarity of vision
- Speed of iteration replaces quality of planning — prototype beats PRD
- Founders stuck in permission loops, polish-as-procrastination, or consensus-seeking are burning their scarcest resource: time-to-clarity
- Expect more competitors in every niche — any feature can be replicated in days, not years
- Engineering team size signals burn rate, not capability

**The AI-interface trap.** "Chat with your X" is table-stakes UI, not product differentiation. Every AI product will have a conversational interface — it's the default interaction layer, not a moat. Value lives in decisions, workflows, deliverables, and saved outcomes — not in the chat window itself.

- **Test**: "If the AI chat disappeared, what tangible artifact does the user walk away with?"
- If the answer is "nothing" or "a conversation transcript," the product is an interface, not a solution
- Complements the AI-substitute test in `/solution-analysis` — that test checks whether AI replaces the product; this one checks whether the product is merely a thin wrapper around AI

## Bootstrapper Philosophy

Farm cash cows, don't hunt unicorns. Build for long-term profitability, not for sale. Self-fund from customer revenue. No VC mindset, no exit-first thinking.

- Revenue, cash flow, and profitability are the metrics that matter
- The structured output from every skill exists to force **founder clarity** — not to pitch VCs or angels
- The audience is the founder, their co-founders, and reality

## User-Investment Lock-In (The Dual-Purpose Flywheel)

The most powerful moat a bootstrapper can build. When customers invest time building on your platform — creating content, importing data, building workflows, training their team, configuring integrations — every hour they invest raises their switching cost.

**Freemium as dual-purpose weapon:** The free tier isn't just marketing (though free beats paid for acquisition). It's simultaneously a retention mechanism. Users who build 20 quizzes, import 10K contacts, or configure 50 automations are not switching to save $20/month. Design for this deliberately.

**Lock-in checklist:**
- Does usage create stored value? (content, data, history, configurations)
- Does the user invest time that's lost if they switch? (setup, learning curve, team adoption)
- Does the product integrate into workflows painful to unplug? (API connections, automations, embedded widgets)
- If the answer to all three is "no", there is no moat.

## Beachhead Drift

Founders often target a different segment than the evidence supports. Any skill that identifies a beachhead or buyer persona must check for drift between the founder's stated target and where the research points.

- **Rating**: ALIGNED (evidence confirms founder's target) / DRIFTED (evidence points elsewhere)
- **Common drift patterns**:
  - Founder targets a broad horizontal audience when a specific vertical has 10x more pain
  - Founder targets enterprise when SMB has faster sales cycles and stronger WTP signals
  - Founder targets end-users when agencies/consultants are the real beachhead
- When DRIFTED: name the evidence-backed segment and explain why it differs from the founder's assumption

## Skill Archetypes

The toolkit has four skill archetypes. Each has different structural patterns:

### Dimension Skills
Deep analysis of one business dimension. Follow the full dimension skill pattern: philosophy, research-first protocol, sub-skill mode, multi-step flow, rated dimensions, validation gates, output template, digest mode. Examples: `/problem-analysis`, `/competitor-analysis`, `/financial-projections`.

### Mentor Skills
Strategic interpretation and scoring. Apply frameworks and judgment to evidence. Don't follow the dimension pattern — they have their own scoring models. Examples: `/venture-sensei`, `/bootstrap-oracle`.

### Generator Skills
Produce actionable artifacts (copy, personas, content plans, SWOT matrices). Research-backed but the output is a **deliverable**, not an evaluation. Key differences from dimension skills:
- No validation gates
- No digest mode (not consumed by orchestrators)
- Output is ready to use, not ready to analyze
- Must function standalone but benefit from prior dimension skill outputs
Examples: `/swot`, `/user-personas`, `/positioning`, `/content-strategy`.

### Meta Skills
Operate across multiple ideas or synthesize multiple skill outputs. Key differences:
- Cross-idea (e.g., `/idea-comparison`) or cross-skill (e.g., `/launch-plan`)
- No validation gates or digest mode
- Designed to consume prior skill outputs but must function standalone
- Output is a decision framework or execution plan
Examples: `/idea-comparison`, `/launch-plan`.

### Filter Skills
Lightweight, opinionated decision filters. Apply core principles to any founder decision — fast, one-page output, no research phase. Key differences from other archetypes:
- No web research — uses only what's already known
- One page max output — brevity is the constraint, not depth
- Opinionated — picks a side, doesn't hedge
- Can review output of other skills as input
- No validation gates, no digest mode
Examples: `/sanity-check`.

### Consumption Rule
Generator and meta skills consume dimension skill outputs when available in the session, but must produce complete, useful output even when run standalone with no prior context. When prior analysis exists, reference it — don't re-research the same ground.

## Universal Skill Rules

These rules apply to every skill in the toolkit. Individual skills may add domain-specific rules but must not contradict these.

1. **Research autonomously** — Use WebSearch and WebFetch aggressively before asking the user anything. Only ask when information is truly unknowable (budget, time constraints, proprietary insight). State all assumptions.
2. **Source every claim** — Founders make decisions based on these outputs — they need to know what's verified and what's guesswork.
   - Distinguish verified data from assumptions: "Competitor X charges $99/mo (verified via pricing page)" vs. "Estimated 500 target companies (assumption based on LinkedIn search)"
   - Note freshness of market data — if older than 12 months, flag it
   - State projection assumptions explicitly so the founder can challenge them
   - When confidence is low, say so: "LOW CONFIDENCE — based on limited data" beats a precise-sounding number built on thin evidence
3. **Use prior intelligence** — If another dimension skill has already been run in this session, reference its findings instead of re-researching the same ground.
4. **Consult references** — Check `references/INDEX.md` before producing analysis. Only open PDFs when specific detail is needed beyond what the index provides.
5. **Distill as original counsel** — Never reference book titles or quote material directly.
6. **End with BOTTOM LINE** — Every skill output must close with a `## BOTTOM LINE` section: a one-sentence summary, an "honest answer" line, and top 3 actions for the next 7 days. This is the first thing busy founders read.

## Sub-Skill Mode Protocol

Every dimension skill can be invoked standalone (via `/skill-name`) or as a sub-skill from `/analyze-idea`.

**Mode detection:** Sub-skill mode is active only when the `/analyze-idea` orchestrator explicitly invokes the skill and passes context. When a user runs `/skill-name` directly, always run in standalone mode — even if prior analysis from other skills exists in the session.

**When invoked as a sub-skill:**
1. Produce both the full report and a digest summary (see Digest Mode below)
2. Skip the "ask ONE clarifying question" step — context comes from the orchestrator

## Digest Mode

When a dimension skill is invoked as a sub-skill from `/analyze-idea`, it must produce a **digest summary** (200-300 words) at the end of its full report, after a `---` separator.

**The digest must include:**
- Dimension verdicts with ratings (e.g., "Pain severity: HAIR-ON-FIRE", "Timing verdict: WINDOW OPEN")
- Validation gate results (e.g., "Gates passed: 5/6 — failing: Gate 3 (no organic channel)")
- Top 2-3 key findings — the most important evidence that shapes the verdict
- The "honest answer" line — one sentence bottom-line verdict
- Any beachhead drift assessment (ALIGNED / DRIFTED)

**What the digest is for:**
- The full report is saved to disk (Phase 5 of analyze-idea)
- The digest is what gets passed to the Oracle scoring phase (Phase 3) — it must contain enough context for the Oracle to score accurately without reading the full report
- This prevents context window overflow when 10 full reports are combined

**Format:**
```
---

## DIGEST (for orchestrator consumption)

**[Skill name] verdict:** [VERDICT RATING]
**Validation gates passed:** [X/N — list failing gates]
**Key findings:**
1. [Most important finding with evidence]
2. [Second finding with evidence]
3. [Third finding if applicable]
**Beachhead drift:** [ALIGNED / DRIFTED — one sentence if drifted]
**The honest answer:** [One sentence — the bottom line]
```
