# kaleb.one

Public app launcher — a Liquid Glass hub for the `*.kaleb.one` constellation.

## Live Apps

| App | URL | Status |
|-----|-----|--------|
| Kitchen | kitchen.kaleb.one | ✅ Live |
| Masks Wiki | masks.kaleb.one | ✅ Live |
| Brain | brain.kaleb.one | ✅ Live |
| World | world.kaleb.one | 🔜 Coming Soon |

## Tech

- Single-page static HTML (no build step)
- Liquid Glass (glassmorphism) aesthetic
- Cloudflare Pages deployment
- Inter + Georgia typography

## Deploy

```bash
CF_TOKEN=*** read "op://Developer/Global Cloudflare Token/credential")
CF_ACCOUNT_ID="e500dc74dca67189444bf0af0b54c39d"
CLOUDFLARE_API_TOKEN="***" CLOUDFLARE_ACCOUNT_ID="$CF_ACCOUNT_ID" \
  npx wrangler pages deploy . --project-name=hub-kaleb-one --branch=main
```