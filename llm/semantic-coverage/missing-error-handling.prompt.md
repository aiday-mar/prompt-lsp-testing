---
mode: default
---

# API Handler With No Error Paths

## Behavior

Accept a JSON request body, validate the fields, query the database, transform the results, and return a JSON response.

## Fields

Required fields: `userId`, `action`, `payload`

## Response

Return the transformed data with a 200 status code.
