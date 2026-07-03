# Agent Tracing Agent Instructions

## Scope

These instructions apply to `docs/agents/tracing/`.

## Focus area

Maintain this folder as the awesome-index scope for observability, spans, telemetry schemas, trace analysis, and standards for AI-agent execution data.

## Folder-specific guidance

- Prefer standards and instrumentation that make agent behavior observable and comparable.
- Note interoperability standards such as OpenTelemetry when relevant.
- Keep optimization frameworks in `agent-optimization` unless the resource is primarily about tracing.

## Required structure

- `README.md` is the category index for this scope.
- Start with `# Agent Tracing` and a concise description of the scope.
- Use `## Contents`, not `## Table of Contents`.
- Keep entries grouped and consistently formatted.
- Prefer `- [Name](URL) - Description.` for verified resources.
- Preserve repo-wide requirements from the root `AGENTS.md` and `docs/standards/README.md`.

## Enforcement

- Run `git diff --check` after edits.
- Run `rg "^## Table of Contents" docs/agents/tracing docs/standards/README.md` before committing documentation changes.
- Check that new entries are relevant to this folder's focus and are not better placed in a sibling category.
