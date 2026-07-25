# 🍉 Gesture Fruit Slicer

A Fruit Ninja-style game controlled entirely by hand gestures — no mouse, no keyboard, no controller. Just point your webcam at yourself and slice the fruit flying across the screen with your fingertip.

Built with plain HTML, CSS, and JavaScript, using [MediaPipe Hands](https://github.com/google/mediapipe) for real-time hand tracking straight from the browser.

## ✨ Features

- **Webcam-based gesture control** — tracks your index fingertip in real time and turns its motion into a slicing blade
- **Two-hand support** — slice with either hand, or both at once
- **Physics-based fruit** — fruit launches, arcs, and falls under gravity, scaled to reach near the top of your screen
- **Combo scoring** — chain slices together for multiplier bonuses
- **Bombs** — slice one and it's game over; everything else is fair game with unlimited lives
- **Juice particle effects & score popups** for satisfying feedback on every slice

## 🎮 How to Play

1. Open the game in a browser (Chrome or Edge recommended) and allow camera access when prompted
2. Show your hand(s) to the camera
3. Swipe your index finger through the fruit as it flies up the screen
4. Score points on every slice — chain slices quickly for combo bonuses
5. Avoid the bombs 💣 — slicing one ends the game

## 🛠️ Tech Stack

- **HTML5 Canvas** for rendering the game
- **MediaPipe Hands** (via CDN) for real-time hand landmark detection
- **Vanilla JavaScript** — no frameworks, no build step

## 🚀 Running Locally

This is a single self-contained HTML file — no installation or build process required.

**Option 1 — Open directly**
Double-click `index.html` to open it in your browser.

**Option 2 — Local server (recommended)**
Some browsers restrict camera access on `file://` URLs, so a local server avoids permission quirks:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000` in your browser.

## 📋 Requirements

- A webcam
- A modern browser (Chrome or Edge recommended for best WebRTC/WASM performance)
- An internet connection (to load MediaPipe from its CDN on first run)

## 🙏 Acknowledgements

Inspired by a gesture-controlled Fruit Ninja demo built via vibe coding, showing how AI-assisted development can turn a laptop webcam into a full game controller.