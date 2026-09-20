# archive-series

Archived nlink-jp projects. Every repository listed here is **read-only on
GitHub** — it accepts no commits, releases, and no pull requests. Nothing here
is maintained. The code and its documentation are kept for reference only.

Projects are grouped by the series they belonged to before they were archived.

> **Licences vary, and this umbrella licenses nothing.** It carries no LICENSE
> of its own, and a licence here would not cover the repositories it points at.
> Most projects below are MIT; `cti-graph` and `cti-primer` are Apache-2.0;
> `lite-llm` and `mail-watcher` carry no licence at all. Check the repository
> you are actually looking at.

## cybersecurity

| Project | Language | Description |
|---------|----------|-------------|
| [ai-ir](https://github.com/nlink-jp/ai-ir) | — | AI-powered incident response analysis — analyzes Slack IR conversation exports to generate summaries, activity reports, role inference, and reusable investigation tactics; superseded by the [incident-review](https://github.com/nlink-jp/incident-review) skill |
| [ai-ir2](https://github.com/nlink-jp/ai-ir2) | — | Next-generation AI-powered IR analysis — one-stop Gemini pipeline that turns a Slack IR export into a comprehensive analysis report in a single command; superseded by the [incident-review](https://github.com/nlink-jp/incident-review) skill |
| [cti-graph](https://github.com/nlink-jp/cti-graph) | — | Local-first threat intelligence attack graph analysis platform — SAGE-inspired, backed by local SQLite |
| [cti-primer](https://github.com/nlink-jp/cti-primer) | — | Generates CTI PIRs (Priority Intelligence Requirements) from business context — BEACON-inspired, runs on local LLMs or dictionary-only mode, no cloud services required |
| [ioc-collector](https://github.com/nlink-jp/ioc-collector) | — | Autonomously researches security incidents from URLs, CVE IDs, or natural language — extracts IoCs into Markdown reports and STIX 2.1 bundles; superseded by the [incident-research](https://github.com/nlink-jp/incident-research) skill (v0.2+) |
| [ir-hub](https://github.com/nlink-jp/ir-hub) | — | IR lifecycle hub — resident Slack ChatOps bot that opens a channel per case, tracks the response with ACL-gated commands, and ingests messages for postmortems and knowledge reuse (Go) |
| [ir-tracker](https://github.com/nlink-jp/ir-tracker) | — | Live IR tracker — continuous ingestion, segmented analysis, and timeline visualization for ongoing incidents via Gemini |
| [mail-triage](https://github.com/nlink-jp/mail-triage) | — | GCS-based email triage — classifies `.eml`/`.msg` files with Gemini and posts results to Slack; runs as a Cloud Run Job |
| [product-research](https://github.com/nlink-jp/product-research) | — | Researches products and services on the web — ToS, privacy, and data security analysis as structured reports; superseded by the [service-research](https://github.com/nlink-jp/service-research) skill |

## lab

| Project | Language | Description |
|---------|----------|-------------|
| [agent-skeleton](https://github.com/nlink-jp/agent-skeleton) | Python | Autonomous agent skeleton — plan-approve-execute loop, per-tool approval, 2-tier memory compression, MCP support **Archived** — no longer used or maintained |
| [agentic-web-search](https://github.com/nlink-jp/agentic-web-search) | Go | Agentic web search **FROZEN** (search API ToS concerns) |
| [log-analyzer](https://github.com/nlink-jp/log-analyzer) | Go | Log analysis tool **Archived** — no longer used or maintained |
| [magi-system](https://github.com/nlink-jp/magi-system) | Python | Multi-agent discussion system with 3 AI personas (MELCHIOR / BALTHASAR / CASPER) **Archived** — no longer used or maintained |
| [magi-system2](https://github.com/nlink-jp/magi-system2) | Python | Multi-persona AI discussion with dynamic persona generation, dual memory, and adaptive facilitation via Gemini **Archived** — no longer used or maintained |
| [mail-watcher](https://github.com/nlink-jp/mail-watcher) | Bash | Mail monitoring workflow — watches for incoming eml/msg files, analyzes with LLM, and posts Slack notifications **Archived** — no longer used or maintained |
| [mcp-skeleton](https://github.com/nlink-jp/mcp-skeleton) | Python | MCP server skeleton — raw JSON-RPC 2.0 over stdio/SSE with API key auth, for learning MCP internals **Archived** — no longer used or maintained |
| [meeting-note](https://github.com/nlink-jp/meeting-note) | Python | Meeting minutes structuring tool — audio/transcript to structured JSON via Gemini, then compile to Markdown/HTML **Archived** — superseded by the [meeting-notes](https://github.com/nlink-jp/meeting-notes) Claude Code Skill |
| [sai](https://github.com/nlink-jp/sai) | Python | Context-aware Slack bot with RAG memory and natural language command execution **Archived** — no longer used or maintained |
| [slack-personal-agent](https://github.com/nlink-jp/slack-personal-agent) | Go/React | Personal Slack knowledge agent — multi-workspace monitoring, channel-scoped RAG over DuckDB with strict 3-tier isolation, Hot/Warm/Cold memory, MITL draft responses |
| [virtual-reviewer](https://github.com/nlink-jp/virtual-reviewer) | Python | AI-powered security review system with LLM expert models — no RAG, UNIX philosophy **Archived** — superseded by the [compliance-review](https://github.com/nlink-jp/compliance-review) Claude Code Skill |
| [workflow-builder](https://github.com/nlink-jp/workflow-builder) | — | LLM-powered workflow builder — generates shell scripts from natural language using CLI tool registry **Archived** (design phase only; never implemented) |

## lite

| Project | Language | Description |
|---------|----------|-------------|
| [lite-llm](https://github.com/nlink-jp/lite-llm) | — | Lightweight CLI for OpenAI-compatible LLM APIs. Supports batch mode, structured output, streaming, and prompt-injection protection. |

## util

| Project | Language | Description |
|---------|----------|-------------|
| [agent-board](https://github.com/nlink-jp/agent-board) | Go | Machine-local shared knowledge board for concurrent AI agent sessions (CLI + hooks + MCP) — worked as built but saw almost no use; no successor |
| [csv-editor](https://github.com/nlink-jp/csv-editor) | Go + React (Wails) | CSV/TSV viewer & editor GUI — superseded by grid-edit |
| [data-agent](https://github.com/nlink-jp/data-agent) | Go + React (Wails) | Data-analysis desktop GUI — superseded by shell-agent-v2 |
| [gem-transcribe](https://github.com/nlink-jp/gem-transcribe) | Python | Audio transcription CLI on Vertex AI Gemini — superseded by gem-scribe |
| [mcp-guardian](https://github.com/nlink-jp/mcp-guardian) | Go | MCP governance proxy — bridging half superseded by mcp-bridge; the governance layer was never adopted in practice |
| [quick-translate](https://github.com/nlink-jp/quick-translate) | Swift | macOS menu-bar translation via a local LLM (OpenAI-compatible API) — superseded by instant-translate |
| [shell-agent](https://github.com/nlink-jp/shell-agent) | Go + Swift | macOS LLM chat & agent — superseded by shell-agent-v2 |

## Adding a newly archived project

1. Archive the repository on GitHub (Settings → Archive this repository).
2. Remove it from its series umbrella: `git submodule deinit -f -- <name>`
   then `git rm -f -- <name>`, and delete its catalog row from that
   umbrella's README.
3. Add it here under its original series: `git submodule add
   https://github.com/nlink-jp/<name>.git <series>/<name>`, and move its
   catalog row into the table above.

`check-org.sh` fails when an archived repository is still registered in an
active series umbrella, so step 2 is not optional.
