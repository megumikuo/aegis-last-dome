# Aegis Last Dome

A retro browser space shooter. One static page plus its soundtrack and PWA icons; no build step.

## Music

- `ready.mp3` loops on the title, hangar and game-over screens.
- `music.mp3` plays during waves.
- `boss.mp3` plays on the wave 5 boss.
- `boss2.mp3` plays on every wave from 10 on, the late game. It was converted from Suno's Opus-in-M4A download so Safari can play it.
- If a boss track fails to load, the game uses the other one, then the main loop sped up with a pulsing bass.
- Open the game over http, not `file://`, or the browser falls back to the built-in placeholder chiptune. `python3 -m http.server` is enough.

## Promo

`promo.mp4` is a 15-second vertical trailer cut from real gameplay with HyperFrames. Its project lives outside git in `promo-video/`.

## Deploy on Vercel

    npx vercel --prod
Deploys automatically from the main branch on GitHub.
