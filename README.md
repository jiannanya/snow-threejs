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
<td></td><td></td><td></td>
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
<td></td><td></td>
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
<td></td><td></td><td></td>
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
