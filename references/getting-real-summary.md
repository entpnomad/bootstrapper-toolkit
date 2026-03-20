# Getting Real — Claude Notes
_Source: “Getting Real: The Smarter, Faster, Easier Way to Build a Successful Web Application” (Basecamp / 37signals)_

This is a **Claude-ready** distillation of the book into:
- **Principles** (how to think)
- **Rules** (what to do / not do)
- **Skills & checklists** (how to execute)

It’s written so you can hand it to an LLM as project “operating constraints” while you design, build, and launch.

---

## How to use this file

When you ask Claude to help with product + build work, paste the relevant sections:

- **Early stage (idea → MVP):** “Core philosophy” + “Starting Line” + “Feature selection” + “Process”.
- **Design + UX:** “Interface design” + “Words”.
- **Shipping + growth:** “Pricing & signup” + “Promotion” + “Support” + “Post-launch”.

Ask for outputs that match the book’s cadence:
- **short cycles** (days/weeks),
- **real screens over documents**,
- **less software**,
- **launch early + iterate**.

---

## Core philosophy

**Getting Real** is a way to build software that favors:
- **Reality over make-believe**: build the real thing (screens + working flows), not charts/specs/wireframes.
- **Smallness**: fewer features, less mass, less overhead, fewer people.
- **Speed through constraint**: fix time + budget, flex scope.
- **Iteration**: ship, learn, adjust; lower the cost of change.
- **Inside-out design**: start with the interface customers use, then work backwards.

It rejects the classic “big planning + big launch + big team” playbook.

---

## The Getting Real mindset (high-signal principles)

### 1) Underdo the competition
Don’t play feature Cold War (“they have 4 features so we need 5”). Beat them by doing **less**, better.

### 2) Solve the obvious problem in front of you
Don’t pre-solve the next 20 hypothetical problems. Ship a clean solution to the one that’s real right now.

### 3) Make decisions that reduce future cost
Prefer choices that:
- simplify UI,
- reduce support load,
- reduce edge cases,
- reduce ongoing maintenance.

### 4) Design + build for the right customers
Not everyone is your customer. Avoid becoming generic.

### 5) Running software is truth
Sketches and docs are approximations. Working software creates alignment and reveals what actually matters.

---

# RULES (operating constraints)

Use these as hard guardrails when Claude suggests “more”:

## Product rules
- **Build half a product that kicks ass**, not a half-assed full product.
- Default answer to feature requests: **No / not now**.
- Treat every feature as an adoption: **build → test → document → support → maintain**.
- Avoid “preference explosion”: fewer toggles/options.
- If it **doesn’t change user behavior**, it probably **doesn’t matter**.
- Ask “what should we remove?” not just “what should we add?”.

## Process rules
- Fix **time + budget**, flex **scope**.
- Ship something real early; iterate.
- Keep cycles short; chase “done”.
- Test in the wild, not in a lab.

## Org rules
- Avoid silos; keep design/dev/copy/support close.
- **Protect maker time**: blocks of uninterrupted work.
- Meetings are last resort; if unavoidable: small, agenda, 30 minutes.

## Writing rules
- Words are UI. Treat copy as product design.
- Prefer short, real words over jargon.
- Kill dead documents; replace with living notes, examples, real screens.

---

# PATTERNS BY PHASE (chapter-by-chapter distillation)

## The Starting Line

### Build Less
- Compete by **not** matching every checkbox.
- Solve the “simple problems” exceptionally well.
- Leave “hairy, nasty” problems for others until you’ve earned them.

**Skill:** Write a one-line scope cut: “We are *not* building X.”

### What’s Your Problem?
- Start with the pain, not the idea.
- If you can’t describe the problem clearly, you can’t ship the right thing.

**Skill:** Problem statement template:
- “People who ___ struggle with ___ because ___. Today they use ___ which fails when ___.”

### Fund Yourself
- Keep burn low, avoid dependency on big funding.
- Constraints push clarity.

