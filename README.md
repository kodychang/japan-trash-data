# japan-trash-data

Monthly-refreshed waste-collection data pack for the Japan Trash Guide iOS app.

- `datapack.json` — schema v1. Cities replace/extend the app's bundled data;
  `districts` carry chōme-level collection days (see the app repo's
  `Tools/ward2json/` for the build pipeline and per-ward status).
- Current district-level coverage: 江戸川区 (136), 渋谷区 (52), 文京区 (33).
- Sources: municipal open data (5374.jp CSV) and ward-office 収集曜日 PDFs,
  verified before publishing. Days can change — always confirm with your ward
  for anything critical.

The app fetches the raw URL of `datapack.json` at most once every 30 days.
