# Agent Payments Protocol (AP2)

An open protocol from Google (announced September 2025) for securely initiating and completing agent-led payments across platforms and payment methods. AP2 provides a payment-agnostic framework spanning cards, stablecoins, and real-time bank transfers, and it addresses authorization, authenticity, and accountability for purchases made by AI agents by representing every purchase as three cryptographically signed mandates: an Intent Mandate, a Cart Mandate, and a Payment Mandate. It is built as an extension of the Agent2Agent (A2A) protocol and is designed to work alongside MCP, and it was developed with 60+ payments and technology partners.

## Contents

- [Announcing Agent Payments Protocol (AP2)](https://cloud.google.com/blog/products/ai-machine-learning/announcing-agents-to-payments-ap2-protocol) - Google Cloud launch announcement.
- [github.com/google-agentic-commerce/AP2](https://github.com/google-agentic-commerce/AP2) - Specification and reference implementations.
- [github.com/google-a2a/a2a-x402](https://github.com/google-a2a/a2a-x402) - A2A x402 extension for agent-based crypto payments.

## Footnotes

- AP2 handles the payment and authorization layer; Google's broader commerce/checkout layer is the [Universal Commerce Protocol (UCP)](./ucp.md).
- The A2A x402 extension was launched with partners including Coinbase, the Ethereum Foundation, and MetaMask; see also the repository's [x402 Payment Protocol](./x402.md) entry.
