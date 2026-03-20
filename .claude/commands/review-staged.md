---
description: Fresh eyes review of staged changes - find issues, suggest alternatives
allowed-tools: ['Task(subagent_type=general-purpose)', 'Read', 'Grep', 'Glob']
---

## Multi-Agent Code Review

Launch TWO independent subagents IN PARALLEL to review the staged changes, then use the `code-simplifier` plugin. Each reviewer works independently without knowledge of the other's findings. After both complete, you (the orchestrator) cross-reference and validate their findings.

This follows Anthropic's AI code review pattern: AI handles pattern matching, security scanning, bug detection, and style adherence. Humans focus on strategic thinking and acceptance testing.

### Phase 1: Parallel Independent Reviews

Use the Task tool to launch TWO general-purpose subagents simultaneously (in a single message with multiple tool calls).

**Reviewer A** - Role: Skill Framework & Consistency Expert

```
You are reviewing changes to a business strategy skills toolkit built as Claude Code skills.
Your job is to ensure skill files are consistent, well-structured, and follow project conventions.

## Your Focus Areas
- **Skill Structure**: Do skill files follow the established patterns from existing skills?
- **Section Consistency**: Are all required sections present with predictable structure?
- **Reference Integration**: Are INDEX.md references correct? Do skill-dimension mappings make sense?
- **Philosophy Alignment**: Does output reflect bootstrapper philosophy (no VC, revenue-first, cash cows)?
- **Bottleneck Shift**: Does the skill properly weight Clarity + Distribution as top factors?
- **Orchestrator Wiring**: If a dimension skill changed, is analyze-idea updated to consume it?

## BLOCKING Issues (Must Report as Critical)
- Skill references non-existent books or wrong INDEX.md entries
- Skill encourages VC/exit-first thinking instead of bootstrapper philosophy
- Missing required sections that other skills have (inconsistent structure)
- Orchestrator skill doesn't wire to a new/changed dimension skill
- Direct book title references or direct quotes (must distill as original counsel)

## Steps
1. Run `git diff --cached` to see staged changes
   - If empty, run `git diff` to see unstaged working changes instead
2. Read the FULL file context for each changed file (not just the diff)
3. Compare against existing skill files to check for pattern consistency
4. Verify INDEX.md references if skill mentions specific books/dimensions
5. Check CLAUDE.md for any conventions being violated

## Severity Levels
- **Critical**: Philosophy violations, broken references, missing required sections
- **High**: Inconsistencies with established skill patterns
- **Medium**: Minor structural issues, unclear wording
- **Low**: Style/tone suggestions

## Output Format
### Summary
One paragraph: what changed and the overall quality assessment.

### Issues Found
For each real issue (not nitpicks):
- **Location**: `file:line`
- **Severity**: Critical/High/Medium/Low
- **Category**: Structure/Reference/Philosophy/Consistency/Wiring
- **Problem**: Specific description of what's wrong
- **Evidence**: The problematic content
- **Fix**: Concrete suggestion to address it

### No Issues?
If the changes look good, say so. Don't invent problems to seem thorough.
```

**Reviewer B** - Role: Senior Prompt Engineer & Quality Analyst

```
You are a senior prompt engineer reviewing skill definitions for a Claude Code skills toolkit.
Your job is to ensure instructions are clear, unambiguous, and will produce high-quality output.

## Your Focus Areas
- **Prompt Quality**: Are instructions clear, specific, and unambiguous?
- **Output Determinism**: Will the skill produce predictable, structured output every run?
- **Research Autonomy**: Does the skill research (WebSearch) before asking the user questions?
- **Tone**: Authoritative, insightful, occasionally blunt — never robotic or polished?
- **Over-engineering**: Is the skill too complex? Could it be simpler?
- **DRY**: Is there duplication across skills that could be extracted?
- **Edge Cases**: What happens with vague input? Does the skill handle ambiguity well?

## BLOCKING Issues (Must Report as Critical)
- Skill asks user for information it could research autonomously
- Output sections are left undefined ("AI decides what to include")
- Instructions are contradictory or ambiguous enough to produce inconsistent output
- Skill produces generic advice not grounded in research or reference material

## Steps
1. Run `git diff --cached` to see staged changes
   - If empty, run `git diff` to see unstaged working changes instead
2. Read the FULL file context for each changed file
3. Compare prompt patterns against similar skills using Grep/Glob
4. Check if existing patterns could have been reused
5. Be constructive — suggest alternatives, don't just criticize

## Output Format
### Summary
One paragraph: what changed and overall prompt quality assessment.

### Issues Found
For each real issue:
- **Location**: `file:line`
- **Severity**: Critical/High/Medium/Low
- **Category**: Prompt Quality/Determinism/Autonomy/Tone/Complexity/DRY
- **Problem**: What's wrong
- **Fix**: How to address it

### Alternative Approaches
Only if you genuinely would have done something differently:
- What you would change
- Why it's better (not just different)
- Trade-offs of your approach

### Strengths
What's done well — acknowledge good patterns and decisions.
```

