# Agentic Web Agent Instructions

## Scope

These instructions apply to `docs/agentic-web/`.

## Focus area

Maintain this folder as the awesome-index scope for the agentic web: projects, frameworks, and protocols that make existing websites first-class participants in the agent ecosystem — either by exposing a site's content to agents for natural-language querying, or by embedding agents that operate the site's own UI through natural language.

## Folder-specific guidance

- Distinguish content-side access (making a site's data answerable in natural language) from control-side automation (driving a site's UI from natural language), and say which side each entry sits on.
- Note each resource's type (framework, library, protocol, or spec) and where it runs (server-side, client-side/in-page, or browser/extension).
- Record the relationship to tracked standards (MCP, A2A, Schema.org) when a resource declares one, and link to `../standards/` rather than restating those specs.
- Keep entries here only when they target the open web; deep agent-capability topics (harnesses, sandboxes, memory) belong in `../agents/`, and interface-generation frameworks belong in `../genUI/`.

## Required structure

- `README.md` is the category index for this scope.
- Start with `# Agentic Web` and a concise description of the scope.
- Use `## Contents` or descriptive catalog sections (for example `## Approaches`), never `## Table of Contents`.
- Keep entries grouped and consistently formatted as `- [Name](URL) - Description.` bullets or tables.
- Preserve repo-wide requirements from the root `AGENTS.md` and `docs/standards/README.md`.

## Enforcement

- Run `git diff --check` after edits.
- Run `rg "^## Table of Contents" docs/agentic-web` before committing documentation changes.
- Run `bun run konsistent` to confirm this folder still provides its `README.md` and `AGENTS.md`.
- Check that new entries fit this folder's focus and are not better placed in a sibling category (`agents`, `genUI`, or `standards`).
