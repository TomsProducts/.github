# NextLayer

> **🚧 Coming Soon** — Products are under active development and rolling out shortly.

---

## Nexlayer — AI Infrastructure Platform

Eight tightly integrated products that give AI agents everything they need to operate in production. Self-hosted. Open-source. Built from the ground up for the way AI systems actually work.

---

### The Products

| | Product | What it does |
|--|---------|-------------|
| 🔐 | **[AgentVault](https://github.com/TomsProducts/AgentVault)** | Zero-trust secret store for AI agents. AES-256-GCM encryption, short-lived vault tokens, per-agent policy scoping. Every agent gets only the secrets it needs. |
| 🔀 | **[FlowMesh](https://github.com/TomsProducts/FlowMesh)** | Visual AI pipeline builder. Wire agents together with drag-and-drop, set cron/webhook triggers, get full step-by-step execution traces. |
| 👁️ | **[WatchGrid](https://github.com/TomsProducts/WatchGrid)** | AI observability platform. Every LLM call, tool use, and error captured in real time. Per-run cost tracking, alert rules, Prometheus metrics. |
| 🌐 | **[ModelRouter](https://github.com/TomsProducts/ModelRouter)** | Unified LLM gateway. Drop-in Anthropic-compatible API that routes to Claude, Gemini, or Ollama. Switch providers platform-wide with one config change. |
| 🛒 | **[AgentShop](https://github.com/TomsProducts/AgentShop)** | AI coding agent dispatch. Kanban board for specialized coding agents (Python, Java, DevOps, Frontend…) running on your own machines via Claude Code CLI. |
| 🧠 | **[BrainVault](https://github.com/TomsProducts/BrainVault)** | Personal AI knowledge base. Write notes, ask questions — get answers cited from your own content, not hallucinated. RAG over your entire history. |
| 📊 | **[PeriodAI](https://github.com/TomsProducts/PeriodAIProduct)** | Business reporting automation. Define a template, connect a data source, set a schedule — AI generates and delivers the narrative report automatically. |
| 📚 | **[WikiLLM](https://github.com/TomsProducts/WikiLLMAgentAndUI)** | Document-to-wiki engine. Drop files into a folder, get a structured cross-linked wiki out. Stays in sync as files change. |

---

### How They Connect

```
AgentVault  ←  all products read secrets from here
ModelRouter  ←  all LLM calls route through here
WatchGrid   ←  all products log events here
FlowMesh    →  orchestrates AgentShop, PeriodAI, WikiLLM, BrainVault
```

Every product is independently useful. Together they form a complete operational layer for AI agents.

---

### Docs & Resources

- 📖 [Full Documentation](https://github.com/TomsProducts/NextLayerDocumentation)
- 🌐 [Platform Website](http://192.168.68.111)
- 🗺️ [Ecosystem Map](http://192.168.68.111/interactions.html)

---

*Built with ♥
