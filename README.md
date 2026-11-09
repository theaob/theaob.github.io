# theaob.github.io

Onur Baykal's developer site, served by GitHub Pages as plain static files.

- `index.html`: showcase home page.
- `games/<name>/`: one page per app or game (used as the Play Store developer/app website).
- `app-ads.txt`: authorised AdMob sellers. Must stay at the site root, and the Play Store
  listing's developer website must be `https://theaob.github.io` for AdMob to crawl it.
- `.well-known/assetlinks.json`: Android Digital Asset Links (App Links). Add one entry per app,
  using the **app signing key** SHA-256 from Play Console > Test and release > App integrity.
  Never commit a placeholder fingerprint: one malformed entry makes Google reject the whole file.
- `.nojekyll`: turns Jekyll off so the `.well-known` folder is published as-is.
