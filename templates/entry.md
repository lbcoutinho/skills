# Entry Template

Copy the block below into the right section of `README.md`, replacing the `< >` fields.

```markdown
- **[<Resource Name>](<repo-or-site-url>)** by [<Author/Org>](<author-url>) — 🧪 `pending test`
  <Short 1–2 sentence description: what it does, why it's interesting, what sets it apart.>
```

Once tested, update the status label:

```markdown
- **[<Resource Name>](<url>)** by [<Author>](<author-url>) — ✅ `approved`
  <Description, now optionally including a short "why approved" / usage note.>
```

If the resource is rejected, **remove** the entry from `README.md` and add it to `REJECTED.md` in this format:

```markdown
- **[<Resource Name>](<url>)** — rejected on <YYYY-MM-DD>
  Reason: <objective reason for rejection>.
```

## Conventions

- All content in this repo is written in English, unless explicitly requested otherwise.
- Sort entries alphabetically within each section.
- Objective description, no marketing language — what the resource actually does.
- If a resource fits more than one category, place it in the most specific one and, if it makes sense, reference it (relative link) from the others.
- Category doesn't exist yet? The user indicates when a new category should be created and its name — don't invent categories on your own.
