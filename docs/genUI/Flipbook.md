# Flipbook

An experimental "visual browser" that reframes the interface itself as generative output. Instead of HTML, a DOM, and hyperlinks, every page in Flipbook is a single high-resolution image rendered in real time by a multimodal model; clicking anywhere in the image generates the next image, diving deeper into whatever was selected. It marks the far end of the generative-UI spectrum — the UI as generated pixels rather than model-composed structured components.

## Contents

- [flipbook.page](https://flipbook.page/) - The experimental visual browser (prototype, access-gated).

## How it works

- **Pixels, not markup.** Each screen is a generated image; even the text is rendered as pixels by the model, with no HTML or overlaid text layer.
- **Click-to-generate navigation.** Selecting any element — a person, an object, or a pixel-rendered word — prompts generation of a new image that explores it.
- **Grounding.** On-screen information comes from a combination of agentic web search and the model's own world knowledge.
- **Optional video mode.** An experimental mode animates transitions as continuous 1080p video via an optimized video model running on serverless GPU infrastructure.

## Footnotes

- Built by a small team with backgrounds at OpenAI, Humane, and Apple; backed by South Park Commons with inference sponsored by Modal.
- Explicitly a prototype: pages take seconds to generate, text rendering is imperfect, outputs can hallucinate, and it does not yet handle complex actions such as form-filling or persistent state.
- Tracked here as a boundary-pushing experiment in generative UI, not a framework or SDK; contrast it with catalog-constrained approaches such as OpenUI and json-render, where models compose safe, structured components.
