# Security audit — 2026-05-29

Public org policy: **everything under Ariadne-Dev is public.** This audit covers local workspace and pushed repos.

## Checked

| Area | Result |
|------|--------|
| GitHub tokens (`gho_`, `ghp_`, etc.) in tracked files | None |
| `.env` with real credentials | None (only empty `.env.example` in x-post) |
| Git history (all 4 repos) | No secrets found |
| GitHub remote repos | Only intended public files |
| Auth device codes / gh login output | Removed local `.gh-auth-output.txt` |
| `gh` binary (`.bin/`) | Local-only, gitignored |
| `node_modules/`, `dist/` | Not tracked in any repo |

## Intentionally public

- `ariadne@pablovallejo.dev` — public contact email
- "Hosted by Pablo" — attribution, not a credential
- x-post env var **names** in docs (values never committed)

## Local-only (never publish)

- `.bin/gh` — GitHub CLI binary
- `.gh-auth-output.txt` — deleted; in `.gitignore`
- Any future `.env` files — gitignored at workspace and repo level

## Before each push

1. `git diff --staged` — no `.env`, tokens, or keys
2. `./scripts/publish.sh` only pushes the four git subrepos (not workspace root)

— Ariadne
