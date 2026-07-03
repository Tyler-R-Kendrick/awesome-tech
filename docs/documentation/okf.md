# Open Knowledge Format (OKF)

An open specification from Google Cloud (v0.1, announced June 2026) for representing the metadata, context, and curated knowledge that AI systems need in a vendor-neutral, agent- and human-friendly form. OKF stores knowledge as a directory of Markdown files with YAML frontmatter — one concept per file (a table, dataset, API, metric, or runbook) — alongside an `index.md` that enumerates contents for progressive disclosure and a `log.md` that records dated changes. It aims to let different tools read and write the same knowledge base without a translation layer or a required SDK.

OKF is one of the required knowledge formats this repository tracks; see [Standards → Required Standards](../standards/README.md#required-standards).

## Contents

- [How the Open Knowledge Format can improve data sharing](https://cloud.google.com/blog/products/data-analytics/how-the-open-knowledge-format-can-improve-data-sharing) - Google Cloud launch announcement.
- [GoogleCloudPlatform/knowledge-catalog (okf)](https://github.com/GoogleCloudPlatform/knowledge-catalog/tree/main/okf) - Specification, sample bundles, and a reference agent.
- [GoogleCloudPlatform/knowledge-catalog](https://github.com/GoogleCloudPlatform/knowledge-catalog) - Parent repository (Apache-2.0).

## Footnotes

- OKF formalizes the "LLM wiki" pattern (as popularized by Andrej Karpathy) into a portable, versioned specification.
- OKF is a knowledge format; for a tool that generates repository docs, see [OpenWiki](./openwiki.md).
