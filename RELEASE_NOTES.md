# Release Notes

## v2.4.2 — 2026-07-29

### Improved

- Settings Transport now switches between `PLAY` and `STOP` in real time.
- Main Transport, Settings Transport, keyboard `Space`, and Media Session share one playback state.
- Settings can start or stop playback without closing the window.
- Audio-start failure returns the interface to the stopped state.
- README now includes usage, privacy, deployment, release, and licensing guidance.
- Licensing notices were consolidated and simplified.
- `COMMERCIAL_LICENSE.md` was renamed to `COMMERCIAL_LICENSING.md`.
- Added the official project URL and commercial contact.

### Licensing

- Software: PolyForm Noncommercial License 1.0.0.
- Designated documentation: CC BY-NC 4.0.
- Commercial use: prior written permission required.
- `1.0595` brand identifiers: excluded from Creative Commons licensing.

## v2.4.1 — 2026-07-29

### Improved

- Moved the version number to the right of the `1.0595` wordmark and reduced its visual weight.
- Changed the CIS from brighter signal blue to a restrained Deep Navy and Muted Steel Blue palette.
- Maintained strong text, focus, and primary-action contrast.
- Presented Pattern, Articulation, and Sound as three parallel Track properties.
- Renamed the Track Sound shortcut from `Settings` to `Edit`.
- Added a concise `About 1.0595` CIS introduction at the beginning of Guide.
- Added a concise copyright and licensing statement at the end of Guide.
- Added GitHub Pages-ready `index.html` and `.nojekyll` files.

### Fixed

- Fixed expanded Track content being constrained at 100% browser zoom on low-height desktop windows.
- Low-height desktop layouts now use natural page scrolling instead of fixed-height clipping.
- Mobile Track rows retain full content height and scroll inside the Track list.
- Added v2.4.0 settings migration to the v2.4.1 storage key.

## v2.4.0 — 2026-07-29

### Added

- New `1.0595` product identity and navy-based CIS.
- Central Settings window with Sound, Log, Guide, and Release Notes views.
- Direct Track-to-Settings navigation.
- English operational interface with Traditional Chinese Guide content and bilingual terminology.
- Complete keyboard shortcut documentation.

### Improved

- Single central state for Main View, Settings, audio scheduling, persistence, and Log snapshots.
- Main View reduced to Tempo, TAP, Subdivision, Master Volume, Track Pattern, Articulation, and sound summaries.
- Sound settings reduced to Sound, Level, Pitch, Length, Brightness, and Noise.
- Immediate valid-input feedback and safe rejection of invalid values.
- Responsive desktop modal and full-screen mobile Settings layouts.

### Removed

- Old `¹²√2` branding.
- Nested sound-setting folds.
- Exposed synthesis details, Preview controls, automatic previews, and language switching.
