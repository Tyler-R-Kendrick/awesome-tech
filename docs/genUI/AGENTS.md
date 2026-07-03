# Generative UI (GenUI) Agent Instructions

## Scope

These instructions apply to `genui/`.

## Focus area

Maintain this folder as the awesome-index scope for generative UI: frameworks, SDKs, protocols, and specs where agents and models produce structured, interactive interfaces instead of only text.

## Folder-specific guidance

- Distinguish core rendering-first GenUI frameworks and specs from adjacent agent/frontend protocols, and label related-but-not-core entries as such.
- Describe whether a resource is a framework, SDK, protocol, or spec, and its primary integration target (host, tool/server, or cross-platform client).
- Keep general agent-to-frontend event protocols as "related" unless they directly render generative UI.

## Required structure

- `README.md` is the category index for this scope.
- Start with `# Generative UI (GenUI)` and a concise description of the scope.
- Use `## Contents` or descriptive catalog sections (for example `## Core projects and specs`), never `## Table of Contents`.
- Keep entries grouped and consistently formatted, whether as tables or `- [Name](URL) - Description.` bullets.
- Preserve repo-wide requirements from the root `AGENTS.md` and `standards/README.md`.

## Enforcement

- Run `git diff --check` after edits.
- Run `rg "^## Table of Contents" genui README.md standards/README.md` before committing documentation changes.
- Check that new entries are relevant to this folder's focus and are not better placed in a sibling category.
