# pulse.solarnebulae.com

Forwards pulse.solarnebulae.com to the Pulse pages on loganchobson.github.io/pulse/,
keeping the path and query (a shared daily is `/daily/?d=N`). `404.html` is the same page,
so any path forwards.

`.well-known/assetlinks.json` is the app-links file for `com.solarsky.pulse` (same as the one on
loganchobson.github.io). Android fetches it from this host to let shared daily links open the app,
so it has to be served here directly, not redirected. `.nojekyll` makes Pages serve dot-folders.
