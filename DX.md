# DX — awesome-tech

Standard: the **Monorepo DX Playbook** (canonical in the `HoBo` repo → `docs/standards/monorepo-dx-playbook.md`,
`https://github.com/Tyler-R-Kendrick/HoBo/blob/main/docs/standards/monorepo-dx-playbook.md`).

## Current state
This is a **curated Markdown content wiki**, not a code repo — most build/typecheck/test/deploy items are **N/A by design**.
bun@1.3.11 **pinned** ✓, single root package, `konsistent` for structural conventions. One thin CI workflow
`konsistent.yml` (pull_request + push:main, **with `concurrency`**) — this is the reference-quality minimal workflow.
Structural/whitespace checks are otherwise **manual-only** (per `AGENTS.md`). No git hooks.

## Adoption checklist (content-repo subset)
1. 🔥 **Add a `pre-commit` hook** running `konsistent` + `git diff --check` — these checks are manual-only today. **[S]**
2. **Add markdown link-check / dead-link** validation to the existing `konsistent.yml` (broken relative links and
   heading-style are currently unenforced). **[S]**
3. **Keep `konsistent.yml` as-is** — it's the reference-quality minimal server-side backstop (structural validation +
   `concurrency`). No Turborepo/typecheck/deploy needed. **[—]**

Workflow policy (playbook §8): a content repo's "build" is its structural validity, which `konsistent` checks; one thin,
`concurrency`-guarded workflow is the correct amount of CI here.
