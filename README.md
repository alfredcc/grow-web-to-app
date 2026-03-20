# Grow Web to App

Static landing page deployed to Cloudflare Pages.

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

This starts Cloudflare Pages local development and serves the site from
`public/`.

## Deploy

```bash
npm run deploy
```

This publishes the site to the Cloudflare Pages project that backs the custom
domain.

## Project structure

- `public/`: static assets served by Cloudflare
- `wrangler.jsonc`: Cloudflare Pages configuration
