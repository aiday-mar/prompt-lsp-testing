---
mode: default
---

# Prompt With Unbalanced Sections

## Setup

Initialize the service.

## Rules

This section is intentionally very long to trigger the heaviest-section diagnostic.

Rule 1: Always validate all user input fields including name, email, phone, address, city, state, zip, country, date of birth, social security number, driver's license, passport number, and any other personally identifiable information before storing in the database or transmitting over the network.

Rule 2: Always sanitize output by escaping HTML entities, stripping script tags, removing event handlers, encoding special characters, validating URLs, checking for data URIs, scanning for SVG injection, filtering CSS expressions, blocking iframe injection, and preventing template injection in all response templates and dynamic content generation.

Rule 3: Always implement comprehensive logging that captures request ID, timestamp, user ID, session ID, IP address, user agent, request method, request path, query parameters, request body hash, response status, response time, error details, stack traces, correlation IDs, and span IDs for distributed tracing across all microservices.

Rule 4: Always enforce rate limiting with per-user limits, per-IP limits, per-endpoint limits, global limits, burst allowances, sliding window calculations, token bucket refill rates, exponential backoff suggestions, retry-after headers, and graceful degradation responses for all public-facing API endpoints.

Rule 5: Always perform authorization checks including role-based access control, attribute-based access control, resource ownership verification, organization membership, team membership, project membership, feature flag evaluation, subscription tier validation, IP allowlist checking, and time-based access restrictions.

Rule 6: Always handle errors with specific error codes, human-readable messages, machine-readable error types, suggested remediation steps, documentation links, support contact information, request correlation IDs, partial success indicators, rollback confirmations, and retry eligibility flags.

Rule 7: Always implement caching with appropriate TTL values, cache key generation, cache invalidation strategies, cache warming procedures, cache stampede prevention, stale-while-revalidate patterns, cache bypass conditions, cache size limits, eviction policies, and cache hit/miss metrics.

Rule 8: Always validate configuration including environment variable presence, type checking, range validation, format validation, dependency checking, circular reference detection, default value application, sensitive value masking, configuration hot-reloading support, and configuration change audit logging.

## Cleanup

Shut down gracefully.
