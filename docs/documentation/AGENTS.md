# Documentation Agent Instructions

## Scope

These instructions apply to `docs/documentation/`.

## Focus area

Maintain this folder as the awesome-index scope for documentation and knowledge tooling and formats: resources that generate, maintain, structure, or represent agent- and LLM-facing documentation, knowledge, and design context.

## Folder-specific guidance

- Track content-authoring resources here (documentation generators, knowledge formats, design-context formats), not agent-to-agent wire protocols — those belong in `docs/standards/`.
- State whether each entry is a tool, a spec/format, or both, and name its originating organization.
- Cross-reference `docs/standards/` when a format is also a required repository standard, and `docs/agents/skills/` for agent-facing capability formats.

## Required structure

- `README.md` is the category index for this scope.
- Start with `# Documentation` and a concise description of the scope.
- Use `## Contents`, not `## Table of Contents`.
- Keep entries grouped and consistently formatted.
- Prefer `- [Name](URL) - Description.` for verified resources.
- Preserve repo-wide requirements from the root `AGENTS.md` and `docs/standards/README.md`.

## Enforcement

- Run `git diff --check` after edits.
- Run `rg "^## Table of Contents" docs/documentation docs/standards/README.md` before committing documentation changes.
- Check that new entries are relevant to this folder's focus and are not better placed in a sibling category.
