# Pairing Room

An installable web app for pairing paint colours and previewing them in a living room, kitchen or bedroom.

## Files
- `index.html`: the whole app (colours, room drawings, logic)
- `manifest.webmanifest`, `icons/`: lets phones install it to the home screen
- `sw.js`: makes it work offline after the first visit
- `.nojekyll`: stops GitHub Pages processing the files

## Put it online with GitHub Pages
1. Create a new repository on GitHub, e.g. `pairing-room`.
2. Upload everything in this folder (keep the `icons` folder).
3. In the repo go to **Settings → Pages**, set Source to **Deploy from a branch**, choose `main` and `/ (root)`, then Save.
4. After a minute it's live at `https://<your-username>.github.io/pairing-room/`.

## Or with Netlify
Drag this folder onto https://app.netlify.com/drop.

## Install on a phone
- iPhone (Safari): Share → Add to Home Screen.
- Android (Chrome): menu → Install app.

## Updating
After editing `index.html`, change `VERSION` at the top of `sw.js` (e.g. `pairing-room-v2`) so installed copies pick up the change.

## Trying it locally
Service workers need a web server, so run `python3 -m http.server` in this folder and open http://localhost:8000.

## Before going public
Colour names and numbers belong to Farrow & Ball and the hex values are unofficial approximations. Before a public launch, consider switching to an original palette or getting permission.
