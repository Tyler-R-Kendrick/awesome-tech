# design.md (DESIGN.md)

A format specification from Google Labs (open-sourced April 2026, alpha) for describing a visual identity — a design system — to coding agents. A `DESIGN.md` file pairs machine-readable design tokens in YAML frontmatter (colors, typography, spacing, corner radii, and component-property mappings) with a human-readable Markdown body that explains the rationale: the tokens give agents exact values, and the prose explains why those values exist and how to apply them. Dropped into a project root, it lets AI coding agents produce on-brand interfaces without re-explaining the design system on each task. The spec originated in Google's Stitch design tool and ships with a CLI to validate tokens, check WCAG contrast, and export to formats such as Tailwind and W3C Design Tokens.

## Contents

- [Stitch and the DESIGN.md spec](https://blog.google/innovation-and-ai/models-and-research/google-labs/stitch-design-md/) - Google announcement of the open-sourced spec.
- [github.com/google-labs-code/design.md](https://github.com/google-labs-code/design.md) - Official repository (Apache-2.0, alpha).
- [Specification](https://github.com/google-labs-code/design.md/blob/main/docs/spec.md) - Draft format specification.

## Footnotes

- `DESIGN.md` is an agent-facing file format in the same family as [Agent Skills](../agents/skills/README.md) (`SKILL.md`) and [Open Knowledge Format](./okf.md); the notion of these as a coordinated "instruction layer" is a community interpretation, not a joint standard.
