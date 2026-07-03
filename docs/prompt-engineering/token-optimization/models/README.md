# Token Optimization Models

Model- and ML-based methods that compress prompts or context into fewer tokens while preserving downstream task performance for large language models.

## Contents

- [LLMLingua-2](https://github.com/microsoft/LLMLingua) - Microsoft's task-agnostic prompt compression model that frames compression as token classification distilled from GPT-4, shipped alongside LLMLingua and LongLLMLingua.
- [Selective Context](https://github.com/liyucheng09/Selective_Context) - Prunes low-information lexical units using a base language model's self-information scores.
- [Gist Tokens](https://github.com/jayelm/gisting) - Compresses prompts into a few reusable "gist" tokens via modified attention masks during instruction tuning.
- [ICAE](https://github.com/getao/icae) - In-Context Autoencoder that compresses long context into a small number of memory slots decodable by a frozen target LLM.
- [500xCompressor](https://github.com/ZongqianLi/500xCompressor) - Compresses up to 500 natural-language tokens into a single token, supporting ratios from roughly 6x to 480x.
- Ornith - Token/prompt-compression resource to verify and describe before linking.

## Footnotes

- LLMLingua-2 paper: [arXiv 2403.12968](https://arxiv.org/abs/2403.12968) (ACL 2024 Findings).
- "Sakana Fugu" was requested for this folder but is a multi-agent orchestrator ([sakana.ai/fugu](https://sakana.ai/fugu/)), not a prompt-compression method, so it is not listed here; it fits agent tooling rather than token compression.
- "Ornith" could not be verified as a compression tool; it is listed unlinked pending a canonical source, per the repository convention for unverified entries.
