# Changelog

All notable changes to this fork are documented here. Format based on
[Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

Downstream fork of [`Big-Xan/adaptive_plant`](https://github.com/Big-Xan/adaptive_plant).
`main` tracks upstream unchanged; fork work lands on `testing`. Entries below are
the changes this fork carries on top of upstream.

## [Unreleased] — fork divergence from `Big-Xan/adaptive_plant`

### Added
- **Image upload in the config & options flows** — pick a photo from your device
  (HEIC supported, EXIF orientation corrected, JPEG/PNG) instead of only entering
  a `/local/...` path. Uploaded images are persisted under `/local/adaptive_plant/`
  and cleaned up when replaced or disabled. Takes priority over the path field.

### Notes
- The per-plant **care-instructions** feature originally carried here was dropped
  on 2026-06-23: upstream shipped its own implementation (v19.2), so we now use
  upstream's. Image upload is the only remaining local-only feature.
