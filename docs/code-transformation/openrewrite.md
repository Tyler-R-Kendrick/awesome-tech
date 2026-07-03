# OpenRewrite

An open-source ecosystem for automated, rules-based refactoring of source code, maintained by Moderne. OpenRewrite parses code into a Lossless Semantic Tree (LST) — a format-preserving, type-attributed model — and applies **recipes**, deterministic search-and-transform operations, to perform framework migrations, dependency and language upgrades, security remediation, and style enforcement across large codebases. Because the transformations are deterministic and preserve original formatting, they are reviewable and repeatable, which is what lets AI coding agents delegate them as trusted tools rather than editing code token by token.

It was created by Jonathan Schneider at Netflix to automate migrating an internal logging library to SLF4J, and later became the foundation of Moderne, the company that stewards the project and sells a platform for running recipes across many repositories at once. Recipes come in two forms: **declarative** recipes compose and configure existing recipes in a `rewrite.yml` file with no compilation, and **imperative** recipes extend `org.openrewrite.Recipe` in Java and delegate to LST **visitors** for full programmatic control. Recipes run locally through the Maven (`rewrite-maven-plugin`) and Gradle (`org.openrewrite.rewrite`) plugins — for example `mvn rewrite:run` or `gradle rewriteRun` — or at scale through the Moderne CLI and Platform.

The framework and LST model are Apache-2.0, as is a large part of the recipe catalog; some recipe modules with significant Moderne or third-party contributions are distributed under the Moderne Source Available License. Open-source parsers and base recipes cover Java, Kotlin, Groovy, and common data and configuration formats (HCL, JSON, Properties, Protobuf, TOML, XML, YAML); additional language parsers (JavaScript/TypeScript, C#, Python, and others) exist, though running recipes against many of them requires a Moderne license.

## Contents

- [docs.openrewrite.org](https://docs.openrewrite.org/) - Official documentation home.
- [Getting started](https://docs.openrewrite.org/running-recipes/getting-started) - Quickstart for running recipes with Maven or Gradle.
- [Recipes](https://docs.openrewrite.org/concepts-and-explanations/recipes) - How recipes, declarative composition, and visitors work.
- [Lossless Semantic Trees](https://docs.openrewrite.org/concepts-and-explanations/lossless-semantic-trees) - The format-preserving, type-attributed code model that recipes operate on.
- [Recipe catalog](https://docs.openrewrite.org/recipes) - Browsable catalog of available recipes grouped by module.
- [Supported languages](https://docs.openrewrite.org/reference/supported-languages) - Languages and formats with parsers and recipes.
- [Licensing](https://docs.openrewrite.org/licensing/openrewrite-licensing) - Apache-2.0 core and Moderne Source Available License terms.
- [openrewrite/rewrite](https://github.com/openrewrite/rewrite) - Core engine repository (Apache-2.0), with links to the project's community channels.
- [Moderne MCP server](https://docs.moderne.io/user-documentation/agent-tools/mcp/overview/) - Local MCP server that gives AI coding agents recipe search and refactoring tools.
- [Moderne agent skills](https://docs.moderne.io/user-documentation/agent-tools/skills/) - Skills that teach coding agents the OpenRewrite recipe workflow.

## Footnotes

- Moderne describes the catalog as more than 3,500 recipes; the catalog page groups them by module rather than stating a running total.
- Agentic use pairs deterministic recipes with model reasoning: the agent selects a recipe by intent and delegates execution to the engine, then handles the residual changes the catalog does not cover. See [MCP](../standards/mcp.md) and [Agent Skills](../agents/skills/README.md).
- The core is Apache-2.0, but recipe modules with significant Moderne or third-party contribution may use the Moderne Source Available License; check a module's license before redistribution.
