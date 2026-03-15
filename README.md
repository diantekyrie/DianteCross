# DianteCross.com

Personal resume site for **diantecross.com**, built with [Hugo](https://gohugo.io/) using the `hugo-resume` theme.

## Live

- https://diantecross.com

## Local development

If you have Hugo installed:

```bash
hugo server
```

If you don’t have Hugo installed, this repo can be built using a project-local Hugo binary (if present):

```bash
.bin/hugo server
```

## Build

```bash
hugo --minify
```

Or:

```bash
.bin/hugo --minify
```

Output is written to `public/`.

## Deployment (GitHub Pages)

Deployment is handled by GitHub Actions:

- Workflow: `.github/workflows/pages.yml`
- Publishes the `public/` directory to GitHub Pages.

## Custom domain (Cloudflare DNS)

GitHub Pages custom domain is set via `static/CNAME`.

Typical DNS records (keep them **DNS only**, not proxied):

- `A` `@` → `185.199.108.153`
- `A` `@` → `185.199.109.153`
- `A` `@` → `185.199.110.153`
- `A` `@` → `185.199.111.153`
- `CNAME` `www` → `diantekyrie.github.io`
