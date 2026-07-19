# Foldout Appcast

Public Sparkle update feed for [Foldout](https://github.com/teobouancheau/foldout-app) (a private macOS app).

Only `appcast.xml` lives here — it advertises version numbers and EdDSA signatures.
The signed DMG assets stay in the private app repo's GitHub Releases and are
downloaded by the app with an authenticated request (GitHub PAT injected at
download time by `SparkleDelegate`). Publishing the feed here lets Sparkle fetch
it over `https` without embedding any credential.

Updated automatically by `scripts/release.sh` in the app repo.
