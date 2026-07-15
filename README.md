# sb2610-safe-harbor-dim
SB 2610 Safe Harbor DIM - Texas cybersecurity safe harbor readiness assessment

## Deployment

**Canonical source of truth:** GitHub `main` (this repo) → **Cloudflare Pages**.

The Cloudflare Pages project connected to this repo is the ONLY production runtime. It auto-deploys from `main` on push, served at the `*.pages.dev` URL.

The standalone Cloudflare Worker (`sb2610-safe-harbor-dim.don-0aa.workers.dev`) is deprecated and must be retired or synced to this repo to prevent version drift. Do not treat the Worker as authoritative.

The `.com` custom domain is held (not public) until explicitly cleared to go live.

`index.html` is fully self-contained: intro → 10 questions → 5-axis scoring (Scope / Standard / Safeguards / Substantiation / Sustained) → Safe Harbor Brief.
