# Test Report — 1.0595 v3.1.0-beta.1 · RevU

Date: 2026-08-12

## Passed
- JavaScript parses with Node `--check`.
- Service worker parses with Node `--check`.
- `manifest.webmanifest` is valid JSON.
- ZIP archive passes integrity test.
- All 115 DOM IDs from v3.0.0-beta.6 RevR remain present.
- No CJK characters detected in the application HTML; software UI remains English.
- Legacy Pattern migration defaults missing `barLength` / `beatCount` to 4 / 4.
- 2/4 model: 1920 ticks/bar, 960 ticks/beat.
- 3/4 model: 2880 ticks/bar, 960 ticks/beat.
- 4/4 model: 3840 ticks/bar, 960 ticks/beat.
- 6/8 model: 2880 ticks/bar, 480 ticks/beat.
- 6/8 Beat 2 / Split 3 / Point 2 maps to 640 ticks.
- Shuffle candidate pools contain unique musical times and at least 16 legal positions for all supplied meter presets.
- PWA application-shell paths all exist.

## Browser E2E limitation
A complete headless Chromium interaction/layout run could not be completed in this execution environment because organization policy blocks both `file://` and localhost navigation in Chromium. This is an environment limitation, not a passing browser-runtime result. Real-device testing is still required before promoting this beta to a stable release.
