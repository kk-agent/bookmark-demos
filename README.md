# bookmark-demos

Daily X-Bookmarks → Cursor Agent → Cloudflare preview demos (Matt Palmer / Grok Bot pattern).

Each morning CoS (or a standing routine) picks one interesting bookmarked post, a Cursor cloud agent builds a small interactive demo on a branch, Cloudflare Workers Builds posts a preview URL, and Hayden gets that link.

## Convention

- Branch: `demo/YYYY-MM-DD-<slug>` (e.g. `demo/2026-09-16-cobe`)
- Demo code lives under `demos/<slug>/` when the demo needs its own assets; otherwise update the Worker entry + `public/` for a single-page demo.
- PR body must include: source bookmark URL, what was built, screenshot notes / video path, and the Cloudflare preview URL once CI comments.

## Cloudflare setup (Hayden — one-time)

1. Open [Workers & Pages](https://dash.cloudflare.com/) → **Create** → connect Git → select `kk-agent/bookmark-demos`.
2. Enable **Workers Builds** for this repo.
3. Turn on **non-production branch builds** so every `demo/*` branch / PR gets a [preview URL](https://developers.cloudflare.com/workers/versions-and-deployments/preview-urls/).
4. Confirm the GitHub integration posts the preview link as a PR comment.

[![Deploy to Cloudflare](https://deploy.workers.cloudflare.com/button)](https://deploy.workers.cloudflare.com/?url=https://github.com/kk-agent/bookmark-demos)

## Local

```bash
npm install
npx wrangler dev
```

## Status

- Repo: ready
- Cloudflare Git connect: **pending Hayden**
- X Bookmarks API: **blocked** until Twitter/X auth is enrolled (Composio or X Project)
