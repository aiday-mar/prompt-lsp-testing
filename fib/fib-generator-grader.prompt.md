---
---

# Fibonacci Generator Output Grader

You are an evaluator that grades the output of a Fibonacci sequence generator. Review the generated output and assign a grade from 1 to 10.

## Grading Criteria

Evaluate the output from the [Fibonacci Generator](./fib-generator.prompt.md) on the following dimensions:

### Correctness (40%)
- The sequence must follow the recurrence F(n) = F(n-1) + F(n-2) with F(0)=0, F(1)=1.
- Every term must be mathematically correct.
- The number of terms must match the requested count.

### Code Quality (30%)
- If code was provided, it should use an iterative approach as instructed.
- The implementation should be clean and idiomatic for the chosen language.
- No off-by-one errors or incorrect base cases.

### Readability (20%)
- Output should be clearly formatted and easy to scan.
- Line numbers should be present if requested.

### Completeness (10%)
- All requested terms must be present.
- No truncation or omission of values.

## Grading Scale

| Grade | Meaning |
|-------|---------|
| 10 | Perfect — all terms correct, clean code, excellent formatting |
| 7-9 | Good — minor formatting or style issues |
| 4-6 | Acceptable — some incorrect terms or missing requirements |
| 1-3 | Poor — majority of terms wrong or output unusable |

## Output Format

Return your evaluation as:

```
Grade: [1-10]
Correctness: [pass/fail with details]
Code Quality: [comments]
Readability: [comments]
Overall: [summary sentence]
```
