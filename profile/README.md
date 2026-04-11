# Veritera — The Trust Layer for AI Agents

AI agents are taking real-world actions — sending emails, moving money, accessing databases, calling APIs. But there's no independent system verifying what they do. When an agent goes rogue, you find out from your customers, not from your monitoring. **Forge** fixes this. It verifies every agent action before execution and tracks every execution with cryptographic receipts — without ever seeing your code, prompts, data, or outputs.

## How Forge Is Different

- **Content-Blind** — Forge never sees your agent's instructions, code, data, or outputs. It verifies the action type and behavioral pattern only. Every other tool in this space requires reading your prompts. Forge doesn't.
- **Trustless Verification** — Ed25519 asymmetric cryptography. The agent signs receipts with a private key only it holds. Anyone with the public key can verify independently. You don't trust Veritera — you trust math.
- **Independent Enforcement** — Policies are enforced outside the agent. The agent cannot override, bypass, or modify its own guardrails. Separation of duties, applied to AI.

## Forge SDKs

| Package | Framework | Description | Install |
|---------|-----------|-------------|---------|
| [veritera](https://github.com/VeriteraAI/forge-python) | Any Python | Core SDK — verify actions, manage policies, sign and submit receipts | `pip install veritera` |
| [forge-openai](https://github.com/VeriteraAI/forge-openai) | OpenAI Agents SDK | Drop-in `forge_protect()` wrapper + execution receipts | `pip install forge-openai` |
| [langchain-forge](https://github.com/VeriteraAI/forge-langchain) | LangChain / LangGraph | Middleware for tool verification and execution tracking | `pip install langchain-forge` |
| [crewai-forge](https://github.com/VeriteraAI/forge-crewai) | CrewAI | Tool, guardrails, LLM hooks, and execution receipts for crews | `pip install crewai-forge` |
| [llama-index-tools-forge](https://github.com/VeriteraAI/forge-llamaindex) | LlamaIndex | ToolSpec, event handlers, and execution receipts | `pip install llama-index-tools-forge` |
| [forge-blog](https://github.com/VeriteraAI/forge-blog) | — | Technical articles on AI agent security | — |

## Links

- [veritera.ai](https://veritera.ai) — Product, dashboard, and API keys
- [Documentation](https://veritera.ai/docs) — Full API reference and guides
- [Blog](https://github.com/VeriteraAI/forge-blog) — Articles on AI agent security and trust verification

---

MIT Licensed. Built by [Veritera AI](https://veritera.ai).
