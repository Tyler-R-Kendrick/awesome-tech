# GenPage

Netflix's end-to-end generative model for constructing the personalized homepage. GenPage reframes homepage building as autoregressive sequence prediction — treating user and request context as a "prompt" and generating the entire multi-row page as the "response" — and replaces a traditional multi-stage candidate-generation and ranking pipeline with a single transformer that optimizes the whole page at once.

## Contents

- [GenPage: Towards End-to-End Generative Homepage Construction at Netflix](https://netflixtechblog.com/genpage-towards-end-to-end-generative-homepage-construction-at-netflix-77146fba8a08) - Netflix Technology Blog article describing the model, training recipe, and production system.

## Key ideas

- **Whole-page generation.** A decoder-only transformer generates rows and their entities in layout order, capturing cross-row and cross-entity interactions that separate ranking stages miss.
- **Domain-specific tokenization.** Each row and each entity (movie, show, game) maps to a single token, giving computational efficiency and enabling constrained decoding to enforce business rules at inference time.
- **LLM-style training recipe.** Pretraining with next-token prediction on historical positive homepage impressions, followed by post-training via weighted binary classification (per-token value from entity-level rewards) or reinforcement learning (page-level optimization against a reward model).
- **Production techniques.** Semantic embedding fusion for cold-start entities, multi-cadence incremental training for model freshness, hybrid row decoding (autoregressive for the first entities, then batch scoring), and pagination that appends in-session engagement signals to the context.

## Footnotes

- Reported results include statistically significant engagement gains over a mature production baseline, roughly 20% lower serving latency, and increased recommendation diversity from RL post-training even without optimizing for diversity directly.
- A key reported insight for generative-UI builders: in this regime, enriching the prompt (what context is provided and how it is tokenized) improved results more than scaling model capacity.
- Reference architecture and case study rather than a reusable framework or SDK; the value here is the approach to whole-page generative composition.
