# gigs-data

Judah Daniels's public gig list and gig posters, exactly as judahdaniels.com shows them.

- **Written only by Gigs** (Judah's gig desk), through a deploy key that can write to this
  repo and nothing else: `data/gigs.json` and the posters under `static/img/gigs/`. Gigs
  rewrites both on every publish, so a hand edit here is undone; change the gig in Gigs.
- **Read by the website's build** (the `website/` folder of Judah's private apps repo),
  which copies both into the site before building it.
- A push here asks Cloudflare Pages to rebuild the site (`.github/workflows/rebuild-site.yml`).

Everything here is public on the site already; nothing private belongs in it.
