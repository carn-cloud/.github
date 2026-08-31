# Carn Cloud public profile

> The `.github` repository for the Carn Cloud GitHub organisation — its public profile
> page.

GitHub renders `profile/README.md` from an organisation's `.github` repository as that
organisation's public profile. This repo holds that one page for **Carn Cloud**, the
seven-product suite at HaPaDa: the short public pitch and the list of products with their
`<name>.carn.cloud` links. It is a content repo — no code, no build, no dependencies. Its
internal counterpart is `carn-cloud/_github/private` (the `.github-private` repo), which
carries the full product handbook.

## Features

- **The organisation profile page** — [profile/README.md](profile/README.md): the suite
  summary and a one-line description of each of the seven products, each linking to its
  own domain.

## Requirements

- Anything that renders Markdown. There is no build step and nothing to install.
- To publish a change: push to this repository's default branch. GitHub picks the page up
  automatically; there is no deploy step.

## Getting started

```sh
cat profile/README.md   # the page as it renders on github.com/carn-cloud
```

## Development

| Path | What lives there |
| ---- | ---------------- |
| `profile/README.md` | The public organisation profile page GitHub renders |

- There is no build, test or lint step; `/check` has nothing to run here.
- **Keep the product list in step** with the four other places that describe the suite:
  `carn-cloud/_github/private/profile/README.md` (the handbook),
  `carn-cloud/lib/web-core/src/suite.ts` (the registry the sites render from),
  `setup/products.yaml` (the canonical keys and colours), and each product's own site.
- This page is **public**. Nothing unreleased, internal or unpriced belongs on it.

## Related repositories

- `carn-cloud/_github/private` — the internal product handbook: per-product pages with
  meaning, branding, interfaces and lifecycle position.
- `carn-cloud/lib/web-core` — `src/suite.ts`, the registry the public sites render the
  same list from.
- `setup` — `products.yaml`, the canonical product taxonomy.

## Licence

Copyright © HaPaDa. All rights reserved.

This is proprietary software (`LicenseRef-Proprietary`). No licence is granted to use,
copy, modify, or distribute it outside HaPaDa.