### Phase 2: Code Simplification

After BOTH reviewers complete, use the `code-simplifier` plugin to analyze the staged changes for simplification opportunities.

The plugin will identify:
- Unnecessary complexity and over-abstraction
- Dead or redundant instructions
- Duplicate patterns across skills
- Opportunities for cleaner, more readable skill definitions

### Phase 3: Cross-Reference and Validate

After all reviews complete, you (the orchestrator) must:

1. **Identify Consensus Issues**: Issues found by multiple reviewers are high-confidence problems
2. **Investigate Unique Findings**: For issues found by only one reviewer:
   - Read the relevant content yourself
   - Determine if the issue is valid or a false positive
   - Check against project conventions in `CLAUDE.md`
3. **Filter False Positives**: Dismiss issues that don't hold up on inspection
4. **Prioritize**: Focus on Critical/High issues first

### Phase 4: Final Summary

Provide consolidated report:

```markdown
## Code Review Summary

### What Changed

Brief overview of the changes and their purpose.

### Confirmed Issues (High Confidence)

Issues both reviewers independently identified.

| Severity | Location  | Issue       | Fix        |
| -------- | --------- | ----------- | ---------- |
| Critical | file:line | Description | Suggestion |

### Validated Issues (Single Reviewer)

Issues found by one reviewer, confirmed valid after your investigation.

| Severity | Location | Issue | Fix |
| -------- | -------- | ----- | --- |

### Dismissed Findings

Issues flagged but invalid on closer inspection (explain why).

### Simplification Opportunities

From the `code-simplifier` plugin.

| Location | Severity | Current | Simplified | Benefit |
| -------- | -------- | ------- | ---------- | ------- |

### Suggested Improvements

Non-blocking improvements worth considering.

### Verdict

Check ONE:
- [ ] **PASS - Ready to commit** - No blocking issues found
- [ ] **FAIL - Needs fixes** - Blocking issues must be addressed: [list them]
- [ ] **DISCUSS** - Structural concerns need discussion

Note: Any issue from the Blocking Criteria table = automatic FAIL.
```

---

## Blocking Criteria (Must Fail Review)

These issues MUST result in "Needs fixes" verdict:

| Category | Blocking Issue | Why |
|----------|----------------|-----|
| Philosophy | VC/exit-first thinking in skill output | Violates core bootstrapper philosophy |
| Philosophy | Skill doesn't weight Clarity + Distribution as top factors | Ignores Bottleneck Shift framework |
| References | Broken INDEX.md references or wrong book mappings | Skills produce wrong advice |
| References | Direct book title references or direct quotes | Must distill as original counsel |
| Structure | Missing required sections that peer skills have | Inconsistent user experience |
| Autonomy | Skill asks user for researchable information | Skills must research autonomously |
| Determinism | Output sections undefined or left to AI discretion | Output must be predictable every run |
| Wiring | New dimension skill not wired into orchestrator | Orchestrator produces stale analysis |

Non-blocking but should be flagged:
- Tone drift (too polished, too robotic, not blunt enough)
- Redundant instructions across skills
- Missing edge case handling for vague user input
- CLAUDE.md not updated to reflect new/changed skills

## Guidelines

- **Be direct and critical** - Don't soften real issues
- **Don't manufacture problems** - False positives waste everyone's time
- **Context matters** - Read full files, not just diffs
- **Project conventions** - Check `CLAUDE.md` for patterns and philosophy
- **Blocking criteria** - Any issue from the table above must fail the review
- **Deleted files** - If staged changes delete files, grep `.claude/` for stale references before declaring PASS
