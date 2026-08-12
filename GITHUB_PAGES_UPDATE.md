# 1.0595 — v3.1.0-beta.1 · RevU

## Major update

### Event interaction
- Tap: toggle one Event.
- Swipe: paint or erase Events.
- Long press (500 ms, stationary): open Event Edit.
- Multi-pointer gestures are tracked independently.
- Desktop right-click is an equivalent Event Edit shortcut.

### Pattern time
Each Pattern now stores:
- `barLength` (quarter-note units)
- `beatCount`

Presets: 2/4, 3/4, 4/4, 6/8, plus Custom.
The scheduler uses each Pattern's own bar duration. Pattern queues switch only at a bar boundary.

### Transport
- START: play or resume.
- PAUSE: preserve musical position.
- STOP: stop and return to bar start.

### Tools
- Controlled Shuffle: randomizes active Event positions only; Event sound/articulation/retrig identity remains attached.
- One-step Undo for Shuffle Track, Clear Track, Clear Pattern, and Bar Structure.

### Cross-device contract
Phone, tablet, laptop, and desktop use the same data model and feature semantics. Layout density can differ, but no feature is intentionally removed by device class.

### Deployment
Upload all files to the GitHub Pages publishing root (`main / (root)`). The service-worker cache key is `1.0595-v3.1.0-beta.1`.
