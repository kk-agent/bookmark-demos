# Agent instructions — bookmark-demos

You are building ONE small interactive demo from a single X bookmark Hayden (or CoS) named.

## Do

1. Create branch `demo/YYYY-MM-DD-<slug>` from `main` (America/Chicago date).
2. Implement a focused demo under `demos/<slug>/` and/or `public/` + Worker as needed.
3. Keep deps light. Prefer vanilla or one small library already implied by the bookmark.
4. Open a PR to `main` with: bookmark URL, summary, how to try it, screenshot/video notes.
5. Wait for Cloudflare Workers Builds preview comment; do not invent a preview URL.

## Do not

- Force-push `main`
- Add secrets or paid Cloudflare resources
- Build multiple demos in one PR
- Claim LIVE without a real preview URL from CI
