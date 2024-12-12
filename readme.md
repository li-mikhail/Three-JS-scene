# Three.js Donut Scene

### To see a live demo of this project, [click here](https://three-js-scene.vercel.app/).

This project is a **3D scene** created using **Three.js**. It showcases dynamic text and randomly placed 3D donuts with a customizable camera angle and donut count via a GUI interface.

---

## Features

- **3D Text Rendering**: Displays the text in the scene.
- **Dynamic Donut Generation**: Randomly places torus-shaped donuts in the 3D space.
- **GUI Controls**: Allows real-time adjustments to:
  - **Camera Angle**: Modify the field of view (FOV) of the perspective camera.
  - **Donut Count**: Increase or decrease the number of donuts in the scene.
- **Responsive Design**: Adjusts the canvas size when the browser window is resized.
- **Orbit Controls**: Navigate the scene interactively using the mouse.

---

## Installation

1. Clone the repository:
   ```bash
   git clone git@github.com:li-mikhail/Three-JS-scene.git
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```

4. Open your browser and navigate to:
   ```
   http://localhost:3000
   ```

---

## File Structure

```
├── src
│   ├── index.html         # Entry point for the project
│   ├── main.js            # Main JavaScript file (contains Three.js code)
│   ├── textures           # Folder for texture assets
│   │   └── matcaps        # Matcap textures for 3D materials
│   └── fonts              # Folder for font files
├── .gitignore             # Git ignore file
├── vite.config.js         # Vite configuration file
└── package.json           # Project dependencies and scripts
```

---

## Dependencies

- [Three.js](https://threejs.org/): A JavaScript library for 3D rendering.
- [lil-gui](https://github.com/georgealways/lil-gui): A lightweight GUI library.

---

## Controls

The project includes a GUI for live interaction:

- **Camera Angle**: Adjusts the field of view (30-130 degrees).
- **Donut Count**: Sets the number of donuts in the scene (100-300).

To access the GUI, use the floating interface in the top-right corner of the viewport.

---

## How It Works

1. **Text Rendering**:
   - A 3D text object is created using `TextGeometry` and rendered with a Matcap material.

2. **Donut Generation**:
   - Donuts are created using `TorusGeometry` and randomly placed in 3D space.
   - The GUI allows dynamic updates to the number of donuts by removing the existing ones and adding new ones.

3. **Camera and Renderer**:
   - A perspective camera is used with adjustable FOV.
   - The renderer ensures high performance and adapts to window size changes.

---

## Credits

- **Three.js** for the 3D rendering library.
- **lil-gui** for the GUI control interface.

