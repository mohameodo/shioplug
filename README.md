# shioplug

Public packs for Shiopa. Themes, accents, languages, icons, dock presets, look/layout, subtitles, and HTTPS stream source plugins.

## Allowed

- Themes (full palettes)
- Accents
- Language packs
- Icon libraries (`iconTheme` and optional remote PNG `icons` map)
- Dock order presets
- Card / look tokens (poster radius, dock radius)
- Home layout prefs
- Subtitle look presets
- Stream `source` / `stream` / `scraper` packs (HTTPS addonBase or streamTemplate only — no executable code)

## Not allowed

Arbitrary JS scrapers, local file URLs, or non-HTTPS endpoints.

## Catalog

`https://raw.githubusercontent.com/mohameodo/shioplug/main/catalog.json`

## Pack kinds

| kind | Purpose |
| --- | --- |
| theme | Color palette |
| accent | Accent color |
| language | Locale strings |
| icon | Dock/icon style library |
| dock | Tab order preset |
| card / look | Poster and dock rounding |
| layout | Home shelf visibility |
| subtitle | Subtitle size/color/background |
| source / stream / scraper | Extra Watch servers via HTTPS JSON |

### Source pack shape

```json
{
  "id": "source-example",
  "name": "Example",
  "kind": "source",
  "version": "1.0.0",
  "serverName": "Example",
  "addonBase": "https://addon.example/manifest",
  "mediaTypes": ["movie", "series"],
  "idMode": "tmdb"
}
```

Or `streamTemplate`: `https://api.example/stream?tmdb={tmdb}&type={type}&s={s}&e={e}` returning `{ "streams": [ { "url": "https://..." } ] }`.

Install / update / remove from **Shioplug** in the app.
