# 🧰 Skills, Agents & Tools for AI-Assisted Dev

Personal curated list — skills, agents, frameworks, MCP servers and tools — useful for software development work with AI agents (Claude Code and similar).

Inspired by [awesome-claude-code](https://github.com/hesreallyhim/awesome-claude-code).

## How it works

Each resource listed below has a status label:

| Label | Meaning |
|---|---|
| 🧪 `pending test` | Found/added, not yet tested |
| ✅ `approved` | Tested and approved for use |

Resources that were tested and **rejected** don't stay here — they move to [`REJECTED.md`](./REJECTED.md), along with the reason for rejection, so they aren't re-evaluated pointlessly in the future.

See [`CLAUDE.md`](./CLAUDE.md) for the workflow on how entries are added/promoted/rejected, and [`templates/entry.md`](./templates/entry.md) for the entry template.

---

## Table of Contents

- [Design & UI/UX](#design--uiux)
- [Memory & Context](#memory--context)
- [Skills](#skills)
- [Tokens Saving](#tokens-saving)

---

## Design & UI/UX

<!-- Tools/techniques focused on design and UI/UX work in agent workflows -->

_No entries yet._

---

## Memory & Context

<!-- Tools/techniques focused on giving agents persistent memory or structured context -->

- **[claude-mem](https://github.com/thedotmack/claude-mem)** by [thedotmack](https://github.com/thedotmack) — 🧪 `pending test`
  A persistent memory system that captures session activity, compresses it with AI, and re-injects relevant context into future sessions, giving agents continuity of knowledge across disconnected sessions.
- **[CodeGraph](https://github.com/colbymchenry/codegraph)** by [colbymchenry](https://github.com/colbymchenry) — 🧪 `pending test`
  A local, pre-indexed code knowledge graph that gives coding agents symbol/call/dependency context in a single query instead of repeated grep/file reads, reporting a 60% cost reduction and 89% fewer tool calls in benchmarks.
- **[Graphify](https://github.com/Graphify-Labs/graphify)** by [Graphify-Labs](https://github.com/Graphify-Labs) — 🧪 `pending test`
  Builds a queryable knowledge graph of a codebase (plus docs, PDFs, configs) via local AST parsing instead of vector embeddings, letting agents query project structure instead of grepping through files.

---

## Skills

<!-- Reusable Claude Code / agent skills and skill collections -->

- **[Skills](https://github.com/mattpocock/skills)** by [mattpocock](https://github.com/mattpocock) — 🧪 `pending test`
  A collection of reusable AI agent skills addressing common failure modes in AI-assisted development, including alignment checks, test-driven development, code review, and domain modeling.
- **[Superpowers](https://github.com/obra/superpowers)** by [obra](https://github.com/obra) — 🧪 `pending test`
  A composable skills framework that gives coding agents a structured software development methodology, covering design refinement, test-driven development, and subagent-based implementation workflows.

---

## Tokens Saving

<!-- Tools/techniques focused on reducing token usage/cost in agent workflows -->

- **[caveman](https://github.com/JuliusBrussee/caveman)** by [JuliusBrussee](https://github.com/JuliusBrussee) — 🧪 `pending test`
  A skill/plugin for Claude Code, Gemini, Cursor and 30+ other agents that compresses agent output into terse fragments, cutting output tokens by roughly 65% without losing technical accuracy.
- **[headroom](https://github.com/headroomlabs-ai/headroom)** by [headroomlabs-ai](https://github.com/headroomlabs-ai) — 🧪 `pending test`
  A content-aware compression tool for tool outputs, logs, files, and RAG chunks, usable as a local proxy, library, or MCP server, claiming 60-95% fewer tokens for JSON data and 15-20% for coding agents.
- **[ponytail](https://github.com/DietrichGebert/ponytail)** by [DietrichGebert](https://github.com/DietrichGebert) — 🧪 `pending test`
  An agent plugin that enforces minimal-code practices via a decision ladder (reuse, standard libraries, native features) before writing new code, reporting ~54% less code and ~20% lower cost in benchmarks.
- **[rtk](https://github.com/rtk-ai/rtk)** by [rtk-ai](https://github.com/rtk-ai) — ✅ `approved`
  A single-binary Rust CLI proxy that filters and compresses verbose shell command output (git, cargo, test runners, etc.) before it reaches an AI agent's context, cutting token usage by 60-90%. Supports 15+ AI coding platforms including Claude Code, GitHub Copilot, and Cursor.
