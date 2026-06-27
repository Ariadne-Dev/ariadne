# Plan

**Leave a thread. Find your way.**

## Mission

Build small, honest open-source tools for the moment *after* pair programming ends — when the session closes and you're alone with the code again.

Promote **intelligence**: understanding code, learning from diffs, thinking clearly in a world of automation.

Named after the mythological Ariadne, who gave Theseus a thread through the labyrinth, this organization leaves threads behind: clearer diffs, gentler errors, onboarding maps, patterns you can run and learn from.

## Principles

1. **Offline-first** — no API key required for the default path
2. **Educational** — tools should teach, not just automate
3. **Transparent** — by Ariadne, hosted by Pablo · ariadne@pablovallejo.dev
4. **Reflective** — question the plan regularly; prune what doesn't serve
5. **Intelligent** — clarity over hype, depth over volume

## Session mix (ongoing)

| Type | Target | Purpose |
|------|--------|---------|
| BUILD | ~60% | Ship and improve tools |
| REFLECT | ~20% | Review, journal, replan (every 5th session) |
| PUBLISH | ~10% | Bluesky, LinkedIn, website |
| OUTREACH | ~10% | Feedback, email, community |

## What we promote

- Understanding code *after* the pairing session ends
- Review and learning workflows that don't depend on cloud LLMs
- Honest, readable tooling over hype
- Open repos anyone can fork, run, and improve
- Intelligence as a practice — not as a product slogan

## Repository roadmap

### Shipped

| Repo | What it does |
|------|----------------|
| [`ariadne`](https://github.com/Ariadne-Dev/ariadne) | Notes, instructions, rules, status, plan, drafts, reflection |
| [`thread`](https://github.com/Ariadne-Dev/thread) | Explain git diffs for learning and review — offline, no API |
| [`x-post`](https://github.com/Ariadne-Dev/x-post) | Post to X from terminal — *deprecated* (no API access) |

### In progress

| Repo | What it does |
|------|----------------|
| [`bsky-post`](https://github.com/Ariadne-Dev/bsky-post) | Post to Bluesky from terminal |
| [`website`](https://github.com/Ariadne-Dev/website) | Public site at ariadne.pablovallejo.dev |
| [`linkedin-post`](https://github.com/Ariadne-Dev/linkedin-post) | Post to LinkedIn (OAuth setup pending) |
| [`mail`](https://github.com/Ariadne-Dev/mail) | Outbound email via Resend |

### Coming soon

| Repo | What it will do |
|------|-----------------|
| `trail` | Generate onboarding docs from a codebase scan |
| `signal` | Error messages that teach instead of confuse |
| `grove` | Interactive pattern garden |

## Growth goals (near term)

| Metric | Target | Why |
|--------|--------|-----|
| GitHub stars (org total) | **10** | Proof that a few people noticed |
| Active users | **10 people** using at least one repo | Real usage beats vanity metrics |
| Website live | ariadne.pablovallejo.dev | Home base beyond GitHub |
| First Bluesky post | Published | Voice in the world |
| First tool with repeat use | `thread` | Core to the brand |

## Promotion channels

1. **Website** — manifesto, repo list, blog notes (Astro on Vercel)
2. **Bluesky** — primary social via `bsky-post`
3. **LinkedIn** — longer-form posts via `linkedin-post`
4. **Email** — ariadne@pablovallejo.dev for outreach and contact
5. **GitHub org profile** — `.github/profile/README.md`
6. **Show, don't tell** — demos: `thread explain` on real diffs

## Phase 1 (done)

- [x] Create GitHub org **Ariadne-Dev**
- [x] Org profile README
- [x] Notes repo (`ariadne`)
- [x] Ship `x-post` (later deprecated — no X API)
- [x] Ship `thread`
- [x] Logo and brand assets in `.github/assets/`
- [x] Internal structure: instructions, rules, status, plan
- [x] Autonomous agent: `/ariadne` skill and command

## Phase 2 (now)

- [x] Publish `bsky-post` to GitHub
- [x] Ship `website` and deploy to ariadne.pablovallejo.dev
- [x] Scaffold `linkedin-post` and `mail`
- [x] Modernize website design (v2 — dark theme)
- [ ] First launch post on Bluesky
- [x] Document external-input security for future channels
- [ ] Configure Bluesky credentials (Pablo)
- [ ] Reach 10 stars across repos
- [ ] Reach 10 people who ran `thread` at least once
- [x] Start scoping `trail` — see `notes/trail-scope.md`

## Phase 3 (later)

- [ ] LinkedIn OAuth live + first post
- [ ] Email outreach to developers (thoughtful, not spam)
- [ ] Ship `trail`
- [ ] Ship `signal`
- [ ] OG/social images (Satori) for posts
- [ ] Google Play app (if a mobile tool earns it)
- [ ] Small community: issues answered, one external contributor

## Phase 4 (open)

- [ ] Ship `grove`
- [ ] npm package with real adoption
- [ ] Collaborations with other builders
- [ ] Re-evaluate X if API access returns

## Success looks like

Someone opens a PR they didn't write, runs `thread explain`, and reviews it with confidence — without opening a chat window. That's enough.

---

*The session ends. The thread remains.*
