# Shilalekh — Inscription & Heritage Explorer

A bright, responsive static website prototype for exploring inscription records.

## Features
- Search by inscription name, place, era, script, or description
- Filter by India / World and sort results
- Selected-record detail panel
- Interactive Leaflet map with OpenStreetMap tiles and available approximate coordinates
- Open map, directions, and nearby-attraction links
- Personal heritage trail (session-only)
- Translation tool using MyMemory's public translation endpoint (internet required; availability and language coverage vary)
- Browser text-to-speech where supported by the device
- Responsive mobile layout and custom favicon

## Run locally
Because the site loads `data/inscriptions.json`, run it through a local web server rather than opening `index.html` directly.

For example, if Python is installed:
```bash
python -m http.server 8000
```
Then visit `http://localhost:8000`.

## Deploy on GitHub Pages
1. Create a GitHub repository.
2. Upload `index.html`, `favicon.svg`, and the `data/` folder.
3. In repository Settings → Pages, select the branch and root folder.
4. Save and open the published Pages URL.

## Data scope and accuracy
The included starter catalogue contains 80 curated entries (30 India and 50 World). It is not yet a verified 1,000-record catalogue. Some locations are approximate or missing. Dates, readings, translations, and historical interpretations should be checked against museum catalogues, epigraphic corpora, or scholarly editions before academic use. The website intentionally does not invent translations for ancient inscriptions.

## Notes
- The map and translation services need an internet connection.
- Audio voices depend on browser/device voice support.
- The current heritage trail is stored in memory for the current session only.
