# 1.0595 — GitHub Pages Update

Version: v3.0.0-beta.3 · RevO

## Upload these files to the GitHub Pages publishing root

- `index.html`
- `manifest.webmanifest`
- `sw.js`
- `favicon.svg`
- `favicon-32.png`
- `apple-touch-icon.png`
- `icon-192.png`
- `icon-512.png`
- `icon-maskable-512.png`
- `.nojekyll`

`VERSION.txt` is optional.

If GitHub Pages is configured as **main / root**, upload these files to the repository root.
If Pages publishes from `/docs`, place all of them together inside `/docs`.

## Phone home-screen icon

### iPhone / iPad
1. Open the GitHub Pages URL in **Safari**.
2. Tap **Share**.
3. Choose **Add to Home Screen**.
4. Keep the name `1.0595` and tap **Add**.

Safari uses `apple-touch-icon.png`.

### Android
1. Open the GitHub Pages URL in **Chrome**.
2. Open the menu.
3. Choose **Install app** or **Add to Home screen**.

Chrome uses `manifest.webmanifest` and the 192/512 icons.

## Important after updating

A service worker caches the app for faster/offline reopening.
After replacing an older version on GitHub Pages:
- refresh the page once after deployment;
- if the old version remains, close/reopen the installed app or reload once online.

The cache name changes with this release, so beta.3 replaces the older cached shell automatically.

## Grid-fit change

The 4×4 pad width is now calculated from the **actual `.pad-stage` width and height** at runtime.
This avoids slight overflow caused by:
- browser address/tool bars,
- Windows display scaling,
- browser zoom,
- laptop viewports shorter than the nominal screen resolution.

## Existing data

beta.3 reads beta.2 as a legacy storage source, so existing local settings migrate forward.
