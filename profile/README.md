# SandBase AI

**One API for LLMs, image generation, video generation, tools, and production AI agents.**

SandBase gives developers one API key and one interface for 2,000+ AI models and 2,000+ APIs, plus runtime infrastructure for sessions, tools, approvals, sandboxed execution, memory, audit trails, replay, and operational visibility.

[Website](https://www.sandbase.ai) · [API Docs](https://www.sandbase.ai/docs/getting-started/) · [Models & APIs](https://www.sandbase.ai/docs/store/) · [Blog](https://blog.sandbase.ai) · [Discord](https://discord.com/invite/P6B5Y4e8TX) · [X](https://x.com/SandbaseAI) · [LinkedIn](https://www.linkedin.com/company/sandbaseai/)

## One API for LLM, Image, and Video Generation

Use SandBase as a unified AI API instead of integrating and maintaining a separate provider for every modality:

- **LLM API:** call chat, reasoning, coding, and embedding models through a unified interface, including an OpenAI-compatible endpoint.
- **Image API:** generate and edit images with models such as Flux through a consistent job API.
- **Video API:** run video generation models such as Kling with asynchronous jobs and production-ready status handling.
- **Tools and data APIs:** add web search, scraping, social, business, finance, and other real-world capabilities with the same SandBase account.

[Get an API key](https://sandbase.ai/console/keys) · [Read the API reference](https://www.sandbase.ai/docs/api-reference/) · [Browse models and APIs](https://www.sandbase.ai/docs/store/) · [Compare unified AI API platforms](https://blog.sandbase.ai/unified-ai-api-llm-image-video-2026/)

## Connect 25 AI clients to 2,000+ models and APIs

[![GitHub stars](https://img.shields.io/github/stars/sandbaseai/cli?style=social)](https://github.com/sandbaseai/cli)
[![Latest release](https://img.shields.io/github/v/release/sandbaseai/cli)](https://github.com/sandbaseai/cli/releases/latest)
[![License](https://img.shields.io/github/license/sandbaseai/cli)](https://github.com/sandbaseai/cli/blob/main/LICENSE)

Use the open-source [SandBase CLI](https://github.com/sandbaseai/cli) to connect Codex, Claude Code, Cursor, Windsurf, Gemini CLI, OpenCode, and other AI clients to one MCP bridge. [Star the project](https://github.com/sandbaseai/cli) or [install the latest release](https://github.com/sandbaseai/cli/releases/latest).

📣 **Latest open-source updates:** [SandBase CLI v0.1.17](https://github.com/sandbaseai/cli/releases/tag/v0.1.17) connects 25 AI client targets to 2,000+ models and APIs · [DSH Plugin Store v0.1.0 Preview 5](https://github.com/sandbaseai/dsh-plugin-store/releases/tag/v0.1.0-preview.5) installs runtime-verified plugins into a local DeepSeek Harness Web profile · [SandBase Harness v0.3.4](https://github.com/sandbaseai/sandbase-harness/releases/tag/v0.3.4) is active in the [official MCP Registry](https://registry.modelcontextprotocol.io/v0.1/servers?search=io.github.sandbaseai%2Fsandbase-harness) · [SandBase Skills v0.3.4](https://github.com/sandbaseai/sandbase-skills/releases/tag/v0.3.4) ships 88 installable Skills as a native DeepSeek Harness bundle

### Connect your coding agent

SandBase CLI detects your installed clients and configures the MCP bridge for
Codex, Claude Code, Cursor, Windsurf, Gemini CLI, OpenCode, and more:

```bash
brew install sandbaseai/tap/sandbaseai-cli
sandbase connect
```

Or run the immutable release directly:

```bash
npx -y https://github.com/sandbaseai/cli/releases/download/v0.1.17/sandbaseai-cli-0.1.17.tgz connect
```

Preview all 25 supported client targets without signing in or changing files:

```bash
npx -y https://github.com/sandbaseai/cli/releases/download/v0.1.17/sandbaseai-cli-0.1.17.tgz catalog --json
```

[Source](https://github.com/sandbaseai/cli) · [Homebrew](https://github.com/sandbaseai/homebrew-tap) · [v0.1.17 release](https://github.com/sandbaseai/cli/releases/tag/v0.1.17) · [Report an issue](https://github.com/sandbaseai/cli/issues/new/choose) · [Star SandBase CLI](https://github.com/sandbaseai/cli)

Codex users can also inspect the [official SandBase Codex plugin](https://github.com/sandbaseai/sandbase-codex-plugin), which packages the same immutable-release MCP bridge with a guided Agent Skill and required security-scanner CI.

Independent discovery: [Official MCP Registry](https://registry.modelcontextprotocol.io/v0.1/servers/io.github.sandbaseai%2Fcli/versions/0.1.17) · [Chinese Independent Developer](https://github.com/1c7/chinese-independent-developer/blob/master/pages/README-Programmer-Edition.md#sandbase---github) · [MCP Registry showcase](https://github.com/modelcontextprotocol/registry/discussions/1584) · [AIMCP](https://www.aimcp.info/en/g/522d366e-114b-4d90-9f1a-552b4b3a9c86) · [VaultPlane](https://www.vaultplane.com/server/sandbase-cli) · [MCPRepository](https://mcprepository.com/sandbaseai/cli) · [Awesome Gemini CLI](https://github.com/Piebald-AI/awesome-gemini-cli#development-tools--utilities) · [Awesome AI API Proxy](https://github.com/howardpen9/awesome-ai-api-proxy#global-gateways--aggregators) · [TensorBlock MCP Index](https://tensorblock.co/mcp/servers/github-sandbaseai-cli-c4e113db) · [SkillsCat](https://skills.cat/skills/sandbaseai/cli/sandbase)

Practical walkthroughs: [Claude Code and Codex workflow](https://github.com/sandbaseai/cli/discussions/47) · [Chinese project page](https://sandbaseai.github.io/cli/zh/) · [Chinese workflow guide](https://github.com/sandbaseai/cli/discussions/48)

### Try it in DeepSeek Harness

Install all 88 Skills as a native DSH bundle directly from GitHub source:

```bash
dsh plugin --profile web add github:sandbaseai/sandbase-skills
dsh web
```

The flagship `multi-source-search` Skill works with host-provided search tools
and needs no SandBase account. Need durable managed-agent sessions as native
DSH MCP tools? See [SandBase Harness v0.3.4](https://github.com/sandbaseai/sandbase-harness/tree/v0.3.4#deepseek-harness), its
[official MCP Registry entry](https://registry.modelcontextprotocol.io/v0.1/servers?search=io.github.sandbaseai%2Fsandbase-harness),
and the [DeepSeek Harness showcase](https://github.com/deepseek-ai/deepseek-harness/discussions/1918).

[Explore Harness](https://github.com/sandbaseai/sandbase-harness#readme) ·
[DSH runtime plugin guide](https://blog.sandbase.ai/deepseek-harness-developer-preview-2026/#add-a-real-third-party-runtime-plugin) ·
[Independent self-hosting guide](https://www.ssdnodes.com/learn/self-host-sandbase-agent-runtime) ·
[Build an auditable research agent](https://blog.sandbase.ai/auditable-research-agent-evidence-ledger-sandbox-replay/) ·
[Star Harness](https://github.com/sandbaseai/sandbase-harness) ·
[Browse Skills](https://github.com/sandbaseai/sandbase-skills#readme) ·
[Star Skills](https://github.com/sandbaseai/sandbase-skills)

### Discover DSH plugins

Browse more than 4,000 tracked plugin packages from over 3,400 public repositories in a native Store inside DeepSeek Harness:

```bash
curl -fL https://github.com/sandbaseai/dsh-plugin-store/releases/download/v0.1.0-preview.5/sandbaseai-dsh-plugin-store-0.1.0-preview.5.tgz -o /tmp/sandbaseai-dsh-plugin-store-0.1.0-preview.5.tgz
dsh plugin --profile web add -w /tmp/sandbaseai-dsh-plugin-store-0.1.0-preview.5.tgz
```

Restart DSH Web, open **Settings**, and select **Store**.

[Open the project site](https://sandbaseai.github.io/dsh-plugin-store/) ·
[View source](https://github.com/sandbaseai/dsh-plugin-store) ·
[Try Preview 5](https://github.com/sandbaseai/dsh-plugin-store/releases/tag/v0.1.0-preview.5) ·
[Star DSH Plugin Store](https://github.com/sandbaseai/dsh-plugin-store)

### Operate DeepSeek Harness from evidence

When a DSH install, Session, tool call, sandbox, or plugin fails, use the
independent **DeepSeek Harness Handbook** to find the first broken boundary.
It currently provides 143 English-canonical, source-backed guides plus local
browser tools that do not upload diagnostic input.

[Run Install Doctor](https://sandbaseai.github.io/deepseek-harness-handbook/install-doctor.html) ·
[Route a failure](https://sandbaseai.github.io/deepseek-harness-handbook/diagnose.html) ·
[Browse all guides](https://github.com/sandbaseai/deepseek-harness-handbook#start-with-your-goal) ·
[Star the Handbook](https://github.com/sandbaseai/deepseek-harness-handbook)

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
| [SandBase CLI](https://github.com/sandbaseai/cli) | One-command MCP onboarding for Cursor, Claude Code, Codex, Windsurf, Gemini CLI, OpenCode, and other agents, with access to 2,000+ AI models and APIs. |
| [SandBase Docs](https://github.com/sandbaseai/sandbase-docs) | Official developer documentation for one API covering LLMs, image, video, audio, embeddings, real-world APIs, and reusable Agents. |
| [SandBase for Codex](https://github.com/sandbaseai/sandbase-codex-plugin) | Official Codex plugin packaging for the SandBase MCP bridge and guided Agent Skill, with a pinned security-scanner workflow. |
| [managed-agents](https://github.com/sandbaseai/managed-agents) | Open-source, local-first managed-agent runtime with a Console, Claude Managed Agents-style resource APIs, skills, files, credential vaults, memory stores, environments, and resumable session events. |
| [deepseek-harness-handbook](https://github.com/sandbaseai/deepseek-harness-handbook) | Independent, agent-first field guide to DeepSeek Harness with source-backed quickstarts, architecture maps, safety boundaries, runnable examples, troubleshooting, and multilingual navigation. |
| [DSH Plugin Store](https://github.com/sandbaseai/dsh-plugin-store) | Native Community and Installed experience for discovering, filtering, installing, and managing packages from more than 3,400 DeepSeek Harness plugin repositories. |
| [awesome-native-agent-platforms](https://github.com/sandbaseai/awesome-native-agent-platforms) | A curated list of infrastructure, runtimes, sandboxes, browsers, model routers, and protocols for building production AI agents. |
| [sandbase-lab-sitecheck](https://github.com/sandbaseai/sandbase-lab-sitecheck) | "Can AI Get It?", a SandBase-powered website AI personality test where an agent visits a site, scores it, writes feedback, assigns personality tags, and generates a shareable card. |
| [awesome-agent-runtime](https://github.com/sandbaseai/awesome-agent-runtime) | A 500-project landscape of agent runtimes, sandboxes, browser agents, MCP/tool protocols, memory layers, observability, and compute platforms. |
| [agent-sandbox-cookbook](https://github.com/sandbaseai/agent-sandbox-cookbook) | Examples, compatibility checks, and field notes for running AI agent tools across sandboxed runtimes. |
| [global-ai-cold-start](https://github.com/sandbaseai/global-ai-cold-start) | A public case study on turning SandBase.ai from an invisible early AI infrastructure product into a searchable, developer-facing trust surface. |

## Start Here

- Building a local-first agent runtime? Start with [SandBase Harness](https://github.com/sandbaseai/sandbase-harness).
- Adding research workflows to your agent? Install the no-account [`multi-source-search`](https://github.com/sandbaseai/sandbase-skills/tree/main/research/multi-source-search) Skill or browse all [SandBase Skills](https://github.com/sandbaseai/sandbase-skills).
- Want to connect your coding agent to tools and models? Install [SandBase CLI](https://github.com/sandbaseai/cli).
- Integrating the SandBase API? Start with the [official developer docs](https://github.com/sandbaseai/sandbase-docs) or the [hosted API guide](https://www.sandbase.ai/docs/getting-started/).
- New to agent infrastructure? Read the [SandBase blog](https://www.sandbase.ai/blog).
- Comparing native agent platforms and runtimes? Start with [Awesome Native Agent Platforms](https://github.com/sandbaseai/awesome-native-agent-platforms).
- Mapping the broader runtime ecosystem? Browse [Awesome Agent Runtime](https://github.com/sandbaseai/awesome-agent-runtime).
- Exploring local-first enterprise agent runtime? Browse [Managed Agents](https://github.com/sandbaseai/managed-agents).
- Building with DeepSeek Harness? Start with the [runtime plugin walkthrough](https://blog.sandbase.ai/deepseek-harness-developer-preview-2026/#add-a-real-third-party-runtime-plugin), then use the [DeepSeek Harness Handbook](https://github.com/sandbaseai/deepseek-harness-handbook) for operator guides, architecture, and troubleshooting.
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
