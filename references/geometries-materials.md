# Geometries & Materials

## Built-in Geometries

```js
new THREE.BoxGeometry(w, h, d)
new THREE.SphereGeometry(radius, widthSeg, heightSeg)
new THREE.CylinderGeometry(radiusTop, radiusBot, height, radialSeg)
new THREE.ConeGeometry(radius, height, radialSeg)
new THREE.TorusGeometry(radius, tube, radialSeg, tubularSeg)
new THREE.TorusKnotGeometry(radius, tube, tubularSeg, radialSeg, p, q)
new THREE.PlaneGeometry(w, h, widthSeg, heightSeg)
new THREE.CircleGeometry(radius, segments)
new THREE.RingGeometry(innerRadius, outerRadius, thetaSeg)
new THREE.CapsuleGeometry(radius, length, capSeg, radialSeg)
new THREE.IcosahedronGeometry(radius, detail)
new THREE.OctahedronGeometry(radius, detail)
new THREE.TetrahedronGeometry(radius, detail)
new THREE.DodecahedronGeometry(radius, detail)
new THREE.LatheGeometry(points, segments)
new THREE.ExtrudeGeometry(shape, options)
new THREE.TubeGeometry(path, tubularSeg, radius, radialSeg, closed)
new THREE.EdgesGeometry(geometry)
new THREE.WireframeGeometry(geometry)
```

## Custom BufferGeometry

```js
const geometry = new THREE.BufferGeometry();
const vertices = new Float32Array([
  -1, -1, 0,   1, -1, 0,   0, 1, 0  // triangle
]);
geometry.setAttribute('position', new THREE.BufferAttribute(vertices, 3));
geometry.computeVertexNormals();
```

## Materials

| Material | Use Case |
|----------|----------|
| `MeshBasicMaterial` | No lighting, flat color/texture |
| `MeshNormalMaterial` | Debug normals (rainbow colors) |
| `MeshLambertMaterial` | Fast diffuse, no specular |
| `MeshPhongMaterial` | Diffuse + specular highlights |
| `MeshStandardMaterial` | PBR — metalness + roughness |
| `MeshPhysicalMaterial` | PBR + clearcoat, transmission, sheen |
| `MeshToonMaterial` | Cartoon/cel shading |
| `MeshDepthMaterial` | Depth buffer visualization |
| `ShaderMaterial` | Custom GLSL vertex + fragment |
| `RawShaderMaterial` | Fully raw GLSL (no built-ins injected) |
| `PointsMaterial` | For Points objects (particles) |
| `LineBasicMaterial` | For Line objects |
| `SpriteMaterial` | For Sprite objects (billboards) |

## MeshStandardMaterial (PBR)

```js
const mat = new THREE.MeshStandardMaterial({
  color: 0xffffff,
  map: texture,           // albedo/diffuse texture
  normalMap: normalTex,  // normal map
  roughnessMap: roughTex,
  metalnessMap: metalTex,
  roughness: 0.5,        // 0=mirror, 1=matte
  metalness: 0.0,        // 0=plastic, 1=metal
  envMap: envTexture,    // environment reflections
  envMapIntensity: 1.0,
  aoMap: aoTexture,      // ambient occlusion
  emissive: 0x000000,
  emissiveMap: emitTex,
});
```

## MeshPhysicalMaterial extras

```js
const mat = new THREE.MeshPhysicalMaterial({
  ...standardProps,
  clearcoat: 1.0,            // lacquer coat
  clearcoatRoughness: 0.1,
  transmission: 1.0,         // glass-like
  thickness: 0.5,
  ior: 1.5,                  // index of refraction
  iridescence: 1.0,          // soap bubble effect
  sheen: 1.0,                // fabric/velvet
  sheenColor: 0xff0000,
});
```

## Wireframe

```js
material.wireframe = true;
// Or use WireframeGeometry:
const wireframe = new THREE.WireframeGeometry(geometry);
const line = new THREE.LineSegments(wireframe, new THREE.LineBasicMaterial({ color: 0x00ff00 }));
scene.add(line);
```
