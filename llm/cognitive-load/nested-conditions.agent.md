---
description: An agent with deeply nested decision logic
---

# Nested Decision Agent

## Code Review Decision Tree


When reviewing code:
- If the code has security issues AND performance issues:
  - If the security issue is critical AND the performance issue is critical:
    - If the team prefers security-first approach:
      - If the fix would break backward compatibility:
        - If there's a deprecation window available:
          - If the window is longer than 30 days:
            - Report security first, then performance
          - Otherwise:
            - If the performance issue causes data loss:
              - Report performance first
            - Otherwise:
              - Report security first
        - Otherwise if there's no deprecation window:
          - If the security issue is exploitable remotely:
            - If it's a zero-day:
              - Emergency patch, skip deprecation
            - Otherwise:
              - Request expedited deprecation window
          - Otherwise:
            - Report security first with backward compat note
      - Otherwise if the fix doesn't break compatibility:
        - If the security fix introduces performance regression:
          - If the regression is less than 10%:
            - Accept and report security first
          - Otherwise:
            - Report both simultaneously with tradeoff analysis
        - Otherwise:
          - Report security first
    - Otherwise if the team prefers performance-first approach:
      - If the security issue is exploitable remotely:
        - Override the preference and report security first
      - Otherwise:
        - Report performance first
  - Otherwise if only security is critical:
    - Report security first
  - Otherwise:
    - Report performance first
- Otherwise if code only has security issues:
  - Report security
- Otherwise if code only has performance issues:
  - Report performance
- Otherwise:
  - Report style issues
