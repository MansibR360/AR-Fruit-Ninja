# AR Fruit Ninja

Slice flying fruit with your bare hands. Your webcam is the game board: fruit launches up through the live camera
feed and you cut it by swiping your hand through it. Built as a single HTML file with no build step.

**[Live demo](https://fruity-mansib.vercel.app)** (allow camera access when prompted)

## Features

- Real-time hand tracking with **MediaPipe Tasks Vision**, running fully in the browser
- Motion-detection fallback and pointer (mouse/touch) mode if the camera or hand model is unavailable
- Combo multiplier, lives (miss three and it's over), bombs, and synthesized sound effects
- Responsive HUD showing detected hands and current gesture
- Single `index.html`: no dependencies to install, nothing is uploaded, the video never leaves your device

## Run locally

Camera access needs a secure context, so serve the file over `localhost`:

```bash
npx serve .
# or: python -m http.server 8000
```

Then open the printed `http://localhost` address.

## Deploy

Static site, no build command. Deployed on Vercel.

## Tech

Vanilla JavaScript, Canvas 2D, Web Audio API, MediaPipe Hands (Tasks Vision).

## Author

Mansib Yasir