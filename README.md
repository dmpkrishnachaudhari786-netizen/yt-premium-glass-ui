# YT Premium Glass UI — PWA

A glassmorphism YouTube Premium UI demo, packaged as an installable, offline-capable Progressive Web App.

## What it is

A single-page UI demo that layers floating "glass" panels over a simulated YouTube environment:

- **Smart command button (FAB)** — opens the Session Analytics dashboard.
- **Session Analytics dashboard** — live watch-time timer, videos watched, shorts watched and shorts skipped.
- **Shorts Feed panel** — draggable (mouse and touch), collapsible, with a "Simulate Next Short" action that updates likes/comments and the session count.

Everything runs locally in the browser. There is no backend, no API key and no tracking.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The whole app — markup, styles and logic in one self-contained file. |
| `manifest.json` | PWA manifest (name, icons, standalone display, theme colours). |
| `sw.js` | Service worker — pre-caches the app shell and serves it offline. |
| `icons/` | App icons: 192, 512, maskable 512 and Apple touch icon. |

## Install as an app

Open the live URL in Chrome (Android) or Safari (iOS) and choose **Add to Home screen** / **Install app**. It then launches full-screen and works without a network connection.

## Notes

- The design is intentionally self-contained: no Tailwind CDN or web-font requests, so the app renders identically offline.
- The Shorts panel is a floating overlay by design — drag it anywhere on the screen.
