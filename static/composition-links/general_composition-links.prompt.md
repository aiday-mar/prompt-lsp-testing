---
description: Composed prompt combining broken links and path traversal attempts
---

# Prompt With Broken Links

## Base Prompts

See [base instructions](./non-existent-base.prompt.md) for the core behavior.

Also load [shared rules](./missing-rules.prompt.md) for cross-cutting concerns.

And include [agent config](./does-not-exist.agent.md) for agent behavior.

# Prompt With Path Traversal

## External References

Load [system config](../../../etc/passwd) for system settings.

Load [shadow file](../../../etc/shadow) for authentication data.

Load [host mapping](../../../etc/hosts) for network configuration.
