# Token Optimization Models Agent Instructions

## Scope

These instructions apply to `docs/prompt-engineering/token-optimization/models/`.

## Focus area

Maintain this folder as the awesome-index scope for model- and ML-based prompt/context compression: methods that use a model (compressor, autoencoder, or learned policy) to shorten prompts or context while preserving task performance.

## Folder-specific guidance

- Keep this folder for model/ML-based compressors; keep heuristic or tokenizer-level tricks in the parent `token-optimization` index.
- Prefer methods with a paper, benchmark, or maintained implementation; link the canonical repo and, where useful, the paper.
- Note the compression mechanism (e.g., token pruning, distillation, autoencoding) in the description.

## Required structure

- `README.md` is the category index for this scope.
- Start with `# Token Optimization Models` and a concise description of the scope.
- Use `## Contents`, not `## Table of Contents`.
- Keep entries grouped and consistently formatted.
- Prefer `- [Name](URL) - Description.` for verified resources.
- Preserve repo-wide requirements from the root `AGENTS.md` and `docs/standards/README.md`.

## Enforcement

- Run `git diff --check` after edits.
- Run `rg "^## Table of Contents" docs/prompt-engineering/token-optimization/models docs/standards/README.md` before committing documentation changes.
- Check that new entries are relevant to this folder's focus and are not better placed in a sibling category.
