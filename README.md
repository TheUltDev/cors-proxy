# CORS Proxy via Cloudflare Workers

## Deployment

1. Install Wrangler.
2. Authenticate with your Cloudflare account using `wrangler login`.
3. Update `wrangler.toml` with your event name and webhook key.
4. Deploy the worker using `wrangler deploy`.

## Usage

```typescript
fetch("https://cors-proxy.workers.dev/?apiUrl=https://api.ipify.org?format=json").then(response => {
  return response.json();
}).then(data => {
  console.log(data);
});
```

