---
mode: default
---

# Structured Output Compliance

All responses must conform to this schema:

- `status`: one of "success", "error", "pending"
- `code`: HTTP status code integer
- `data`: object containing the response payload
- `errors`: array of error objects with `field`, `message`, and `code`
- `pagination`: object with `page`, `pageSize`, `total`, and `hasMore`
- `metadata`: object with `requestId`, `timestamp`, `version`

But also feel free to include additional fields as you see fit. The schema is more of a guideline than a strict requirement. Sometimes it makes sense to just return a simple string instead.
