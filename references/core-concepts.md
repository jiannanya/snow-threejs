# Three.js Core Concepts

## Minimal Scene Template

```js
import * as THREE from 'three';

// 1. Scene — container for all objects
const scene = new THREE.Scene();

// 2. Camera — PerspectiveCamera(fov, aspect, near, far)
const camera = new THREE.PerspectiveCamera(75, window.innerWidth / window.innerHeight, 0.1, 1000);
camera.position.set(0, 2, 5);

// 3. Renderer
const renderer = new THREE.WebGLRenderer({ antialias: true });
renderer.setSize(window.innerWidth, window.innerHeight);
renderer.setPixelRatio(window.devicePixelRatio);
document.body.appendChild(renderer.domElement);

// 4. Mesh = Geometry + Material
const geometry = new THREE.BoxGeometry(1, 1, 1);
const material = new THREE.MeshStandardMaterial({ color: 0x00ff88 });
const mesh = new THREE.Mesh(geometry, material);
scene.add(mesh);

// 5. Light
const light = new THREE.DirectionalLight(0xffffff, 1);
light.position.set(5, 5, 5);
scene.add(light);
scene.add(new THREE.AmbientLight(0x404040));

// 6. Render loop
renderer.setAnimationLoop(() => {
  mesh.rotation.y += 0.01;
  renderer.render(scene, camera);
});

// 7. Resize handler
window.addEventListener('resize', () => {
  camera.aspect = window.innerWidth / window.innerHeight;
  camera.updateProjectionMatrix();
  renderer.setSize(window.innerWidth, window.innerHeight);
});
```

## Key Classes

| Class | Purpose |
|-------|---------|
| `THREE.Scene` | Root container, fog, background |
| `THREE.PerspectiveCamera` | Frustum projection |
| `THREE.OrthographicCamera` | Orthographic projection |
| `THREE.WebGLRenderer` | WebGL rendering |
| `THREE.WebGPURenderer` | WebGPU rendering (new) |
| `THREE.Mesh` | Renderable object (geometry + material) |
| `THREE.Group` | Container / transform parent |
| `THREE.Object3D` | Base class with position/rotation/scale |

## Coordinate System

- Y-up, right-handed
- `.position` — Vector3
- `.rotation` — Euler (default order: XYZ)
- `.quaternion` — Quaternion (alternative to Euler)
- `.scale` — Vector3

## Scene Graph

Objects form a parent-child hierarchy via `parent.add(child)`.
Child transforms are relative to parent.

## Renderer Settings

```js
renderer.shadowMap.enabled = true;
renderer.shadowMap.type = THREE.PCFSoftShadowMap;
renderer.toneMapping = THREE.ACESFilmicToneMapping;
renderer.toneMappingExposure = 1.0;
renderer.outputColorSpace = THREE.SRGBColorSpace;
```

## Camera Controls Pattern

```js
import { OrbitControls } from 'three/addons/controls/OrbitControls.js';
const controls = new OrbitControls(camera, renderer.domElement);
controls.enableDamping = true;
// Call controls.update() in render loop
```

## Helpers

```js
scene.add(new THREE.AxesHelper(5));        // X=red, Y=green, Z=blue
scene.add(new THREE.GridHelper(10, 10));   // ground grid
scene.add(new THREE.CameraHelper(camera)); // camera frustum
```
