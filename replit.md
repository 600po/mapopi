# Walter Farm — African Farming Community Platform

## Overview

pnpm workspace monorepo using TypeScript. The main product is **Walter Farm**, a richly decorated African farming social community web app. Contact: 0743 035 900.

## Product Features
- **Feed** tab — Social post feed with images, like/comment/share interactions
- **Explore** tab — Infinite-scroll AI content (AgTech, harvest, markets, herbs, etc.), Farm Videos section (YouTube embeds), AI masonry grid
- **Activities** tab — Sports & Community / Manures & Soil / Weather & Climate sections, each AI-powered with real images and live Gemini news
- **Live Farm Events panel** — 20-second auto-refresh AI news ticker; click any headline to open full Gemini-written article
- **AI Weather card** — Gemini-generated realistic farming weather by location, auto-refreshes every 5 min
- **AI Search** — Gemini-powered search overlay (press `/` to open)
- **News Article Modal** — Full readable articles for any news item: headline, 4 paragraphs, pull quote, key facts, related topics
- **Dark mode** — Toggle in header
- **Footer** — Walter Farm branding + clickable contact number 0743 035 900

## Gemini API Endpoints (all at `/api/farming/`)
- `GET /weather` — AI weather for a location
- `GET /live-events` — 6 live farming news events (refreshes every 20s client-side)
- `GET /explore` — AI masonry cards (infinite scroll)
- `GET /activities?category=sports|manures|weather` — Activity-specific AI news cards
- `GET /news-article?headline=&category=&region=` — Full readable article generator
- `GET /search?q=` — AI farming search results

## Stack

- **Monorepo tool**: pnpm workspaces
- **Node.js version**: 24
- **Package manager**: pnpm
- **TypeScript version**: 5.9
- **API framework**: Express 5
- **Database**: PostgreSQL + Drizzle ORM
- **Validation**: Zod (`zod/v4`), `drizzle-zod`
- **API codegen**: Orval (from OpenAPI spec)
- **Build**: esbuild (CJS bundle)

## Key Commands

- `pnpm run typecheck` — full typecheck across all packages
- `pnpm run build` — typecheck + build all packages
- `pnpm --filter @workspace/api-spec run codegen` — regenerate API hooks and Zod schemas from OpenAPI spec
- `pnpm --filter @workspace/db run push` — push DB schema changes (dev only)
- `pnpm --filter @workspace/api-server run dev` — run API server locally

See the `pnpm-workspace` skill for workspace structure, TypeScript setup, and package details.
