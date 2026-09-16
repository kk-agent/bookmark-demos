# bookmark-demos

Daily X-Bookmarks → Cursor Agent → Cloudflare preview demos (Matt Palmer / Grok Bot pattern).

## Convention

- Branch: `demo/YYYY-MM-DD-<slug>`
- Demo code under `demos/<slug>/` and/or `public/`
- PR body: bookmark URL, summary, screenshot notes, Cloudflare preview URL (from CI only)

## Cloudflare setup (Hayden — one-time)

1. Workers & Pages → Create → connect Git → `kk-agent/bookmark-demos`
2. Enable Workers Builds + non-production branch builds for [preview URLs](https://developers.cloudflare.com/workers/versions-and-deployments/preview-urls/)

[![Deploy to Cloudflare](https://deploy.workers.cloudflare.com/button)](https://deploy.workers.cloudflare.com/?url=https://github.com/kk-agent/bookmark-demos)

## Local

```bash
npm install && npx wrangler dev
```
