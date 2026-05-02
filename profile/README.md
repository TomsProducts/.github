<div align="center">

<img src="./logo.svg" alt="Janorix" width="380" />

<br/><br/>

### The Gateway Layer for AI Agents

**10 tightly integrated products that give AI agents everything they need to operate in production.**
Self-hosted · Open-source · Named for Janus, the Roman god of gateways and beginnings.

[![Docs](https://img.shields.io/badge/docs-Documentation-blue?style=flat-square)](https://github.com/TomsProducts/NextLayerDocumentation)
[![Integrations](https://img.shields.io/badge/integrations-MCP%20%7C%20Claude%20%7C%20Copilot-purple?style=flat-square)](https://github.com/TomsProducts/Integrations)
[![Bootstrap](https://img.shields.io/badge/quickstart-bootstrap.sh-green?style=flat-square)](https://github.com/TomsProducts/Integrations/blob/main/bootstrap.sh)

</div>

---

## Platform Overview

Janorix is a complete operational layer for AI agents — named for **Janus**, the Roman god of gateways, beginnings, and transitions. Like its namesake, Janorix stands at the threshold between human intent and AI execution, routing every request, securing every secret, and remembering every lesson.

---

## Products

### 🔐 Identity & Security

| Product | Description |
|---------|-------------|
| **[AI Identity Server](https://github.com/TomsProducts/AIIdenityServer)** | Central SSO and authentication for all Janorix products. JWT-based, supports all services via a unified login. |
| **[AgentVault](https://github.com/TomsProducts/AgentVault)** | Zero-trust secret store for AI agents. AES-256-GCM encryption, short-lived vault tokens, per-agent policy scoping. Every agent gets only the secrets it needs — nothing more. |

### 🤖 Agent Intelligence

| Product | Description |
|---------|-------------|
| **[AgentBrain](https://github.com/TomsProducts/AgentBrain)** | Persistent memory system for AI agents. Three-layer architecture: working memory (24h), episodic memory (90d), and long-term lessons extracted by a nightly dream cycle. |
| **[BrainVault](https://github.com/TomsProducts/BrainVault)** | Personal AI knowledge base. Write notes, ask questions — get answers cited from your own content. RAG over your entire note history, not hallucinated responses. |

### ⚙️ Orchestration & Routing

| Product | Description |
|---------|-------------|
| **[FlowMesh](https://github.com/TomsProducts/FlowMesh)** | Visual AI pipeline builder. Wire agents together with drag-and-drop, set cron and webhook triggers, get full step-by-step execution traces. |
| **[ModelRouter](https://github.com/TomsProducts/ModelRouter)** | Unified LLM gateway. Drop-in Anthropic-compatible API that routes to Claude, Gemini, or Ollama. Switch providers platform-wide with a single config change. |
| **[AgentShop](https://github.com/TomsProducts/AgentShop)** | AI coding agent dispatch. Kanban board for specialized agents (Python, Java, DevOps, React…) running on your own machines via Claude Code CLI. |

### 📊 Observability & Knowledge

| Product | Description |
|---------|-------------|
| **[WatchGrid](https://github.com/TomsProducts/WatchGrid)** | AI observability platform. Every LLM call, tool use, and error captured in real time. Per-run cost tracking, alert rules, and Prometheus metrics export. |
| **[PeriodAI](https://github.com/TomsProducts/PeriodAIProduct)** | Business reporting automation. Define a template, connect a data source, set a schedule — AI generates and delivers the narrative report automatically. |
| **[WikiLLM](https://github.com/TomsProducts/WikiLLMAgentAndUI)** | Document-to-wiki engine. Drop files into a folder, get a structured, cross-linked wiki out. Stays in sync as files change. |

---

## How It All Connects

```
┌─────────────────────────────────────────────────────────────┐
│                     AI Identity Server                       │
│              (SSO · JWT · all products auth here)            │
└──────────────────────────┬──────────────────────────────────┘
                           │
          ┌────────────────┼────────────────┐
          ▼                ▼                ▼
     AgentVault       ModelRouter       WatchGrid
    (secrets for     (all LLM calls    (all events
     all agents)      route here)       logged here)
          │                │                │
          └────────────────┼────────────────┘
                           │
          ┌────────────────┼────────────────┐
          ▼                ▼                ▼
      FlowMesh         AgentBrain        BrainVault
    (pipelines)        (memory)          (notes/RAG)
          │
    ┌─────┴──────┐
    ▼            ▼
AgentShop    PeriodAI / WikiLLM
(coding       (reporting +
 agents)       knowledge)
```

---

## Quick Start

Clone the entire platform workspace on any machine in one command:

```bash
git clone https://github.com/TomsProducts/Integrations.git integrations
bash integrations/bootstrap.sh ~/janorix
```

This bootstraps the full workspace:
```
~/janorix/
├── products/        # 10 independent product repos
├── integrations/    # MCP server, Claude + Copilot integration
├── infrastructure/  # Docker Compose files for every product
├── docs/            # Platform documentation
├── website/         # Product pages
└── memory/          # Agent lessons and knowledge exports
```

---

## Integrations

Janorix ships with first-class support for AI coding assistants:

- **Claude Code** — full `CLAUDE.md` agent instructions across all products
- **GitHub Copilot CLI** — MCP server exposes all 9 products as native tools
- **MCP Protocol** — `janorix_mcp.py` gives any MCP-compatible client access to AgentBrain, BrainVault, AgentVault, WatchGrid, FlowMesh, ModelRouter, AgentShop, PeriodAI, and WikiLLM

See [`TomsProducts/Integrations`](https://github.com/TomsProducts/Integrations) for setup guides.

---

## Resources

| | Link |
|--|------|
| 📖 | [Platform Documentation](https://github.com/TomsProducts/JanorixDocumentation) |
| 🚀 | [Bootstrap Script](https://github.com/TomsProducts/Integrations/blob/main/bootstrap.sh) |
| 🧩 | [MCP Server](https://github.com/TomsProducts/Integrations/blob/main/mcp-server/janorix_mcp.py) |
| 🏗️ | [Infrastructure / Docker Compose](https://github.com/TomsProducts/infastructure) |
| 🧠 | [Agent Memory Store](https://github.com/TomsProducts/AIMemory-AgentsMemory) |
| 🌐 | [Product Website](https://github.com/TomsProducts/WebSite) |

---

<div align="center">

*Built with ♥ by the Janorix team*

</div>
