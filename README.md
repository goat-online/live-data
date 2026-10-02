# live-data — GOAT Online

Data files that change on their own schedule and are read straight from
GitHub by the sites' visitors, so they update without a site deploy.

**This repo is public.** Anything in it can be read by anyone. Only public
listings go here: never notes, client details, email addresses, keys or
anything else that is not already meant for the website.

One folder per site, named after the site's slug:

| File | Read by | Written by |
|---|---|---|
| `goat-hotel/whatson.json` | `sites/goat-hotel/assets/js/whats-on.js` (What's On page) | the "Goat Hotel — daily What's On update" scheduled task, every morning |

Pages read a file from
`https://raw.githubusercontent.com/goat-online/live-data/main/<slug>/<file>`.
Change a file's path or name only together with the page that reads it.
