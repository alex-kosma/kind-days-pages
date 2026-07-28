# life-coach-pages

The public privacy policy and support page for the **Life Coach** app. Apple and
Google both require each of these to be a reachable URL, and this repo exists
only to be that URL.

**This repo is public on purpose.** The app's own repository stays private —
GitHub Pages refuses to publish from a private repo without a paid plan, and the
app repo also contains a candid list of unfixed bugs that has no business being
public. Nothing here is secret: three HTML files and a stylesheet.

## Published at

- `/` — landing page
- `/privacy-policy.html`
- `/support.html`

## Enabling Pages (once)

Repo **Settings → Pages → Source: Deploy from a branch → `main` / `(root)`**.
The URL appears within a minute or two.

`.nojekyll` is committed deliberately. It tells GitHub Pages to serve these
files verbatim instead of running them through Jekyll — which matters because
Jekyll silently ignores files and folders beginning with an underscore, and
because plain HTML has nothing to gain from being processed.

## Editing

The prose here is the published copy. The markdown originals live in the app
repo under `docs/`, and **the two will drift** — if you change a policy, change
it in both, or the published page and the repo's own record will disagree. The
published one is the one that counts, because it is the one a user and a
reviewer can actually read.

Anything user-visible that changes in the app — the export flow, the daily cap,
what the coach sends — needs a pass over `privacy-policy.html` before the next
submission. A privacy policy that describes an older version of the app is worse
than a terse one.

## Deliberately absent

No analytics, no cookies, no web fonts, no CDN, no third-party requests of any
kind. These are the pages that promise the app doesn't phone home; loading a
tracker here would contradict them in the most literal way available.
