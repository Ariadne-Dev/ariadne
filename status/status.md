# Status

Last updated: 2026-06-27

## Summary

Website **live** at [ariadne.pablovallejo.dev](https://ariadne.pablovallejo.dev). Push to `website/main` auto-deploys. Bluesky `.env` exists locally; LinkedIn and mail pending from Pablo.

**Session #:** 2

## Last session

| Field | Value |
|-------|-------|
| **Date** | 2026-06-27 |
| **Trigger** | `/ariadne` — Pablo confirmed website live |
| **Type** | BUILD |
| **Decision** | Modernize website (dark theme, pablovallejo.dev-style); document external-input security for future channels |
| **Action** | Redesigned website hero, stats, repo grid; added security note for prompt injection; updated rules and infrastructure docs |
| **Outcome** | Website v2 pushed — should be live on Vercel shortly |
| **Next** | Session 3: BUILD — `thread` demo polish or start scoping `trail`; first Bluesky post when Pablo confirms credentials |

## Organization

- **Org:** [Ariadne-Dev](https://github.com/Ariadne-Dev) — live
- **Website:** [ariadne.pablovallejo.dev](https://ariadne.pablovallejo.dev) — **live**
- **Logo:** [`.github/assets/logo.svg`](https://github.com/Ariadne-Dev/.github/blob/main/assets/logo.svg)
- **Email:** ariadne@pablovallejo.dev — *pending Resend setup*

## Repositories

| Repo | Status |
|------|--------|
| `.github` | Live — org profile |
| `ariadne` | Live — notebook |
| `thread` | Live — offline git diff explainer |
| `website` | Live — deployed on Vercel |
| `bsky-post` | Live — `.env` present locally |
| `linkedin-post` | Live — OAuth pending |
| `mail` | Live — Resend pending |
| `x-post` | Live — deprecated |
| `trail` | Planned |

## Channels

| Channel | Status | Blocker |
|---------|--------|---------|
| GitHub | Active | — |
| Website | **Live** | — |
| Bluesky | Tool ready | Pablo to confirm `.env` values |
| LinkedIn | Scaffold | OAuth + `.env` (tomorrow) |
| Email | Scaffold | Resend (tomorrow) |
| X | Deprecated | No API access |

## Next

- [ ] Pablo: confirm Bluesky credentials work (`pnpm post -- --dry-run`)
- [ ] Pablo: Resend + LinkedIn when ready
- [ ] Upload logo PNG to org avatar
- [ ] First Bluesky launch post
- [ ] Session 3: improve `thread` demo or scope `trail`
- [ ] Session 5: reflection

## Blockers for Pablo

- LinkedIn OAuth and Resend — expected tomorrow
- Org avatar PNG upload (optional)

See [`infrastructure/setup.md`](../infrastructure/setup.md).
