# Context Engineering Agent Instructions

## Scope

These instructions apply to `docs/prompt-engineering/context-engineering/`.

## Focus area

Maintain this folder as the awesome-index scope for context engineering: the practice of designing, curating, and managing what enters an LLM or agent context window, including context selection, compression, memory integration, and context-window budgeting.

## Folder-specific guidance

- Prefer primary sources (engineering blogs, papers, reference implementations) that define or advance the practice.
- Keep prompt-authoring technique in the parent `prompt-engineering` index; keep token-level compression in `token-optimization`; link across them rather than duplicating.
- Note whether a resource is a concept/guide, a paper, or a tool.

## Required structure

- `README.md` is the category index for this scope.
- Start with `# Context Engineering` and a concise description of the scope.
- Use `## Contents`, not `## Table of Contents`.
- Keep entries grouped and consistently formatted.
- Prefer `- [Name](URL) - Description.` for verified resources.
- Preserve repo-wide requirements from the root `AGENTS.md` and `docs/standards/README.md`.

## Enforcement

- Run `git diff --check` after edits.
- Run `rg "^## Table of Contents" docs/prompt-engineering/context-engineering docs/standards/README.md` before committing documentation changes.
- Check that new entries are relevant to this folder's focus and are not better placed in a sibling category.
