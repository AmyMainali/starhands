# starhands

A hand-tracked star sandbox in the browser. Your webcam reads both hands and you play with a sky of little hand-drawn stars: grab them, launch new ones, gather and throw them, and draw constellations. Stars bounce off each other and chime.

**Live:** https://amymainali.github.io/starhands

## Gestures

**One hand**

| Gesture | What it does |
|---|---|
| ☝ Point | Aim. Brackets lock onto the nearest star |
| 🤏 Pinch on a star | Pick it up and move it. Flick and release to throw |
| 🤏 Pinch on empty sky | Pull back like a slingshot, release to launch a new star |
| ✋ Open palm | Push stars away |
| ✊ Fist | Gather stars into a glowing ball. Open your hand to throw them |

**Two hands**

| Combo | What it does |
|---|---|
| ✊ + ☝ | Draw constellations: the pointing finger links every star it touches |
| ☝ + ☝ | Stars swirl after your fingertips |
| 🤏 + 🤏 | Grab the whole sky: twist to rotate, pull apart to zoom |
| 👏 Clap | Shockwave |

## Features

- Night mode (moonlit duotone camera) and day mode (bright camera)
- Sound made live with the Web Audio API
- Mouse mode for trying it without a camera: drag stars, drag the sky to use the slingshot, hold Space / X / L / F, use the scroll wheel, press Q

## Run locally

The camera needs https or localhost, so opening the file directly won't work. Serve the folder instead:

```bash
npx serve .
```

Hand tracking uses [MediaPipe Hand Landmarker](https://ai.google.dev/edge/mediapipe/solutions/vision/hand_landmarker), which runs entirely in your browser. Video never leaves your device.
