# Agentic Resource Discovery (ARD)

An open discovery-layer specification (draft, reference implementations launched June 2026) that lets AI agents find tools, skills, and other agents at runtime through semantic, natural-language search against federated, domain-anchored registries. ARD replaces the "install-first, hardcode the location, use-later" model with runtime discovery, and it sits in front of protocols such as MCP, A2A, and Agent Skills rather than replacing them: an agent uses ARD to locate a capability, then connects to it over the appropriate underlying protocol. It is developed by a cross-industry working group, with Hugging Face maintaining a reference implementation.

## Contents

- [agenticresourcediscovery.org](https://agenticresourcediscovery.org/) - Official specification site (Apache-2.0).
- [github.com/ards-project/ard-spec](https://github.com/ards-project/ard-spec) - Specification repository.
- [github.com/huggingface/hf-discover](https://github.com/huggingface/hf-discover) - Hugging Face reference implementation indexing Skills, MCP servers, and Spaces.
- [Agentic Resource Discovery launch](https://huggingface.co/blog/agentic-resource-discovery-launch) - Hugging Face launch announcement.

## Footnotes

- ARD is a multi-organization effort; Hugging Face contributes the `hf-discover` reference implementation rather than owning the specification.
- Some launch coverage describes ARD as governed under the Linux Foundation; that governance claim is not confirmed on the specification repository and should be verified before citing.
