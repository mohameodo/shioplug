# shioplug

Public theme packs for Shiopa.

## Allowed

- Theme color packs
- Accent / palette packs
- Icon set packs
- Language / locale packs

## Not allowed

- Custom stream sources
- Stream / scraper / extractor plugins
- Anything that fetches or plays third-party video URLs

Shiopa will not load stream or source plugins from this repo or anywhere else.

## Pack format

Each pack is a folder under `packs/`:

```
packs/
  night-extra/
    pack.toon
    README.md
```

`pack.toon` example:

```
id: night-extra
name: Night Extra
kind: theme
version: 1.0.0
theme: night
accent: "#7C9CFF"
