# AGENTS.md

This is an [awesome-list](https://awesome.re) repository — a curated collection of AI agent resources maintained entirely in [README.md](README.md).

## Project Structure

- `README.md` — The awesome list itself (all content lives here)
- `CONTRIBUTING.md` — Contribution guidelines for pull requests

There is no build system, test suite, or application code.

## Entry Format

Every list item must follow this exact format:

```
- [Resource Name](https://example.com) - Brief description that starts with a capital letter and ends with a period.
```

- One resource per line, one PR per resource.
- Descriptions: short, descriptive, capitalized, period-terminated.
- Deduplicate before adding — search existing entries first.

## Editing Rules

- Only edit `README.md` to add, remove, or update list entries.
- Place entries under the correct category section.
- New categories or restructuring existing ones is allowed.
- Do not reorder existing entries unless specifically asked.
- See [CONTRIBUTING.md](CONTRIBUTING.md) for full guidelines.

## Commit Convention

Use this format for all commits:

```
feat(<category>): add <Resource Name>
```

- `<category>` is the lowercase section name from README.md (e.g., `skills`, `frameworks`, `tutorials`, `leaderboard`, `agents`, `tools`, `applications`, `research`).
- For multiple resources in one commit, list categories: `feat(leaderboard,frameworks): add X, Y, and Z`.
- Use `chore:` for non-content changes (e.g., repo setup, CI, docs fixes).
