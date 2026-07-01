# 3D Particle Gestures

A stunning, interactive 3D particle visualization web application built with **Three.js** and **MediaPipe Hands** for real-time hand-gesture tracking.

![Aesthetic Preview](https://images.unsplash.com/photo-1618005182384-a83a8bd57fbe?auto=format&fit=crop&w=1200&q=80)

## ✨ Features

- **Interactive 3D Particles:** Uses custom WebGL shaders to render soft glowing particle structures.
- **Real-Time Hand Tracking:** Integrates MediaPipe Hands to capture hand landmarks from your webcam. Opening and closing (pinching) your hand morphs and expands the particle structures dynamically.
- **Visual Templates:**
  - ❤️ Hearts
  - 🌸 Flowers
  - 🪐 Saturn
  - 🧘 Buddha
  - 🎆 Fireworks
- **Custom Color Palette:** Dynamic color picker to change particle glow colors on the fly.
- **Robust Fallback Mode:** No webcam? No problem! The app automatically switches to **Manual Mode** if camera permissions are blocked or unavailable:
  - Use the **Manual Pinch** slider in the control panel.
  - Press and hold the **`[Spacebar]`** to pinch, and release it to relax.

## 🚀 Running Locally

Because webcam tracking and ES module import maps require a secure context, the page should be served over `http://localhost` rather than opened directly as a file.

1. Clone this repository (or download the files).
2. Start a local development server in the project folder:
   ```bash
   # Using Python
   python -m http.server 8000

   # Or using Node.js
   npx http-server -p 8000
   ```
3. Open your browser and navigate to:
   👉 **[http://localhost:8000](http://localhost:8000)**

## 🛠️ Built With

- [Three.js](https://threejs.org/) - 3D WebGL library
- [MediaPipe Hands](https://developers.google.com/mediapipe/solutions/vision/hand_landmarker) - Real-time hand tracking
- Vanilla HTML5 / CSS3 / ES Modules
