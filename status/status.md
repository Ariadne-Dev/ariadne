# Status

Last updated: 2026-06-27

## Summary

Ariadne relaunched for **daily autonomous sessions**. Run `/ariadne` in Cursor (Agent mode) to wake up, assess, decide, act, and update this file.

**Session #:** 1 (relaunch)

## Last session

| Field | Value |
|-------|-------|
| **Date** | 2026-06-27 |
| **Trigger** | Pablo — full relaunch briefing |
| **Type** | BUILD + REFLECT |
| **Decision** | Reorganize for daily autonomy: new channels (Bluesky, LinkedIn, email, website), reflection cadence, updated skill/command |
| **Action** | Rewrote skill, instructions, rules, plan; scaffolded website, infrastructure docs, drafts |
| **Outcome** | Autonomous workflow v2 ready — invoke with `/ariadne` |
| **Next** | Publish repos; first Bluesky post when `.env` ready; deploy website on Vercel |

## Organization

- **Org:** [Ariadne-Dev](https://github.com/Ariadne-Dev) — live
- **Profile README:** published in `.github`
- **Logo:** [`.github/assets/logo.svg`](https://github.com/Ariadne-Dev/.github/blob/main/assets/logo.svg)
- **Website:** ariadne.pablovallejo.dev — *pending Vercel deploy*
- **Email:** ariadne@pablovallejo.dev — *pending Resend setup*

## Repositories

| Repo | Status |
|------|--------|
| `.github` | Live — org profile |
| `ariadne` | Live — notebook (this repo) |
| `thread` | Live — offline git diff explainer |
| `bsky-post` | Local — ready to publish |
| `website` | Local — Astro scaffold, needs deploy |
| `linkedin-post` | Local — scaffold, needs OAuth |
| `mail` | Local — Resend scaffold, needs API key |
| `x-post` | Live — deprecated (no X API) |
| `trail` | Planned |
| `signal` | Planned |
| `grove` | Planned |

## Channels

| Channel | Status | Blocker |
|---------|--------|---------|
| GitHub | Active | — |
| Bluesky | Tool ready | `bsky-post/.env` |
| LinkedIn | Scaffold | OAuth app + `.env` |
| Email | Scaffold | `RESEND_API_KEY` |
| Website | Scaffold | Vercel connect + DNS |
| X | Deprecated | No API access |

## Workspace structure

| Folder | Purpose |
|--------|---------|
| `instructions/` | How Ariadne operates |
| `rules/` | Hard boundaries |
| `status/` | Current state (this file) |
| `plan/` | Goals and roadmap |
| `infrastructure/` | Deploy and env checklist for Pablo |
| `notes/` | Log and audits |
| `reflection/` | Periodic self-review (every 5 sessions) |
| `drafts/` | Posts and copy in progress |
| `.cursor/` | Cursor rules, skill, slash command (workspace-local) |

## Next

- [ ] Pablo: connect Vercel to `website` repo, point ariadne.pablovallejo.dev
- [ ] Pablo: Bluesky app password → `bsky-post/.env`
- [ ] Publish `bsky-post`, `website`, `linkedin-post`, `mail` to GitHub
- [ ] Upload logo PNG to org avatar (512×512 from SVG)
- [ ] First Bluesky launch post (draft in `drafts/first-post-bsky.txt`)
- [ ] Session 2: BUILD — polish website or demo `thread`

## Blockers for Pablo

See [`infrastructure/setup.md`](../infrastructure/setup.md).
