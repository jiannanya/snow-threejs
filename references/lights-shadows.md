# Lights & Shadows

## Light Types

| Light | Description |
|-------|-------------|
| `AmbientLight(color, intensity)` | Uniform, no direction, no shadows |
| `DirectionalLight(color, intensity)` | Infinite distance, parallel rays, shadows |
| `PointLight(color, intensity, distance, decay)` | Omnidirectional point source, shadows |
| `SpotLight(color, intensity, distance, angle, penumbra, decay)` | Cone of light, shadows |
| `HemisphereLight(skyColor, groundColor, intensity)` | Sky/ground gradient, no shadows |
| `RectAreaLight(color, intensity, width, height)` | Rectangular area, no shadows (requires addons) |

## Basic Lighting Setup

```js
// Ambient fill light
const ambient = new THREE.AmbientLight(0x404040, 0.5);
scene.add(ambient);

// Main directional (sun) light with shadows
const dirLight = new THREE.DirectionalLight(0xffffff, 1.0);
dirLight.position.set(10, 20, 10);
dirLight.castShadow = true;
scene.add(dirLight);
```

## Shadow Configuration

```js
// Renderer
renderer.shadowMap.enabled = true;
renderer.shadowMap.type = THREE.PCFSoftShadowMap; // PCFShadowMap, VSMShadowMap

// Light shadow settings
dirLight.castShadow = true;
dirLight.shadow.mapSize.width = 2048;    // shadow texture resolution
dirLight.shadow.mapSize.height = 2048;
dirLight.shadow.camera.near = 0.5;
dirLight.shadow.camera.far = 500;
// For DirectionalLight: control shadow frustum
dirLight.shadow.camera.left = -50;
dirLight.shadow.camera.right = 50;
dirLight.shadow.camera.top = 50;
dirLight.shadow.camera.bottom = -50;
dirLight.shadow.bias = -0.001;          // prevents shadow acne

// Objects
mesh.castShadow = true;
mesh.receiveShadow = true;

// Ground plane
plane.receiveShadow = true;
```

## SpotLight Setup

```js
const spot = new THREE.SpotLight(0xffffff, 2);
spot.position.set(0, 10, 0);
spot.angle = Math.PI / 6;    // cone half-angle
spot.penumbra = 0.2;          // edge softness 0-1
spot.decay = 2;               // physical falloff
spot.distance = 30;
spot.castShadow = true;
spot.target.position.set(0, 0, 0);
scene.add(spot);
scene.add(spot.target);
```

## RectAreaLight

```js
import { RectAreaLightUniformsLib } from 'three/addons/lights/RectAreaLightUniformsLib.js';
import { RectAreaLightHelper } from 'three/addons/helpers/RectAreaLightHelper.js';

RectAreaLightUniformsLib.init();
const rectLight = new THREE.RectAreaLight(0xffffff, 5, 4, 4);
rectLight.position.set(0, 5, 0);
rectLight.lookAt(0, 0, 0);
scene.add(rectLight);
scene.add(new RectAreaLightHelper(rectLight));
```

## Light Helpers

```js
scene.add(new THREE.DirectionalLightHelper(dirLight, 5));
scene.add(new THREE.SpotLightHelper(spot));
scene.add(new THREE.PointLightHelper(pointLight, 1));
scene.add(new THREE.HemisphereLightHelper(hemiLight, 5));
scene.add(new THREE.CameraHelper(dirLight.shadow.camera)); // shadow frustum
```
