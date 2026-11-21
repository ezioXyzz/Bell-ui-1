# Ezioz E-Bell — School Operations Console

A desktop-first, static web prototype for a school's electronic bell control room. It uses the supplied school photograph as a full-bleed, cover-cropped background with a dark glass treatment; the original image ratio is preserved. Red, blue, and green are the primary system accents.

## Run locally

Serve this directory from a local HTTP server (do not open `index.html` directly, because browser asset and script behavior is more consistent over HTTP):

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080` in a browser. The layout is designed for desktop monitors and adapts for smaller screens.

## Included interactions

- Overview clock, next-bell countdown, scheduler toggle, timeline, activity log, and quick actions.
- Schedule presets, weekday assignment, editable event rows, holiday chips, and save feedback.
- Manual soundboard, simulated playback states, and emergency lockout.
- Sound library table, missing-file state, preview controls, and Windows directory integration placeholders.
- PIN-gated Advanced Settings (demo PIN `1234`), speaker controls, CSV activity-log export, and an always-available Emergency Stop/reset.
- Hover, active, toast, floating, and entrance animations with a `prefers-reduced-motion` fallback.

Audio playback and Windows-specific integrations are prototype simulations; connect the native Windows audio engine and filesystem APIs for production operation. No user data is sent to a server.
