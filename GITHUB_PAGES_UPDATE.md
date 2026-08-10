# 1.0595 — GitHub Pages Update

Version: v3.0.0-beta.5 · RevQ

## Main change
This package updates the app icon set to the selected fourth concept: the minimal pulse-pad icon.

Updated assets:
- favicon-32.png
- favicon.svg
- apple-touch-icon.png
- icon-192.png
- icon-512.png
- icon-maskable-512.png

## Upload
Replace the files in the GitHub Pages publishing root with all files from this package.

Current recommended Pages source:
- Branch: `main`
- Folder: `/(root)`

## Cache / installed app
The service-worker cache name is now `1.0595-v3.0.0-beta.5`, so the new deployment supersedes beta.4.

After deployment:
1. Open the website once while online.
2. Refresh once.
3. If the old icon remains on the home screen, remove the old shortcut / installed app and add it again.

Existing beta.4 local settings migrate into beta.5.