### Fix Time and Budget, Flex Scope
- Time and money are the constants.
- Scope is the variable.

**Skill:** “Scope triage”:
- Must-have (core promise)
- Nice-to-have (after launch)
- Won’t-have (avoid distraction)

### Have an Enemy
- Differentiate by opposing something users dislike (bloat, complexity, IT overhead, etc.).
- Your “enemy” shapes product decisions and marketing language.

**Skill:** Enemy statement:
- “Our enemy is ___ (e.g., ‘bloated project management’). We win by ___.”

### It Shouldn’t Be a Chore
- If using your app feels like work, you’ve already lost.
- Remove friction, reduce required steps, simplify.

---

## Stay Lean

### Less Mass
- Every new feature adds weight: code, UI, tests, docs, support.
- Lightweight products move faster and adapt faster.

### Lower Your Cost of Change
- Build systems and habits that make change cheap.
- Cheap change enables iteration; expensive change traps you.

### The Three Musketeers
- Strong products combine: **design + code + words**.
- Don’t treat copy as an afterthought.

### Embrace Constraints
- Constraints are creative fuel: small team, short timeline, limited budget.

### Be Yourself
- Don’t erase your voice to please everyone.
- Specific beats generic.

---

## Priorities

### What’s the Big Idea?
- Your product needs a sharp, memorable promise.
- A big idea is not a feature list.

**Skill:** Big idea one-liner:
- “We help ___ do ___ without ___.”

### Ignore Details Early On
- Early: focus on flow and core value.
- Details become clear once something runs.

### It’s a Problem When It’s a Problem
- Don’t optimize prematurely.
- Solve issues when they’re real and recurring.

### Hire the Right Customers
- The “wrong customers” demand edge cases and endless preferences.
- The “right customers” value your opinionated simplicity.

### Scale Later
- Don’t build infrastructure, org charts, or “enterprise readiness” too early.
- Earn complexity.

### Make Opinionated Software
- Opinionated products reduce choice overload.
- They set defaults and teach a way of working.

---

## Feature Selection

### Half, Not Half-Assed
- Cut your feature list in half. Then cut again.
- Start with the heart of the product.

### It Just Doesn’t Matter
- Great product judgment = knowing what not to care about.
- If it doesn’t matter, don’t spend time on it.

### Start With No
- Default to “no / not now”.
- The features worth building will keep resurfacing.

### Hidden Costs
- Every feature has ongoing cost: complexity + support + docs + maintenance.

### Can You Handle It?
- Don’t promise what you can’t sustain.
- Design offers that fit your operational reality.

### Human Solutions
- Build general tools; let users create their own conventions.
- Don’t hard-code every edge case into software.

### Forget Feature Requests
- Read requests; don’t maintain a massive backlog.
- If it matters, users will keep reminding you.

### Hold the Mayo
- Ask customers what they *don’t* want.
- Removing is often the best improvement.

---

## Process

### Race to Running Software
- Running software creates alignment and reveals truth.
- Skip perfect planning; get something working.

### Rinse and Repeat
- Expect to redo things. Iteration is normal.
- Launch → observe → adjust → repeat.

### From Idea to Implementation
- Don’t get stuck in “idea phase”.
- Convert ideas into real screens and flows quickly.

### Avoid Preferences
- Preferences create a combinatorial support/testing nightmare.
- Prefer smart defaults + small set of modes.

### “Done!”
- Shipping requires finishing.
- “Almost done” is a trap.

### Test in the Wild
- Real users + real context beat artificial labs.

### Shrink Your Time
- Smaller timeboxes increase focus and momentum.

---

## The Organization

### Unity (no silos)
- Keep design/dev/copy/support/marketing connected.
- Shared context reduces rework.

### Alone Time
- Protect uninterrupted blocks.
- Interruption kills deep work.

**Practice:** half-day “no talk” rule, or daily maker blocks.

