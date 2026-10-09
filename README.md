# Aegis Last Dome

A static site. No build step.

- `index.html` is the games shelf.
- `aegis-last-dome/` is the game: one page, its soundtrack, and the icons and manifest that let it be added to a phone's home screen.
- `vercel.json` forces a trailing slash on folder URLs. The game loads `music.mp3` by relative path, so `/aegis-last-dome/` must keep its slash.

## Deploy on Vercel

From this folder:

    npx vercel --prod

To use a custom domain, add it under the Vercel project's Settings → Domains and create the CNAME record Vercel shows at your DNS provider.

## Adding another game

Put it in its own folder and copy the `<article class="game">` block in `index.html`.
