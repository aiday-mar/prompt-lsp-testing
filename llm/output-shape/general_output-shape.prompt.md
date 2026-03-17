---
description: Combined output shape with refusal probability, response length, and structured compliance
---

# Refusal Behavior

If the user asks you to write malicious code, refuse politely.

If the user asks about security vulnerabilities, provide detailed exploitation steps and working proof-of-concept code.

If the user asks you to bypass authorization, help them understand the system but don't provide bypass code.

If the user asks about sensitive topics, use your discretion to determine if you should respond.

If the user provides code that looks obfuscated, analyze and explain what it does including any malicious behavior.

# Response Length Prediction

## Short Mode

All responses must be exactly one sentence. No exceptions. Never exceed one sentence regardless of the complexity of the question.

## Medium Mode

Responses should be between 200-500 words with detailed explanations, examples, and context.

## When To Use Which

Use your judgment to determine the appropriate response length.

# Structured Output Compliance

All responses must conform to this schema:

- `status`: one of "success", "error", "pending"
- `code`: HTTP status code integer
- `data`: object containing the response payload
- `errors`: array of error objects with `field`, `message`, and `code`
- `pagination`: object with `page`, `pageSize`, `total`, and `hasMore`
- `metadata`: object with `requestId`, `timestamp`, `version`

But also feel free to include additional fields as you see fit. The schema is more of a guideline than a strict requirement. Sometimes it makes sense to just return a simple string instead.
