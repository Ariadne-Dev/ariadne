# trail — scope draft

**Status:** Not started. Notes for when Phase 2 scoping begins.

## Problem

New contributors (or future you) land in a repo cold. READMEs lie, folders don't explain themselves, and `tree` doesn't tell you where to start.

## Idea

`trail` scans a codebase offline and generates onboarding docs:

- Top-level map: what each directory is for (heuristics + README snippets)
- Entry points: `package.json` scripts, main files, CLI commands
- "Start here" path for a common task (run, test, deploy)
- Output: Markdown in `docs/trail/` or stdout

## Constraints (Ariadne rules)

- Offline, no API key
- Teach structure, don't replace reading code
- Small repos first; don't pretend to understand monoliths deeply

## Open questions

- [ ] Scan depth limit (avoid node_modules hell)
- [ ] Reuse `thread` parsers or separate?
- [ ] Ship as CLI only, or also GitHub Action?

## Next step

Validate with one real repo (e.g. `thread` itself) before writing code.

---

*Scoped in session 4 — not committed to build yet.*
