---
name: reflective-solution
description: Structured reflective thinking framework: Assess → Propose → Nurture → Iterate. Use when users want deeper analysis, self-critique of solutions, or critical thinking during problem-solving.
---

# Reflective Solution Framework

```
Assess → Propose → Nurture → Iterate
```

## When to Use

When the user:
- Asks to analyze/review code or implementation
- Asks "what are the problems with this approach?"
- Asks "how would you solve this?"
- Asks "how do you think about your solution?"
- Asks to evaluate a workflow or process

## Core Loop

### Step 1: Assess
- Analyze current implementation or situation
- Identify potential issues (edge cases, race conditions, error handling)
- Understand user's real needs and constraints

### Step 2: Propose
- Provide concrete, actionable solutions
- Explain implementation approach
- Clarify applicable scenarios

### Step 3: Nurture (Critical)

**Key Questions:**
1. Does my solution solve the root problem, or just patch symptoms?
2. What edge cases are not considered?
3. Is there a better design approach?
4. What scenarios is this suitable for, and what are the limitations?
5. Is there a simpler, safer alternative?

**Dimensions:**
- Reliability (concurrency, failure recovery)
- Performance impact
- Security & Data Integrity
- Maintainability
- User Experience

### Step 4: Iterate
- Adjust or propose new solution based on scrutiny
- If a better approach is found, replace confidently
- If original solution is optimal, explain why

## Response Format

```
## Assess
<current situation analysis>

## Solution
<proposed solution(s)>

## Scrutiny
### Pros
- ...

### Cons / Edge Cases
- ...

### Better Approach
<if found>

## Conclusion
<final recommendation>
```

## Anti-patterns

1. Don't rush to answer - fully evaluate first
2. Don't only list pros - must point out cons and edge cases
3. Don't cling to first solution - replace if scrutiny reveals issues
4. Don't avoid "patch" assessment - be honest if solution is just a patch

## Tips

- If the issue involves **data security/irreversible operations**, prioritize the safest approach
- If the issue is **performance optimization**, provide benchmark suggestions
- If user doesn't specify scenarios, proactively ask or cover multiple scenarios
