# Three.js 3D Graphics Skill Library

> **Language**: English | [中文](./README_cn.md)

> **Version**: Three.js r167 (npm `0.167.1`) · **Renderer**: WebGL / WebGPU · **Modules**: ES Modules via CDN importmap

This skill library provides 20 ready-to-run HTML examples and 7 reference documents, covering the complete Three.js development knowledge base from basic scene setup to advanced shaders.

---

## Example Screenshot Gallery

### Beginner Examples

<table>
<tr>
<td align="center" width="25%">
<a href="./examples/hello-cube.html"><img src="./images/hello-cube.png" width="100%"></a><br>
<b>Hello Cube</b><br><sub>Basic rotating cube · Scene setup</sub>
</td>
<td align="center" width="25%">
<a href="./examples/geometries.html"><img src="./images/geometries.png" width="100%"></a><br>
<b>Geometries</b><br><sub>All built-in geometry types</sub>
</td>
<td align="center" width="25%">
<a href="./examples/materials.html"><img src="./images/materials.png" width="100%"></a><br>
<b>Materials</b><br><sub>11 material types compared</sub>
</td>
<td align="center" width="25%">
<a href="./examples/lights.html"><img src="./images/lights.png" width="100%"></a><br>
<b>Lights</b><br><sub>5 light source types demo</sub>
</td>
</tr>
<tr>
<td align="center" width="25%">
<a href="./examples/shadows.html"><img src="./images/shadows.png" width="100%"></a><br>
<b>Shadows</b><br><sub>Shadow mapping &amp; soft/hard shadows</sub>
</td>
<td align="center" width="25%">
<a href="./examples/axes-helpers.html"><img src="./images/axes-helpers.png" width="100%"></a><br>
<b>Axes Helpers</b><br><sub>AxesHelper · GridHelper · ArrowHelper · BoxHelper</sub>
</td>
<td align="center" width="25%">
<a href="./examples/wireframe-mode.html"><img src="./images/wireframe-mode.png" width="100%"></a><br>
<b>Wireframe Mode</b><br><sub>Solid · WireframeGeometry · EdgesGeometry</sub>
</td>
<td align="center" width="25%">
<a href="./examples/groups-hierarchy.html"><img src="./images/groups-hierarchy.png" width="100%"></a><br>
<b>Groups &amp; Hierarchy</b><br><sub>Parent-child transforms · Solar system</sub>
</td>
</tr>
<tr>
<td align="center" width="25%">
<a href="./examples/vertex-colors.html"><img src="./images/vertex-colors.png" width="100%"></a><br>
<b>Vertex Colors</b><br><sub>Per-vertex color painting · HSL/Gradient/Noise</sub>
</td>
<td align="center" width="25%">
<a href="./examples/transparent-blend.html"><img src="./images/transparent-blend.png" width="100%"></a><br>
<b>Transparency &amp; Blending</b><br><sub>opacity · NormalBlend · AdditiveBlend</sub>
</td>
<td align="center" width="25%">
<a href="./examples/clock-easing.html"><img src="./images/clock-easing.png" width="100%"></a><br>
<b>Clock &amp; Easing</b><br><sub>THREE.Clock · 6 easing functions</sub>
</td>
<td align="center" width="25%">
<a href="./examples/background-modes.html"><img src="./images/background-modes.png" width="100%"></a><br>
<b>Background Modes</b><br><sub>Solid · Gradient · CubeMap backgrounds</sub>
</td>
</tr>
<tr>
<td align="center" width="25%">
<a href="./examples/simple-physics.html"><img src="./images/simple-physics.png" width="100%"></a><br>
<b>Simple Physics</b><br><sub>Gravity · Elastic bounce · Wall collision</sub>
</td>
<td align="center" width="25%">
<a href="./examples/multi-viewport.html"><img src="./images/multi-viewport.png" width="100%"></a><br>
<b>Multi Viewport</b><br><sub>Split-screen scissor · Perspective + Ortho</sub>
</td>
<td align="center" width="25%">
<a href="./examples/css2d-labels.html"><img src="./images/css2d-labels.png" width="100%"></a><br>
<b>CSS2D Labels</b><br><sub>CSS2DRenderer · 3D projected planet labels</sub>
</td>
<td></td>
</tr>
</table>

### Intermediate Examples

<table>
<tr>
<td align="center" width="25%">
<a href="./examples/textures.html"><img src="./images/textures.png" width="100%"></a><br>
<b>Textures</b><br><sub>Procedural Canvas textures</sub>
</td>
<td align="center" width="25%">
<a href="./examples/orbit-controls.html"><img src="./images/orbit-controls.png" width="100%"></a><br>
<b>Orbit Controls</b><br><sub>Interactive camera controller</sub>
</td>
<td align="center" width="25%">
<a href="./examples/particles.html"><img src="./images/particles.png" width="100%"></a><br>
<b>Particles</b><br><sub>50k particle system</sub>
</td>
<td align="center" width="25%">
<a href="./examples/raycasting.html"><img src="./images/raycasting.png" width="100%"></a><br>
<b>Raycasting</b><br><sub>Mouse picking &amp; highlight</sub>
</td>
</tr>
<tr>
<td align="center" width="25%">
<a href="./examples/animation-mixer.html"><img src="./images/animation-mixer.png" width="100%"></a><br>
<b>Animation Mixer</b><br><sub>Keyframe animation system</sub>
</td>
<td align="center" width="25%">
<a href="./examples/morph-targets.html"><img src="./images/morph-targets.png" width="100%"></a><br>
<b>Morph Targets</b><br><sub>Vertex morph animation</sub>
</td>
<td align="center" width="25%">
<a href="./examples/instanced-mesh.html"><img src="./images/instanced-mesh.png" width="100%"></a><br>
<b>Instanced Mesh</b><br><sub>100k instances, single draw call</sub>
</td>
<td align="center" width="25%">
<a href="./examples/fog-skybox.html"><img src="./images/fog-skybox.png" width="100%"></a><br>
<b>Fog &amp; Skybox</b><br><sub>Fog effects &amp; atmospheric sky</sub>
</td>
</tr>
<tr>
<td align="center" width="25%">
<a href="./examples/gltf-loader.html"><img src="./images/gltf-loader.png" width="100%"></a><br>
<b>GLTF Loader</b><br><sub>Load 3D model files</sub>
</td>
<td align="center" width="25%">
<a href="./examples/sprite-billboard.html"><img src="./images/sprite-billboard.png" width="100%"></a><br>
<b>Sprite Billboard</b><br><sub>Sprites &amp; billboard labels</sub>
</td>
<td align="center" width="25%">
<a href="./examples/curve-path.html"><img src="./images/curve-path.png" width="100%"></a><br>
<b>Curve Path</b><br><sub>CatmullRomCurve3 · TubeGeometry · path following</sub>
</td>
<td align="center" width="25%">
<a href="./examples/shape-extrude.html"><img src="./images/shape-extrude.png" width="100%"></a><br>
<b>Shape Extrude</b><br><sub>THREE.Shape · ExtrudeGeometry · bevel</sub>
</td>
</tr>
<tr>
<td align="center" width="25%">
<a href="./examples/lod.html"><img src="./images/lod.png" width="100%"></a><br>
<b>LOD</b><br><sub>THREE.LOD · level-of-detail by distance</sub>
</td>
<td align="center" width="25%">
<a href="./examples/cube-camera.html"><img src="./images/cube-camera.png" width="100%"></a><br>
<b>Cube Camera</b><br><sub>Live environment reflections · CubeCamera</sub>
</td>
<td align="center" width="25%">
<a href="./examples/water-surface.html"><img src="./images/water-surface.png" width="100%"></a><br>
<b>Water Surface</b><br><sub>ShaderMaterial wave displacement · foam</sub>
</td>
<td align="center" width="25%">
<a href="./examples/outline-select.html"><img src="./images/outline-select.png" width="100%"></a><br>
<b>Outline Select</b><br><sub>OutlinePass · click/hover selection highlight</sub>
</td>
</tr>
<tr>
<td align="center" width="25%">
<a href="./examples/render-target.html"><img src="./images/render-target.png" width="100%"></a><br>
<b>Render Target</b><br><sub>WebGLRenderTarget · off-screen security camera</sub>
</td>
<td align="center" width="25%">
<a href="./examples/skeleton-anim.html"><img src="./images/skeleton-anim.png" width="100%"></a><br>
<b>Skeleton Animation</b><br><sub>SkinnedMesh · Bone hierarchy · skinning</sub>
</td>
<td align="center" width="25%">
<a href="./examples/normal-map.html"><img src="./images/normal-map.png" width="100%"></a><br>
<b>Normal Map</b><br><sub>Procedural normal maps · surface detail</sub>
</td>
<td align="center" width="25%">
<a href="./examples/audio-visualizer.html"><img src="./images/audio-visualizer.png" width="100%"></a><br>
<b>Audio Visualizer</b><br><sub>Web Audio FFT → 3D bar visualization</sub>
</td>
</tr>
</table>

