# AGENTS.md

## Purpose
Public API for transliterating Russian Cyrillic text to Latin.

## Repository Role
- Category: `*.api.airat.top` (public API project).
- Deployment platform: Cloudflare Workers.
- Main files: `worker.js`, `wrangler.toml`.

## API Summary
- Live endpoint: `https://translit.api.airat.top`.
- Status page: `https://status.airat.top`.
- Supports `GET` and `POST` with `text` input.
- Health route: `/health`.

## AI Working Notes
- Keep transliteration mapping backward-compatible.
- Keep `400` validation for missing input text.
- Keep CORS enabled and response schema stable (`text`, `translit`).
