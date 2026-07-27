---
name: curate-resource
description: Adds, approves, or rejects a resource (skill, agent, framework, tool) in this repository's curated list. Use when the user gives a link to a new repo/tool to add, says they tested and approved a resource already listed, or says a resource was rejected/isn't good.
---

# Curate Resource

Keeps `README.md` and `REJECTED.md` in this repository up to date, following the flow described in `CLAUDE.md`. All content produced (README text, PR title/body, commit messages) must be in English, unless the user explicitly asks for another language.

## When to use

- User sends a URL of a new repository/tool → **add**.
- User says "I tested X and approved it" / "mark X as approved" → **approve**.
- User says "X isn't good" / "I rejected X" / "remove X" → **reject**.

## Step by step

### 1. Add a new resource

1. Check whether the link already exists in `README.md` or `REJECTED.md` (search by URL). If it already exists, tell the user instead of duplicating it.
2. If the user didn't specify the category in the same message, **ask** which category to use before proceeding. Never guess or invent a category — categories are only created when the user explicitly names one.
3. Fetch the link's content (WebFetch on the repo README, or the page) to understand: what it does, what it's for, author/org.
4. Insert the entry alphabetically in the chosen section, following `templates/entry.md`, with the `🧪 \`pending test\`` label. Remove the `_No entries yet._` placeholder if it's the first entry.
5. Commit and push automatically, opening a PR for approval (or pushing to the existing open PR branch — see step 4 below). Confirm to the user which section the entry was added to, with a 1-line summary of what the resource is.

### 2. Approve an existing resource

1. Find the entry in `README.md` (by name or link).
2. Swap `🧪 \`pending test\`` for `✅ \`approved\``.
3. If the user gives usage context ("worked well for X"), fold it into the description as a short note.
4. Commit and push automatically to a PR for approval.

### 3. Reject an existing resource

1. Find the entry in `README.md`.
2. Remove it from `README.md`.
3. Add it to `REJECTED.md`, following the template, with today's date and the reason. If the user didn't give a reason, ask before recording one — a generic reason doesn't help future decisions.
4. Commit and push automatically to a PR for approval.

### 4. Git / PR conventions

- Always commit and push automatically — never leave the change uncommitted waiting for an explicit push request.
- If there's already an open PR covering this branch, push additional commits to it rather than opening a new one.
- Keep the PR description minimal: `"Added <repo> to <Category>"`, `"Approved <repo>"`, `"Rejected <repo>"`. Use bullet points only if there's more than one highlight to report.

## Rules

- Keep alphabetical order within each section.
- Objective descriptions, no marketing tone, 1–2 sentences.
- Everything written in English by default.
