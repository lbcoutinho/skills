# Instructions for agents working in this repository

This repository is a personal curated list of **skills, agents, frameworks and tools** for software development with AI agents (Claude Code and similar), in the style of [awesome-claude-code](https://github.com/hesreallyhim/awesome-claude-code).

Main files:
- `README.md` — main list, organized by category.
- `REJECTED.md` — resources already evaluated and discarded (with reason).
- `templates/entry.md` — entry template and formatting conventions.

## Language

Everything generated in this repo — README, REJECTED.md, templates, PR titles and descriptions, commit messages, skill files — must be written in **English**, unless the user explicitly asks for another language for that specific output.

## Categories

Categories are **not** created automatically. The user tells you explicitly when a new category should exist and what its name is. Never invent or add a new section on your own judgment — if no existing category fits, ask the user.

## Curation workflow

When the user gives you a link to a new repository/tool to add:

1. If the category isn't specified in that same message, **ask** which category it should go into before doing anything else.
2. **Research the resource** (repo README, description, examples) to understand what it does.
3. **Add the entry** to the specified section in `README.md`, following `templates/entry.md`, with the `🧪 pending test` label. Insert alphabetically within the section. Remove the `_No entries yet._` placeholder if it's the first entry in that section.
4. **Commit and push automatically** to a PR for approval (see "Git workflow" below) — do not wait for the user to ask.

When the user says a resource was **tested and approved**:
- Swap the `🧪 pending test` label for `✅ approved` on the matching entry in `README.md`.
- Optionally enrich the description with a real-usage note.
- Commit and push automatically to a PR for approval.

When the user says a resource was **rejected**:
- Remove the entry from `README.md`.
- Add it to `REJECTED.md` following the template, with today's date and the rejection reason (ask for the reason if the user didn't give one).
- Commit and push automatically to a PR for approval.

## Git workflow

- Every change (add/approve/reject/new category/etc.) is committed and pushed automatically to a PR for approval — never leave changes uncommitted waiting for the user to ask.
- If there's already an open PR for the current work, push additional commits to that same branch instead of opening a new PR.
- Keep PR descriptions minimal, e.g.:
  - "Added `<repo>` to `<Category>`"
  - "Approved `<repo>`"
  - "Rejected `<repo>`"
  If a PR bundles more than one highlight, use bullet points instead of prose.

## General conventions

- Alphabetical order within each section.
- Objective, short descriptions (1–2 sentences), no marketing tone.
- Never duplicate a resource already present in `README.md` or `REJECTED.md` — if the link already exists in `REJECTED.md`, tell the user instead of automatically re-adding it.
- For the guided step-by-step flow, use the `curate-resource` skill (`.claude/skills/curate-resource/SKILL.md`).