### Meetings Are Toxic
- Meetings destroy flow and often produce little.
- If you must meet: agenda, minimal attendees, 30-minute hard stop.

### Seek and Celebrate Small Victories
- Release something small frequently.
- Use “4-hour wins” to maintain morale and momentum.

---

## Staffing

### Hire Less and Hire Later
- Small teams move faster.
- Hiring adds communication overhead.

### Kick the Tires
- Test people with real work before long commitments.

### Actions, Not Words
- Judge by output, not credentials.

### Get Well-Rounded Individuals
- Look for T-shaped people who can cross boundaries.

### You Can’t Fake Enthusiasm
- Motivation matters; enthusiasm is hard to manufacture.

### Wordsmiths
- Strong writing is a competitive advantage.

---

## Interface Design

### Interface First
- Start with the screens people will use.
- Build from the customer experience backwards.

### Epicenter Design
- Identify the “heart” screen/flow.
- Design outward from that epicenter.

### Three State Solution
For every UI element, design 3 states:
1) Normal
2) Empty
3) Error

### The Blank Slate
- Empty states are the first-run experience.
- Teach, guide, and reduce anxiety when there’s “nothing here yet.”

### Get Defensive
- Assume users will:
  - misread,
  - make mistakes,
  - abandon mid-flow.
- Design to prevent and recover gracefully.

### Context Over Consistency
- Consistency is useful, but not sacred.
- Prioritize what makes sense *here* over rigid global rules.

### Copywriting Is Interface Design
- Microcopy is part of UX.
- Words can prevent support tickets.

### One Interface
- Avoid “beginner vs advanced” split interfaces.
- Keep one coherent UI; let power come from mastery, not hidden complexity.

---

## Code

### Less Software
- Fewer moving parts.
- Prefer simple architectures.

### Optimize for Happiness
- Developer happiness matters: readable, maintainable code wins long-term.

### Code Speaks
- Let working code and UI make the case, not documents.

### Manage Debt
- Debt accumulates; track it intentionally.
- Pay it down before it blocks iteration.

### Open Doors
- Stay flexible: avoid irreversible lock-in too early.

---

## Words

### There’s Nothing Functional About a Functional Spec
- Specs are “illusion of agreement.”
- Real screens are truth.

### Don’t Do Dead Documents
- Docs rot. Prefer living notes tied to real features.

### Tell Me a Quick Story
- Use narrative to explain flows.

### Use Real Words
- Avoid jargon. Write like a human.

### Personify Your Product
- Give the product a consistent voice.

---

## Pricing and Signup

### Free Samples
- Let people try the real thing.

### Easy On, Easy Off
- Reduce commitment anxiety: easy signup, easy cancel, transparent terms.

### Silly Rabbit, Tricks Are for Kids
- Avoid manipulative pricing tricks.

### A Softer Bullet
- Instead of “hard sell”, reduce friction and let product value convince.

---

## Promotion

### Hollywood Launch
- Treat launch like an event.
- Build anticipation and a clear narrative.

### A Powerful Promo Site
- Your marketing site should explain the big idea quickly.
- Show, don’t tell: screenshots, benefits, examples.

### Ride the Blog Wave
- Use consistent publishing to sustain attention.

### Solicit Early
- Get feedback and early customers before “perfect.”

### Promote Through Education
- Teach people how to think about the problem.

### Feature Food
- Regularly highlight small product improvements.

### Track Your Logs
- Measure what people do.

### Inline Upsell
- Upgrade prompts inside the product, at the right moment.

### Name Hook
- Naming matters. A good name is easier to share.

---

## Support

### Feel The Pain
- Don’t outsource learning.
- Support is product research.

### Zero Training
- Aim for a product that requires minimal training.

### Answer Quick
- Speed matters. Responsiveness builds trust.

### Tough Love
- Don’t let support become “custom development by email.”

### In Fine Forum
- Use public threads when possible: answers scale.

### Publicize Your Screwups
- Own mistakes publicly; it increases credibility.

---

## Post-Launch