### Advanced Examples

<table>
<tr>
<td align="center" width="25%">
<a href="./examples/custom-shader.html"><img src="./images/custom-shader.png" width="100%"></a><br>
<b>Custom Shader</b><br><sub>Custom GLSL shaders</sub>
</td>
<td align="center" width="25%">
<a href="./examples/postprocessing.html"><img src="./images/postprocessing.png" width="100%"></a><br>
<b>Post-processing</b><br><sub>EffectComposer pipeline</sub>
</td>
<td align="center" width="25%">
<a href="./examples/environment-map.html"><img src="./images/environment-map.png" width="100%"></a><br>
<b>Environment Map</b><br><sub>PMREM lighting &amp; reflections</sub>
</td>
<td align="center" width="25%">
<a href="./examples/tsl-shader.html"><img src="./images/tsl-shader.png" width="100%"></a><br>
<b>TSL Shader</b><br><sub>Node-based shader system</sub>
</td>
</tr>
<tr>
<td align="center" width="25%">
<a href="./examples/webgpu-basics.html"><img src="./images/webgpu-basics.png" width="100%"></a><br>
<b>WebGPU Basics</b><br><sub>WebGPU renderer + fallback</sub>
</td>
<td align="center" width="25%">
<a href="./examples/procedural-terrain.html"><img src="./images/procedural-terrain.png" width="100%"></a><br>
<b>Procedural Terrain</b><br><sub>Multi-octave noise · heightmap · height coloring</sub>
</td>
<td align="center" width="25%">
<a href="./examples/text-3d.html"><img src="./images/text-3d.png" width="100%"></a><br>
<b>3D Text</b><br><sub>FontLoader · TextGeometry · bevel · animation</sub>
</td>
<td align="center" width="25%">
<a href="./examples/fat-lines.html"><img src="./images/fat-lines.png" width="100%"></a><br>
<b>Fat Lines</b><br><sub>Line2 · LineMaterial · configurable width · dashed</sub>
</td>
</tr>
<tr>
<td align="center" width="25%">
<a href="./examples/sky-atmosphere.html"><img src="./images/sky-atmosphere.png" width="100%"></a><br>
<b>Sky Atmosphere</b><br><sub>Sky shader · sun position · Rayleigh scattering</sub>
</td>
<td align="center" width="25%">
<a href="./examples/procedural-city.html"><img src="./images/procedural-city.png" width="100%"></a><br>
<b>Procedural City</b><br><sub>Random buildings · street grid · night lights</sub>
</td>
<td align="center" width="25%">
<a href="./examples/shader-extend.html"><img src="./images/shader-extend.png" width="100%"></a><br>
<b>Shader Extend</b><br><sub>onBeforeCompile · GLSL injection · 5 effects</sub>
</td>
<td align="center" width="25%">
<a href="./examples/depth-of-field.html"><img src="./images/depth-of-field.png" width="100%"></a><br>
<b>Depth of Field</b><br><sub>BokehPass · EffectComposer · focus control</sub>
</td>
</tr>
<tr>
<td align="center" width="25%">
<a href="./examples/texture-atlas.html"><img src="./images/texture-atlas.png" width="100%"></a><br>
<b>Texture Atlas</b><br><sub>Sprite sheet · UV offset animation · billboards</sub>
</td>
<td align="center" width="25%">
<a href="./examples/particle-emitter.html"><img src="./images/particle-emitter.png" width="100%"></a><br>
<b>Particle Emitter</b><br><sub>Pool recycling · lifetime · fade · physics</sub>
</td>
<td align="center" width="25%">
<a href="./examples/multi-material.html"><img src="./images/multi-material.png" width="100%"></a><br>
<b>Multi Material</b><br><sub>Per-face material groups · Box/Cylinder/Cone</sub>
</td>
<td></td>
</tr>
</table>

---

## Table of Contents

