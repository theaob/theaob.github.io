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
- `support/`: one page with every app's privacy policy, terms and "report a problem" link. Add new apps here.
- `sitemap.xml`, `robots.txt` and the JSON-LD block in `index.html`: update them when an app is added.
- Analytics: GoatCounter (`theaob.goatcounter.com`, cookie-free). Outbound card links carry
  `data-goatcounter-click` so store and download clicks show up as events.
- `favicon.svg` plus `img/favicon-32.png` and `img/apple-touch-icon.png` (the "OB" monogram).