### One Month Tuneup
- Launch is the start.
- Spend the first month fixing friction and sharpening the core.

### Keep the Posts Coming
- Maintain momentum with updates + writing.

### Better, Not Beta
- Don’t hide behind “beta.”
- Be real: ship quality, improve continuously.

### All Bugs Are Not Created Equal
- Prioritize bugs that hurt core flows.

### Ride Out the Storm
- Launch brings noise; stay calm, keep shipping.

### Keep Up With the Joneses
- Watch competitors, but don’t copy reflexively.

### Beware the Bloat Monster
- Growth invites complexity.
- Keep cutting.

### Go With The Flow
- Follow what users actually do, not what you hoped they’d do.

---

# SKILLS & CHECKLISTS (Claude-friendly execution tools)

## A) “Half product” MVP cutter
1. List all features you want.
2. Mark the **epicenter**: the one flow that must work.
3. Cut everything not required for that epicenter.
4. Cut again: remove anything that’s “nice”.
5. Ship that.

Output format for Claude:
- Epicenter flow (1 paragraph)
- Must-have screens (list)
- Explicit non-goals (list)
- First iteration metrics (list)

## B) Feature pressure test (Start with No)
For any proposed feature, answer:
- What problem does it solve?
- What happens if we don’t build it?
- What’s the hidden cost (UI, code paths, support, docs)?
- Is there a human workaround?
- Does it create preferences/options?
- Does it move the big idea forward?

Decision:
- **No**, **Not now**, or **Yes (with constraints)**.

## C) Three-state UI worksheet
For each component/screen:
- Normal: what users expect.
- Empty: what users see on day 1.
- Error: what breaks and how we recover.

## D) Blank slate checklist
- Explain what this area is.
- Show first step.
- Provide an example.
- Offer a safe action (no fear).

## E) Copy-as-design checklist
- Replace jargon with real words.
- Reduce support tickets with microcopy.
- Make buttons action-oriented.
- Remove unnecessary help text; keep only what prevents mistakes.

## F) Meeting minimization rules
- Prefer async written updates.
- If meeting is unavoidable: 30 minutes, agenda, minimal attendees.
- End with a decision + next action.

## G) Launch playbook (Hollywood launch)
- Build promo site around: problem → big idea → proof (screens) → pricing → FAQ.
- Prepare educational content that teaches the problem space.
- Ship to early users; collect testimonials.
- Launch event: email + blog + social + partners.
- Post-launch: weekly small victories and public updates.

## H) Support loop
- Treat support as a product input stream.
- Tag issues by: UX confusion, missing feature, bug, edge case.
- Fix the top confusion points in UI/copy first.

---

# PROMPT PACK (copy/paste into Claude)

## 1) Turn an idea into a Getting Real plan
“Use Getting Real principles. Given this product idea: <idea> and these constraints: <time/budget/team>, produce:
- Big idea (1 sentence)
- Enemy statement
- Epicenter flow
- MVP ‘half product’ scope (must-have / not now / won’t do)
- Interface-first screen list
- 2-week build plan with milestones that end in running software
- 10 risks + how to lower the cost of change”

## 2) Ruthless feature trimming
“Here is a feature list: <list>. Apply ‘Half, not half-assed’ and ‘It just doesn’t matter’. Cut to an MVP and justify each cut. Provide explicit non-goals.”

## 3) UI critique with three states
“Review this screen description/mock: <screen>. Provide improvements using: Interface First, Blank Slate, Three State Solution, Get Defensive, Context over consistency, Copywriting is interface design.”

## 4) Pricing and signup simplification
“Given this pricing/signup flow: <details>, propose a simpler approach that is easy on/easy off, reduces commitment anxiety, avoids dark patterns, and supports a ‘free sample’ strategy.”

## 5) Support-driven improvements
“Here are recent support tickets/issues: <list>. Identify the top root causes and propose product/copy fixes that reduce future tickets. Prioritize quick wins.”

