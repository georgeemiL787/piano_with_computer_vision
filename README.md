# Paper Piano (Drawn Piano with OpenCV)

## Overview

Paper Piano lets you play a virtual piano by drawing a keyboard on a piece of paper. Using your webcam and computer vision (OpenCV), the app detects your drawn piano and your finger touches, playing real piano sounds for each key.

- **Draw a rectangle and dots for keys on paper**
- **Point your camera at the paper**
- **Touch the dots to play notes**

---

> **🎬 Demo Video:** Want to see it in action? [Download and watch the demo video here!](./Demo%20Video.mp4)

---

## Features
- Real-time piano key detection using OpenCV
- Play sounds by touching drawn dots
- Adjustable detection settings via a control panel
- Easy setup and cross-platform (Windows, Mac, Linux)

---

## Quick Start

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/paper-piano.git
cd paper-piano
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
pip install mediapipe
```

### 3. Prepare Your Paper Piano
- Use a blank sheet of white paper.
- Draw a **rectangle** (this is the piano area).
- Inside the rectangle, draw **dots** (with a black marker/pen) for each piano key you want (e.g., 7 dots for a C-major scale).

**Example:**

```
+-----------------------+
|   o  o  o  o  o  o  o |
|                       |
|                       |
+-----------------------+
```

- Make sure the dots are bold and clearly visible.

### 4. Run the Application
```bash
python paper-piano/main.py
```

### 5. Play!
- Point your webcam at the paper so the rectangle and all dots are visible.
- Use the control panel to adjust detection settings if needed.
- When the dots are detected and labeled, press **"Freeze Points"** in the control panel.
- Touch the dots with your fingers to play notes!

---

## Troubleshooting

- **No sound?**
  - Make sure your `sounds/` folder contains piano sound files (e.g., `1.wav`, `2.wav`, ...).
  - Check your speakers/headphones and system volume.
  - Try running `pip install playsound` if you see sound errors.

- **Dots not detected?**
  - Use a darker marker/pen for the dots.
  - Adjust the blur and Canny thresholds in the control panel.
  - Ensure good lighting and minimal glare.

- **App closes immediately?**
  - Make sure your webcam is connected and not used by another app.

---

## Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.

---

## License

MIT License. See [LICENSE](LICENSE) for details. 
