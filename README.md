# @astrojs/cloudflare 15 beta silently ignores wrangler.jsonc

```sh
npm install
npm run build
cat .cloudflare/output/v0/workers/default/worker.config.json
```

The build succeeds, but the generated Worker config has the `package.json` name instead of `my-production-worker`, and no `compatibility_date`, `nodejs_compat`, `vars` or D1 binding from `wrangler.jsonc`.
