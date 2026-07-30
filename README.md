# softwaredonkey.com

Homepage for **SoftwareDonkey** — an independent app studio.
SoftwareDonkey is a DBA of JacobNollette.com LLC.

## How it works

- Static site, single `index.html`, no build step, no dependencies.
- Deployed to **GitHub Pages** by [`.github/workflows/deploy.yml`](.github/workflows/deploy.yml) on every push to `main`.
- Custom domain `softwaredonkey.com` — DNS lives in Cloudflare, managed as Terraform in the
  `jnllc/services` monorepo under `cloudflare/softwaredonkey.com/` (apex + `www` CNAME →
  `jnllc.github.io`, DNS-only so GitHub can provision the TLS certificate).

## Editing

Edit `index.html`, push to `main`. That's it — the donkey carries the rest.
