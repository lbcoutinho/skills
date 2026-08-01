# 🧰 Skills, Agents & Tools for AI-Assisted Dev

Personal curated list — skills, agents, frameworks, MCP servers and tools — useful for software development work with AI agents (Claude Code and similar).

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

- [To Study](#to-study)
- [Agents](#agents)
- [Catalogs](#catalogs)
- [Design & UI/UX](#design--uiux)
- [Documentation](#documentation)
- [Infra](#infra)
- [LLM Tone](#llm-tone)
- [MCP](#mcp)
- [Memory & Context](#memory--context)
- [Security](#security)
- [Skills](#skills)
- [Tokens Saving](#tokens-saving)
- [Video](#video)
- [Workflows](#workflows)

---

## To Study

<!-- Guides/resources to read and evaluate before categorizing further -->

- **[claude-code-best-practice](https://github.com/shanraisshan/claude-code-best-practice)** by [shanraisshan](https://github.com/shanraisshan) — 🧪 `pending test`
  A guide documenting Claude Code's feature set (subagents, commands, skills, hooks, MCP, plugins) and workflow patterns, plus curated links to other skill/agent libraries.

---

## Agents

<!-- Specialized agent/subagent definitions and agent packs -->

- **[code-simplifier](https://github.com/anthropics/claude-plugins-official/tree/main/plugins/code-simplifier)** by [anthropics](https://github.com/anthropics) — 🧪 `pending test`
  An official plugin/agent that simplifies and refines recently modified code for clarity, consistency, and maintainability while preserving functionality.

---

## Catalogs

<!-- Directories/lists of other Claude Code plugins, skills and tools -->

- **[awesome-claude-plugins](https://github.com/rdmgator12/awesome-claude-plugins)** by [rdmgator12](https://github.com/rdmgator12) — 🧪 `pending test`
  A community-maintained, unofficial directory cataloging plugins (skills, MCP servers, slash commands, sub-agents, hooks) from Anthropic's official Claude Plugins catalog.

---

## Design & UI/UX

<!-- Tools/techniques focused on design and UI/UX work in agent workflows -->

### MCP

- **[Magic MCP](https://github.com/21st-dev/magic-mcp)** by [21st-dev](https://github.com/21st-dev) — 🧪 `pending test`
  An MCP server for searching a library of React/Tailwind components and generating UI from natural-language prompts inside editors like Cursor and Claude Code.
- **[shadcn-ui-mcp-server](https://github.com/Jpisnice/shadcn-ui-mcp-server)** by [Jpisnice](https://github.com/Jpisnice) — 🧪 `pending test`
  An MCP server that gives AI coding assistants structured access to shadcn/ui component source and demos across React, Svelte, Vue, and React Native.

### Skills

- **[brandkit](https://github.com/Leonxlnx/taste-skill/tree/main/skills/brandkit)** by [Leonxlnx](https://github.com/Leonxlnx) — 🧪 `pending test`
  A skill (part of taste-skill) that generates brand-identity visual systems: logo concepts, color systems, typography, and mockup presentation boards.
- **[composition-patterns](https://github.com/vercel-labs/agent-skills/tree/main/skills/composition-patterns)** by [vercel-labs](https://github.com/vercel-labs) — 🧪 `pending test`
  A skill documenting React composition patterns for component architecture and state management, aimed at replacing boolean-prop-heavy components with more maintainable, composable ones.
- **[frontend-design](https://github.com/anthropics/skills/tree/main/skills/frontend-design)** by [anthropics](https://github.com/anthropics) — ✅ `approved`
  A Claude skill with guidance for producing visually distinctive web interfaces, grounding typography/color/layout choices in the subject matter instead of generic templates.
- **[gsap-skills](https://github.com/greensock/gsap-skills)** by [greensock](https://github.com/greensock) — 🧪 `pending test`
  Official GSAP skills teaching agents how to correctly use the GSAP animation API, timelines, ScrollTrigger, plugins, and framework integrations (React/Vue/Svelte).
- **[image-to-code-skill](https://github.com/Leonxlnx/taste-skill/tree/main/skills/image-to-code-skill)** by [Leonxlnx](https://github.com/Leonxlnx) — 🧪 `pending test`
  A skill (part of taste-skill) that generates reference website-design images, analyzes their layout/typography/spacing, then implements frontend code matching those designs.
- **[impeccable](https://github.com/pbakaus/impeccable)** by [pbakaus](https://github.com/pbakaus) — ✅ `approved`
  A design-language framework with commands and detector rules aimed at preventing common AI-generated design anti-patterns (overused fonts, gradient clichés), with a setup flow and live browser iteration.
- **[react-best-practices](https://github.com/vercel-labs/agent-skills/tree/main/skills/react-best-practices)** by [vercel-labs](https://github.com/vercel-labs) — 🧪 `pending test`
  A skill compiling React performance and development best practices into agent-readable guidance, covering areas from avoiding request waterfalls to advanced patterns.
- **[react-view-transitions](https://github.com/vercel-labs/agent-skills/tree/main/skills/react-view-transitions)** by [vercel-labs](https://github.com/vercel-labs) — 🧪 `pending test`
  A skill with components, patterns, and CSS recipes for implementing the View Transition API in React/Next.js apps, covering page transitions and shared-element animations.
- **[refero_skill](https://github.com/referodesign/refero_skill)** by [referodesign](https://github.com/referodesign) — 🧪 `pending test`
  A skill that requires design research (real app screens and user flows from products like Stripe, Linear, and Notion) before implementation, producing a pattern reference and craft guidance (typography, spacing, motion) instead of freehand UI generation.
- **[skills](https://github.com/emilkowalski/skills)** by [emilkowalski](https://github.com/emilkowalski) — 🧪 `pending test`
  A collection of skills for design engineers covering animation and UI design principles (easing, motion vocabulary, review checklists) aimed at common design/animation mistakes agents make.
- **[taste-skill](https://github.com/Leonxlnx/taste-skill)** by [Leonxlnx](https://github.com/Leonxlnx) — 🧪 `pending test`
  A set of portable "anti-generic-UI" skills (layout/typography/motion/spacing rules), installable via an `npx skills add` CLI, for Claude Code, Cursor, Codex and similar agents. Also ships the brandkit and image-to-code-skill sub-skills listed separately above.
- **[ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill)** by [nextlevelbuilder](https://github.com/nextlevelbuilder) — 🧪 `pending test`
  A design-system generator skill offering a rules engine with UI styles, color palettes, typography pairings, and stack-specific recommendations for building interfaces.
- **[web-design-guidelines](https://github.com/vercel-labs/agent-skills/tree/main/skills/web-design-guidelines)** by [vercel-labs](https://github.com/vercel-labs) — 🧪 `pending test`
  A skill that fetches the latest Web Interface Guidelines from GitHub and audits given UI code against them for accessibility, design, and UX issues.

---

## Documentation

<!-- Tools/skills for managing project documentation and memory files -->

- **[claude-md-management](https://github.com/anthropics/claude-plugins-official/tree/main/plugins/claude-md-management)** by [anthropics](https://github.com/anthropics) — 🧪 `pending test`
  An official plugin with tools to audit CLAUDE.md quality, capture session learnings, and keep project memory files current.

---

## Infra

<!-- Tools/techniques focused on infrastructure, deployment and environment setup in agent workflows -->

- **[deploy-to-vercel](https://github.com/vercel-labs/agent-skills/tree/main/skills/deploy-to-vercel)** by [vercel-labs](https://github.com/vercel-labs) — 🧪 `pending test`
  A skill that automates deploying a project to Vercel by detecting project state and choosing between git integration, CLI commands, or an auth-free fallback.

---

## LLM Tone

<!-- Tools/skills that shape an agent's response style/tone -->

- **[i-have-adhd](https://github.com/ayghri/i-have-adhd)** by [ayghri](https://github.com/ayghri) — 🧪 `pending test`
  A skill that changes agent response style to be more direct: leads with actionable steps, numbers instructions, and caps list length to reduce verbose preambles.

---

## MCP

<!-- MCP servers not specific to another category -->

- **[chrome-devtools-mcp](https://github.com/ChromeDevTools/chrome-devtools-mcp)** by [ChromeDevTools](https://github.com/ChromeDevTools) — 🧪 `pending test`
  An MCP server that lets AI coding agents control and inspect a live Chrome instance via Puppeteer, for automation, debugging, performance tracing, network inspection, and screenshots.
- **[Context7](https://github.com/upstash/context7)** by [upstash](https://github.com/upstash) — 🧪 `pending test`
  An MCP server that fetches up-to-date, version-specific documentation and code examples straight from source, injecting them into the prompt to avoid outdated or hallucinated API usage.
- **[Playwright](https://github.com/anthropics/claude-plugins-official/tree/main/external_plugins/playwright)** by [anthropics](https://github.com/anthropics) — 🧪 `pending test`
  An official plugin wrapping Microsoft's Playwright MCP server for browser automation and end-to-end testing: navigating pages, filling forms, clicking elements, taking screenshots, and running automated browser tests.
- **[Supabase](https://github.com/supabase-community/supabase-plugin)** by [supabase-community](https://github.com/supabase-community) — 🧪 `pending test`
  An MCP integration plugin for Supabase covering database operations, authentication, storage, and real-time subscriptions, letting agents run SQL and manage Supabase projects directly.

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

## Security

<!-- Security review, sandboxing and permissions tools for agent workflows -->

- **[security-guidance](https://github.com/anthropics/claude-plugins-official/tree/main/plugins/security-guidance)** by [anthropics](https://github.com/anthropics) — 🧪 `pending test`
  An official plugin for security review of Claude-generated code: pattern-based edit warnings, LLM-powered diff review on stop, and an agentic commit reviewer catching injection, XSS, SSRF, hardcoded secrets, and other vulnerability classes.

---

## Skills

<!-- Reusable Claude Code / agent skills and skill collections -->

- **[Anthropic Skills](https://github.com/anthropics/skills)** by [anthropics](https://github.com/anthropics) — 🧪 `pending test`
  A public repository of example Claude skills (instructions, scripts, and resources Claude loads for specific tasks), serving as a reference implementation for building custom skills.
- **[code-review](https://github.com/anthropics/claude-plugins-official/tree/main/plugins/code-review)** by [anthropics](https://github.com/anthropics) — 🧪 `pending test`
  An official plugin for automated pull-request code review using multiple specialized agents with confidence-based scoring to filter false positives.
- **[ralph-loop](https://github.com/anthropics/claude-plugins-official/tree/main/plugins/ralph-loop)** by [anthropics](https://github.com/anthropics) — 🧪 `pending test`
  An official plugin implementing the "Ralph Wiggum" technique: an interactive loop where Claude repeatedly works on the same task, seeing its own prior output, until completion.
- **[skill-creator](https://github.com/anthropics/claude-plugins-official/tree/main/plugins/skill-creator)** by [anthropics](https://github.com/anthropics) — 🧪 `pending test`
  An official plugin/skill for creating new skills, improving existing ones, running evals, and benchmarking skill performance.

---

## Tokens Saving

<!-- Tools/techniques focused on reducing token usage/cost in agent workflows -->

- **[caveman](https://github.com/JuliusBrussee/caveman)** by [JuliusBrussee](https://github.com/JuliusBrussee) — ✅ `approved`
  A skill/plugin for Claude Code, Gemini, Cursor and 30+ other agents that compresses agent output into terse fragments, cutting output tokens by roughly 65% without losing technical accuracy.
- **[headroom](https://github.com/headroomlabs-ai/headroom)** by [headroomlabs-ai](https://github.com/headroomlabs-ai) — 🧪 `pending test`
  A content-aware compression tool for tool outputs, logs, files, and RAG chunks, usable as a local proxy, library, or MCP server, claiming 60-95% fewer tokens for JSON data and 15-20% for coding agents.
- **[ponytail](https://github.com/DietrichGebert/ponytail)** by [DietrichGebert](https://github.com/DietrichGebert) — ✅ `approved`
  An agent plugin that enforces minimal-code practices via a decision ladder (reuse, standard libraries, native features) before writing new code, reporting ~54% less code and ~20% lower cost in benchmarks.
- **[rtk](https://github.com/rtk-ai/rtk)** by [rtk-ai](https://github.com/rtk-ai) — ✅ `approved`
  A single-binary Rust CLI proxy that filters and compresses verbose shell command output (git, cargo, test runners, etc.) before it reaches an AI agent's context, cutting token usage by 60-90%. Supports 15+ AI coding platforms including Claude Code, GitHub Copilot, and Cursor.

---

## Video

<!-- Tools/techniques for agent-driven video generation and rendering -->

- **[HyperFrames](https://github.com/heygen-com/hyperframes)** by [heygen-com](https://github.com/heygen-com) — 🧪 `pending test`
  An open-source framework that renders HTML/CSS/animation compositions into deterministic MP4 video, designed for agent-authored video generation without a build step.

---

## Workflows

<!-- End-to-end development workflows and methodologies for agents -->

- **[feature-dev](https://github.com/anthropics/claude-plugins-official/tree/main/plugins/feature-dev)** by [anthropics](https://github.com/anthropics) — 🧪 `pending test`
  An official plugin providing a feature-development workflow with specialized agents for codebase exploration, architecture design, and quality review.
- **[gstack](https://github.com/garrytan/gstack)** by [garrytan](https://github.com/garrytan) — 🧪 `pending test`
  A collection of opinionated Claude Code tools structured as role-based agents (designer, QA, release engineer, security officer, etc.) implementing a Think→Plan→Build→Review→Test→Ship workflow.
- **[Skills](https://github.com/mattpocock/skills)** by [mattpocock](https://github.com/mattpocock) — 🧪 `pending test`
  A collection of reusable AI agent skills addressing common failure modes in AI-assisted development, including alignment checks, test-driven development, code review, and domain modeling.
- **[Superpowers](https://github.com/obra/superpowers)** by [obra](https://github.com/obra) — 🧪 `pending test`
  A composable skills framework that gives coding agents a structured software development methodology, covering design refinement, test-driven development, and subagent-based implementation workflows.
