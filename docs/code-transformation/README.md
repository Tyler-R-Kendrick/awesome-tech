# Code Transformation

Deterministic, rules-based engines that refactor and migrate source code at scale by parsing it into a structured model and applying reusable, repeatable transformations rather than editing text directly. In agentic workflows these engines act as trusted tools: an AI agent can delegate a well-defined change to a deterministic, reviewable transformation instead of rewriting code token by token, and reserve model reasoning for the parts no rule covers.

## Contents

- [OpenRewrite](./openrewrite.md) - Moderne's open-source auto-refactoring ecosystem built on Lossless Semantic Trees and recipes, with MCP and agent-skill integrations.

## Related

- [Model Context Protocol (MCP)](../standards/mcp.md) - Interface through which agents can invoke transformation recipes as tools.
- [Agent Skills](../agents/skills/README.md) - Skill format used to teach agents transformation-tool workflows.
