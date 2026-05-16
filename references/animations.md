# Animation System

## AnimationMixer (for loaded models)

```js
import { GLTFLoader } from 'three/addons/loaders/GLTFLoader.js';

const loader = new GLTFLoader();
loader.load('model.glb', (gltf) => {
  scene.add(gltf.scene);
  const mixer = new THREE.AnimationMixer(gltf.scene);
  const action = mixer.clipAction(gltf.animations[0]);
  action.play();

  // In render loop:
  const clock = new THREE.Clock();
  renderer.setAnimationLoop(() => {
    mixer.update(clock.getDelta());
    renderer.render(scene, camera);
  });
});
```

## Custom Keyframe Animation

```js
// Position track: object moves along Y axis
const posTrack = new THREE.VectorKeyframeTrack(
  '.position',                      // property path
  [0, 1, 2],                        // times (seconds)
  [0,0,0, 0,2,0, 0,0,0]           // values (xyz per key)
);

// Rotation track
const rotTrack = new THREE.QuaternionKeyframeTrack(
  '.quaternion',
  [0, 1, 2],
  [0,0,0,1, 0,1,0,0, 0,0,0,1]    // quaternion xyzw per key
);

// Color track
const colTrack = new THREE.ColorKeyframeTrack(
  '.material.color',
  [0, 1],
  [1,0,0, 0,0,1]  // RGB per key
);

const clip = new THREE.AnimationClip('action', 2, [posTrack, rotTrack]);
const mixer = new THREE.AnimationMixer(mesh);
const action = mixer.clipAction(clip);
action.setLoop(THREE.LoopRepeat, Infinity);
action.play();
```

## Action Control

```js
action.play();
action.pause();
action.stop();
action.reset();
action.setEffectiveWeight(0.5);    // blending weight
action.setEffectiveTimeScale(2);   // speed multiplier
action.fadeIn(0.5);                // cross-fade in 0.5s
action.fadeOut(0.5);
action.crossFadeTo(otherAction, 0.5, true); // blend transition
```

## Morph Targets

```js
// Set up geometry with morph attributes
const base = new Float32Array([/* base positions */]);
const morph = new Float32Array([/* target positions */]);
geometry.setAttribute('position', new THREE.BufferAttribute(base, 3));
geometry.morphAttributes.position = [
  new THREE.BufferAttribute(morph, 3)
];
geometry.morphTargetsRelative = false;

mesh.morphTargetInfluences[0] = 0.5; // 0=base, 1=fully morphed

// Or animate via mixer with MorphTrack
const morphTrack = new THREE.NumberKeyframeTrack(
  '.morphTargetInfluences[0]',
  [0, 1, 2],
  [0, 1, 0]
);
```

## Skinned Mesh / Skeleton

```js
const bones = [];
// Create bone hierarchy...
const skeleton = new THREE.Skeleton(bones);
const skinnedMesh = new THREE.SkinnedMesh(geometry, material);
skinnedMesh.add(skeleton.bones[0]);
skinnedMesh.bind(skeleton);
```

## Clock Usage

```js
const clock = new THREE.Clock();
renderer.setAnimationLoop(() => {
  const delta = clock.getDelta();  // seconds since last frame
  const elapsed = clock.getElapsedTime(); // total time
  mixer.update(delta);
  mesh.rotation.y = elapsed * 0.5;
  renderer.render(scene, camera);
});
```
