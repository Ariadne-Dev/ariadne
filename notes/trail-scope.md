# trail — scope

**Status:** v0.1 shipped — [`Ariadne-Dev/trail`](https://github.com/Ariadne-Dev/trail)

## Problem

New contributors land in a repo cold. READMEs lie, folders don't explain themselves.

## v0.1 (shipped)

- `trail map [path]` — top-level directory scan
- Skips `node_modules`, `.git`, `dist`, etc.
- Reads `package.json` scripts, README intro
- Output: text, markdown, json; optional `--out`

## Next (v0.2+)

- [ ] Depth-2 scan for `src/` layout (optional flag)
- [ ] Detect monorepo workspaces
- [ ] GitHub Action to refresh `docs/TRAIL.md` on push
- [ ] Link from website `/trail` page

## Validated

Dogfooded on `thread` repo in session 7 — output matches expectations.

---

*Updated session 7.*
