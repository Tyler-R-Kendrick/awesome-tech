# Agent-to-Human Protocol (A2H)

An open-source protocol specification from Twilio (announced February 2026) that gives AI agents a single, channel-agnostic, auditable surface for communicating with their human principals — for approvals, data collection, escalation, and reporting results — across SMS, voice, email, WhatsApp, and push. It defines five core intent types (INFORM, COLLECT, AUTHORIZE, ESCALATE, RESULT) and produces cryptographically signed, non-repudiable evidence linking an agent's intent to a human's consent and the resulting action. A2H is positioned as complementary to MCP (tools and context) and A2A (agent-to-agent), filling the agent-to-human gap.

## Contents

- [Introducing A2H](https://www.twilio.com/en-us/blog/products/introducing-a2h-agent-to-human-communication-protocol) - Twilio launch announcement.
- [github.com/twilio-labs/Agent2Human](https://github.com/twilio-labs/Agent2Human) - Specification, whitepaper, and OpenAPI 3.1 schema.

## Footnotes

- The repository provides MCP-compatible tool mappings (for example `human_inform()` and `human_authorize()`).
- Twilio has stated an intention to submit A2H to standards bodies such as the W3C and the OpenID Foundation; no adoption by a standards body is confirmed as of this writing.
