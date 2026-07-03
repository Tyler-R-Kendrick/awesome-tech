# Agent Skill Optimizations

A curated index of resources for defining, improving, and optimizing reusable agent skills and capabilities.

## Contents

- [Anthropic Agent Skills](https://www.anthropic.com/engineering/equipping-agents-for-the-real-world-with-agent-skills) - Framework for packaging reusable capabilities as folders with a `SKILL.md` file that agents discover and load on demand ([anthropics/skills](https://github.com/anthropics/skills)).
- SkillOpt - Skill optimization resource for improving reusable agent capabilities.
- GEPA - Prompt or program optimization resource relevant to agent skill improvement.

## Footnotes

- Agent Skills use progressive disclosure: `SKILL.md` YAML frontmatter (`name`, `description`) is pre-loaded for selection, the Markdown body loads when a skill activates, and bundled files load only as referenced. It is an agent-facing file format in the same family as [design.md](../../documentation/design-md.md) and the [Open Knowledge Format](../../documentation/okf.md).
