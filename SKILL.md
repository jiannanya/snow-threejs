---
name: snow-three
description: "snow-three is a Three.js 3D graphics skill. Use when: creating 3D scenes, WebGL/WebGPU rendering, 3D animations, particle systems, shaders, post-processing effects, physics simulations, model loading (GLTF/OBJ/FBX), camera controls, raycasting, instanced rendering, environment maps, shadows, textures, TSL shaders. Covers all Three.js core APIs and addon features."
argument-hint: "Describe the 3D effect or scene you want to create"
---

# snow-three

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
| [axes-helpers.html](./examples/axes-helpers.html) | AxesHelper, GridHelper, ArrowHelper, BoxHelper | Beginner |
| [wireframe-mode.html](./examples/wireframe-mode.html) | Wireframe, WireframeGeometry, EdgesGeometry | Beginner |
| [groups-hierarchy.html](./examples/groups-hierarchy.html) | Group hierarchy, solar system parent-child | Beginner |
| [vertex-colors.html](./examples/vertex-colors.html) | Per-vertex color painting on geometry | Beginner |
| [transparent-blend.html](./examples/transparent-blend.html) | Transparency, blending modes, depthWrite | Beginner |
| [clock-easing.html](./examples/clock-easing.html) | THREE.Clock, easing functions animation | Beginner |
| [background-modes.html](./examples/background-modes.html) | Scene background: solid, gradient, CubeMap | Beginner |
| [simple-physics.html](./examples/simple-physics.html) | Manual gravity, elastic bounce, wall collision | Beginner |
| [multi-viewport.html](./examples/multi-viewport.html) | Split-screen scissor/viewport rendering | Beginner |
| [css2d-labels.html](./examples/css2d-labels.html) | CSS2DRenderer planet labels in 3D space | Beginner |
| [curve-path.html](./examples/curve-path.html) | CatmullRomCurve3, TubeGeometry, path following | Intermediate |
| [shape-extrude.html](./examples/shape-extrude.html) | THREE.Shape, ExtrudeGeometry, bevel | Intermediate |
| [lod.html](./examples/lod.html) | THREE.LOD level-of-detail with distance | Intermediate |
| [cube-camera.html](./examples/cube-camera.html) | CubeCamera live environment reflections | Intermediate |
| [water-surface.html](./examples/water-surface.html) | ShaderMaterial wave displacement, foam | Intermediate |
| [outline-select.html](./examples/outline-select.html) | OutlinePass selection highlight via EffectComposer | Intermediate |
| [render-target.html](./examples/render-target.html) | WebGLRenderTarget off-screen rendering | Intermediate |
| [skeleton-anim.html](./examples/skeleton-anim.html) | SkinnedMesh, Bone hierarchy animation | Intermediate |
| [normal-map.html](./examples/normal-map.html) | Procedural normal map textures, bump detail | Intermediate |
| [audio-visualizer.html](./examples/audio-visualizer.html) | Web Audio API FFT → 3D bar visualization | Intermediate |
| [procedural-terrain.html](./examples/procedural-terrain.html) | Multi-octave noise heightmap terrain | Advanced |
| [text-3d.html](./examples/text-3d.html) | FontLoader, TextGeometry, 3D text animation | Advanced |
| [fat-lines.html](./examples/fat-lines.html) | Line2, LineMaterial, configurable line width | Advanced |
| [sky-atmosphere.html](./examples/sky-atmosphere.html) | Sky shader, sun position, water surface | Advanced |
| [procedural-city.html](./examples/procedural-city.html) | Random procedural building city generation | Advanced |
| [shader-extend.html](./examples/shader-extend.html) | onBeforeCompile GLSL injection into StandardMaterial | Advanced |
| [depth-of-field.html](./examples/depth-of-field.html) | BokehPass depth of field, EffectComposer | Advanced |
| [texture-atlas.html](./examples/texture-atlas.html) | Sprite sheet UV offset animation, billboards | Advanced |
| [particle-emitter.html](./examples/particle-emitter.html) | Particle pool with lifetime, fade, physics | Advanced |
| [multi-material.html](./examples/multi-material.html) | Per-face material groups on single mesh | Advanced |

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
