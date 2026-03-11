---
mode: default
---

# JSON Response Formatter

All responses must be in JSON format with the following structure:

- A `status` field (string: "success" or "error")
- A `data` field (object: the response payload)
- A `metadata` field (object: timing and version info)
- An `errors` array (only present on error responses)

Ensure the JSON is valid, properly indented, and uses camelCase keys.
