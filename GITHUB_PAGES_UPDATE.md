# 1.0595 — GitHub Pages Update

Version: v3.0.0-beta.6 · RevR

## Mobile adaptive-grid fix
This release changes how phone pad sizing works. The app no longer trusts the CSS grid row height on mobile. Instead, it reads the live Visual Viewport and subtracts the measured interface elements around the pad stage, then solves the largest 4×4 grid that fits both available width and height.

It also performs a second viewport-boundary check after layout. If browser rounding or a dynamic address bar still causes clipping, the grid is reduced once more.

Triggers include:
- Visual Viewport resize
- Visual Viewport scroll / browser chrome movement
- window resize
- orientation change
- ResizeObserver
- pageshow

## Version / cache
- App: v3.0.0-beta.6
- Package: RevR
- Service-worker cache: `1.0595-v3.0.0-beta.6`
- beta.5 local settings migrate forward.

The installed PWA now checks for a new service worker on load and reloads once when the new worker takes control.

## Upload
Upload all files in this package to the GitHub Pages root.
Pages source should remain:
- `main`
- `/(root)`
