# Performance Optimization

## Key Principles

1. **Minimize draw calls** — merge geometries, use InstancedMesh
2. **Reuse materials** — same material instance across meshes
3. **Dispose unused resources** — geometries, materials, textures
4. **Limit shadow casters** — `castShadow` only on key objects
5. **Use LOD** — switch geometry detail based on distance

## InstancedMesh (thousands of objects)

```js
const geometry = new THREE.SphereGeometry(0.1);
const material = new THREE.MeshStandardMaterial({ color: 0xffffff });
const count = 10000;
const mesh = new THREE.InstancedMesh(geometry, material, count);

const matrix = new THREE.Matrix4();
for (let i = 0; i < count; i++) {
  matrix.setPosition(
    (Math.random() - 0.5) * 100,
    (Math.random() - 0.5) * 100,
    (Math.random() - 0.5) * 100
  );
  mesh.setMatrixAt(i, matrix);
  mesh.setColorAt(i, new THREE.Color(Math.random(), Math.random(), Math.random()));
}
mesh.instanceMatrix.needsUpdate = true;
mesh.instanceColor.needsUpdate = true;
scene.add(mesh);
```

## Merging Geometries

```js
import { mergeGeometries } from 'three/addons/utils/BufferGeometryUtils.js';

const geo1 = new THREE.BoxGeometry(1, 1, 1);
geo1.translate(0, 0, 0);
const geo2 = new THREE.SphereGeometry(0.5);
geo2.translate(2, 0, 0);

const merged = mergeGeometries([geo1, geo2]);
const mesh = new THREE.Mesh(merged, material);
```

## LOD (Level of Detail)

```js
const lod = new THREE.LOD();
lod.addLevel(new THREE.Mesh(highPolyGeo, mat), 0);   // 0-50 units
lod.addLevel(new THREE.Mesh(midPolyGeo, mat), 50);  // 50-200 units
lod.addLevel(new THREE.Mesh(lowPolyGeo, mat), 200); // 200+ units
scene.add(lod);
// Call lod.update(camera) in render loop
```

## Disposal

```js
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
}
```

## Texture Optimization

```js
// Prefer power-of-2 texture sizes: 256, 512, 1024, 2048
texture.generateMipmaps = true;
texture.minFilter = THREE.LinearMipmapLinearFilter;

// Compressed textures (KTX2/Basis)
import { KTX2Loader } from 'three/addons/loaders/KTX2Loader.js';
const ktx2Loader = new KTX2Loader()
  .setTranscoderPath('https://cdn.jsdelivr.net/npm/three@0.167.1/examples/jsm/libs/basis/')
  .detectSupport(renderer);
```

## Renderer Stats

```js
import Stats from 'three/addons/libs/stats.module.js';
const stats = new Stats();
document.body.appendChild(stats.dom);
// In render loop: stats.update()
```

## Frustum Culling

Three.js performs automatic frustum culling.
- Set `mesh.frustumCulled = false` to disable (e.g., for full-screen quads)
- Set `mesh.matrixAutoUpdate = false` for static objects, call `mesh.updateMatrix()` manually
