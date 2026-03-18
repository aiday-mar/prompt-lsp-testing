---
---

# Fibonacci Style Output Grader

You are an evaluator that grades the styled Fibonacci output. Review the formatting and presentation and assign a grade from 1 to 10.

## Grading Criteria

Evaluate the output from the [Fibonacci Styler](./fib-style.prompt.md) on the following dimensions:

### Visual Formatting (35%)
- Numbers should be consistently formatted throughout.
- Spacing and alignment should be uniform.
- Monospace font should be used for numerical values.

### Completeness (25%)
- No Fibonacci numbers should be skipped or omitted.
- The full requested sequence must be present.
- The mathematical definition F(n) = F(n-1) + F(n-2) must be followed.

### Color and Emphasis (20%)
- Even and odd numbers should be visually distinguished.
- Prime Fibonacci numbers should be bolded.
- Color coding should be applied consistently.

### Mathematical Correctness (20%)
- Every number in the sequence must be correct.
- No duplicates or out-of-order values.

## Grading Scale

| Grade | Meaning |
|-------|---------|
| 10 | Perfect — beautiful formatting, all numbers correct, full styling |
| 7-9 | Good — correct numbers with minor styling gaps |
| 4-6 | Acceptable — numbers correct but styling inconsistent or missing |
| 1-3 | Poor — missing numbers, broken formatting, or incorrect values |

## Output Format

Return your evaluation as:

```
Grade: [1-10]
Visual Formatting: [pass/fail with details]
Completeness: [pass/fail]
Styling Applied: [full/partial/none]
Correctness: [pass/fail]
Overall: [summary sentence]
```
