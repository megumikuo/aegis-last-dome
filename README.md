# Aegis Last Dome

A retro browser space shooter. One static page plus its soundtrack and PWA icons; no build step.

## Music

- `ready.mp3` loops on the title, hangar and game-over screens.
- `music.mp3` plays during waves.
- Boss waves (every 5th) and every wave from 10 on get a tense mix: the main loop sped up with a pulsing bass. To use a dedicated boss track instead, add the file and set `TRACKS.boss` in `index.html`.
- Open the game over http, not `file://`, or the browser falls back to the built-in placeholder chiptune. `python3 -m http.server` is enough.

## Deploy on Vercel

    npx vercel --prod
Deploys automatically from the main branch on GitHub.
