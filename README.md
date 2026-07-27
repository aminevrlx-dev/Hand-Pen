# Hand Pen — Gesture Drawing

A browser-based gesture drawing application that transforms your index finger into a virtual pen. Draw in mid-air using your webcam with no installation, backend, or additional software required.

---

# **DESCRIPTION**

Hand Pen lets you draw naturally by tracking your hand through your webcam using MediaPipe Hands. Your index finger becomes a virtual brush, allowing you to create glowing golden strokes on a dark canvas. The app includes undo/redo functionality, automatic stroke smoothing, mobile support, and a clean minimalist interface inspired by moonlight aesthetics.

---

# **SYSTEM REQUIREMENTS**

- **Browser:** Chrome or Edge (recommended), Firefox
- **Hardware:** Webcam
- **Internet Connection:** Required to load MediaPipe models on first launch
- **Local Server:** Required (cannot run directly from a local HTML file)

---

# **INSTALLATION AND SETUP**

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/HandPen.git
cd HandPen
```

### 2. Start a local server

The application uses ES modules and webcam permissions, so it must run through HTTP.

Install the **Live Server** extension in VS Code and click **Go Live**.

### 3. Open in your browser

```
http://localhost:5500
```

Allow camera access when prompted.

---

# **PROJECT STRUCTURE**

```
HandPen/
├── index.html        # Main application
├── assets/           # Optional assets
└── README.md
```

---

# **CONTROLS**

| Action | Control |
|---|---|
| Draw (Desktop) | Hold **Shift** while moving your index finger |
| Draw (Mobile) | Point your index finger toward the camera |
| Undo | **Z** key or Undo button (mobile) |
| Redo | **X** key or Redo button (mobile) |
| Clear Canvas | **Spacebar** |

---

# **APPLICATION LOGIC**

1. Open the application and allow webcam access.
2. The app detects your hand using MediaPipe Hands.
3. Your index finger is tracked in real time with smoothing for fluid movement.
4. On desktop, hold **Shift** to start drawing.
5. On mobile devices, drawing starts automatically when your finger is detected.
6. Each stroke is stored independently, allowing undo and redo operations.
7. Rotate your phone horizontally for the best experience.

---

# **FEATURES**

- ✨ Real-time hand tracking
- 🌙 Elegant dark interface
- ✏️ Air drawing with your finger
- 📱 Mobile and desktop support
- ↶ Undo / Redo system
- 🎯 Smoothed pointer movement
- 🚫 No account required
- 💻 Runs entirely in the browser
- ⚡ No backend needed
- 🎨 Glowing golden brush effect

---

# **TECH STACK**

- **MediaPipe Hands** — Real-time hand landmark detection
- **MediaPipe Camera Utils** — Webcam integration
- **Canvas 2D API** — Drawing and rendering
- **JavaScript (Vanilla ES6)** — Application logic
- **HTML5 & CSS3** — User interface

All external dependencies are loaded through CDN.

---

# **TROUBLESHOOTING GUIDE**

### **Camera doesn't start**

Make sure no other application (Zoom, Teams, Discord, OBS, etc.) is currently using your webcam.

---

### **Hand is not detected**

Ensure:

- Your hand is fully visible.
- The room has adequate lighting.
- Your webcam is clean.
- Your index finger remains inside the camera frame.

---

### **Drawing feels unstable**

Move your finger slowly and keep it within the camera view. Better lighting significantly improves tracking accuracy.

---

### **Blank screen**

Run the application from a local HTTP server instead of opening the HTML file directly.

---

### **Undo/Redo doesn't work**

Undo and redo only apply after at least one completed stroke has been created.

---

# **BROWSER COMPATIBILITY**

| Browser | Support |
|---|---|
| Chrome | ✅ Recommended |
| Microsoft Edge | ✅ Recommended |
| Firefox | ✅ Compatible |
| Safari | ⚠ Limited |
| Mobile Chrome | ✅ Supported |
| Mobile Safari | ⚠ Limited |

---

# **FUTURE IMPROVEMENTS**

- Multiple brush colors
- Brush size adjustment
- Gesture-based color selection
- Save drawing as PNG
- Background customization
- Eraser gesture
- Multi-hand drawing
- Pressure simulation
- Fullscreen mode
- Layer support

---

# **LICENSE**

MIT License — Free to use, modify, and distribute.
