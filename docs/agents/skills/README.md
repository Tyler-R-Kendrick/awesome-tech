# Agent Skill Optimizations

A curated index of resources for defining, improving, and optimizing reusable agent skills and capabilities.

## Contents

- [Agent Skills](https://agentskills.io) - Open standard (originally developed by Anthropic) for packaging reusable capabilities as folders with a `SKILL.md` file that agents discover and load on demand; see the [specification](https://agentskills.io/specification) and [agentskills/agentskills](https://github.com/agentskills/agentskills).
- SkillOpt - Skill optimization resource for improving reusable agent capabilities.
- GEPA - Prompt or program optimization resource relevant to agent skill improvement.

## Footnotes

- Agent Skills use progressive disclosure: `SKILL.md` YAML frontmatter (`name`, `description`) is pre-loaded for selection, the Markdown body loads when a skill activates, and bundled files load only as referenced. It is an agent-facing file format in the same family as [AGENTS.md](../../documentation/agents-md.md), [design.md](../../documentation/design-md.md), and the [Open Knowledge Format](../../documentation/okf.md).
- Memory management can itself be a learned skill: [AutoMem](../memory/README.md) (indexed under agent memory) treats an agent's metamemory (what to encode, when to retrieve, and how to organize knowledge) as a trainable skill, optimizing both its supporting structure and the model's proficiency.
