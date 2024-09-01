# Three.js

3 things important to Three.js

- Scene (Scene graph)
  - Allows you to set up, in 3D coordinates, what is to be rendered by Three.js
  - Scene extends Object3D.
- Camera
  - Describes **Frustum** to be rendered. Frustum is the dimensions inside the scene.
  - **Perspective camera** mimics the way the human eye sees. Common projection mode used when rendering 3D scenes.
  - **Orthographic camera**
- Renderer

`OrbitControls` allows you to change angles of objects.

## Coordinate

Negative x is left and positive x is right of the screen.

Positive z is closer to you, nd negative z is further away.

Positive y is up, and negative y is down.

## Sky box

```
const scene = new THREE.Scene();
scene.background = new THREE.CubeTextureLoader()
  .setPath("https://sbcode.net/img/")
  .load(["px.png", "nx.png", "py.png", "ny.png", "pz.png", "nz.png"]);
```

## TypeScript

In JavaScipt, you can make things up, invent things, that's what they call **dynamically typed**. Whereas TypeScript is predominantly statically typed, meaning we have to be correct. TypeScript enforces that I'm doing correctly. TypeScript is more strict than JavaScript.

## Dat GUI

GUI to interact with Three.js

`npm install dat.gui@latest --save-dev`

`npm install @types/dat.gui@latest --save-dev`
