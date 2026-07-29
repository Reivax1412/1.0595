# 1.0595 v2.4.2 Test Report

Test date: 2026-07-29

## Result

- Browser integration checks: **55 / 55 passed**
- Native IndexedDB Log write/read: **passed**
- JavaScript syntax check: **passed**
- Browser page errors: **none detected**
- Console errors: **none detected**

## Verified

### Transport

- Main View starts and stops playback.
- Settings Transport changes from `PLAY` to `STOP` while playing.
- Settings Transport changes from `STOP` to `PLAY` when stopped.
- Main View and Settings remain synchronized.
- Keyboard `Space` updates both Transport controls.
- Settings View changes do not stop playback.

### Inputs and real-time response

- BPM and Tap Tempo
- Master Volume synchronization
- Split parsing, sorting, validation, and state protection
- Articulation cycling
- Sound, Level, Pitch, Length, Brightness, and Noise
- Preset reset behavior
- Real-time Track summary updates
- Playback-time parameter updates

### Input and output

- Log commit and append-only deletion markers
- JSON Log import and export
- Local settings serialization
- IndexedDB persistence with localStorage fallback
- v2.3.2 and v2.4.1 settings migration

### Layout

- Desktop fixed workspace
- Low-height desktop natural scrolling at 100% browser zoom
- Full-screen mobile Settings
- Mobile horizontal-overflow protection

## Static checks

- Single-file application
- No external JavaScript libraries
- No external web fonts, images, or audio samples
- No Analytics or application-level network data transmission
- No duplicate active Transport state

## Limitation

Automated tests verify state changes, scheduling paths, browser execution, input/output, and responsive layout. Final sound character and relative loudness should still be checked manually with the intended headphones or speakers.
