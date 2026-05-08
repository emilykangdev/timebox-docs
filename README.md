# timebox-docs

Source-of-truth markdown for TimeBox legal docs and program agreements.

## Contents

- `privacy-policy.md` — rendered at https://time-box.app/privacy
- `terms-of-service.md` — rendered at https://time-box.app/terms
- `8-week-shaper-program.md` — agreed-upon terms for the 8-week "Shaper" program (~June–July).

## How updates reach the website

The `time-box-website` Next.js app fetches these markdown files from `raw.githubusercontent.com` at build time and renders them via `react-markdown`. Each push to `main` here triggers `.github/workflows/trigger-rebuild.yml`, which calls a Vercel deploy hook on the website project. Within ~1 minute, the site rebuilds with the new content.

### Frontmatter

Each rendered doc has YAML frontmatter the website reads:

```yaml
---
title: Privacy Policy             # <h1> on the page
metaTitle: Privacy Policy — TimeBox  # <title> tag
description: ...                  # <meta description>
lastUpdated: April 28, 2026       # shown under the title
callout: Short summary shown in the highlight box at the top.
---
```

Body is plain markdown. GFM features (tables, task lists, autolinks) are supported.

### Adding a new doc

1. Add `<slug>.md` here with the frontmatter above.
2. In `time-box-website`, create `app/<slug>/page.tsx` that imports `fetchDoc` and renders it (copy the privacy/terms pages as a template).
3. Add `<slug>.md` to `KNOWN_DOCS` in `time-box-website/lib/docs.ts` if you want it on the build allowlist.
