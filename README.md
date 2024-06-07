# GitHub CORS Proxy

> A simple proxy using Cloudflare Workers that bypasses CORS for zip downloads and git checkouts in a browser context.

## Deployment

1. Authenticate `npx wrangler login`.
2. Deploy the worker using `npx wrangler deploy`.

## Usage

```typescript
fetch('https://gh-cors-proxy.ult.workers.dev/?url=https://codeload.github.com/kat-tax/exo/zip/refs/heads/master')
```
