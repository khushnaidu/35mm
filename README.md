# 35mm.contact

Static site for the 35mm app: landing page, `/privacy`, `/support`.
Plain HTML + one stylesheet, no build step. Hosted on Vercel.

## Deploy

1. Push this folder to its own GitHub repo.
2. Vercel → Add New → Project → import the repo. Framework preset: **Other**, no build command.
3. Project → Settings → Domains → add `35mm.contact` and `www.35mm.contact` (www redirects to the apex).

## Later (ADR 0001 §8)

- `/.well-known/apple-app-site-association` for universal links. `vercel.json` already serves it as JSON.
- `/l/[id]`, `/p/[id]`, `/person/[id]` fallback pages with Open Graph tags.
