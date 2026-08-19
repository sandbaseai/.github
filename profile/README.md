# SandBase AI

**The safe runtime layer for enterprise AI agents.**

SandBase helps teams move agents from demos to production with runtime infrastructure for sessions, tools, approvals, sandboxed execution, memory, audit trails, replay, and operational visibility.

[Website](https://www.sandbase.ai) · [Docs](https://www.sandbase.ai/docs) · [Blog](https://www.sandbase.ai/blog) · [Discord](https://discord.com/invite/P6B5Y4e8TX) · [X](https://x.com/SandbaseAI) · [LinkedIn](https://www.linkedin.com/company/sandbaseai/)

📣 **Latest open-source update:** [One-command access to 2,000+ AI models for coding agents](https://github.com/sandbaseai/.github/discussions/9) · [Read the 25-client MCP setup guide](https://blog.sandbase.ai/sandbase-cli-mcp-bridge-25-ai-clients/)

### Connect your coding agent

SandBase CLI detects your installed clients and configures the MCP bridge for
Codex, Claude Code, Cursor, Windsurf, Gemini CLI, OpenCode, and more:

```bash
npx -y @sandbaseai/cli connect
```

Preview all 25 supported client targets without signing in or changing files:

```bash
npx -y https://github.com/sandbaseai/cli/releases/download/v0.1.17/sandbaseai-cli-0.1.17.tgz catalog --json
```

[Source](https://github.com/sandbaseai/cli) · [v0.1.17 release](https://github.com/sandbaseai/cli/releases/tag/v0.1.17) · [Report an issue](https://github.com/sandbaseai/cli/issues/new/choose) · [Star SandBase CLI](https://github.com/sandbaseai/cli)

### Try it in DeepSeek Harness

Add the portable, no-account research Skill to any DSH project directly from
GitHub source:

```bash
npx --yes github:sandbaseai/sandbase-skills add multi-source-search
dsh web
```

Need durable managed-agent sessions as native DSH MCP tools? See the
[official DeepSeek Harness showcase](https://github.com/deepseek-ai/deepseek-harness/discussions/1918)
and the [verified v0.3.2 integration guide](https://github.com/sandbaseai/sandbase-harness/tree/v0.3.2/examples/deepseek-harness).

## Why SandBase

Modern agents are no longer just chat interfaces. They call tools, run code, inspect files, browse the web, trigger workflows, and act on behalf of users.

That creates a new infrastructure problem:

- where does generated code run?
- which tools can the agent call?
- who is the agent acting for?
- what happens before a sensitive action runs?
- how do teams observe, replay, and debug agent behavior?

SandBase is built around those runtime questions. The open-source path starts with local-first managed agents; the hosted SandBase platform adds managed sandboxes, team controls, observability, connectors, and production support.

## What We Build

| Area | Focus |
| --- | --- |
| Agent runtime | Sessions, event logs, replay, memory, and resumable agent execution |
| Tool governance | MCP/tools, permissions, approval patterns, and action policies |
| Sandboxed execution | Safer code, shell, file, browser, and workspace operations |
| Multi-executor support | Runtime patterns that can work across Claude, OpenAI, local models, and custom executors |
| Observability | Logs, audit trails, status, and operational surfaces for agent runs |
| Open resources | Ecosystem maps, cookbooks, labs, and growth playbooks for builders |

## Featured Projects

| Project | What it is for |
| --- | --- |
| [SandBase Harness](https://github.com/sandbaseai/sandbase-harness) | Local-first TypeScript agent runtime with sandboxed execution, MCP integration, approvals, event streams, replay, DeepSeek V4 support, and a containerized MCP bridge. |
| [SandBase Skills](https://github.com/sandbaseai/sandbase-skills) | 88 installable Agent Skills across Codex, Claude Code, Cursor, and Gemini CLI; the flagship multi-source research workflow runs with host search tools and no SandBase account. |
| [SandBase CLI](https://github.com/sandbaseai/cli) | One-command MCP onboarding for Cursor, Claude Code, Codex, Windsurf, Gemini CLI, OpenCode, and other agents, with access to 2,000+ AI models. |
| [managed-agents](https://github.com/sandbaseai/managed-agents) | Open-source, local-first managed-agent runtime with a Console, Claude Managed Agents-style resource APIs, skills, files, credential vaults, memory stores, environments, and resumable session events. |
| [deepseek-harness-handbook](https://github.com/sandbaseai/deepseek-harness-handbook) | Independent, agent-first field guide to DeepSeek Harness with source-backed quickstarts, architecture maps, safety boundaries, runnable examples, troubleshooting, and multilingual navigation. |
| [awesome-native-agent-platforms](https://github.com/sandbaseai/awesome-native-agent-platforms) | A curated list of infrastructure, runtimes, sandboxes, browsers, model routers, and protocols for building production AI agents. |
| [sandbase-lab-sitecheck](https://github.com/sandbaseai/sandbase-lab-sitecheck) | "Can AI Get It?", a SandBase-powered website AI personality test where an agent visits a site, scores it, writes feedback, assigns personality tags, and generates a shareable card. |
| [awesome-agent-runtime](https://github.com/sandbaseai/awesome-agent-runtime) | A 500-project landscape of agent runtimes, sandboxes, browser agents, MCP/tool protocols, memory layers, observability, and compute platforms. |
| [agent-sandbox-cookbook](https://github.com/sandbaseai/agent-sandbox-cookbook) | Examples, compatibility checks, and field notes for running AI agent tools across sandboxed runtimes. |
| [global-ai-cold-start](https://github.com/sandbaseai/global-ai-cold-start) | A public case study on turning SandBase.ai from an invisible early AI infrastructure product into a searchable, developer-facing trust surface. |

## Start Here

- Building a local-first agent runtime? Start with [SandBase Harness](https://github.com/sandbaseai/sandbase-harness).
- Adding research workflows to your agent? Install the no-account [`multi-source-search`](https://github.com/sandbaseai/sandbase-skills/tree/main/research/multi-source-search) Skill or browse all [SandBase Skills](https://github.com/sandbaseai/sandbase-skills).
- Want to connect your coding agent to tools and models? Install [SandBase CLI](https://github.com/sandbaseai/cli).
- New to agent infrastructure? Read the [SandBase blog](https://www.sandbase.ai/blog).
- Comparing native agent platforms and runtimes? Start with [Awesome Native Agent Platforms](https://github.com/sandbaseai/awesome-native-agent-platforms).
- Mapping the broader runtime ecosystem? Browse [Awesome Agent Runtime](https://github.com/sandbaseai/awesome-agent-runtime).
- Exploring local-first enterprise agent runtime? Browse [Managed Agents](https://github.com/sandbaseai/managed-agents).
- Building with DeepSeek Harness? Use the [DeepSeek Harness Handbook](https://github.com/sandbaseai/deepseek-harness-handbook) for operator guides, architecture, and troubleshooting.
- Building agents that run code or call tools? Read the [Agent Sandbox Cookbook](https://github.com/sandbaseai/agent-sandbox-cookbook).
- Want to see an agent judge a website? Try [SandBase Lab Sitecheck](https://github.com/sandbaseai/sandbase-lab-sitecheck).
- Following SandBase updates? Join [Discord](https://discord.com/invite/P6B5Y4e8TX) or follow [@SandbaseAI](https://x.com/SandbaseAI).

## Builder Topics

We care about infrastructure that helps agents act safely and reliably:

- agent runtime and execution boundaries
- MCP servers, tool protocols, and action schemas
- sandboxed compute for code, shell, browser, and file operations
- model gateways and multi-model routing
- evals, tracing, replay, and observability
- authorization, approvals, and pre-action policy checks
- long-running workflows and distributed execution for agents

If you are building in this direction, we would love to learn from you.
