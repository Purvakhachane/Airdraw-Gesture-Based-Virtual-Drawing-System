# Air Draw ✋🎨

A vision-based drawing application that lets you draw on screen using only your hand and webcam — no mouse or stylus needed.

> **This is a modified version of [arefmalek/airdraw](https://github.com/arefmalek/airdraw).**  
> Changes made by [@hira-ishtiaq](https://github.com/hira-ishtiaq):
> - Fixed MediaPipe compatibility for version 0.10.x (updated `solutions` API usage)
> - Tested and set up for Windows with Python 3.10

---

## Demo

![Demo of all functionality: Draw, Hover, Erase, and Translate](./demo_gifs/demo.gif)

---

## Setup (Windows)

### 1. Clone the repo
```bash
git clone https://github.com/hira-ishtiaq/airdraw.git
cd airdraw
```

### 2. Create a virtual environment
```bash
py -3.10 -m venv venv
venv\Scripts\activate
```

### 3. Install dependencies
```bash
pip install opencv-python mediapipe numpy matplotlib
```

### 4. Run the app
```bash
py -3.10 airdraw.py
```

> **Note:** This project requires Python 3.10. MediaPipe does not yet support Python 3.12+.

---

## Gestures

| Gesture | Fingers | Action |
|---|---|---|
| ☝️ Hover | Index finger only | Move around without drawing |
| ✌️ Draw | Index + Middle fingers | Draw on screen |
| 🤟 Erase | Index + Middle + Ring fingers | Erase drawings within radius |
| 🤘 Translate | Index + Pinky fingers | Move existing shapes |

---

## Tech Stack

- **Python 3.10**
- **MediaPipe** — real-time hand landmark detection
- **OpenCV** — camera feed and rendering
- **NumPy** — linear algebra for gesture recognition

---

## Original Project

This is based on [arefmalek/airdraw](https://github.com/arefmalek/airdraw) by Aref Malek.  
Read the original [blog post](https://arefmalek.github.io/blog/Airdraw/) for a deeper technical writeup.

---

## License

This project is licensed under the [Mozilla Public License 2.0](LICENSE.md) — same as the original project.