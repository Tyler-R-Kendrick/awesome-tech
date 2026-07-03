# Agent Isolation Agent Instructions

## Scope

These instructions apply to `docs/agents/sandboxes/`.

## Focus area

Maintain this folder as the awesome-index scope for sandboxing, permissions, containment, policy controls, and safe execution environments for AI agents.

## Folder-specific guidance

- Prioritize security-relevant containment and policy mechanisms.
- Describe the isolation boundary clearly: process, filesystem, network, browser, container, or policy layer.
- Avoid weakening repository-wide guidance about standard enforcement or ingestion policy.

## Required structure

- `README.md` is the category index for this scope.
- Start with `# Agent Isolation` and a concise description of the scope.
- Use `## Contents`, not `## Table of Contents`.
- Keep entries grouped and consistently formatted.
- Prefer `- [Name](URL) - Description.` for verified resources.
- Preserve repo-wide requirements from the root `AGENTS.md` and `docs/standards/README.md`.

## Enforcement

- Run `git diff --check` after edits.
- Run `rg "^## Table of Contents" docs/agents/sandboxes docs/standards/README.md` before committing documentation changes.
- Check that new entries are relevant to this folder's focus and are not better placed in a sibling category.
