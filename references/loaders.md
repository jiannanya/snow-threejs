# Loaders & Assets

## Texture Loading

```js
const loader = new THREE.TextureLoader();
const texture = loader.load('image.jpg', (tex) => {
  tex.colorSpace = THREE.SRGBColorSpace;
  tex.wrapS = THREE.RepeatWrapping;
  tex.wrapT = THREE.RepeatWrapping;
  tex.repeat.set(4, 4);
});

// Async version
const tex = await loader.loadAsync('image.jpg');
```

## GLTF / GLB Loader (recommended format)

```js
import { GLTFLoader } from 'three/addons/loaders/GLTFLoader.js';
import { DRACOLoader } from 'three/addons/loaders/DRACOLoader.js';

const dracoLoader = new DRACOLoader();
dracoLoader.setDecoderPath('https://cdn.jsdelivr.net/npm/three@0.167.1/examples/jsm/libs/draco/');

const loader = new GLTFLoader();
loader.setDRACOLoader(dracoLoader);
loader.load('model.glb', (gltf) => {
  scene.add(gltf.scene);
  // gltf.animations — animation clips
  // gltf.cameras — cameras in model
  // gltf.scene — root group
});
```

## OBJ + MTL Loader

```js
import { OBJLoader } from 'three/addons/loaders/OBJLoader.js';
import { MTLLoader } from 'three/addons/loaders/MTLLoader.js';

const mtlLoader = new MTLLoader();
mtlLoader.load('model.mtl', (materials) => {
  materials.preload();
  const objLoader = new OBJLoader();
  objLoader.setMaterials(materials);
  objLoader.load('model.obj', (obj) => scene.add(obj));
});
```

## FBX Loader

```js
import { FBXLoader } from 'three/addons/loaders/FBXLoader.js';
const loader = new FBXLoader();
loader.load('model.fbx', (fbx) => {
  fbx.scale.setScalar(0.01);
  scene.add(fbx);
  const mixer = new THREE.AnimationMixer(fbx);
  mixer.clipAction(fbx.animations[0]).play();
});
```

## HDR Environment Map

```js
import { RGBELoader } from 'three/addons/loaders/RGBELoader.js';

const pmremGenerator = new THREE.PMREMGenerator(renderer);
new RGBELoader().load('environment.hdr', (hdrTexture) => {
  const envMap = pmremGenerator.fromEquirectangular(hdrTexture).texture;
  scene.environment = envMap;   // PBR lighting
  scene.background = envMap;    // background
  hdrTexture.dispose();
  pmremGenerator.dispose();
});
```

## Loading Manager (progress tracking)

```js
const manager = new THREE.LoadingManager(
  () => console.log('All loaded!'),
  (url, loaded, total) => console.log(`${(loaded/total*100).toFixed(0)}%`),
  (url) => console.error('Error loading:', url)
);
const loader = new THREE.TextureLoader(manager);
```

## Font Loader (3D Text)

```js
import { FontLoader } from 'three/addons/loaders/FontLoader.js';
import { TextGeometry } from 'three/addons/geometries/TextGeometry.js';

const fontLoader = new FontLoader();
fontLoader.load('https://cdn.jsdelivr.net/npm/three@0.167.1/examples/fonts/helvetiker_regular.typeface.json', (font) => {
  const textGeo = new TextGeometry('Hello Three.js', {
    font, size: 0.5, depth: 0.1,
    curveSegments: 12, bevelEnabled: true,
    bevelThickness: 0.01, bevelSize: 0.02
  });
  textGeo.center();
  scene.add(new THREE.Mesh(textGeo, new THREE.MeshStandardMaterial({ color: 0xffffff })));
});
```
