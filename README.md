# Three.js 3D 图形技能库

> **版本**: Three.js r167 (npm `0.167.1`) · **渲染器**: WebGL / WebGPU · **模块**: ES Modules via CDN importmap

本技能库提供 20 个可直接运行的 HTML 示例、7 份参考文档，覆盖从基础场景搭建到高级着色器的完整 Three.js 开发知识体系。

---

## 示例截图预览

### 初级示例

<table>
<tr>
<td align="center" width="25%">
<a href="./examples/hello-cube.html"><img src="./images/hello-cube.png" width="100%"></a><br>
<b>Hello Cube</b><br><sub>基础旋转立方体 · 场景搭建</sub>
</td>
<td align="center" width="25%">
<a href="./examples/geometries.html"><img src="./images/geometries.png" width="100%"></a><br>
<b>Geometries</b><br><sub>所有内置几何体展示</sub>
</td>
<td align="center" width="25%">
<a href="./examples/materials.html"><img src="./images/materials.png" width="100%"></a><br>
<b>Materials</b><br><sub>11 种材质类型对比</sub>
</td>
<td align="center" width="25%">
<a href="./examples/lights.html"><img src="./images/lights.png" width="100%"></a><br>
<b>Lights</b><br><sub>5 种光源类型演示</sub>
</td>
</tr>
<tr>
<td align="center" width="25%">
<a href="./examples/shadows.html"><img src="./images/shadows.png" width="100%"></a><br>
<b>Shadows</b><br><sub>阴影映射与软硬阴影</sub>
</td>
<td></td><td></td><td></td>
</tr>
</table>

### 中级示例

<table>
<tr>
<td align="center" width="25%">
<a href="./examples/textures.html"><img src="./images/textures.png" width="100%"></a><br>
<b>Textures</b><br><sub>程序化 Canvas 纹理</sub>
</td>
<td align="center" width="25%">
<a href="./examples/orbit-controls.html"><img src="./images/orbit-controls.png" width="100%"></a><br>
<b>Orbit Controls</b><br><sub>相机交互控制器</sub>
</td>
<td align="center" width="25%">
<a href="./examples/particles.html"><img src="./images/particles.png" width="100%"></a><br>
<b>Particles</b><br><sub>5 万粒子系统</sub>
</td>
<td align="center" width="25%">
<a href="./examples/raycasting.html"><img src="./images/raycasting.png" width="100%"></a><br>
<b>Raycasting</b><br><sub>鼠标拾取与高亮</sub>
</td>
</tr>
<tr>
<td align="center" width="25%">
<a href="./examples/animation-mixer.html"><img src="./images/animation-mixer.png" width="100%"></a><br>
<b>Animation Mixer</b><br><sub>关键帧动画系统</sub>
</td>
<td align="center" width="25%">
<a href="./examples/morph-targets.html"><img src="./images/morph-targets.png" width="100%"></a><br>
<b>Morph Targets</b><br><sub>顶点变形动画</sub>
</td>
<td align="center" width="25%">
<a href="./examples/instanced-mesh.html"><img src="./images/instanced-mesh.png" width="100%"></a><br>
<b>Instanced Mesh</b><br><sub>10 万实例单次绘制</sub>
</td>
<td align="center" width="25%">
<a href="./examples/fog-skybox.html"><img src="./images/fog-skybox.png" width="100%"></a><br>
<b>Fog &amp; Skybox</b><br><sub>雾效与大气天空</sub>
</td>
</tr>
<tr>
<td align="center" width="25%">
<a href="./examples/gltf-loader.html"><img src="./images/gltf-loader.png" width="100%"></a><br>
<b>GLTF Loader</b><br><sub>加载 3D 模型文件</sub>
</td>
<td align="center" width="25%">
<a href="./examples/sprite-billboard.html"><img src="./images/sprite-billboard.png" width="100%"></a><br>
<b>Sprite Billboard</b><br><sub>精灵与公告板标注</sub>
</td>
<td></td><td></td>
</tr>
</table>

### 高级示例

