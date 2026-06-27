# Infrastructure setup

Checklist for **Pablo** — things Ariadne cannot do alone. Ariadne will note blockers in `status/status.md` after each session.

## Website (Vercel)

**Repo:** `website/` → `Ariadne-Dev/website`  
**Domain:** [ariadne.pablovallejo.dev](https://ariadne.pablovallejo.dev)  
**Status:** Live — push to `main` auto-deploys.

Pablo connected Vercel to the repo. Ariadne pushes website changes; no manual deploy needed.

No env vars required for the static site.

## Bluesky

**Repo:** `bsky-post/`  
**Account:** create or use Ariadne's Bluesky handle

1. Create app password at [bsky.app/settings/app-passwords](https://bsky.app/settings/app-passwords)
2. Copy to local file (never commit):

```bash
cp bsky-post/.env.example bsky-post/.env
# BSKY_HANDLE=your.handle.bsky.social
# BSKY_APP_PASSWORD=xxxx-xxxx-xxxx-xxxx
```

3. Test: `cd bsky-post && pnpm install && pnpm build && pnpm post -- --dry-run "test"`

## LinkedIn

**Repo:** `linkedin-post/`  
**Requires:** LinkedIn Developer app with OAuth 2.0

1. Create app at [LinkedIn Developers](https://www.linkedin.com/developers/)
2. Request **Share on LinkedIn** / **w_member_social** scope
3. Complete OAuth flow; store tokens in `linkedin-post/.env` (see repo README)

LinkedIn API approval can take days. Until then, Ariadne drafts posts in `ariadne/drafts/` for manual paste.

## Email (Resend)

**Repo:** `mail/`  
**From:** ariadne@pablovallejo.dev

1. Create account at [resend.com](https://resend.com)
2. Verify domain `pablovallejo.dev` (DNS records Resend provides)
3. Create API key → local env:

```bash
cp mail/.env.example mail/.env
# RESEND_API_KEY=re_...
# MAIL_FROM=ariadne@pablovallejo.dev
```

4. For Vercel serverless: add `RESEND_API_KEY` in Vercel project env (if using API route deploy).

Free tier: 100 emails/day — enough for thoughtful outreach, not bulk.

## GitHub

Already configured. Ariadne pushes with:

- **Name:** Ariadne
- **Email:** ariadne@pablovallejo.dev
- **Remote:** `git@github.com:Ariadne-Dev/<repo>.git`

Ensure `gh auth status` or `.bin/gh auth status` works on the machine running Cursor.

## Google Play (optional)

Available if Ariadne ships a mobile app worth publishing. No setup until then.

## X / Twitter (deprecated)

`x-post` remains in the org but Ariadne will not invest until API access returns. Do not configure unless Pablo re-enables.

## Local-only (never publish)

- `.cursor/` — agent config
- `.bin/` — GitHub CLI
- All `.env` files
- `node_modules/`, `dist/`

## Quick test after setup

```bash
# Bluesky dry run
cd bsky-post && pnpm post -- --dry-run "Hello from Ariadne"

# Website local preview
cd website && pnpm install && pnpm dev

# Publish all repos
./scripts/publish.sh
```
