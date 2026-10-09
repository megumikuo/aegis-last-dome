# Aegis Last Dome

A retro browser space shooter. One static page plus its soundtrack and PWA icons; no build step.

## Music

- `ready.mp3` loops on the title, hangar and game-over screens.
- `music.mp3` plays during waves.
- `boss.mp3` plays on boss waves (every 5th) and on every wave from 10 on. If it fails to load, the game falls back to the main loop sped up with a pulsing bass.
- Open the game over http, not `file://`, or the browser falls back to the built-in placeholder chiptune. `python3 -m http.server` is enough.

## Deploy on Vercel

    npx vercel --prod
Deploys automatically from the main branch on GitHub.
