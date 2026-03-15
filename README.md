# Interactive Hand-Tracking Particle System ✨

A fully functional, single-file HTML web application that features a real-time, interactive 3D particle system. This project leverages your webcam to track hand gestures, allowing you to dynamically control particle scaling and expansion, all rendered beautifully in the browser!

An interactive 3D particle system built with Three.js and Google's MediaPipe for real-time hand tracking via webcam. Users can dynamically manipulate shapes—like spheres, hearts, and flowers—and colors using finger-distance gestures for intuitive, physics-based control within a sleek glassmorphism UI. Perfect for creative web-based experiments.

## ✨ Features

- 👋 **Real-Time Hand Tracking:** Powered by MediaPipe. The system calculates the tension of your hand (open vs. closed) to control the expansion and scaling of the particle cloud.
- 🌌 **Rich 3D Graphics:** Built with Three.js using custom shaders to render thousands of performant, glowing particles.
- 🔄 **Shape Morphing:** Smoothly morph the 8,000 particles between different intricate templates using Tween.js:
  - 💖 Heart
  - 🌸 Flower
  - 🪐 Saturn
  - 🧘 Buddha Silhouette
  - 🎆 Fireworks
- 🎨 **Real-time Color Customization:** Pick and change the particle color instantly with the built-in color picker.
- ⚡ **Zero Setup:** It's all contained in a single `index.html` file. No build steps, no bundlers!

## 🚀 How to Run

Because modern browsers restrict webcam access for local files on the `file://` protocol, you will need to serve this file using a local web server.

### Option 1: Using Python (Recommended)
1. Open your terminal/command prompt in the directory containing `index.html`.
2. Run the following command:
   ```bash
   python -m http.server 8000
   ```
3. Open your browser and navigate to `http://localhost:8000`.

### Option 2: Using VS Code
1. Install the **Live Server** extension in Visual Studio Code.
2. Open `index.html` in VS Code.
3. Click "Go Live" in the bottom right corner of the window.

### Option 3: Using Node.js
If you have Node.js installed, you can use `http-server`:
```bash
npx http-server
```

**Note:** When the page loads, your browser will prompt you for camera access. You must **Allow** camera permissions for the interactive hand-tracking to function.

## 🛠️ Technology Stack

- **Vanilla HTML / CSS / JavaScript**
- **[Three.js](https://threejs.org/)** - 3D rendering and custom shaders
- **[MediaPipe Hands](https://developers.google.com/mediapipe/solutions/vision/hand_landmarker)** - Machine learning models for real-time hand-tracking
- **[Tween.js](https://github.com/tweenjs/tween.js/)** - Smooth mathematical interpolations for shape morphing

## 🎮 How to Interact

1. Put your hand up to your webcam so it is fully visible.
2. Wait for the UI to indicate "Hands Detected - Gestures Active".
3. **Open and spread your hand** to expand and enlarge the particle system.
4. **Close your hand into a fist** to contract and shrink the particle system.
5. Watch the particles organically float and react to your gestures!

---

*Built locally with modern web AI tools.*
