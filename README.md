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

- [Tokens Saving](#tokens-saving)

---

## Tokens Saving

<!-- Tools/techniques focused on reducing token usage/cost in agent workflows -->

- **[rtk](https://github.com/rtk-ai/rtk)** by [rtk-ai](https://github.com/rtk-ai) — ✅ `approved`
  A single-binary Rust CLI proxy that filters and compresses verbose shell command output (git, cargo, test runners, etc.) before it reaches an AI agent's context, cutting token usage by 60-90%. Supports 15+ AI coding platforms including Claude Code, GitHub Copilot, and Cursor.
