# Token Optimization Agent Instructions

## Scope

These instructions apply to `token-optimization/`.

## Focus area

Maintain this folder as the awesome-index scope for token and context reduction: prompt compression, context pruning, tokenizer-level techniques, and tooling that lowers token or context cost for LLM and agent workloads.

## Folder-specific guidance

- Identify what is reduced: prompt size, context window usage, output length, or overall token cost.
- Prefer entries with reproducible methods, papers, benchmarks, or working code.
- Keep broader optimization work (cost, latency, trajectory quality) in `agent-optimization` unless it is specifically about token or context reduction.

## Required structure

- `README.md` is the category index for this scope.
- Start with `# Token Optimization` and a concise description of the scope.
- Use `## Contents`, not `## Table of Contents`.
- Keep entries grouped and consistently formatted.
- Prefer `- [Name](URL) - Description.` for verified resources.
- Preserve repo-wide requirements from the root `AGENTS.md` and `standards/README.md`.

## Enforcement

- Run `git diff --check` after edits.
- Run `rg "^## Table of Contents" token-optimization README.md standards/README.md` before committing documentation changes.
- Check that new entries are relevant to this folder's focus and are not better placed in a sibling category.
