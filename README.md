# HEXVYR website

Public product showcase for [HEXVYR](https://github.com/clementGilardy/hexvyr), hosted on GitHub Pages.

**Published URL:** https://clementgilardy.github.io/hexvyr-website/

This site supports Riot Games Production API application review. It describes the desktop companion; it is not a web version of the app.

## Contents

| Path | Purpose |
|------|---------|
| `index.html` | Product page |
| `privacy.html` | Privacy / data-handling information |
| `styles.css` | Shared styles (no build step) |
| `fonts/` | Self-hosted OFL fonts (Syne, Source Sans 3) |
| `riot.txt` | Riot Developer Portal ownership verification — **do not rename or edit** |
| `favicon.svg` | Site icon |

## Local preview

No build tools are required.

```powershell
# From this repository root
python -m http.server 8080
# or
npx --yes serve .
```

Then open `http://localhost:8080/` (or the port printed by the server).

Because GitHub Pages serves the project under `/hexvyr-website/`, prefer relative links (already used) when adding pages or assets.

## Publishing

1. Commit changes on `main`.
2. Push to `origin`.
3. GitHub Pages is configured to deploy from the `main` branch root.
4. Wait for the Pages build, then check:
   - https://clementgilardy.github.io/hexvyr-website/
   - https://clementgilardy.github.io/hexvyr-website/privacy.html
   - https://clementgilardy.github.io/hexvyr-website/riot.txt

## Maintenance notes

- Keep product claims aligned with the shipped desktop app. Do not invent features, screenshots, download links, or contact addresses.
- There is currently **no public release** and **no public support email**; the product page states that explicitly.
- Do not add analytics, cookies, or third-party trackers.
- Preserve `riot.txt` filename and exact contents so Riot verification keeps working.
- Fonts are licensed under the SIL Open Font License (see upstream [google/fonts](https://github.com/google/fonts) OFL packages for Syne and Source Sans 3).

## Related issue

Product-site requirements: [hexvyr#237](https://github.com/clementGilardy/hexvyr/issues/237).
