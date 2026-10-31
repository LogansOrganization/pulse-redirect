# pulse.solarnebulae.com

The Pulse web pages, served by GitHub Pages at pulse.solarnebulae.com.

- `daily/` is the web version of today's daily puzzle, and where shared results link (`/daily/?d=N`).
  It's a copy of `pulse/daily/` on loganchobson.github.io (still there for links from older builds);
  its puzzle code must match `game/src/Polarity/Puzzle.cpp`, so copy it again after changing either.
- `privacy/index.html` is the privacy policy linked from the Play Store listing and the game. It's a
  copy of `site/pulse/privacy/index.html` in the game repo; copy it again after changing it there.
- `.well-known/assetlinks.json` is the app-links file for `com.solarsky.pulse`. Android fetches it
  from this host to let shared daily links open the app. `.nojekyll` makes Pages serve dot-folders.
- `app-ads.txt` lists the AdMob publisher. AdMob reads it from the root domain, so the
  solarnebulae.com site has a copy too.
- `index.html` and `404.html` send visitors to today's daily.
