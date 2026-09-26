# omniexporter-legal

Public privacy policy pages for the OmniExporter Chrome extension
portfolio (Airbnb Listing & Comp Exporter, Trustpilot Reviews
Exporter, Ad Library Exporter for Meta, Reddit Post & Comment
Exporter, Zillow Listings Exporter), served as static HTML via GitHub Pages.

This repo exists separately from the extensions' own source repos so
those can stay private while these pages — which need to be publicly
reachable by Chrome Web Store's review crawler, not just by a signed-in
human — stay public. Each extension's own `PRIVACY.md` /
`privacy_policy_artifact.html` is the source of truth for wording;
these files are kept in sync with those by hand when either changes.

Previously these were published as Claude Artifacts, which turned out
to return a JS-only loading shell (no policy text, `noindex, nofollow`)
to an unauthenticated crawler — that caused both the Airbnb and
Trustpilot Chrome Web Store submissions to be rejected for an
unreachable/invalid privacy policy link. Static HTML on GitHub Pages
doesn't have that problem.

Live URLs (once Pages is enabled, source: main branch, root):
- `https://omniexporter-ctrl.github.io/omniexporter-legal/airbnb-privacy.html`
- `https://omniexporter-ctrl.github.io/omniexporter-legal/trustpilot-privacy.html`
- `https://omniexporter-ctrl.github.io/omniexporter-legal/meta-privacy.html`
- `https://omniexporter-ctrl.github.io/omniexporter-legal/reddit-privacy.html`
- `https://omniexporter-ctrl.github.io/omniexporter-legal/zillow-privacy.html`
