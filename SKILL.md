---
name: threejs
description: "Three.js 3D graphics skill. Use when: creating 3D scenes, WebGL/WebGPU rendering, 3D animations, particle systems, shaders, post-processing effects, physics simulations, model loading (GLTF/OBJ/FBX), camera controls, raycasting, instanced rendering, environment maps, shadows, textures, TSL shaders. Covers all Three.js core APIs and addon features."
argument-hint: "Describe the 3D effect or scene you want to create"
---

# Three.js 3D Graphics Skill

Three.js (r184+) — JavaScript 3D library supporting WebGL and WebGPU renderers.

## Capabilities

- **Scene Setup**: Scene, Camera (Perspective/Orthographic), Renderer (WebGL/WebGPU)
- **Geometries**: Box, Sphere, Cylinder, Torus, Plane, Custom BufferGeometry, and 20+ more
- **Materials**: MeshBasicMaterial, MeshStandardMaterial, MeshPhysicalMaterial, ShaderMaterial, and more
- **Lights**: Ambient, Directional, Point, Spot, RectArea, Hemisphere
- **Animations**: AnimationMixer, KeyframeTrack, morph targets, skinning
- **Controls**: OrbitControls, FlyControls, DragControls, TransformControls
- **Loaders**: GLTFLoader, OBJLoader, FBXLoader, TextureLoader, HDRLoader
- **Post-processing**: Bloom, SSAO, DOF, FXAA, Glitch, Film, and 30+ passes
- **Physics**: Rapier, Ammo.js, Jolt integration
- **WebXR**: AR/VR support via ARButton/VRButton
- **TSL**: Three.js Shader Language (node-based shader system)
- **WebGPU**: Next-gen renderer with compute shaders

## Quick Reference

- [Core Concepts](./references/core-concepts.md) — Scene, Camera, Renderer, render loop
- [Geometries & Materials](./references/geometries-materials.md) — All built-in types
- [Lights & Shadows](./references/lights-shadows.md) — Lighting setup patterns
- [Animation System](./references/animations.md) — AnimationMixer, keyframes, morphs
- [Loaders & Assets](./references/loaders.md) — Loading 3D models and textures
- [Post-processing](./references/postprocessing.md) — EffectComposer passes
- [Performance](./references/performance.md) — Optimization patterns

## CDN Import (ES Modules)

```html
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
</script>
```

## Examples Index

| File | Topic | Difficulty |
|------|-------|-----------|
| [hello-cube.html](./examples/hello-cube.html) | Basic rotating cube, scene setup | Beginner |
| [geometries.html](./examples/geometries.html) | All built-in geometry types | Beginner |
| [materials.html](./examples/materials.html) | Material types comparison | Beginner |
| [lights.html](./examples/lights.html) | All light types showcase | Beginner |
| [shadows.html](./examples/shadows.html) | Shadow mapping setup | Beginner |
| [textures.html](./examples/textures.html) | Texture loading & UV mapping | Intermediate |
| [orbit-controls.html](./examples/orbit-controls.html) | OrbitControls camera navigation | Intermediate |
| [particles.html](./examples/particles.html) | Particle system with Points | Intermediate |
| [raycasting.html](./examples/raycasting.html) | Mouse picking & interaction | Intermediate |
| [animation-mixer.html](./examples/animation-mixer.html) | AnimationMixer & keyframes | Intermediate |
| [morph-targets.html](./examples/morph-targets.html) | Morph target animations | Intermediate |
| [instanced-mesh.html](./examples/instanced-mesh.html) | InstancedMesh for performance | Intermediate |
| [custom-shader.html](./examples/custom-shader.html) | ShaderMaterial with GLSL | Advanced |
| [postprocessing.html](./examples/postprocessing.html) | EffectComposer + Bloom | Advanced |
| [environment-map.html](./examples/environment-map.html) | HDR environment & reflections | Advanced |
| [fog-skybox.html](./examples/fog-skybox.html) | Fog, sky, and atmosphere | Intermediate |
| [gltf-loader.html](./examples/gltf-loader.html) | Loading GLTF 3D models | Intermediate |
| [sprite-billboard.html](./examples/sprite-billboard.html) | Sprites and billboards | Intermediate |
| [tsl-shader.html](./examples/tsl-shader.html) | TSL node-based shaders | Advanced |
| [webgpu-basics.html](./examples/webgpu-basics.html) | WebGPU renderer | Advanced |

## Procedure

When creating a Three.js scene:

1. **Setup**: Create `Scene`, `Camera`, `WebGLRenderer` → append `renderer.domElement` to DOM
2. **Content**: Add meshes (`Mesh = Geometry + Material`), lights, helpers
3. **Loop**: Use `renderer.setAnimationLoop()` or `requestAnimationFrame` for animation
4. **Controls**: Add `OrbitControls` for interactive camera
5. **Resize**: Handle `window.resize` to update camera aspect and renderer size
6. **Cleanup**: Dispose geometries, materials, textures on unmount

## Official Resources

- Docs: https://threejs.org/docs/
- Examples: https://threejs.org/examples/
- Manual: https://threejs.org/manual/
- Forum: https://discourse.threejs.org/
