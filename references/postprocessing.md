# Post-Processing

## EffectComposer Setup

```js
import { EffectComposer } from 'three/addons/postprocessing/EffectComposer.js';
import { RenderPass } from 'three/addons/postprocessing/RenderPass.js';
import { UnrealBloomPass } from 'three/addons/postprocessing/UnrealBloomPass.js';
import { OutputPass } from 'three/addons/postprocessing/OutputPass.js';

const composer = new EffectComposer(renderer);
composer.addPass(new RenderPass(scene, camera));
composer.addPass(new UnrealBloomPass(
  new THREE.Vector2(window.innerWidth, window.innerHeight),
  1.5,  // strength
  0.4,  // radius
  0.85  // threshold
));
composer.addPass(new OutputPass());

// Replace renderer.render() with:
composer.render();
```

## Available Passes

| Pass | Effect |
|------|--------|
| `RenderPass` | Base scene render (always first) |
| `OutputPass` | Tone mapping + color space (always last) |
| `UnrealBloomPass` | Glow/bloom effect |
| `BloomPass` | Simple bloom |
| `BokehPass` | Depth of field |
| `FilmPass` | Film grain + scanlines |
| `GlitchPass` | Digital glitch |
| `DotScreenPass` | Dot screen / halftone |
| `HalftonePass` | Halftone |
| `FXAAPass` | FXAA anti-aliasing |
| `SMAAPass` | SMAA anti-aliasing |
| `SSAARenderPass` | Supersampling AA |
| `SSAOPass` | Screen-space AO |
| `SAOPass` | Scalable AO |
| `GTAOPass` | GTAO |
| `SSRPass` | Screen-space reflections |
| `AfterimagePass` | Motion trail / echo |
| `GammaCorrectionShader` (via ShaderPass) | Gamma correction |
| `RenderPixelatedPass` | Pixelation / retro |
| `OutlinePass` | Object outline |
| `ShaderPass` | Custom shader effect |

## ShaderPass (custom effect)

```js
import { ShaderPass } from 'three/addons/postprocessing/ShaderPass.js';
import { RGBShiftShader } from 'three/addons/shaders/RGBShiftShader.js';

const rgbShift = new ShaderPass(RGBShiftShader);
rgbShift.uniforms['amount'].value = 0.003;
composer.addPass(rgbShift);
```

## Outline Pass

```js
import { OutlinePass } from 'three/addons/postprocessing/OutlinePass.js';

const outlinePass = new OutlinePass(
  new THREE.Vector2(window.innerWidth, window.innerHeight),
  scene, camera
);
outlinePass.selectedObjects = [mesh1, mesh2];
outlinePass.edgeStrength = 3;
outlinePass.edgeGlow = 1;
outlinePass.edgeThickness = 1;
outlinePass.visibleEdgeColor.set(0xffffff);
composer.addPass(outlinePass);
```

## Resize Handling

```js
window.addEventListener('resize', () => {
  renderer.setSize(window.innerWidth, window.innerHeight);
  composer.setSize(window.innerWidth, window.innerHeight);
  camera.aspect = window.innerWidth / window.innerHeight;
  camera.updateProjectionMatrix();
});
```
