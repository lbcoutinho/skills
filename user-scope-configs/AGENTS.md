## Plan and docs

- Plans are written directly into the GitHub issue body with `## Implementation Plan`, `## Acceptance Criteria`, `## Tests`, never to a local plan file
- When decision deviates from ticket's original plan, add comment to Issue explaining deviation.

## Ticket workflow (follow for every task)

- Don't create issues in Github without explicit ask.
- Never work on the main worktree. Always create new worktree when starting any work.
- Branch-per-implementation — Commit + push to feature branch, open pull request to `main`.
- Always use skill `create-issue` to open issue for one ticket at a time. If not available then stop and ask.
- Always use skill `create-commit` for commits. If not available then stop and ask.
- Always use skill `create-pr` to open PRs. If not available then stop and ask.
- Do regular commits. Commit on every step finished.
- Never execute lint, format, typecheck, unit tests, e2e test, API client regenerate or any command that user can quickly run manually after coding is done. Commit the changes and print the commands the user needs to run in order.

## Writing

- ADRs/PRDs/plans may sacrifice prose grammar for token economy
- Use subagent with Haiku model for any writing prose task: docs, plans, prd, etc.

## Agentic workflow

- When implementing code, use a subagent for each step/task/block. Analyze the plan and create a dependency tree to understand what can be done in parallel and what's sequential. Use the main session exclusively to coordinate the subagents.

## Conventions

- Never merge PRs — user reviews and merges.
- English (en-US) everywhere — code, comments, commit messages, etc.

<!-- CODEX_START -->
@/home/leandro/.codex/RTK.md
<!-- CODEX_END -->
