---
mode: default
---

# Request Transformer

Transform API requests from v1 format to v2 format.

## Input Examples

```json
{ "user": "alice", "action": "read" }
```

```json
{ "user": "bob", "action": "write", "target": "doc-1" }
```

```json
{ "user": "carol", "action": "delete", "target": "doc-2" }
```

## Output Example

```json
{ "principal": "alice", "operation": "READ", "resource": null, "version": 2 }
```
