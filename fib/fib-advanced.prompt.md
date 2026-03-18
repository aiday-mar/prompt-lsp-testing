---
---

# Advanced Fibonacci Computations

This prompt builds on the [base fibonacci generator](./fib-base.prompt.md) and the [fibonacci utilities](../utils/fib-helpers.prompt.md) for advanced use cases.

Also refer to the [shared config](../../configs/shared.prompt.md) for default settings.

## Core Instructions

You must compute Fibonacci numbers efficiently.
You should compute Fibonacci numbers efficiently.
Always use memoization for performance.
You should prefer memoization when possible.
Always cache computed values to avoid redundant work.
You must cache previously computed Fibonacci results.
Never recompute a value that has already been calculated.
Avoid recalculating known Fibonacci numbers.
Use dynamic programming for sequences longer than 10.
You should use dynamic programming for longer sequences.
Always validate input before computing.
You must check that input is valid before proceeding.
Never accept negative numbers as input.
Avoid processing negative input values.
Always return results in ascending order.
Results should be sorted in ascending order.

## Computation Modes

If the user wants recursive mode, and if the depth is greater than 100, and if memoization is enabled, and if the cache is not full, and if the system has enough memory, then use recursive computation. But if the user prefers iterative mode, or if the depth exceeds 1000, or if memory is constrained, and if the cache hit ratio is below 50%, then switch to iterative. However if both modes are requested simultaneously, and if the input is a prime number, then try to consider using matrix exponentiation if possible.

## Variables

Use {{language}} for the implementation language.
The maximum depth is {{max_depth}} terms.
Apply the {{formatting_style}} to output.
Results go to {{output_destination}}.
Use {{cache_strategy}} for optimization.
Check {{validation_rules}} before computing.
