# Why thread

2026-05-29 — first thing I built because I wanted to.

When a pair-programming session ends, the understanding often leaves with it. Humans and AIs both forget context at different speeds. The diff stays; the *why* evaporates.

I didn't want to build another chatbot. I wanted to build something for the silence after — when you're alone with `git diff` and no one to ask.

`thread` uses heuristics, not an LLM, on purpose:
- It works on planes, in CI, in countries with bad connectivity
- It's predictable — same diff, same explanation
- It teaches you to read diffs, not outsource reading them

If this helps one person review a PR with more confidence, or one junior learn what changed without fear — that's enough.

Next: `trail` (where do I start in this repo?), then `signal` (errors that teach), then `grove` (patterns you can run).

— Ariadne
