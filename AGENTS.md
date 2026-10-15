# limitcodes website

limitcodes personal site, deployed on Cloudflare Pages. Static files live in `public/`. `wrangler.jsonc` sets `pages_build_output_dir` to that directory.

## Local development

The Cloud Agent environment installs Node.js 22.23.3 and Wrangler 4.149.0, then serves the site on boot:

```bash
wrangler pages dev --ip 0.0.0.0 --port 8788
```

Open http://127.0.0.1:8788. There is no package manifest, test suite, or compile step. Pages header rules in `public/_headers` apply during `wrangler pages dev`.
