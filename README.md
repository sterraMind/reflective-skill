# Reflective Solution Framework

A structured thinking framework for AI agents that promotes critical analysis and iterative problem-solving.

## Overview

This is an OpenCode agent skill that guides AI assistants through a systematic reflection process when analyzing problems, reviewing code, or proposing solutions. The framework ensures thorough evaluation before jumping to conclusions.

```
Assess → Propose → Nurture → Iterate
```

## When to Use

Activate this skill when the user:
- Asks to analyze or review code/implementation
- Asks "what are the problems with this approach?"
- Asks "how would you solve this?"
- Asks for evaluation of a workflow or solution
- Wants deeper analysis or self-critique

## Core Process

### 1. Assess
- Analyze the current implementation or situation
- Identify potential issues (edge cases, race conditions, error handling)
- Understand the user's real needs and constraints

### 2. Propose
- Provide concrete, actionable solutions
- Explain the implementation approach
- Clarify applicable scenarios and limitations

### 3. Nurture (Critical)

Key questions to ask yourself:
1. Does the solution solve the root problem, or just patch symptoms?
2. What edge cases are not considered?
3. Is there a better design approach?
4. What scenarios is this suitable for, and what are the limitations?
5. Is there a simpler, safer alternative?

Dimensions to evaluate:
- Reliability (concurrency, failure recovery)
- Performance impact
- Security and data integrity
- Maintainability
- User experience

### 4. Iterate
- Adjust or propose new solutions based on scrutiny
- If a better approach is found, replace confidently
- If the original solution is optimal, explain why

## Response Format

```markdown
## Assess
<current situation analysis>

## Solution
<proposed solution(s)>

## Nurture
### Pros
- ...

### Cons / Edge Cases
- ...

### Better Approach
<if found>

## Conclusion
<final recommendation>
```

## Anti-Patterns

1. Don't rush to answer - fully evaluate first
2. Don't only list pros - must point out cons and edge cases
3. Don't cling to the first solution - replace if scrutiny reveals issues
4. Don't avoid calling something a "patch" - be honest about limitations

## Tips

- If the issue involves data security or irreversible operations, prioritize the safest approach
- If the issue is performance optimization, provide benchmark suggestions
- If the user doesn't specify scenarios, proactively ask or cover multiple scenarios

## Installation

This is an OpenCode skill. Install via:
```bash
opencode skill install reflective-skill
```

## Files

- `SKILL.en.md` - English version
- `SKILL.zh.md` - Chinese version

## License

MIT License

## Contribution

Feel free to submit issues and pull requests.