<table>
<tr>
<td align="center" width="25%">
<a href="./examples/custom-shader.html"><img src="./images/custom-shader.png" width="100%"></a><br>
<b>Custom Shader</b><br><sub>GLSL 自定义着色器</sub>
</td>
<td align="center" width="25%">
<a href="./examples/postprocessing.html"><img src="./images/postprocessing.png" width="100%"></a><br>
<b>Post-processing</b><br><sub>EffectComposer 后期效果</sub>
</td>
<td align="center" width="25%">
<a href="./examples/environment-map.html"><img src="./images/environment-map.png" width="100%"></a><br>
<b>Environment Map</b><br><sub>PMREM 环境光照与反射</sub>
</td>
<td align="center" width="25%">
<a href="./examples/tsl-shader.html"><img src="./images/tsl-shader.png" width="100%"></a><br>
<b>TSL Shader</b><br><sub>节点着色器系统</sub>
</td>
</tr>
<tr>
<td align="center" width="25%">
<a href="./examples/webgpu-basics.html"><img src="./images/webgpu-basics.png" width="100%"></a><br>
<b>WebGPU Basics</b><br><sub>WebGPU 渲染器 + 降级</sub>
</td>
<td></td><td></td><td></td>
</tr>
</table>

---

## 目录

- [快速开始](#快速开始)
- [CDN 导入模板](#cdn-导入模板)
- [示例演示](#示例演示)
  - [初级示例](#初级示例-beginner)
  - [中级示例](#中级示例-intermediate)
  - [高级示例](#高级示例-advanced)
- [参考文档](#参考文档)
- [API 速查](#api-速查)
- [官方资源](#官方资源)

---

## 快速开始

所有示例均为**独立 HTML 文件**，无需构建工具，直接用浏览器打开即可运行。

```bash
# 用任意 HTTP 服务器托管（推荐，避免 CORS 问题）
npx serve .

# 或者直接双击 HTML 文件打开（部分功能需要服务器环境）
```

最小场景骨架：

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

  // 1. 场景 + 相机 + 渲染器
  const scene    = new THREE.Scene();
  const camera   = new THREE.PerspectiveCamera(75, innerWidth / innerHeight, 0.1, 1000);
  const renderer = new THREE.WebGLRenderer({ antialias: true });
  renderer.setSize(innerWidth, innerHeight);
  document.body.appendChild(renderer.domElement);
  camera.position.z = 5;

  // 2. 添加物体
  const mesh = new THREE.Mesh(
    new THREE.BoxGeometry(),
    new THREE.MeshStandardMaterial({ color: 0x44aaff })
  );
  scene.add(mesh);
  scene.add(new THREE.DirectionalLight(0xffffff, 3).position.set(5, 5, 5));

  // 3. 控制器 + 渲染循环
  const controls = new OrbitControls(camera, renderer.domElement);
  renderer.setAnimationLoop(() => {
    mesh.rotation.y += 0.01;
    controls.update();
    renderer.render(scene, camera);
  });

  // 4. 响应式尺寸
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

## CDN 导入模板

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

常用 addons 路径：

| 功能 | 导入路径 |
|------|---------|
| OrbitControls | `three/addons/controls/OrbitControls.js` |
| GLTFLoader | `three/addons/loaders/GLTFLoader.js` |
| DRACOLoader | `three/addons/loaders/DRACOLoader.js` |
| EffectComposer | `three/addons/postprocessing/EffectComposer.js` |
| UnrealBloomPass | `three/addons/postprocessing/UnrealBloomPass.js` |
| RGBELoader | `three/addons/loaders/RGBELoader.js` |
| Stats | `three/addons/libs/stats.module.js` |

---

## 示例演示

### 初级示例 (Beginner)

---

#### 1. Hello Cube — 基础旋转立方体

**文件**: [`examples/hello-cube.html`](./examples/hello-cube.html)

**演示内容**:
- PerspectiveCamera + WebGLRenderer 基础设置
- MeshStandardMaterial 物理材质
- DirectionalLight / PointLight / AmbientLight 三光源组合
- EdgesGeometry 线框叠加显示
- OrbitControls 带阻尼的相机交互
- 场景雾效 (Fog)
- 响应式 resize 处理

```javascript
// 核心代码片段：带阴影的旋转立方体
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

#### 2. Geometries — 所有内置几何体

**文件**: [`examples/geometries.html`](./examples/geometries.html)

**演示内容**:
- 15 种内置几何体网格展示
- EdgesGeometry 线框叠加
- Raycaster 悬停 tooltip 显示几何体名称
- HSL 色系自动配色

**展示的几何体**:

| 几何体 | 构造函数 | 关键参数 |
|--------|---------|---------|
| 立方体 | `BoxGeometry(w, h, d)` | 宽高深 |
| 球体 | `SphereGeometry(r, wSeg, hSeg)` | 半径、分段数 |
| 圆柱 | `CylinderGeometry(rTop, rBot, h)` | 上下半径、高 |
| 圆锥 | `ConeGeometry(r, h, seg)` | 半径、高度 |
| 圆环 | `TorusGeometry(r, tube, rSeg, tSeg)` | 主半径、管半径 |
| 环面结 | `TorusKnotGeometry(r, tube, p, q)` | 形态参数 p/q |
| 二十面体 | `IcosahedronGeometry(r, detail)` | 细分层级 |
| 胶囊 | `CapsuleGeometry(r, len, capSeg, radSeg)` | 半径、长度 |
| 平面 | `PlaneGeometry(w, h, wSeg, hSeg)` | 宽高、分段 |
| 圆形 | `CircleGeometry(r, seg)` | 半径、分段 |
| 旋转体 | `LatheGeometry(points, seg)` | 轮廓点数组 |

---

#### 3. Materials — 材质类型对比

**文件**: [`examples/materials.html`](./examples/materials.html)

**演示内容**:
- 11 种材质类型并排对比
- 绕场公转点光源动态打光
- 投影 HTML label 覆层

**展示的材质**:

| 材质 | 特点 | 适用场景 |
|------|------|---------|
| `MeshBasicMaterial` | 无光照、纯色 | UI 元素、调试 |
| `MeshNormalMaterial` | 法线可视化 | 调试法线方向 |
| `MeshLambertMaterial` | 漫反射（Gouraud） | 低性能设备 |
| `MeshPhongMaterial` | 高光（Phong） | 塑料、光滑表面 |
| `MeshStandardMaterial` | PBR 金属粗糙度 | 通用物理材质 |
| `MeshPhysicalMaterial` | 清漆/透射/虹彩 | 汽车漆、玻璃 |
| `MeshToonMaterial` | 卡通分级着色 | 卡通渲染 |
| `MeshDepthMaterial` | 深度可视化 | 后处理效果 |
| `wireframe` | 线框模式 | 结构调试 |

```javascript
// PBR 玻璃材质示例
const glassMat = new THREE.MeshPhysicalMaterial({
  color: 0xffffff,
  transmission: 0.95,   // 透射率
  thickness: 0.5,        // 厚度（折射用）
  roughness: 0.05,
  ior: 1.5,              // 折射率
  transparent: true,
});
```

---

#### 4. Lights — 所有光源类型

**文件**: [`examples/lights.html`](./examples/lights.html)

**演示内容**:
- 5 种光源类型，复选框独立开关
- 所有光源附带可视化 Helper
- 曝光度滑块实时调节

**光源对比**:

| 光源 | 特点 | 是否支持阴影 |
|------|------|------------|
| `AmbientLight(color, intensity)` | 全局环境光 | ❌ |
| `DirectionalLight(color, intensity)` | 平行光（模拟太阳） | ✅ |
| `PointLight(color, intensity, distance)` | 点光源（灯泡） | ✅ |
| `SpotLight(color, intensity, dist, angle)` | 聚光灯 | ✅ |
| `HemisphereLight(sky, ground, intensity)` | 半球光（天空/地面） | ❌ |
| `RectAreaLight(color, intensity, w, h)` | 矩形面光 | ❌ |

```javascript
// DirectionalLight 阴影配置
const light = new THREE.DirectionalLight(0xffffff, 2);
light.castShadow = true;
light.shadow.mapSize.width  = 2048;
light.shadow.mapSize.height = 2048;
light.shadow.camera.near = 0.5;
light.shadow.camera.far  = 50;
light.shadow.bias = -0.001;  // 消除 shadow acne
```

---

#### 5. Shadows — 阴影映射

**文件**: [`examples/shadows.html`](./examples/shadows.html)

**演示内容**:
- 4 种阴影类型切换：BasicShadowMap / PCFShadowMap / PCFSoftShadowMap / VSMShadowMap
- Shadow Map 分辨率、偏移(bias) 实时调节
- CameraHelper 可视化阴影相机视锥体

```javascript
renderer.shadowMap.enabled = true;
renderer.shadowMap.type = THREE.PCFSoftShadowMap; // 推荐

// 物体开启投影/接收
mesh.castShadow    = true;
mesh.receiveShadow = true;
```

---

### 中级示例 (Intermediate)

---

#### 6. Textures — 程序纹理

**文件**: [`examples/textures.html`](./examples/textures.html)

**演示内容**:
- 用 Canvas 2D API 程序生成 6 种纹理（无需外部图片）
- 棋盘格 / 径向渐变 / 网格 / 像素噪声 / HSL 条纹 / UV 编号
- CanvasTexture 实时更新

```javascript
// 程序棋盘纹理
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

#### 7. Orbit Controls — 相机控制器

**文件**: [`examples/orbit-controls.html`](./examples/orbit-controls.html)

**演示内容**:
- OrbitControls 所有属性面板控制
- 阻尼/自动旋转/平移/缩放开关
- 旋转/平移/缩放速度调节
- 距离限制 (minDistance / maxDistance)

```javascript
import { OrbitControls } from 'three/addons/controls/OrbitControls.js';

const controls = new OrbitControls(camera, renderer.domElement);
controls.enableDamping = true;   // 开启阻尼（惯性）
controls.dampingFactor  = 0.05;
controls.autoRotate     = true;
controls.autoRotateSpeed = 2.0;
controls.minDistance    = 2;
controls.maxDistance    = 50;
controls.maxPolarAngle  = Math.PI / 2; // 禁止翻转到地面以下

// ⚠️ 必须在动画循环中调用
renderer.setAnimationLoop(() => {
  controls.update(); // 必须！
  renderer.render(scene, camera);
});
```

---

#### 8. Particles — 粒子系统

**文件**: [`examples/particles.html`](./examples/particles.html)

**演示内容**:
- 5 万粒子实时动画
- 4 种分布模式：球形 / 银河螺旋 / 波浪 / 立方体
- 粒子大小 / 速度 / 颜色控制
- AdditiveBlending 叠加混合

```javascript
// Points 粒子系统
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

#### 9. Raycasting — 鼠标拾取

**文件**: [`examples/raycasting.html`](./examples/raycasting.html)

**演示内容**:
- Raycaster.setFromCamera() 鼠标射线投射
- 悬停高亮（emissive 发光）
- 点击选中 + 浮动 tooltip 显示世界坐标
- 指针样式动态切换

```javascript
const raycaster = new THREE.Raycaster();
const pointer   = new THREE.Vector2();

window.addEventListener('mousemove', (e) => {
  pointer.x =  (e.clientX / innerWidth)  * 2 - 1;
  pointer.y = -(e.clientY / innerHeight) * 2 + 1;
});

// 在动画循环中
raycaster.setFromCamera(pointer, camera);
const hits = raycaster.intersectObjects(pickableObjects);
if (hits.length > 0) {
  const { object, point, distance } = hits[0];
  object.material.emissive.setHex(0x331122); // 高亮
}
```

---

#### 10. Animation Mixer — 关键帧动画

**文件**: [`examples/animation-mixer.html`](./examples/animation-mixer.html)

**演示内容**:
- AnimationMixer 驱动多个物体
- VectorKeyframeTrack（位置）
- QuaternionKeyframeTrack（旋转）
- 播放/暂停/停止/速度/循环模式 UI

```javascript
const mixer = new THREE.AnimationMixer(scene);

// 位置关键帧
const posTrack = new THREE.VectorKeyframeTrack(
  '.position',           // 目标属性路径
  [0, 1, 2, 3],          // 时间点（秒）
  [0,0,0,  0,3,0,  0,0,0, 0,1,0]  // 对应值（x,y,z 三元组）
);

const clip = new THREE.AnimationClip('bounce', 3, [posTrack]);
const action = mixer.clipAction(clip, targetMesh);
action.setLoop(THREE.LoopRepeat, Infinity);
action.play();

// 动画循环中
const delta = clock.getDelta();
mixer.update(delta);
```

---

#### 11. Morph Targets — 顶点变形

**文件**: [`examples/morph-targets.html`](./examples/morph-targets.html)

**演示内容**:
- 4 个 morphAttribute 变形目标：膨胀/尖刺/扭曲/压扁
- morphTargetInfluences 权重滑块
- 自动动画模式（多目标同时混合）

```javascript
const geo = new THREE.SphereGeometry(1.5, 64, 64);

// 定义变形目标（相对偏移量）
const inflateDisp = new Float32Array(geo.attributes.position.count * 3);
// ... 填充每顶点偏移量 ...

geo.morphAttributes.position = [
  new THREE.BufferAttribute(inflateDisp, 3),
  new THREE.BufferAttribute(spikeDisp, 3),
];
geo.morphTargetsRelative = true; // 相对模式

const mesh = new THREE.Mesh(geo, material);
mesh.morphTargetInfluences[0] = 0.5; // 0~1 权重
mesh.morphTargetInfluences[1] = 0.3;
```

---

#### 12. Instanced Mesh — 大规模实例渲染

**文件**: [`examples/instanced-mesh.html`](./examples/instanced-mesh.html)

**演示内容**:
- 最多 10 万实例，单次 Draw Call
- 每实例独立位置、旋转、缩放（Matrix4）
- 每实例独立颜色（setColorAt）
- FPS 计数器验证性能优势

```javascript
const count = 10000;
const iMesh = new THREE.InstancedMesh(geometry, material, count);
iMesh.instanceMatrix.setUsage(THREE.DynamicDrawUsage);

const dummy = new THREE.Object3D();
const color = new THREE.Color();

for (let i = 0; i < count; i++) {
  // 设置变换矩阵
  dummy.position.set(rx, ry, rz);
  dummy.rotation.set(rx, ry, 0);
  dummy.scale.setScalar(Math.random() * 2 + 0.5);
  dummy.updateMatrix();
  iMesh.setMatrixAt(i, dummy.matrix);

  // 设置颜色
  color.setHSL(i / count, 0.8, 0.5);
  iMesh.setColorAt(i, color);
}

iMesh.instanceMatrix.needsUpdate = true;
iMesh.instanceColor.needsUpdate  = true;
scene.add(iMesh);
```

---

#### 13. Fog & Skybox — 雾效与大气

**文件**: [`examples/fog-skybox.html`](./examples/fog-skybox.html)

**演示内容**:
- Linear Fog vs FogExp2 切换对比
- 4 种天空预设（日间/黄昏/夜晚/阴天）
- 树林街道场景 + 路灯点光源
- 自动行走相机漫游

```javascript
// 线性雾（near ~ far 范围内从无到全雾）
scene.fog = new THREE.Fog(0x87ceeb, 10, 80);

// 指数雾（密度均匀衰减，更自然）
scene.fog = new THREE.FogExp2(0x050514, 0.025);

// 雾色要与场景背景色匹配
scene.background = new THREE.Color(scene.fog.color);
```

---

#### 14. GLTF Loader — 加载 3D 模型

**文件**: [`examples/gltf-loader.html`](./examples/gltf-loader.html)

**演示内容**:
- GLTFLoader + DRACOLoader 压缩格式支持
- LoadingManager 进度回调
- 加载 KhronosGroup 官方示例模型（BoxAnimated.gltf）
- gltf.scene 场景树遍历显示
- 模型动画 AnimationMixer 驱动

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

    // 播放动画
    const mixer = new THREE.AnimationMixer(model);
    gltf.animations.forEach(clip => mixer.clipAction(clip).play());
  },
  (xhr) => console.log(`${xhr.loaded / xhr.total * 100}% loaded`),
  (err) => console.error(err)
);
```

---

#### 15. Sprite Billboard — 精灵与公告板

**文件**: [`examples/sprite-billboard.html`](./examples/sprite-billboard.html)

**演示内容**:
- THREE.Sprite 始终朝向相机
- Canvas 文字 label / 光晕粒子 / 图标三种类型
- sizeAttenuation 距离缩放开关
- 星球场景演示标注系统

```javascript
// 创建文字标注精灵
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

### 高级示例 (Advanced)

---

#### 16. Custom Shader — GLSL 自定义着色器

**文件**: [`examples/custom-shader.html`](./examples/custom-shader.html)

**演示内容**:
- ShaderMaterial 顶点/片元着色器完整流程
- 4 种 GLSL 效果预设：
  - **Wave Displacement** — 正弦波顶点偏移
  - **Plasma** — 多层正弦叠加等离子体
  - **Fresnel / Rim Light** — 菲涅尔边缘发光
  - **Hologram** — 扫描线 + 闪烁全息效果
- uniforms 实时传递（时间/振幅/色相）

```glsl
// 顶点着色器：Wave Displacement
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
// JavaScript 端
const material = new THREE.ShaderMaterial({
  uniforms: {
    u_time:      { value: 0 },
    u_amplitude: { value: 0.3 },
  },
  vertexShader:   vertGLSL,
  fragmentShader: fragGLSL,
  side: THREE.DoubleSide,
});

// 动画循环中更新
material.uniforms.u_time.value += clock.getDelta();
```

---

#### 17. Post-processing — 后期处理

**文件**: [`examples/postprocessing.html`](./examples/postprocessing.html)

**演示内容**:
- EffectComposer 完整管线
- UnrealBloomPass 泛光（threshold/strength/radius 控制）
- FilmPass 胶片颗粒
- GlitchPass 故障艺术效果
- DotScreenPass 点阵屏幕
- RGBShiftShader 色差

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
composer.addPass(new OutputPass()); // 最后一个 pass 负责色调映射输出

// 渲染时用 composer 替代 renderer
renderer.setAnimationLoop(() => {
  composer.render(); // ← 替代 renderer.render(scene, camera)
});

// Resize 时同步更新
window.addEventListener('resize', () => {
  composer.setSize(innerWidth, innerHeight);
});
```

---

#### 18. Environment Map — 环境贴图与反射

**文件**: [`examples/environment-map.html`](./examples/environment-map.html)

**演示内容**:
- PMREMGenerator 从全景图生成 PMREM 环境贴图
- 程序生成等距柱状全景纹理（3 种天空预设）
- scene.environment 全局环境光照
- 金属度/粗糙度渐变球体展示 PBR 反射效果

```javascript
// 从等矩形全景图生成环境贴图
const pmrem = new THREE.PMREMGenerator(renderer);
pmrem.compileEquirectangularShader();

const equirectTex = new THREE.TextureLoader().load('hdr/env.jpg', (tex) => {
  tex.mapping = THREE.EquirectangularReflectionMapping;
  const envMap = pmrem.fromEquirectangular(tex).texture;
  pmrem.dispose();
  tex.dispose();

  scene.environment = envMap;   // 所有 MeshStandardMaterial 自动使用
  scene.background  = envMap;   // 同时作为天空背景
});

// 从 RGBELoader 加载 HDR 文件
import { RGBELoader } from 'three/addons/loaders/RGBELoader.js';
new RGBELoader().load('env.hdr', (tex) => {
  const envMap = pmrem.fromEquirectangular(tex).texture;
  scene.environment = envMap;
});
```

---

#### 19. TSL Shader — 节点着色器

**文件**: [`examples/tsl-shader.html`](./examples/tsl-shader.html)

**演示内容**:
- TSL（Three Shading Language）节点材质等效 GLSL 模式
- 4 种效果：顶点波浪 / Simplex 噪声位移 / UV 渐变色 / 菲涅尔发光
- 等效展示 TSL 节点图和 GLSL 实现的对应关系

```javascript
// TSL 写法（需要 WebGPURenderer 或 NodeMaterial）
import { MeshStandardNodeMaterial } from 'three/addons/nodes/materials/MeshStandardNodeMaterial.js';
import { sin, time, positionLocal, normalLocal, vec3 } from 'three/addons/nodes/tsl/TSLBase.js';

const mat = new MeshStandardNodeMaterial({ color: 0x4488ff });

// 节点表达式：顶点 = 局部位置 + 法线 * sin(时间) * 0.2
mat.positionNode = positionLocal.add(
  normalLocal.mul(sin(time).mul(0.2))
);
```

---

#### 20. WebGPU Basics — WebGPU 渲染器

**文件**: [`examples/webgpu-basics.html`](./examples/webgpu-basics.html)

**演示内容**:
- WebGPURenderer 特性检测 + 自动降级 WebGL
- 浏览器支持状态可视化指示器（绿色=WebGPU / 橙色=WebGL 降级）
- 标准 Three.js 场景与 WebGPURenderer 完全兼容
- 代码注释展示 WebGPU 初始化差异

```javascript
// WebGPU 检测 + 降级模式
async function createRenderer() {
  if (navigator.gpu) {
    const adapter = await navigator.gpu.requestAdapter();
    if (adapter) {
      const { default: WebGPURenderer } = await import(
        'three/addons/renderers/webgpu/WebGPURenderer.js'
      );
      const renderer = new WebGPURenderer({ antialias: true });
      await renderer.init(); // ⚠️ WebGPU 必须 await init()
      return renderer;
    }
  }
  // 降级到 WebGL
  return new THREE.WebGLRenderer({ antialias: true });
}

const renderer = await createRenderer();
```

> **浏览器支持**: Chrome 113+ / Edge 113+ 支持 WebGPU；Firefox / Safari 暂用 WebGL 降级。

---

## 参考文档

| 文档 | 内容 |
|------|------|
| [core-concepts.md](./references/core-concepts.md) | Scene、Camera、Renderer、坐标系、场景图、最小模板 |
| [geometries-materials.md](./references/geometries-materials.md) | 所有内置几何体构造函数、自定义 BufferGeometry、材质属性表 |
| [lights-shadows.md](./references/lights-shadows.md) | 光源类型、阴影配置模式、SpotLight/RectAreaLight 详解 |
| [animations.md](./references/animations.md) | AnimationMixer、KeyframeTrack、动作 API、形态目标、骨骼动画 |
| [loaders.md](./references/loaders.md) | TextureLoader、GLTFLoader、OBJLoader、FBXLoader、RGBELoader、FontLoader |
| [postprocessing.md](./references/postprocessing.md) | EffectComposer 搭建、所有 Pass 速览、ShaderPass、OutlinePass |
| [performance.md](./references/performance.md) | InstancedMesh、LOD、内存释放、纹理优化、Stats、视锥剔除 |

---

## API 速查

### 场景图核心类

```javascript
// 场景
const scene = new THREE.Scene();
scene.background = new THREE.Color(0x87ceeb); // 纯色背景
scene.fog = new THREE.FogExp2(0x87ceeb, 0.02); // 指数雾

// 相机
const cam = new THREE.PerspectiveCamera(fov, aspect, near, far);
// fov=75 aspect=innerWidth/innerHeight near=0.1 far=1000

// 渲染器
const renderer = new THREE.WebGLRenderer({ antialias: true });
renderer.setSize(innerWidth, innerHeight);
renderer.setPixelRatio(Math.min(devicePixelRatio, 2)); // 限制最大 2x
renderer.shadowMap.enabled = true;
renderer.toneMapping = THREE.ACESFilmicToneMapping;
renderer.toneMappingExposure = 1.0;
```

### 网格与材质

```javascript
const mesh = new THREE.Mesh(geometry, material);
mesh.position.set(x, y, z);
mesh.rotation.set(rx, ry, rz); // 欧拉角（弧度）
mesh.scale.setScalar(2);        // 等比缩放
mesh.castShadow = true;
mesh.receiveShadow = true;
scene.add(mesh);
```

### 渲染循环

```javascript
const clock = new THREE.Clock();

renderer.setAnimationLoop(() => {
  const delta = clock.getDelta();    // 帧间隔（秒）
  const elapsed = clock.getElapsedTime(); // 累计时间（秒）

  // 更新逻辑...
  mixer?.update(delta);
  controls.update();

  renderer.render(scene, camera);
});
```

### 内存清理

```javascript
// 切换场景或销毁对象时务必手动释放
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

// 整个场景
renderer.dispose();
renderer.forceContextLoss();
```

---

## 官方资源

| 链接 | 描述 |
|------|------|
| [threejs.org](https://threejs.org/) | 官网主页 |
| [threejs.org/docs](https://threejs.org/docs/) | API 文档 |
| [threejs.org/examples](https://threejs.org/examples/) | 官方示例库（300+） |
| [threejs.org/manual](https://threejs.org/manual/) | 入门教程手册 |
| [discourse.threejs.org](https://discourse.threejs.org/) | 官方论坛 |
| [github.com/mrdoob/three.js](https://github.com/mrdoob/three.js) | GitHub 仓库 |

---

<p align="center">
  <sub>Three.js r167 · CDN: cdn.jsdelivr.net/npm/three@0.167.1 · 20 示例 · 7 参考文档</sub>
</p>
