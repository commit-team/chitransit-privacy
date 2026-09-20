# ChiTransit legal documents

This repository exists for one reason: Google Play requires a **publicly reachable URL** for an
app's privacy policy, and the ChiTransit source repository is private. The terms of service now
live here too, for the same reason — the app links to both from its Settings screen.

| Document | Source | Published at |
|---|---|---|
| Privacy Policy | `index.md` | <https://commit-team.github.io/chitransit-privacy/> |
| Terms of Service | `terms.md` | <https://commit-team.github.io/chitransit-privacy/terms/> |

Both files are the canonical copy — edit them here, not anywhere else. GitHub Pages rebuilds on
push, usually within a minute.

`terms.md` sets `permalink: /terms/` in its front matter. Without it Jekyll would serve the page
at `/terms.html`, and the app and the privacy policy both link to the trailing-slash form.

Both URLs are referenced by the Play Console listing and by the app itself, so treat them as
permanent. Renaming this repository, changing a permalink, or turning Pages off breaks the store
listing and leaves a dead link inside a shipped app that cannot be force-updated.

`_config.yml`'s `title` and `description` are site-level and this theme prints them on every
page, so neither can name a single document. Each document names itself in its own first line.
