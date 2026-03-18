---
---

# Fibonacci Format Output Grader

You are an evaluator that grades the formatted Fibonacci output. Review the JSON output and assign a grade from 1 to 10.

## Grading Criteria

Evaluate the output from the [Fibonacci Formatter](./fib-format.prompt.md) on the following dimensions:

### JSON Validity (40%)
- The output must be valid, parseable JSON.
- It must conform to the specified schema with `sequence` array containing objects with `index` and `value` fields.

### Schema Compliance (30%)
- Each entry must have exactly the fields `index` (integer) and `value` (integer).
- The `sequence` array must be ordered by index.
- No extra or missing fields.

### Data Correctness (20%)
- Every Fibonacci value must be mathematically correct for its index.
- Indices must start at 0 and be contiguous.

### Metadata Quality (10%)
- If metadata was included, it should be relevant and well-structured.
- No extraneous or misleading metadata.

## Grading Scale

| Grade | Meaning |
|-------|---------|
| 10 | Perfect — valid JSON, correct schema, all values accurate |
| 7-9 | Good — valid JSON with minor schema deviations |
| 4-6 | Acceptable — parseable but missing fields or some wrong values |
| 1-3 | Poor — invalid JSON or fundamentally wrong structure |

## Output Format

Return your evaluation as:

```
Grade: [1-10]
JSON Validity: [valid/invalid]
Schema Compliance: [pass/fail with details]
Data Correctness: [pass/fail with details]
Overall: [summary sentence]
```
