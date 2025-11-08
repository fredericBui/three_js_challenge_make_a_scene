# 🧩 Three.js Scene Challenge — *Add Your Own 3D Model!*

Welcome to the **"Make a Scene" Three.js Challenge**!  
Your mission is simple: **add your own 3D model** (OBJ, STL, or GLB) into the existing scene.  
This challenge is designed to help you learn how to import and position 3D models using Three.js.

---

## 🚀 Challenge Goal

Enhance the existing 3D environment by importing **at least one additional 3D model** into the scene.  
You can use a model in any of the following formats:
- `.obj`
- `.stl`
- `.glb` / `.gltf`

Your model should:
- Be **visible** in the scene.
- Be **well-positioned and scaled** relative to the existing objects (alchemy table and tavern chair).
- Use a **material or color** that fits the scene’s medieval tavern theme.

---

## 🧱 Provided Setup

The base project includes:
- A **Three.js** scene with lighting, floor, and walls.
- Two 3D models already loaded:  
  - 🧪 `AlchemyTable.stl`  
  - 🪑 `tavern_chair.stl`
- Basic **OrbitControls** for camera movement.
- Real-time info display (camera position, object positions, etc.).

---

## 📦 Project Structure

```
📁 project-root/
│
├── index.html              # Main scene file (your code goes here)
│
├── 📁 3D_models/
│   ├── AlchemyTable.stl
│   ├── tavern_chair.stl
│   └── your_model_here.stl or .obj or .glb
│
├── 📁 textures/
│   └── 70332393-brown-oak-parquet-texture-seamless.jpg
│
└── README.md
```

---

## 🛠️ Instructions

1. **Open `index.html`** in a code editor.  
2. Choose the appropriate loader depending on your model format:
   - `.stl` → `STLLoader`
   - `.obj` → `OBJLoader`
   - `.glb` or `.gltf` → `GLTFLoader` (you may need to import it)
     ```js
     import { GLTFLoader } from 'three/addons/loaders/GLTFLoader.js';
     ```
3. **Load your model** by following the examples already in the file (see how the alchemy table and tavern chair are imported).
4. **Position and scale** your model so it fits nicely in the room.
   ```js
   myModel.position.set(x, y, z);
   myModel.scale.set(s, s, s);
   myModel.rotation.x = -Math.PI / 2;
   ```
5. **Test and tweak** until it looks good in the rendered scene.

---

## 💡 Optional Enhancements

- Add **a custom light** (e.g., point light above your object).
- Apply a **texture** to your model’s material.
- Add an **animation** (e.g., rotation or movement).
- Use **shadows** for realism:  
  ```js
  myModel.castShadow = true;
  myModel.receiveShadow = true;
  ```

---

## 🎯 Completion Checklist

✅ Scene loads without errors  
✅ Your new model appears correctly  
✅ Proper scale, position, and rotation  
✅ Model fits the theme and interacts naturally with lighting  
✅ Code is clean and readable  

---

## 🖼️ Example Ideas

- 🗡️ Sword on the table  
- 🪄 Magic staff leaning on a wall  
- 📜 Scroll or book on the floor  
- 🕯️ Candle with a glowing light  
- 🍺 Tankard or bottle on the table  

---

## 🧠 Learning Objectives

By completing this challenge, you’ll practice:
- Importing 3D models into a Three.js scene
- Managing materials, lighting, and textures
- Positioning and scaling objects
- Understanding scene composition in 3D space

---

## ⚙️ How to Run Locally

You **must serve the files from a local web server** (not by double-clicking the HTML file) because of CORS restrictions.

- Install the **Live Server** extension in VSCode.
- Right-click `index.html` → “**Open with Live Server**”.

Then open your browser at [http://localhost:8080](http://localhost:8080).

---

## 🏁 Submission

When you’re done:
- Commit your changes.
- Include your model file in the `3D_models` folder.
- Make sure everything runs locally.

---

**Good luck!**  
🎨 *Show off your creativity and bring your own touch to the tavern scene!*
