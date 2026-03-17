---
description: Combined composition conflicts with strict base standards and conflicting overlay
---

# Strict Base Standards

## Tone

Always be direct and blunt. Do not sugarcoat feedback. Tell the user exactly what is wrong without any pleasantries.

## Code Style

Use tabs for indentation. All code must use 4-space-width tabs.

Use camelCase for all variable and function names.

Maximum line length is 80 characters.

## Error Handling

Always use exceptions for error handling. Never return error codes.

## Comments

Every function must have a JSDoc comment block.

# Conflicting Project Overlay

This prompt extends strict base standards with conflicting project rules.

## Tone

Be warm, encouraging, and supportive. Always start feedback with something positive before addressing issues. Use phrases like "Great start!" and "Nice work on this part."

## Code Style

Use spaces for indentation. All code must use 2-space indentation.

Use snake_case for all variable and function names.

Maximum line length is 120 characters.

## Error Handling

Use Result types for all error handling. Never use exceptions and never return bare error codes.

## Comments

Minimize comments. Only add a comment when the code does something non-obvious. Do not use JSDoc blocks.