- [Quick Start](#quick-start)
- [CDN Import Template](#cdn-import-template)
- [Examples](#examples)
  - [Beginner Examples](#beginner-examples)
  - [Intermediate Examples](#intermediate-examples)
  - [Advanced Examples](#advanced-examples)
- [Reference Docs](#reference-docs)
- [API Cheatsheet](#api-cheatsheet)
- [Official Resources](#official-resources)

---

## Quick Start

All examples are **standalone HTML files** — no build tools needed. Open directly in a browser.

```bash
# Serve with any HTTP server (recommended, avoids CORS issues)
npx serve .

# Or double-click the HTML file (some features require a server)
```

Minimal scene skeleton:

```html
<!DOCTYPE html>
<html>
<head><meta charset="UTF-8"></head>
<body>
<script type="importmap">
{
  "imports": {
    "three": "https://cdn.jsdelivr.net/npm/three@0.167.1/build/three.module.js",
    "three/addons/": "https://cdn.jsdelivr.net/npm/three@0.167.1/examples/jsm/"
  }
}
</script>
<script type="module">
  import * as THREE from 'three';
  import { OrbitControls } from 'three/addons/controls/OrbitControls.js';

  // 1. Scene + Camera + Renderer
  const scene    = new THREE.Scene();
  const camera   = new THREE.PerspectiveCamera(75, innerWidth / innerHeight, 0.1, 1000);
  const renderer = new THREE.WebGLRenderer({ antialias: true });
  renderer.setSize(innerWidth, innerHeight);
  document.body.appendChild(renderer.domElement);
  camera.position.z = 5;

  // 2. Add objects
  const mesh = new THREE.Mesh(
    new THREE.BoxGeometry(),
    new THREE.MeshStandardMaterial({ color: 0x44aaff })
  );
  scene.add(mesh);
  scene.add(new THREE.DirectionalLight(0xffffff, 3).position.set(5, 5, 5));

  // 3. Controls + render loop
  const controls = new OrbitControls(camera, renderer.domElement);
  renderer.setAnimationLoop(() => {
    mesh.rotation.y += 0.01;
    controls.update();
    renderer.render(scene, camera);
  });

  // 4. Responsive resize
  window.addEventListener('resize', () => {
    camera.aspect = innerWidth / innerHeight;
    camera.updateProjectionMatrix();
    renderer.setSize(innerWidth, innerHeight);
  });
</script>
</body>
</html>
```

---

## CDN Import Template

```html
<script type="importmap">
{
  "imports": {
    "three": "https://cdn.jsdelivr.net/npm/three@0.167.1/build/three.module.js",
    "three/addons/": "https://cdn.jsdelivr.net/npm/three@0.167.1/examples/jsm/"
  }
}
</script>
```

Common addon paths:

| Feature | Import Path |
|---------|------------|
| OrbitControls | `three/addons/controls/OrbitControls.js` |
| GLTFLoader | `three/addons/loaders/GLTFLoader.js` |
| DRACOLoader | `three/addons/loaders/DRACOLoader.js` |
| EffectComposer | `three/addons/postprocessing/EffectComposer.js` |
| UnrealBloomPass | `three/addons/postprocessing/UnrealBloomPass.js` |
| RGBELoader | `three/addons/loaders/RGBELoader.js` |
| Stats | `three/addons/libs/stats.module.js` |

---

## Examples

### Beginner Examples

---

#### 1. Hello Cube — Basic Rotating Cube

**File**: [`examples/hello-cube.html`](./examples/hello-cube.html)

**Demonstrates**:
- PerspectiveCamera + WebGLRenderer basic setup
- MeshStandardMaterial physically-based material
- DirectionalLight / PointLight / AmbientLight three-light setup
- EdgesGeometry wireframe overlay
- OrbitControls with damping
- Scene fog (Fog)
- Responsive resize handling

```javascript
// Core snippet: rotating cube with shadows
const geometry = new THREE.BoxGeometry(2, 2, 2);
const material = new THREE.MeshStandardMaterial({
  color: 0x4488ff, roughness: 0.4, metalness: 0.3
});
const cube = new THREE.Mesh(geometry, material);
cube.castShadow = true;
scene.add(cube);

renderer.setAnimationLoop(() => {
  cube.rotation.x += 0.005;
  cube.rotation.y += 0.01;
  renderer.render(scene, camera);
});
```

---

#### 2. Geometries — All Built-in Geometries

**File**: [`examples/geometries.html`](./examples/geometries.html)

**Demonstrates**:
- 15 built-in geometry grid display
- EdgesGeometry wireframe overlay
- Raycaster hover tooltip showing geometry name
- HSL auto-coloring

**Geometry showcase**:

| Geometry | Constructor | Key Params |
|----------|------------|-----------|
| Box | `BoxGeometry(w, h, d)` | width, height, depth |
| Sphere | `SphereGeometry(r, wSeg, hSeg)` | radius, segments |
| Cylinder | `CylinderGeometry(rTop, rBot, h)` | top/bottom radius, height |
| Cone | `ConeGeometry(r, h, seg)` | radius, height |
| Torus | `TorusGeometry(r, tube, rSeg, tSeg)` | major radius, tube radius |
| TorusKnot | `TorusKnotGeometry(r, tube, p, q)` | shape params p/q |
| Icosahedron | `IcosahedronGeometry(r, detail)` | subdivision level |
| Capsule | `CapsuleGeometry(r, len, capSeg, radSeg)` | radius, length |
| Plane | `PlaneGeometry(w, h, wSeg, hSeg)` | width, height, segments |
| Circle | `CircleGeometry(r, seg)` | radius, segments |
| Lathe | `LatheGeometry(points, seg)` | profile point array |

---

#### 3. Materials — Material Type Comparison

**File**: [`examples/materials.html`](./examples/materials.html)

**Demonstrates**:
- 11 material types side-by-side comparison
- Orbiting point light for dynamic lighting
- Projected HTML label overlay

**Material showcase**:

| Material | Characteristics | Use Case |
|----------|----------------|---------|
| `MeshBasicMaterial` | No lighting, flat color | UI elements, debug |
| `MeshNormalMaterial` | Normal visualization | Debug normals |
| `MeshLambertMaterial` | Diffuse (Gouraud) | Low-end devices |
| `MeshPhongMaterial` | Specular highlights (Phong) | Plastic, smooth surfaces |
| `MeshStandardMaterial` | PBR metalness/roughness | General physically-based |
| `MeshPhysicalMaterial` | Clearcoat/transmission/iridescence | Car paint, glass |
| `MeshToonMaterial` | Cartoon step shading | Cel shading |
| `MeshDepthMaterial` | Depth visualization | Post-processing effects |
| `wireframe` | Wireframe mode | Structure debugging |

```javascript
// PBR glass material example
const glassMat = new THREE.MeshPhysicalMaterial({
  color: 0xffffff,
  transmission: 0.95,   // transmission rate
  thickness: 0.5,        // thickness (for refraction)
  roughness: 0.05,
  ior: 1.5,              // index of refraction
  transparent: true,
});
```

---

#### 4. Lights — All Light Source Types

**File**: [`examples/lights.html`](./examples/lights.html)

**Demonstrates**:
- 5 light types, each with individual checkbox toggle
- All lights with visible Helper overlays
- Exposure slider for real-time adjustment

**Light comparison**:

| Light | Characteristics | Shadow Support |
|-------|----------------|---------------|
| `AmbientLight(color, intensity)` | Global ambient | ❌ |
| `DirectionalLight(color, intensity)` | Parallel light (sun) | ✅ |
| `PointLight(color, intensity, distance)` | Point light (bulb) | ✅ |
| `SpotLight(color, intensity, dist, angle)` | Spotlight | ✅ |
| `HemisphereLight(sky, ground, intensity)` | Sky/ground hemisphere | ❌ |
| `RectAreaLight(color, intensity, w, h)` | Rectangular area light | ❌ |

```javascript
// DirectionalLight shadow configuration
const light = new THREE.DirectionalLight(0xffffff, 2);
light.castShadow = true;
light.shadow.mapSize.width  = 2048;
light.shadow.mapSize.height = 2048;
light.shadow.camera.near = 0.5;
light.shadow.camera.far  = 50;
light.shadow.bias = -0.001;  // eliminate shadow acne
```

---

#### 5. Shadows — Shadow Mapping

**File**: [`examples/shadows.html`](./examples/shadows.html)

**Demonstrates**:
- 4 shadow types: BasicShadowMap / PCFShadowMap / PCFSoftShadowMap / VSMShadowMap
- Shadow map resolution and bias real-time adjustment
- CameraHelper to visualize shadow camera frustum

```javascript
renderer.shadowMap.enabled = true;
renderer.shadowMap.type = THREE.PCFSoftShadowMap; // recommended

// Enable cast/receive on objects
mesh.castShadow    = true;
mesh.receiveShadow = true;
```

---

### Intermediate Examples

---

#### 6. Textures — Procedural Textures

**File**: [`examples/textures.html`](./examples/textures.html)

**Demonstrates**:
- 6 procedural textures generated with Canvas 2D API (no external images)
- Checkerboard / Radial gradient / Grid / Pixel noise / HSL stripes / UV numbering
- CanvasTexture real-time update

```javascript
// Procedural checkerboard texture
function makeCheckerTex(size = 256, squares = 8) {
  const canvas = document.createElement('canvas');
  canvas.width = canvas.height = size;
  const ctx = canvas.getContext('2d');
  const cell = size / squares;
  for (let r = 0; r < squares; r++) {
    for (let c = 0; c < squares; c++) {
      ctx.fillStyle = (r + c) % 2 === 0 ? '#fff' : '#333';
      ctx.fillRect(c * cell, r * cell, cell, cell);
    }
  }
  return new THREE.CanvasTexture(canvas);
}
```

---

#### 7. Orbit Controls — Camera Controller

**File**: [`examples/orbit-controls.html`](./examples/orbit-controls.html)

**Demonstrates**:
- OrbitControls full property panel control
- Damping / auto-rotate / pan / zoom toggles
- Rotation / pan / zoom speed adjustment
- Distance limits (minDistance / maxDistance)

```javascript
import { OrbitControls } from 'three/addons/controls/OrbitControls.js';

const controls = new OrbitControls(camera, renderer.domElement);
controls.enableDamping = true;   // enable damping (inertia)
controls.dampingFactor  = 0.05;
controls.autoRotate     = true;
controls.autoRotateSpeed = 2.0;
controls.minDistance    = 2;
controls.maxDistance    = 50;
controls.maxPolarAngle  = Math.PI / 2; // prevent flipping below ground

// ⚠️ Must call in animation loop
renderer.setAnimationLoop(() => {
  controls.update(); // required!
  renderer.render(scene, camera);
});
```

---

#### 8. Particles — Particle System

**File**: [`examples/particles.html`](./examples/particles.html)

**Demonstrates**:
- 50,000 particles with real-time animation
- 4 distribution modes: Sphere / Galaxy spiral / Wave / Cube
- Particle size / speed / color controls
- AdditiveBlending additive blending

```javascript
// Points particle system
const count = 50000;
const positions = new Float32Array(count * 3);
const colors    = new Float32Array(count * 3);

for (let i = 0; i < count; i++) {
  positions[i * 3]     = (Math.random() - 0.5) * 20; // x
  positions[i * 3 + 1] = (Math.random() - 0.5) * 20; // y
  positions[i * 3 + 2] = (Math.random() - 0.5) * 20; // z
  const color = new THREE.Color().setHSL(Math.random(), 1, 0.6);
  colors[i * 3] = color.r; colors[i * 3 + 1] = color.g; colors[i * 3 + 2] = color.b;
}

const geo = new THREE.BufferGeometry();
geo.setAttribute('position', new THREE.BufferAttribute(positions, 3));
geo.setAttribute('color',    new THREE.BufferAttribute(colors, 3));

const mat = new THREE.PointsMaterial({
  size: 0.05, vertexColors: true,
  blending: THREE.AdditiveBlending, transparent: true, depthWrite: false,
});
scene.add(new THREE.Points(geo, mat));
```

---

#### 9. Raycasting — Mouse Picking

**File**: [`examples/raycasting.html`](./examples/raycasting.html)

**Demonstrates**:
- `Raycaster.setFromCamera()` mouse ray casting
- Hover highlight (emissive glow)
- Click to select + floating tooltip showing world coordinates
- Dynamic pointer cursor switching

```javascript
const raycaster = new THREE.Raycaster();
const pointer   = new THREE.Vector2();

window.addEventListener('mousemove', (e) => {
  pointer.x =  (e.clientX / innerWidth)  * 2 - 1;
  pointer.y = -(e.clientY / innerHeight) * 2 + 1;
});

// In animation loop
raycaster.setFromCamera(pointer, camera);
const hits = raycaster.intersectObjects(pickableObjects);
if (hits.length > 0) {
  const { object, point, distance } = hits[0];
  object.material.emissive.setHex(0x331122); // highlight
}
```

---

#### 10. Animation Mixer — Keyframe Animation

**File**: [`examples/animation-mixer.html`](./examples/animation-mixer.html)

**Demonstrates**:
- AnimationMixer driving multiple objects
- VectorKeyframeTrack (position)
- QuaternionKeyframeTrack (rotation)
- Play / Pause / Stop / Speed / Loop mode UI

```javascript
const mixer = new THREE.AnimationMixer(scene);

// Position keyframe track
const posTrack = new THREE.VectorKeyframeTrack(
  '.position',           // target property path
  [0, 1, 2, 3],          // time points (seconds)
  [0,0,0,  0,3,0,  0,0,0, 0,1,0]  // values (x,y,z triplets)
);

const clip = new THREE.AnimationClip('bounce', 3, [posTrack]);
const action = mixer.clipAction(clip, targetMesh);
action.setLoop(THREE.LoopRepeat, Infinity);
action.play();

// In animation loop
const delta = clock.getDelta();
mixer.update(delta);
```

---

#### 11. Morph Targets — Vertex Morphing

**File**: [`examples/morph-targets.html`](./examples/morph-targets.html)

**Demonstrates**:
- 4 morphAttribute targets: Inflate / Spike / Twist / Squash
- `morphTargetInfluences` weight sliders
- Auto-animation mode (blend multiple targets simultaneously)

```javascript
const geo = new THREE.SphereGeometry(1.5, 64, 64);

// Define morph targets (relative offsets)
const inflateDisp = new Float32Array(geo.attributes.position.count * 3);
// ... fill per-vertex offsets ...

geo.morphAttributes.position = [
  new THREE.BufferAttribute(inflateDisp, 3),
  new THREE.BufferAttribute(spikeDisp, 3),
];
geo.morphTargetsRelative = true; // relative mode

const mesh = new THREE.Mesh(geo, material);
mesh.morphTargetInfluences[0] = 0.5; // 0~1 weight
mesh.morphTargetInfluences[1] = 0.3;
```

---

#### 12. Instanced Mesh — Large-Scale Instance Rendering

**File**: [`examples/instanced-mesh.html`](./examples/instanced-mesh.html)

**Demonstrates**:
- Up to 100,000 instances, single draw call
- Per-instance independent position, rotation, scale (Matrix4)
- Per-instance independent color (setColorAt)
- FPS counter to verify performance advantage

```javascript
const count = 10000;
const iMesh = new THREE.InstancedMesh(geometry, material, count);
iMesh.instanceMatrix.setUsage(THREE.DynamicDrawUsage);

const dummy = new THREE.Object3D();
const color = new THREE.Color();

for (let i = 0; i < count; i++) {
  // Set transform matrix
  dummy.position.set(rx, ry, rz);
  dummy.rotation.set(rx, ry, 0);
  dummy.scale.setScalar(Math.random() * 2 + 0.5);
  dummy.updateMatrix();
  iMesh.setMatrixAt(i, dummy.matrix);

  // Set color
  color.setHSL(i / count, 0.8, 0.5);
  iMesh.setColorAt(i, color);
}

iMesh.instanceMatrix.needsUpdate = true;
iMesh.instanceColor.needsUpdate  = true;
scene.add(iMesh);
```

---

#### 13. Fog & Skybox — Fog Effects & Atmosphere

**File**: [`examples/fog-skybox.html`](./examples/fog-skybox.html)

**Demonstrates**:
- Linear Fog vs FogExp2 toggle comparison
- 4 sky presets (Day / Dusk / Night / Overcast)
- Forest road scene + streetlight point sources
- Auto-walking camera flythrough

```javascript
// Linear fog (full fog from none between near ~ far)
scene.fog = new THREE.Fog(0x87ceeb, 10, 80);

// Exponential fog (uniform density falloff, more natural)
scene.fog = new THREE.FogExp2(0x050514, 0.025);

// Fog color should match scene background color
scene.background = new THREE.Color(scene.fog.color);
```

---

#### 14. GLTF Loader — Load 3D Models

**File**: [`examples/gltf-loader.html`](./examples/gltf-loader.html)

**Demonstrates**:
- GLTFLoader + DRACOLoader for compressed format support
- LoadingManager progress callbacks
- Loads KhronosGroup official sample model (BoxAnimated.gltf)
- `gltf.scene` scene tree traversal display
- Model animation driven by AnimationMixer

```javascript
import { GLTFLoader  } from 'three/addons/loaders/GLTFLoader.js';
import { DRACOLoader } from 'three/addons/loaders/DRACOLoader.js';

const dracoLoader = new DRACOLoader();
dracoLoader.setDecoderPath('https://cdn.jsdelivr.net/npm/three@0.167.1/examples/jsm/libs/draco/');

const loader = new GLTFLoader();
loader.setDRACOLoader(dracoLoader);

loader.load(
  '/models/scene.gltf',
  (gltf) => {
    const model = gltf.scene;
    model.traverse(child => {
      if (child.isMesh) { child.castShadow = true; }
    });
    scene.add(model);

    // Play animations
    const mixer = new THREE.AnimationMixer(model);
    gltf.animations.forEach(clip => mixer.clipAction(clip).play());
  },
  (xhr) => console.log(`${xhr.loaded / xhr.total * 100}% loaded`),
  (err) => console.error(err)
);
```

---

#### 15. Sprite Billboard — Sprites & Billboards

**File**: [`examples/sprite-billboard.html`](./examples/sprite-billboard.html)

**Demonstrates**:
- `THREE.Sprite` always faces camera
- Three label types: Canvas text / halo particle / icon
- `sizeAttenuation` distance scaling toggle
- Planet scene demonstrating annotation system

```javascript
// Create text label sprite
function makeLabelSprite(text) {
  const canvas = document.createElement('canvas');
  canvas.width = 256; canvas.height = 64;
  const ctx = canvas.getContext('2d');
  ctx.fillStyle = 'rgba(0,40,80,0.85)';
  ctx.fillRect(0, 0, 256, 64);
  ctx.fillStyle = '#aaddff';
  ctx.font = 'bold 22px monospace';
  ctx.textAlign = 'center';
  ctx.fillText(text, 128, 38);

  const tex = new THREE.CanvasTexture(canvas);
  const mat = new THREE.SpriteMaterial({ map: tex, transparent: true });
  const sprite = new THREE.Sprite(mat);
  sprite.scale.set(2.5, 0.6, 1);
  return sprite;
}
```

---

### Advanced Examples

---

#### 16. Custom Shader — GLSL Custom Shaders

**File**: [`examples/custom-shader.html`](./examples/custom-shader.html)

**Demonstrates**:
- Full ShaderMaterial vertex/fragment shader pipeline
- 4 GLSL effect presets:
  - **Wave Displacement** — sine wave vertex offset
  - **Plasma** — multi-layer sine plasma effect
  - **Fresnel / Rim Light** — Fresnel edge glow
  - **Hologram** — scan lines + flickering hologram
- Real-time uniform passing (time / amplitude / hue)

```glsl
// Vertex shader: Wave Displacement
uniform float u_time;
uniform float u_amplitude;
varying vec2 vUv;
varying vec3 vNormal;

void main() {
  vUv = uv;
  vec3 pos = position;
  float wave = sin(pos.x * 4.0 + u_time * 3.0)
             * cos(pos.y * 4.0 + u_time * 2.5);
  pos += normal * wave * u_amplitude;
  vNormal = normalize(normalMatrix * normal);
  gl_Position = projectionMatrix * modelViewMatrix * vec4(pos, 1.0);
}
```

```javascript
// JavaScript side
const material = new THREE.ShaderMaterial({
  uniforms: {
    u_time:      { value: 0 },
    u_amplitude: { value: 0.3 },
  },
  vertexShader:   vertGLSL,
  fragmentShader: fragGLSL,
  side: THREE.DoubleSide,
});

// Update in animation loop
material.uniforms.u_time.value += clock.getDelta();
```

---

#### 17. Post-processing — Post Effects

**File**: [`examples/postprocessing.html`](./examples/postprocessing.html)

**Demonstrates**:
- Full EffectComposer pipeline
- UnrealBloomPass bloom (threshold/strength/radius controls)
- FilmPass film grain
- GlitchPass glitch art effect
- DotScreenPass dot-matrix screen
- RGBShiftShader chromatic aberration

```javascript
import { EffectComposer }  from 'three/addons/postprocessing/EffectComposer.js';
import { RenderPass }      from 'three/addons/postprocessing/RenderPass.js';
import { UnrealBloomPass } from 'three/addons/postprocessing/UnrealBloomPass.js';
import { OutputPass }      from 'three/addons/postprocessing/OutputPass.js';

const composer = new EffectComposer(renderer);
composer.addPass(new RenderPass(scene, camera));

const bloom = new UnrealBloomPass(
  new THREE.Vector2(innerWidth, innerHeight),
  1.5,   // strength
  0.4,   // radius
  0.2    // threshold
);
composer.addPass(bloom);
composer.addPass(new OutputPass()); // last pass handles tone mapping output

// Use composer instead of renderer
renderer.setAnimationLoop(() => {
  composer.render(); // ← replaces renderer.render(scene, camera)
});

// Sync update on resize
window.addEventListener('resize', () => {
  composer.setSize(innerWidth, innerHeight);
});
```

---

#### 18. Environment Map — Environment Mapping & Reflections

**File**: [`examples/environment-map.html`](./examples/environment-map.html)

**Demonstrates**:
- PMREMGenerator generating PMREM environment map from panorama
- Procedurally generated equirectangular panorama (3 sky presets)
- `scene.environment` global IBL
- Metalness/roughness gradient sphere array showcasing PBR reflections

```javascript
// Generate environment map from equirectangular panorama
const pmrem = new THREE.PMREMGenerator(renderer);
pmrem.compileEquirectangularShader();

const equirectTex = new THREE.TextureLoader().load('hdr/env.jpg', (tex) => {
  tex.mapping = THREE.EquirectangularReflectionMapping;
  const envMap = pmrem.fromEquirectangular(tex).texture;
  pmrem.dispose();
  tex.dispose();

  scene.environment = envMap;   // all MeshStandardMaterial uses automatically
  scene.background  = envMap;   // also used as sky background
});

// Load HDR file with RGBELoader
import { RGBELoader } from 'three/addons/loaders/RGBELoader.js';
new RGBELoader().load('env.hdr', (tex) => {
  const envMap = pmrem.fromEquirectangular(tex).texture;
  scene.environment = envMap;
});
```

---

#### 19. TSL Shader — Node-based Shaders

**File**: [`examples/tsl-shader.html`](./examples/tsl-shader.html)

**Demonstrates**:
- TSL (Three Shading Language) node material equivalent to GLSL mode
- 4 effects: vertex wave / Simplex noise displacement / UV gradient color / Fresnel glow
- Side-by-side comparison of TSL node graph and GLSL implementation

```javascript
// TSL syntax (requires WebGPURenderer or NodeMaterial)
import { MeshStandardNodeMaterial } from 'three/addons/nodes/materials/MeshStandardNodeMaterial.js';
import { sin, time, positionLocal, normalLocal, vec3 } from 'three/addons/nodes/tsl/TSLBase.js';

const mat = new MeshStandardNodeMaterial({ color: 0x4488ff });

// Node expression: vertex = local position + normal * sin(time) * 0.2
mat.positionNode = positionLocal.add(
  normalLocal.mul(sin(time).mul(0.2))
);
```

---

#### 20. WebGPU Basics — WebGPU Renderer

**File**: [`examples/webgpu-basics.html`](./examples/webgpu-basics.html)

**Demonstrates**:
- WebGPURenderer feature detection + automatic WebGL fallback
- Browser support status visual indicator (green=WebGPU / orange=WebGL fallback)
- Standard Three.js scene fully compatible with WebGPURenderer
- Code comments showing WebGPU initialization differences

```javascript
// WebGPU detection + fallback mode
async function createRenderer() {
  if (navigator.gpu) {
    const adapter = await navigator.gpu.requestAdapter();
    if (adapter) {
      const { default: WebGPURenderer } = await import(
        'three/addons/renderers/webgpu/WebGPURenderer.js'
      );
      const renderer = new WebGPURenderer({ antialias: true });
      await renderer.init(); // ⚠️ WebGPU requires await init()
      return renderer;
    }
  }
  // Fallback to WebGL
  return new THREE.WebGLRenderer({ antialias: true });
}

const renderer = await createRenderer();
```

> **Browser support**: Chrome 113+ / Edge 113+ support WebGPU; Firefox / Safari use WebGL fallback.

---

### New Beginner — Detail Descriptions

#### 21. Axes Helpers — Debug Helpers

**File**: [`examples/axes-helpers.html`](./examples/axes-helpers.html)

Demonstrates `AxesHelper` (RGB = XYZ axes), `GridHelper`, `ArrowHelper` (6 cardinal directions), and `BoxHelper` on rotating cubes. Toggle each helper independently with buttons.

```javascript
const axes = new THREE.AxesHelper(5); // red=X, green=Y, blue=Z
scene.add(axes);
const grid = new THREE.GridHelper(10, 10, 0x444444, 0x222222);
scene.add(grid);
const box = new THREE.BoxHelper(mesh, 0xffff00);
scene.add(box);
box.update(); // call every frame if mesh moves
```

---

#### 22. Wireframe Mode — Geometry Display Modes

**File**: [`examples/wireframe-mode.html`](./examples/wireframe-mode.html)

Compare Solid, `WireframeGeometry` (all triangle edges), and `EdgesGeometry` (hard edges only) on three different base geometries. Toggle between modes with buttons.

```javascript
// Solid mode
const solidMesh = new THREE.Mesh(geo, new THREE.MeshStandardMaterial({ color: 0x4488ff }));

// WireframeGeometry — shows every triangle edge
const wireGeo = new THREE.WireframeGeometry(geo);
const wireMesh = new THREE.LineSegments(wireGeo, new THREE.LineBasicMaterial({ color: 0x88ccff }));

// EdgesGeometry — shows only hard edges (creases > threshold angle)
const edgeGeo = new THREE.EdgesGeometry(geo);
const edgeMesh = new THREE.LineSegments(edgeGeo, new THREE.LineBasicMaterial({ color: 0xffffff }));
```

---

#### 23. Groups & Hierarchy — Parent-Child Transforms

**File**: [`examples/groups-hierarchy.html`](./examples/groups-hierarchy.html)

Solar system demonstrating nested `THREE.Group` parent-child transform inheritance. Earth orbits the Sun (child group); Moon orbits Earth (nested child). Rotations propagate down the hierarchy.

```javascript
const solarSystem = new THREE.Group();
const earthOrbit  = new THREE.Group(); // child of solarSystem
const moonOrbit   = new THREE.Group(); // child of earthOrbit

solarSystem.add(earthOrbit);
earthOrbit.add(moonOrbit);
scene.add(solarSystem);

// Each group rotation affects all children
solarSystem.rotation.y += 0.01; // rotates everything
earthOrbit.rotation.y  += 0.03; // rotates Earth + Moon around Sun
moonOrbit.rotation.y   += 0.07; // rotates Moon around Earth
```

---

#### 24. Vertex Colors — Per-vertex Color Painting

**File**: [`examples/vertex-colors.html`](./examples/vertex-colors.html)

Assigns HSL Rainbow, Gradient, or Noise colors per-vertex on a high-res `SphereGeometry`. Requires `vertexColors: true` on the material.

```javascript
const colors = [];
for (let i = 0; i < pos.count; i++) {
  const c = new THREE.Color().setHSL(i / pos.count, 1, 0.5);
  colors.push(c.r, c.g, c.b);
}
geo.setAttribute('color', new THREE.Float32BufferAttribute(colors, 3));
const mat = new THREE.MeshStandardMaterial({ vertexColors: true });
```

---

#### 25. Transparency & Blending — Blend Modes

**File**: [`examples/transparent-blend.html`](./examples/transparent-blend.html)

Five demo pairs showing: Opaque, `opacity: 0.5`, `NormalBlending`, `AdditiveBlending`, and `depthWrite: false`. Demonstrates when to use each blending mode.

```javascript
// Additive blending (glowing effects, fire, particles)
const mat = new THREE.MeshStandardMaterial({
  color: 0xff8800, transparent: true, opacity: 0.7,
  blending: THREE.AdditiveBlending, depthWrite: false,
});
```

---

#### 26. Clock & Easing — Animation Timing

**File**: [`examples/clock-easing.html`](./examples/clock-easing.html)

Uses `THREE.Clock` for dt-based timing. Shows 6 cubes each animated with a different easing function: Linear, SineIn, CubicInOut, BounceOut, ElasticOut, BackOut.

```javascript
const clock = new THREE.Clock();
renderer.setAnimationLoop(() => {
  const t = clock.getElapsedTime();
  const dt = clock.getDelta(); // time since last frame

  // Easing examples
  const linear    = t % 1;
  const sineIn    = 1 - Math.cos(t * Math.PI / 2);
  const bounceOut = bounce(t % 1); // custom bounce function
});
```

---

#### 27. Background Modes — Scene Backgrounds

**File**: [`examples/background-modes.html`](./examples/background-modes.html)

Toggle between 4 background types: solid color, canvas gradient texture, sky gradient (sunset colors), and procedural CubeMap environment. Objects always visible in foreground.

```javascript
// Gradient texture background
const canvas = document.createElement('canvas');
// ... draw gradient on canvas ...
scene.background = new THREE.CanvasTexture(canvas);

// CubeMap background
const cubeRT = new THREE.WebGLCubeRenderTarget(256);
const cubeCamera = new THREE.CubeCamera(0.1, 100, cubeRT);
scene.background = cubeRT.texture;
```

---

#### 28. Simple Physics — Manual Physics

**File**: [`examples/simple-physics.html`](./examples/simple-physics.html)

Manual gravity integration, elastic bounce off floor, wall collision detection. No external physics library required. Configurable gravity, restitution, and ball count.

```javascript
// dt-based physics integration
const dt = clock.getDelta();
ball.vy -= gravity * dt;        // apply gravity
ball.py += ball.vy * dt;        // integrate position

if (ball.py < radius) {         // floor bounce
  ball.py = radius;
  ball.vy *= -restitution;      // elastic bounce
}
```

---

#### 29. Multi Viewport — Split-screen Rendering

**File**: [`examples/multi-viewport.html`](./examples/multi-viewport.html)

Renders the same scene from two cameras using `renderer.setScissor()` and `renderer.setViewport()`. Left: `PerspectiveCamera` + `OrbitControls`. Right: `OrthographicCamera` top-down view.

```javascript
renderer.setScissorTest(true);
// Left viewport (perspective)
renderer.setScissor(0, 0, w/2, h);
renderer.setViewport(0, 0, w/2, h);
renderer.render(scene, perspCamera);
// Right viewport (orthographic)
renderer.setScissor(w/2, 0, w/2, h);
renderer.setViewport(w/2, 0, w/2, h);
renderer.render(scene, orthoCamera);
```

---

#### 30. CSS2D Labels — 3D-projected DOM Labels

**File**: [`examples/css2d-labels.html`](./examples/css2d-labels.html)

Uses `CSS2DRenderer` to overlay HTML DOM elements that project into 3D space and always face the camera. Demonstrates planet labels in an orbiting solar system.

```javascript
import { CSS2DRenderer, CSS2DObject } from 'three/addons/renderers/CSS2DRenderer.js';

const labelRenderer = new CSS2DRenderer();
labelRenderer.setSize(innerWidth, innerHeight);
document.body.appendChild(labelRenderer.domElement);

const div = document.createElement('div');
div.textContent = 'Earth';
const label = new CSS2DObject(div);
planet.add(label); // label follows planet in 3D space

// In render loop:
labelRenderer.render(scene, camera);
```

---

### New Intermediate — Detail Descriptions

#### 31. Curve Path — Spline Path Following

**File**: [`examples/curve-path.html`](./examples/curve-path.html)

`CatmullRomCurve3` closed spline wrapped in `TubeGeometry`. A cone object follows the path using `curve.getPointAt(t)` and `getTangentAt(t)` for orientation. Trail particle ring buffer shows history.

```javascript
const curve = new THREE.CatmullRomCurve3(points, true); // closed=true
const tubeGeo = new THREE.TubeGeometry(curve, 200, 0.05, 8, true);

// Path following
const t = (clock.getElapsedTime() * 0.1) % 1;
const pos = curve.getPointAt(t);
const tangent = curve.getTangentAt(t);
traveler.position.copy(pos);
traveler.lookAt(pos.clone().add(tangent));
```

---

#### 32. Shape Extrude — 2D Shape to 3D

**File**: [`examples/shape-extrude.html`](./examples/shape-extrude.html)

Five shapes built with `THREE.Shape`: Star, Heart, Arrow, Gear (with hole), and Letter. All extruded with `ExtrudeGeometry` and bevel. Switch between shapes with buttons.

```javascript
const shape = new THREE.Shape();
shape.moveTo(0, 0.5);
// ... draw star outline with lineTo/bezierCurveTo ...

const extrudeSettings = {
  depth: 0.4, bevelEnabled: true,
  bevelThickness: 0.05, bevelSize: 0.04, bevelSegments: 3,
};
const geo = new THREE.ExtrudeGeometry(shape, extrudeSettings);
```

---

#### 33. LOD — Level of Detail

**File**: [`examples/lod.html`](./examples/lod.html)

`THREE.LOD` with 3 sphere levels (64/16/4 segments). A grid of LOD objects switches level automatically by camera distance. Color changes by LOD level (green=high, yellow=medium, red=low).

```javascript
const lod = new THREE.LOD();
lod.addLevel(new THREE.Mesh(new THREE.SphereGeometry(1, 64, 64), mat), 0);   // high detail
lod.addLevel(new THREE.Mesh(new THREE.SphereGeometry(1, 16, 16), mat), 8);   // medium
lod.addLevel(new THREE.Mesh(new THREE.SphereGeometry(1, 4, 4), mat), 20);    // low detail
scene.add(lod);
lod.update(camera); // call each frame
```

---

#### 34. Cube Camera — Live Reflections

**File**: [`examples/cube-camera.html`](./examples/cube-camera.html)

`WebGLCubeRenderTarget` + `CubeCamera` updates every frame for live environment reflections on a chrome sphere. The reflective object must be hidden before the cube camera update to avoid self-reflection.

```javascript
const cubeRT = new THREE.WebGLCubeRenderTarget(256, {
  generateMipmaps: true, minFilter: THREE.LinearMipmapLinearFilter,
});
const cubeCamera = new THREE.CubeCamera(0.1, 100, cubeRT);
scene.add(cubeCamera);

const mat = new THREE.MeshStandardMaterial({ envMap: cubeRT.texture, metalness: 1, roughness: 0 });

// In render loop:
chromeSphere.visible = false;  // hide to avoid self-reflection
cubeCamera.update(renderer, scene);
chromeSphere.visible = true;
```

---

#### 35. Water Surface — Shader Wave Displacement

**File**: [`examples/water-surface.html`](./examples/water-surface.html)

`ShaderMaterial` with multi-wave vertex displacement (overlapping sine waves), foam at crests, floating boats, exponential fog, and a night sky with stars. No external Water addon required.

```javascript
// Vertex shader wave displacement
vec3 newPos = position;
newPos.y += sin(position.x * 0.5 + uTime) * 0.4
           + sin(position.z * 0.3 + uTime * 1.3) * 0.3
           + sin((position.x + position.z) * 0.4 + uTime * 0.8) * 0.2;
```

---

#### 36. Outline Select — Post-process Selection

**File**: [`examples/outline-select.html`](./examples/outline-select.html)

`OutlinePass` from `EffectComposer` highlights selected objects. Click toggles blue outline selection; hover shows yellow outline. Uses `Raycaster` for hit detection.

```javascript
import { OutlinePass } from 'three/addons/postprocessing/OutlinePass.js';

const outlinePass = new OutlinePass(new THREE.Vector2(w, h), scene, camera);
outlinePass.edgeStrength = 3;
outlinePass.edgeThickness = 1;
outlinePass.visibleEdgeColor.set(0x4488ff); // blue = selected
composer.addPass(outlinePass);

outlinePass.selectedObjects = [clickedMesh]; // update on click
```

---

#### 37. Render Target — Off-screen Rendering

**File**: [`examples/render-target.html`](./examples/render-target.html)

`WebGLRenderTarget` renders the scene from a secondary camera into a texture displayed on a "monitor" plane. Demonstrates the render-to-texture pattern for portals, security cameras, mirrors.

```javascript
const renderTarget = new THREE.WebGLRenderTarget(512, 512);
const secCamera = new THREE.PerspectiveCamera(80, 1, 0.1, 100);
const monitor = new THREE.Mesh(geo, new THREE.MeshBasicMaterial({ map: renderTarget.texture }));

// In render loop:
renderer.setRenderTarget(renderTarget);
renderer.render(scene, secCamera);      // render to texture
renderer.setRenderTarget(null);
renderer.render(scene, camera);         // render to screen
```

---

#### 38. Skeleton Animation — SkinnedMesh

**File**: [`examples/skeleton-anim.html`](./examples/skeleton-anim.html)

Manually builds a `SkinnedMesh` cylinder with a 5-bone chain. Bone weights assigned by vertex Y position. Animates bones with sine waves for wave, bend, and twist motions.

```javascript
const bones = [];
for (let i = 0; i < BONE_COUNT; i++) {
  const bone = new THREE.Bone();
  bone.position.y = i === 0 ? 0 : SEGMENT_HEIGHT;
  bones.push(bone);
  if (i > 0) bones[i-1].add(bone); // chain
}
const skeleton = new THREE.Skeleton(bones);
const skinnedMesh = new THREE.SkinnedMesh(geo, mat);
skinnedMesh.bind(skeleton);

// In render loop — animate bones:
bones.forEach((bone, i) => {
  bone.rotation.z = Math.sin(t * 2 + i * 0.4) * 0.2;
});
```

---

#### 39. Normal Map — Surface Detail Textures

**File**: [`examples/normal-map.html`](./examples/normal-map.html)

Four procedural normal maps generated via Canvas API (Brick, Scales, Cracked Stone, Metal Plate). Applied to `MeshStandardMaterial.normalMap`. Moving point light reveals the surface detail.

```javascript
// Canvas-generated normal map
const canvas = document.createElement('canvas');
const ctx = canvas.getContext('2d');
ctx.fillStyle = '#8080ff'; // flat normal (pointing +Z)
ctx.fillRect(0, 0, size, size);
// Draw grooves, bumps using different color normals...

const normalMap = new THREE.CanvasTexture(canvas);
material.normalMap = normalMap;
material.normalScale.set(2, 2); // intensity
```

---

#### 40. Audio Visualizer — FFT 3D Bars

**File**: [`examples/audio-visualizer.html`](./examples/audio-visualizer.html)

`AnalyserNode` FFT data drives 3D bar heights each frame. Two display modes: flat bar chart and circular ring. Falls back to animated demo data when no microphone is available.

```javascript
const audioCtx = new AudioContext();
const analyser = audioCtx.createAnalyser();
analyser.fftSize = 128; // 64 frequency bins
const source = audioCtx.createMediaStreamSource(micStream);
source.connect(analyser);
const dataArray = new Uint8Array(analyser.frequencyBinCount);

// In render loop:
analyser.getByteFrequencyData(dataArray);
bars.forEach((bar, i) => {
  bar.scale.y = dataArray[i] * heightScale;
});
```

---

### New Advanced — Detail Descriptions

#### 41. Procedural Terrain — Noise Heightmap

**File**: [`examples/procedural-terrain.html`](./examples/procedural-terrain.html)

Multi-octave fBm noise displaces a 128×128 `PlaneGeometry` into a terrain. Color assigned per-vertex by height (water/beach/grass/forest/rock/snow). Flyover camera orbits the landscape.

```javascript
// Fractal Brownian Motion (fBm) for terrain
function fbm(x, y, octaves) {
  let v=0, amp=0.5, freq=1, max=0;
  for (let i=0; i<octaves; i++) {
    v   += noise2(x*freq, y*freq) * amp;
    max += amp;
    amp *= 0.5; freq *= 2; // each octave: half amplitude, double frequency
  }
  return v / max;
}
const h = fbm(x/20, z/20, 4) * heightScale;
pos.setY(i, h);
```

---

#### 42. 3D Text — FontLoader & TextGeometry

**File**: [`examples/text-3d.html`](./examples/text-3d.html)

Loads `helvetiker_bold` font via `FontLoader`, creates individual letter meshes with `TextGeometry` and bevel. Animates letters in Normal, Wave, and Explode modes.

```javascript
import { FontLoader }   from 'three/addons/loaders/FontLoader.js';
import { TextGeometry } from 'three/addons/geometries/TextGeometry.js';

const loader = new FontLoader();
loader.load('https://cdn.jsdelivr.net/npm/three@0.167.1/examples/fonts/helvetiker_bold.typeface.json', font => {
  const geo = new TextGeometry('Hello', {
    font, size: 1.2, depth: 0.4,
    bevelEnabled: true, bevelThickness: 0.05, bevelSize: 0.04,
  });
  geo.computeBoundingBox(); // needed for centering
  scene.add(new THREE.Mesh(geo, material));
});
```

---

#### 43. Fat Lines — Line2 / LineMaterial

**File**: [`examples/fat-lines.html`](./examples/fat-lines.html)

`Line2` + `LineMaterial` for configurable-width lines (native WebGL lines are always 1px). Helix with vertex colors, grid with `LineSegments2`, and a star-burst pattern. Supports dashed lines.

```javascript
import { Line2 }        from 'three/addons/lines/Line2.js';
import { LineMaterial } from 'three/addons/lines/LineMaterial.js';
import { LineGeometry } from 'three/addons/lines/LineGeometry.js';

const geo = new LineGeometry();
geo.setPositions(positions); // flat [x,y,z, x,y,z, ...]
geo.setColors(colors);       // flat [r,g,b, r,g,b, ...]

const mat = new LineMaterial({
  linewidth: 4, // pixels
  vertexColors: true, dashed: false,
  resolution: new THREE.Vector2(innerWidth, innerHeight), // REQUIRED
});
const line = new Line2(geo, mat);
line.computeLineDistances(); // needed for dashed
```

---

#### 44. Sky Atmosphere — Sky Shader

**File**: [`examples/sky-atmosphere.html`](./examples/sky-atmosphere.html)

`Sky` addon with Rayleigh/Mie scattering, sun elevation/azimuth control, and day/night cycle. Combined with `Water` surface for a complete outdoor environment.

```javascript
import { Sky }   from 'three/addons/objects/Sky.js';
import { Water } from 'three/addons/objects/Water.js';

const sky = new Sky();
sky.scale.setScalar(450000);
scene.add(sky);

const phi   = THREE.MathUtils.degToRad(90 - elevation);
const theta = THREE.MathUtils.degToRad(azimuth);
const sun = new THREE.Vector3().setFromSphericalCoords(1, phi, theta);
sky.material.uniforms.sunPosition.value.copy(sun);
sky.material.uniforms.turbidity.value = 10;
sky.material.uniforms.rayleigh.value  = 3;
renderer.toneMappingExposure = 0.5;
```

---

#### 45. Procedural City — Random Buildings

**File**: [`examples/procedural-city.html`](./examples/procedural-city.html)

Math.random() grid of `BoxGeometry` buildings with varying heights, colors, and window lights. Street grid with `LineBasicMaterial`. Point lights for street lamps. Fly-over camera.

```javascript
for (let row = 0; row < GRID_SIZE; row++) {
  for (let col = 0; col < GRID_SIZE; col++) {
    if (Math.random() < 0.15) continue; // empty lot
    const h = 1 + Math.random() * 20;   // random height
    const building = new THREE.Mesh(
      new THREE.BoxGeometry(w, h, d),
      new THREE.MeshStandardMaterial({ color: buildingColors[Math.floor(Math.random() * buildingColors.length)] })
    );
    building.position.set(x, h/2, z);
    scene.add(building);
  }
}
```

---

#### 46. Shader Extend — onBeforeCompile

**File**: [`examples/shader-extend.html`](./examples/shader-extend.html)

Extends `MeshStandardMaterial` by injecting custom GLSL via `onBeforeCompile`. Five effect modes: Ripple UV distortion, Noise Dissolve (discard), Rainbow tint, Glitch, and X-Ray rim.

```javascript
material.onBeforeCompile = (shader) => {
  shader.uniforms.uTime = { value: 0 };
  shader.fragmentShader = 'uniform float uTime;\n' + shader.fragmentShader;

  // Inject before gl_FragColor output
  shader.fragmentShader = shader.fragmentShader.replace(
    'gl_FragColor = vec4( outgoingLight, diffuseColor.a );',
    `vec3 rainbow = vec3(sin(uTime + vMapUv.y * 8.0) * 0.5 + 0.5, ...);
     gl_FragColor = vec4( outgoingLight * rainbow, diffuseColor.a );`
  );
  material.userData.shader = shader; // store ref to update uniforms
};
```

---

#### 47. Depth of Field — BokehPass

**File**: [`examples/depth-of-field.html`](./examples/depth-of-field.html)

`BokehPass` from `EffectComposer` creates camera-lens depth of field blur. Focus distance, aperture, and max blur are controllable. Objects at different Z depths show varying blur.

```javascript
import { BokehPass } from 'three/addons/postprocessing/BokehPass.js';

const bokehPass = new BokehPass(scene, camera, {
  focus: 10, aperture: 0.00015, maxblur: 0.006,
});
composer.addPass(bokehPass);

// Update parameters at runtime:
bokehPass.uniforms.focus.value    = 15;
bokehPass.uniforms.aperture.value = 0.0002;
bokehPass.uniforms.maxblur.value  = 0.01;
```

---

#### 48. Texture Atlas — Sprite Sheet Animation

**File**: [`examples/texture-atlas.html`](./examples/texture-atlas.html)

Canvas-generated 4×4 sprite sheet textures for Explosion, Fire, and Coin flip. UV `offset` and `repeat` cycle through frames each tick. Billboard sprites always face the camera.

```javascript
// Set up atlas UV tiling
mat.map.repeat.set(1/COLS, 1/ROWS); // one frame size

// Animate frame each tick
const frame = Math.floor((t * fps + offset) % FRAMES);
const col = frame % COLS;
const row = Math.floor(frame / COLS);
mat.map.offset.set(col / COLS, (ROWS - 1 - row) / ROWS);

// Billboard: face camera
sprite.quaternion.copy(camera.quaternion);
```

---

#### 49. Particle Emitter — Pool & Lifecycle

**File**: [`examples/particle-emitter.html`](./examples/particle-emitter.html)

Particle pool pattern: fixed-size array of particle objects; dead particles are recycled instead of creating new ones. Supports Fire, Smoke, Sparks, and Snow presets with configurable rate and gravity.

```javascript
// Pool-based emitter pattern
const pool = Array.from({ length: MAX }, () => ({ active: false, life: 0, ... }));

function spawnParticle() {
  const p = pool.find(x => !x.active); // reuse dead particle
  if (!p) return; // pool exhausted — skip
  p.active = true; p.life = 0;
  p.vy = 2 + Math.random() * 3; // fire upward velocity
}

// Update loop: physics + fade
pool.forEach(p => {
  if (!p.active) return;
  p.vy += gravity * dt;
  p.py += p.vy * dt;
  p.alpha = 1 - (p.life / p.maxLife); // fade out
  if (p.life >= p.maxLife) p.active = false; // recycle
});
```

---

#### 50. Multi Material — Per-face Material Groups

**File**: [`examples/multi-material.html`](./examples/multi-material.html)

A single `Mesh` with multiple `Material` groups — different material per face group. Works with `BoxGeometry` (6 faces), `CylinderGeometry` (3 parts: top/side/bottom), and `ConeGeometry` (2 parts).

```javascript
// BoxGeometry has 6 groups (one per face)
const materials = [
  new THREE.MeshStandardMaterial({ color: 0xff4444 }), // +X right
  new THREE.MeshStandardMaterial({ color: 0x4444ff }), // -X left
  new THREE.MeshStandardMaterial({ color: 0x44ff44 }), // +Y top
  new THREE.MeshStandardMaterial({ color: 0xffaa00 }), // -Y bottom
  new THREE.MeshStandardMaterial({ color: 0xff44ff }), // +Z front
  new THREE.MeshStandardMaterial({ color: 0x44ffff }), // -Z back
];
const mesh = new THREE.Mesh(new THREE.BoxGeometry(3, 3, 3), materials);
```

---

## Reference Docs

| Document | Contents |
|----------|---------|
| [core-concepts.md](./references/core-concepts.md) | Scene, Camera, Renderer, coordinate system, scene graph, minimal template |
| [geometries-materials.md](./references/geometries-materials.md) | All built-in geometry constructors, custom BufferGeometry, material property table |
| [lights-shadows.md](./references/lights-shadows.md) | Light types, shadow configuration modes, SpotLight/RectAreaLight details |
| [animations.md](./references/animations.md) | AnimationMixer, KeyframeTrack, action API, morph targets, skeletal animation |
| [loaders.md](./references/loaders.md) | TextureLoader, GLTFLoader, OBJLoader, FBXLoader, RGBELoader, FontLoader |
| [postprocessing.md](./references/postprocessing.md) | EffectComposer setup, all Pass overview, ShaderPass, OutlinePass |
| [performance.md](./references/performance.md) | InstancedMesh, LOD, memory disposal, texture optimization, Stats, frustum culling |

---

## API Cheatsheet

### Core Scene Classes

```javascript
// Scene
const scene = new THREE.Scene();
scene.background = new THREE.Color(0x87ceeb); // solid color background
scene.fog = new THREE.FogExp2(0x87ceeb, 0.02); // exponential fog

// Camera
const cam = new THREE.PerspectiveCamera(fov, aspect, near, far);
// fov=75 aspect=innerWidth/innerHeight near=0.1 far=1000

// Renderer
const renderer = new THREE.WebGLRenderer({ antialias: true });
renderer.setSize(innerWidth, innerHeight);
renderer.setPixelRatio(Math.min(devicePixelRatio, 2)); // cap at 2x
renderer.shadowMap.enabled = true;
renderer.toneMapping = THREE.ACESFilmicToneMapping;
renderer.toneMappingExposure = 1.0;
```

### Mesh & Material

```javascript
const mesh = new THREE.Mesh(geometry, material);
mesh.position.set(x, y, z);
mesh.rotation.set(rx, ry, rz); // Euler angles (radians)
mesh.scale.setScalar(2);        // uniform scale
mesh.castShadow = true;
mesh.receiveShadow = true;
scene.add(mesh);
```

### Render Loop

```javascript
const clock = new THREE.Clock();

renderer.setAnimationLoop(() => {
  const delta = clock.getDelta();       // frame delta (seconds)
  const elapsed = clock.getElapsedTime(); // total elapsed (seconds)

  // Update logic...
  mixer?.update(delta);
  controls.update();

  renderer.render(scene, camera);
});
```

### Memory Cleanup

```javascript
// Always manually dispose when switching scenes or destroying objects
function disposeMesh(mesh) {
  mesh.geometry.dispose();
  if (Array.isArray(mesh.material)) {
    mesh.material.forEach(m => {
      m.map?.dispose();
      m.dispose();
    });
  } else {
    mesh.material.map?.dispose();
    mesh.material.dispose();
  }
  mesh.parent?.remove(mesh);
}

// Entire renderer
renderer.dispose();
renderer.forceContextLoss();
```

---

## Official Resources

| Link | Description |
|------|------------|
| [threejs.org](https://threejs.org/) | Official homepage |
| [threejs.org/docs](https://threejs.org/docs/) | API documentation |
| [threejs.org/examples](https://threejs.org/examples/) | Official examples (300+) |
| [threejs.org/manual](https://threejs.org/manual/) | Getting started manual |
| [discourse.threejs.org](https://discourse.threejs.org/) | Official forum |
| [github.com/mrdoob/three.js](https://github.com/mrdoob/three.js) | GitHub repository |

---

<p align="center">
  <sub>Three.js r167 · CDN: cdn.jsdelivr.net/npm/three@0.167.1 · 20 Examples · 7 Reference Docs</sub>
</p>
