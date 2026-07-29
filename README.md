# 1.0595

A precise four-track browser metronome for editable beat positions, per-event articulation, and per-track synthesized sound.

- **Current version:** v2.4.2
- **Web app:** <https://reivax1412.github.io/1.0595/>
- **Official project:** <https://github.com/Reivax1412/1.0595>

## Highlights

- 10–1000 BPM with Tap Tempo
- Four independent Tracks
- Editable Split positions within each beat
- Normal, Tenuto, Accent, Marcato, and Staccato events
- Per-track Sound, Level, Pitch, Length, Brightness, and Noise
- Synchronized Main and Settings Transport controls
- Append-only local Log with optional settings snapshots
- JSON Log import and export
- Responsive desktop and mobile layouts
- Single-file, offline-capable application

## Use

### Online

Open the GitHub Pages site:

<https://reivax1412.github.io/1.0595/>

### Offline

Download the release ZIP, extract it, and open `1.0595-v2.4.2.html` in a modern browser. No installation or network connection is required.

## Main controls

- **START / STOP:** controls playback from the Main View
- **TAP:** estimates Tempo from repeated taps
- **Subdivision:** applies common beat divisions
- **Pattern:** accepts comma-separated positions from `0` to less than `1`
- **Articulation:** click an event to cycle its articulation
- **Edit:** opens the selected Track directly in Sound Settings

The Settings header provides a synchronized dynamic Transport:

- Stopped → `PLAY`
- Playing → `STOP`

## Keyboard shortcuts

| Shortcut | Action |
|---|---|
| `Space` | Start or stop playback |
| `T` | Tap Tempo |
| `Arrow Up / Down` | Tempo ±1 |
| `Shift + Arrow Up / Down` | Tempo ±5 |
| `Esc` | Close Settings |
| `Enter / Space` on an Articulation event | Cycle Articulation |
| `Delete / Backspace` on an Articulation event | Reset to Normal |

Global shortcuts do not run while an input, select, textarea, button, or link has focus.

## Data and privacy

1.0595 stores settings and Log entries locally in the browser.

- Settings: `localStorage`
- Log: IndexedDB, with `localStorage` fallback
- Analytics: none
- Cookies: none
- User accounts: none
- Application-level data transmission: none

JSON import and export are processed locally by the browser.

## GitHub Pages

The repository root is ready for branch-based GitHub Pages deployment:

```text
index.html
.nojekyll
README.md
LICENSE.md
COMMERCIAL_LICENSING.md
CIS.md
RELEASE_NOTES.md
TEST_REPORT_v2.4.2.md
```

Configure GitHub Pages to deploy from `main` and `/(root)`. Every push to the publishing source updates the site.

## Project files

- `index.html` — GitHub Pages entry point
- `1.0595-v2.4.2.html` — versioned offline application
- `LICENSE.md` — software and documentation licensing
- `COMMERCIAL_LICENSING.md` — commercial-use contact and scope
- `CIS.md` — concise visual identity guidance
- `RELEASE_NOTES.md` — version history
- `TEST_REPORT_v2.4.2.md` — verification results

## Development

Developed and maintained by **WENGJINGDE**. Generative AI is used solely as an assisting tool; product direction, review, integration, testing, and maintenance are performed by the project owner.

The application uses no external JavaScript libraries, web fonts, images, or audio samples. Sound is synthesized locally with the Web Audio API.

## Licensing

- **Software:** PolyForm Noncommercial License 1.0.0
- **Designated documentation:** CC BY-NC 4.0
- **Commercial use:** separate written permission required
- **Brand identifiers:** excluded from Creative Commons licensing

See [LICENSE.md](LICENSE.md) and [COMMERCIAL_LICENSING.md](COMMERCIAL_LICENSING.md).

Commercial licensing contact: **xavierweng.1912@gmail.com**

© 2026 WENGJINGDE
