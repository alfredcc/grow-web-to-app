# Grow Web to App

Static landing page deployed to Cloudflare Pages, with an optional Worker
preview/deploy path kept for debugging.

## Requirements

- Node.js 22+
- npm 10+

## Install

```bash
npm install
```

## Local development

```bash
npm run dev
```

This starts Wrangler locally with the Worker config and serves the site from
`public/`.

## Remote preview

```bash
npm run preview
```

This uses Cloudflare's remote runtime, so you need to log in first:

```bash
npx wrangler login
```

## Deploy

```bash
npm run deploy
```

This publishes the site to the Cloudflare Pages project that backs the custom
domain.

## Worker deploy

```bash
npm run deploy:worker
```

This publishes the same static assets to the standalone `workers.dev` URL.

## Project structure

- `public/`: static assets served by Cloudflare
- `wrangler.jsonc`: Cloudflare Pages configuration
- `wrangler.worker.jsonc`: Cloudflare Worker configuration
