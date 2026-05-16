# Three.js 3D 图形技能库

> **语言**: 中文 | [English](./README.md)

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

## 新增示例（30个）

### 新增初级示例

<table>
<tr>
<td align="center" width="25%">
<a href="./examples/axes-helpers.html"><img src="./images/axes-helpers.png" width="100%"></a><br>
<b>坐标轴辅助器</b><br><sub>AxesHelper · GridHelper · ArrowHelper · BoxHelper</sub>
</td>
<td align="center" width="25%">
<a href="./examples/wireframe-mode.html"><img src="./images/wireframe-mode.png" width="100%"></a><br>
<b>线框模式</b><br><sub>实体 · WireframeGeometry · EdgesGeometry 对比</sub>
</td>
<td align="center" width="25%">
<a href="./examples/groups-hierarchy.html"><img src="./images/groups-hierarchy.png" width="100%"></a><br>
<b>组与层级</b><br><sub>父子变换 · 太阳系层级结构</sub>
</td>
<td align="center" width="25%">
<a href="./examples/vertex-colors.html"><img src="./images/vertex-colors.png" width="100%"></a><br>
<b>顶点颜色</b><br><sub>逐顶点着色 · HSL/渐变/噪声三种模式</sub>
</td>
</tr>
<tr>
<td align="center" width="25%">
<a href="./examples/transparent-blend.html"><img src="./images/transparent-blend.png" width="100%"></a><br>
<b>透明与混合</b><br><sub>opacity · 普通混合 · 叠加混合</sub>
</td>
<td align="center" width="25%">
<a href="./examples/clock-easing.html"><img src="./images/clock-easing.png" width="100%"></a><br>
<b>时钟与缓动</b><br><sub>THREE.Clock · 6种缓动函数对比</sub>
</td>
<td align="center" width="25%">
<a href="./examples/background-modes.html"><img src="./images/background-modes.png" width="100%"></a><br>
<b>背景模式</b><br><sub>纯色 · 渐变纹理 · CubeMap 环境贴图</sub>
</td>
<td align="center" width="25%">
<a href="./examples/simple-physics.html"><img src="./images/simple-physics.png" width="100%"></a><br>
<b>简单物理</b><br><sub>重力 · 弹性碰撞 · 墙壁边界检测</sub>
</td>
</tr>
<tr>
<td align="center" width="25%">
<a href="./examples/multi-viewport.html"><img src="./images/multi-viewport.png" width="100%"></a><br>
<b>多视口渲染</b><br><sub>scissor 分屏 · 透视 + 正交双摄像机</sub>
</td>
<td align="center" width="25%">
<a href="./examples/css2d-labels.html"><img src="./images/css2d-labels.png" width="100%"></a><br>
<b>CSS2D 标签</b><br><sub>CSS2DRenderer · 3D 投影 HTML 标签</sub>
</td>
<td></td><td></td>
</tr>
</table>

### 新增中级示例

<table>
<tr>
<td align="center" width="25%">
<a href="./examples/curve-path.html"><img src="./images/curve-path.png" width="100%"></a><br>
<b>曲线路径</b><br><sub>CatmullRomCurve3 · TubeGeometry · 路径跟随</sub>
</td>
<td align="center" width="25%">
<a href="./examples/shape-extrude.html"><img src="./images/shape-extrude.png" width="100%"></a><br>
<b>形状拉伸</b><br><sub>THREE.Shape · ExtrudeGeometry · 倒角</sub>
</td>
<td align="center" width="25%">
<a href="./examples/lod.html"><img src="./images/lod.png" width="100%"></a><br>
<b>细节层次</b><br><sub>THREE.LOD · 按距离切换细节级别</sub>
</td>
<td align="center" width="25%">
<a href="./examples/cube-camera.html"><img src="./images/cube-camera.png" width="100%"></a><br>
<b>立方体摄像机</b><br><sub>CubeCamera · 实时环境反射</sub>
</td>
</tr>
<tr>
<td align="center" width="25%">
<a href="./examples/water-surface.html"><img src="./images/water-surface.png" width="100%"></a><br>
<b>水面效果</b><br><sub>ShaderMaterial 波浪位移 · 浪花泡沫</sub>
</td>
<td align="center" width="25%">
<a href="./examples/outline-select.html"><img src="./images/outline-select.png" width="100%"></a><br>
<b>描边选择</b><br><sub>OutlinePass · 点击/悬停高亮描边</sub>
</td>
<td align="center" width="25%">
<a href="./examples/render-target.html"><img src="./images/render-target.png" width="100%"></a><br>
<b>渲染目标</b><br><sub>WebGLRenderTarget · 离屏渲染安全摄像头</sub>
</td>
<td align="center" width="25%">
<a href="./examples/skeleton-anim.html"><img src="./images/skeleton-anim.png" width="100%"></a><br>
<b>骨骼动画</b><br><sub>SkinnedMesh · 骨骼层级 · 蒙皮权重</sub>
</td>
</tr>
<tr>
<td align="center" width="25%">
<a href="./examples/normal-map.html"><img src="./images/normal-map.png" width="100%"></a><br>
<b>法线贴图</b><br><sub>程序化法线贴图 · 表面凹凸细节</sub>
</td>
<td align="center" width="25%">
<a href="./examples/audio-visualizer.html"><img src="./images/audio-visualizer.png" width="100%"></a><br>
<b>音频可视化</b><br><sub>Web Audio FFT → 3D 频谱柱状图</sub>
</td>
<td></td><td></td>
</tr>
</table>

### 新增高级示例

<table>
<tr>
<td align="center" width="25%">
<a href="./examples/procedural-terrain.html"><img src="./images/procedural-terrain.png" width="100%"></a><br>
<b>程序化地形</b><br><sub>多倍频噪声高度图 · 按高度着色</sub>
</td>
<td align="center" width="25%">
<a href="./examples/text-3d.html"><img src="./images/text-3d.png" width="100%"></a><br>
<b>3D 文字</b><br><sub>FontLoader · TextGeometry · 倒角 · 动画</sub>
</td>
<td align="center" width="25%">
<a href="./examples/fat-lines.html"><img src="./images/fat-lines.png" width="100%"></a><br>
<b>粗线渲染</b><br><sub>Line2 · LineMaterial · 可调线宽 · 虚线</sub>
</td>
<td align="center" width="25%">
<a href="./examples/sky-atmosphere.html"><img src="./images/sky-atmosphere.png" width="100%"></a><br>
<b>天空大气</b><br><sub>Sky 着色器 · 太阳位置 · 瑞利散射</sub>
</td>
</tr>
<tr>
<td align="center" width="25%">
<a href="./examples/procedural-city.html"><img src="./images/procedural-city.png" width="100%"></a><br>
<b>程序化城市</b><br><sub>随机建筑 · 街道网格 · 夜晚灯光</sub>
</td>
<td align="center" width="25%">
<a href="./examples/shader-extend.html"><img src="./images/shader-extend.png" width="100%"></a><br>
<b>着色器扩展</b><br><sub>onBeforeCompile · GLSL 注入 · 5种特效</sub>
</td>
<td align="center" width="25%">
<a href="./examples/depth-of-field.html"><img src="./images/depth-of-field.png" width="100%"></a><br>
<b>景深效果</b><br><sub>BokehPass · EffectComposer · 焦距控制</sub>
</td>
<td align="center" width="25%">
<a href="./examples/texture-atlas.html"><img src="./images/texture-atlas.png" width="100%"></a><br>
<b>纹理图集</b><br><sub>精灵表 · UV 偏移帧动画 · 广告牌</sub>
</td>
</tr>
<tr>
<td align="center" width="25%">
<a href="./examples/particle-emitter.html"><img src="./images/particle-emitter.png" width="100%"></a><br>
<b>粒子发射器</b><br><sub>对象池复用 · 生命周期 · 淡出 · 物理</sub>
</td>
<td align="center" width="25%">
<a href="./examples/multi-material.html"><img src="./images/multi-material.png" width="100%"></a><br>
<b>多材质</b><br><sub>单网格多材质分组 · 每面独立材质</sub>
</td>
<td></td><td></td>
</tr>
</table>

---

### 新增初级示例详解

#### 21. 坐标轴辅助器 — Debug 助手

演示 `AxesHelper`（RGB = XYZ 轴）、`GridHelper`、`ArrowHelper`（6个方向箭头）和 `BoxHelper`。可独立开关每种助手。

```javascript
const axes = new THREE.AxesHelper(5); // 红=X, 绿=Y, 蓝=Z
scene.add(axes);
const grid = new THREE.GridHelper(10, 10, 0x444444, 0x222222);
scene.add(grid);
const box = new THREE.BoxHelper(mesh, 0xffff00);
scene.add(box);
box.update(); // 每帧调用（如果网格移动）
```

---

#### 22. 线框模式 — 几何体显示模式

对比实体、`WireframeGeometry`（所有三角形边）和 `EdgesGeometry`（仅硬边）三种显示模式。

```javascript
// WireframeGeometry — 显示所有三角形边
const wireGeo  = new THREE.WireframeGeometry(geo);
const wireMesh = new THREE.LineSegments(wireGeo, new THREE.LineBasicMaterial());

// EdgesGeometry — 仅显示折角大于阈值的边
const edgeGeo  = new THREE.EdgesGeometry(geo);
const edgeMesh = new THREE.LineSegments(edgeGeo, new THREE.LineBasicMaterial({ color: 0xffffff }));
```

---

#### 23. 组与层级 — 父子变换继承

太阳系演示：地球绕太阳公转（子 Group），月亮绕地球公转（孙 Group）。旋转沿层级向下传播。

```javascript
const solarSystem = new THREE.Group();
const earthOrbit  = new THREE.Group(); // solarSystem 的子
const moonOrbit   = new THREE.Group(); // earthOrbit 的子

solarSystem.add(earthOrbit);
earthOrbit.add(moonOrbit);
scene.add(solarSystem);

solarSystem.rotation.y += 0.01; // 影响所有后代
earthOrbit.rotation.y  += 0.03; // 影响地球和月亮
moonOrbit.rotation.y   += 0.07; // 仅影响月亮
```

---

#### 24. 顶点颜色 — 逐顶点着色

对高细分 `SphereGeometry` 每个顶点赋色。三种模式：HSL 彩虹、渐变、噪声。需 `vertexColors: true`。

```javascript
const colors = [];
for (let i = 0; i < pos.count; i++) {
  const c = new THREE.Color().setHSL(i / pos.count, 1, 0.5);
  colors.push(c.r, c.g, c.b);
}
geo.setAttribute('color', new THREE.Float32BufferAttribute(colors, 3));
const mat = new THREE.MeshStandardMaterial({ vertexColors: true });
```

---

#### 25. 透明与混合 — 混合模式

5对演示：不透明、`opacity: 0.5`、`NormalBlending`、`AdditiveBlending`、`depthWrite: false`。

```javascript
// 叠加混合（发光效果、火焰、粒子）
const mat = new THREE.MeshStandardMaterial({
  transparent: true, opacity: 0.7,
  blending: THREE.AdditiveBlending, depthWrite: false,
});
```

---

#### 26. 时钟与缓动 — 动画时序

用 `THREE.Clock` 实现 dt 时基动画。6个方块各用不同缓动：线性、正弦入、三次曲线、弹跳、弹性、回退。

```javascript
const clock = new THREE.Clock();
renderer.setAnimationLoop(() => {
  const t = clock.getElapsedTime();
  const dt = clock.getDelta(); // 距上一帧的时间
  // 各种缓动函数...
});
```

---

#### 27. 背景模式 — 场景背景

切换4种背景：纯色、Canvas 渐变纹理、天空渐变（日落）、程序化 CubeMap 环境。

```javascript
// 渐变纹理背景
const canvas = document.createElement('canvas');
// ... 在 canvas 上绘制渐变 ...
scene.background = new THREE.CanvasTexture(canvas);
```

---

#### 28. 简单物理 — 手写物理模拟

dt 时基重力积分，弹性地面碰撞，墙壁边界检测。无需外部物理引擎。

```javascript
const dt = clock.getDelta();
ball.vy -= gravity * dt;       // 施加重力
ball.py += ball.vy * dt;       // 积分位置

if (ball.py < radius) {        // 地面碰撞
  ball.py = radius;
  ball.vy *= -restitution;     // 弹性反弹
}
```

---

#### 29. 多视口渲染 — 分屏渲染

用 `renderer.setScissor()` + `renderer.setViewport()` 将同一场景渲染到两个视口。

```javascript
renderer.setScissorTest(true);
renderer.setScissor(0, 0, w/2, h);
renderer.setViewport(0, 0, w/2, h);
renderer.render(scene, perspCamera);  // 左：透视摄像机

renderer.setScissor(w/2, 0, w/2, h);
renderer.setViewport(w/2, 0, w/2, h);
renderer.render(scene, orthoCamera);  // 右：正交摄像机
```

---

#### 30. CSS2D 标签 — 3D 投影 DOM 标签

用 `CSS2DRenderer` 将 HTML 元素投影到 3D 空间，标签始终朝向摄像机。

```javascript
import { CSS2DRenderer, CSS2DObject } from 'three/addons/renderers/CSS2DRenderer.js';

const label = new CSS2DObject(divElement);
planet.add(label); // 标签跟随行星移动

// 渲染循环中：
labelRenderer.render(scene, camera);
```

---

### 新增中级示例详解

#### 31. 曲线路径 — 样条曲线路径跟随

`CatmullRomCurve3` 闭合样条曲线 + `TubeGeometry` 管道，物体沿路径运动，粒子轨迹环形缓冲区。

```javascript
const curve = new THREE.CatmullRomCurve3(points, true); // closed=true
const t = (clock.getElapsedTime() * 0.1) % 1;
const pos     = curve.getPointAt(t);
const tangent = curve.getTangentAt(t);
traveler.position.copy(pos);
traveler.lookAt(pos.clone().add(tangent)); // 朝向切线方向
```

---

#### 32. 形状拉伸 — 2D 轮廓到 3D 几何

用 `THREE.Shape` 绘制5种轮廓（星形、心形、箭头、齿轮+内孔、字母），`ExtrudeGeometry` 拉伸成3D。

```javascript
const shape = new THREE.Shape();
// ... 用 moveTo / lineTo / bezierCurveTo 绘制轮廓 ...
const geo = new THREE.ExtrudeGeometry(shape, {
  depth: 0.4, bevelEnabled: true,
  bevelThickness: 0.05, bevelSize: 0.04,
});
```

---

#### 33. 细节层次 — LOD

`THREE.LOD` 按摄像机距离自动切换三档细节（64/16/4 段球体）。颜色变化直观显示当前 LOD 级别。

```javascript
const lod = new THREE.LOD();
lod.addLevel(new THREE.Mesh(new THREE.SphereGeometry(1, 64, 64), mat), 0);  // 近距高精
lod.addLevel(new THREE.Mesh(new THREE.SphereGeometry(1, 16, 16), mat), 8);  // 中距中精
lod.addLevel(new THREE.Mesh(new THREE.SphereGeometry(1, 4,  4),  mat), 20); // 远距低精
lod.update(camera); // 每帧调用
```

---

#### 34. 立方体摄像机 — 实时反射

`WebGLCubeRenderTarget` + `CubeCamera` 每帧更新，实现镀铬球体的实时环境反射。

```javascript
const cubeRT = new THREE.WebGLCubeRenderTarget(256);
const cubeCamera = new THREE.CubeCamera(0.1, 100, cubeRT);
const mat = new THREE.MeshStandardMaterial({ envMap: cubeRT.texture, metalness: 1, roughness: 0 });

// 每帧：隐藏反射对象 → 更新 CubeCamera → 显示
chromeSphere.visible = false;
cubeCamera.update(renderer, scene);
chromeSphere.visible = true;
```

---

#### 35. 水面效果 — Shader 波浪位移

`ShaderMaterial` 顶点着色器中叠加多个正弦波位移，实现水面效果。无需外部 Water 插件。

```javascript
// 顶点着色器中的波浪叠加
newPos.y += sin(position.x * 0.5 + uTime) * 0.4
          + sin(position.z * 0.3 + uTime * 1.3) * 0.3
          + sin((position.x + position.z) * 0.4 + uTime * 0.8) * 0.2;
```

---

#### 36. 描边选择 — 后处理选中高亮

`OutlinePass` 高亮选中对象轮廓。点击切换蓝色选中描边，悬停显示黄色预览描边。

```javascript
import { OutlinePass } from 'three/addons/postprocessing/OutlinePass.js';
const outlinePass = new OutlinePass(new THREE.Vector2(w, h), scene, camera);
outlinePass.visibleEdgeColor.set(0x4488ff); // 蓝色=已选中
composer.addPass(outlinePass);
outlinePass.selectedObjects = [clickedMesh]; // 点击时更新
```

---

#### 37. 渲染目标 — 离屏渲染

`WebGLRenderTarget` 将场景从第二个摄像机渲染到纹理，显示在场景内的"监视器"平面上。

```javascript
const rt = new THREE.WebGLRenderTarget(512, 512);
const monitor = new THREE.Mesh(geo, new THREE.MeshBasicMaterial({ map: rt.texture }));

// 渲染循环：先渲染到 RT，再渲染主场景
renderer.setRenderTarget(rt);
renderer.render(scene, secCamera);
renderer.setRenderTarget(null);
renderer.render(scene, camera);
```

---

#### 38. 骨骼动画 — SkinnedMesh

手动构建骨骼链，蒙皮权重按顶点 Y 坐标分配。用正弦波驱动骨骼旋转，实现挥手/弯曲/扭转。

```javascript
const skeleton = new THREE.Skeleton(bones);
const skinnedMesh = new THREE.SkinnedMesh(geo, mat);
skinnedMesh.bind(skeleton);

// 每帧驱动骨骼
bones.forEach((bone, i) => {
  bone.rotation.z = Math.sin(t * 2 + i * 0.4) * 0.2;
});
```

---

#### 39. 法线贴图 — 表面凹凸细节

用 Canvas API 程序化生成法线贴图（砖墙/鱼鳞/裂石/金属板），动态移动灯光揭示表面细节。

```javascript
// Canvas 生成法线贴图（蓝色=#8080ff 表示垂直法线）
ctx.fillStyle = '#8080ff'; // 平面法线
ctx.fillRect(0, 0, size, size);
// 用不同颜色绘制沟槽、凸起...
material.normalMap = new THREE.CanvasTexture(canvas);
material.normalScale.set(2, 2); // 强度
```

---

#### 40. 音频可视化 — FFT 3D 柱状图

`AnalyserNode` 每帧获取 FFT 频谱数据，驱动3D柱形高度。支持柱状/圆环两种布局，无麦克风时自动演示。

```javascript
const analyser = audioCtx.createAnalyser();
analyser.fftSize = 128; // 64个频率桶
const dataArray = new Uint8Array(analyser.frequencyBinCount);

// 每帧：
analyser.getByteFrequencyData(dataArray);
bars.forEach((bar, i) => { bar.scale.y = dataArray[i] * scale; });
```

---

### 新增高级示例详解

#### 41. 程序化地形 — 噪声高度图

多倍频 fBm 噪声位移128×128平面几何体，顶点按高度着色（水/沙滩/草地/森林/岩石/雪地）。

```javascript
function fbm(x, y, octaves) {
  let v=0, amp=0.5, freq=1, max=0;
  for (let i=0; i<octaves; i++) {
    v += noise2(x*freq, y*freq) * amp;
    max += amp; amp *= 0.5; freq *= 2;
  }
  return v / max;
}
const h = fbm(x/20, z/20, 4) * heightScale;
pos.setY(i, h);
```

---

#### 42. 3D 文字 — FontLoader & TextGeometry

加载 helvetiker_bold 字体，用 `TextGeometry` 创建单个字母网格并添加倒角。支持正常/波浪/爆炸三种动画。

```javascript
import { FontLoader }   from 'three/addons/loaders/FontLoader.js';
import { TextGeometry } from 'three/addons/geometries/TextGeometry.js';

loader.load(fontUrl, font => {
  const geo = new TextGeometry('A', {
    font, size: 1.2, depth: 0.4,
    bevelEnabled: true, bevelThickness: 0.05,
  });
});
```

---

#### 43. 粗线渲染 — Line2 / LineMaterial

`LineMaterial` 支持任意像素宽度（原生 WebGL 线固定1px）。支持顶点颜色、虚线，`resolution` 参数必须设置。

```javascript
import { Line2 }        from 'three/addons/lines/Line2.js';
import { LineMaterial } from 'three/addons/lines/LineMaterial.js';
import { LineGeometry } from 'three/addons/lines/LineGeometry.js';

const mat = new LineMaterial({
  linewidth: 4, vertexColors: true,
  resolution: new THREE.Vector2(innerWidth, innerHeight), // 必须！
});
const line = new Line2(geo, mat);
line.computeLineDistances(); // 虚线需要
```

---

#### 44. 天空大气 — Sky 着色器

`Sky` 插件实现瑞利/米氏散射大气，可调太阳仰角/方位角/浑浊度，配合 `Water` 实现完整室外场景。

```javascript
import { Sky } from 'three/addons/objects/Sky.js';
const sky = new Sky();
sky.scale.setScalar(450000);
scene.add(sky);

const phi   = THREE.MathUtils.degToRad(90 - elevation);
const theta = THREE.MathUtils.degToRad(azimuth);
sky.material.uniforms.sunPosition.value.setFromSphericalCoords(1, phi, theta);
```

---

#### 45. 程序化城市 — 随机建筑群

Math.random() 网格随机生成不同高度/颜色建筑，街道线条，点光源路灯，夜间窗户灯，绕飞摄像机。

```javascript
for (let row = 0; row < SIZE; row++) {
  for (let col = 0; col < SIZE; col++) {
    if (Math.random() < 0.15) continue; // 空地
    const h = 1 + Math.random() * 20;
    const building = new THREE.Mesh(
      new THREE.BoxGeometry(w, h, d),
      new THREE.MeshStandardMaterial({ color: randomColor })
    );
    building.position.set(x, h/2, z);
    scene.add(building);
  }
}
```

---

#### 46. 着色器扩展 — onBeforeCompile

通过 `onBeforeCompile` 向 `MeshStandardMaterial` 注入自定义 GLSL。5种特效：UV 波纹/噪声溶解/彩虹着色/故障/X射线。

```javascript
material.onBeforeCompile = (shader) => {
  shader.uniforms.uTime = { value: 0 };
  shader.fragmentShader = 'uniform float uTime;\n' + shader.fragmentShader;
  shader.fragmentShader = shader.fragmentShader.replace(
    'gl_FragColor = vec4( outgoingLight, diffuseColor.a );',
    `// 在标准输出之后注入自定义 GLSL
     gl_FragColor = vec4( outgoingLight * customEffect, diffuseColor.a );`
  );
};
```

---

#### 47. 景深效果 — BokehPass

`BokehPass` 实现摄像机镜头景深模糊，可调焦距/光圈/最大模糊量，不同 Z 深度的物体模糊程度不同。

```javascript
import { BokehPass } from 'three/addons/postprocessing/BokehPass.js';
const bokehPass = new BokehPass(scene, camera, { focus: 10, aperture: 0.00015, maxblur: 0.006 });
composer.addPass(bokehPass);
// 实时更新参数：
bokehPass.uniforms.focus.value    = sliderValue;
bokehPass.uniforms.aperture.value = 0.0002;
```

---

#### 48. 纹理图集 — 精灵表帧动画

Canvas 程序化生成4×4精灵表（爆炸/火焰/金币旋转），每帧更新 UV `offset` 切换帧。广告牌始终朝向摄像机。

```javascript
mat.map.repeat.set(1/COLS, 1/ROWS); // 单帧大小
// 每帧切换 UV 偏移
const frame = Math.floor((t * fps + offset) % FRAMES);
const col = frame % COLS, row = Math.floor(frame / COLS);
mat.map.offset.set(col / COLS, (ROWS-1-row) / ROWS);
sprite.quaternion.copy(camera.quaternion); // 广告牌朝向
```

---

#### 49. 粒子发射器 — 对象池模式

固定大小粒子池，死亡粒子原地复用（无 GC 压力）。支持火焰/烟雾/火花/雪花4种预设，可调发射率和重力。

```javascript
const pool = Array.from({ length: MAX }, () => ({ active: false, life: 0 }));

function spawnParticle() {
  const p = pool.find(x => !x.active); // 复用死亡粒子
  if (!p) return; // 池已满，跳过
  p.active = true; p.life = 0;
  p.vy = 2 + Math.random() * 3;
}

// 每帧更新
pool.forEach(p => {
  if (!p.active) return;
  p.vy += gravity * dt; p.py += p.vy * dt;
  if (p.life >= p.maxLife) p.active = false; // 回收
});
```

---

#### 50. 多材质 — 每面独立材质

单个 `Mesh` 接受材质数组，每个 Group 对应一个材质。`BoxGeometry` 6面、`CylinderGeometry` 3部分、`ConeGeometry` 2部分均支持。

```javascript
const materials = [
  new THREE.MeshStandardMaterial({ color: 0xff4444 }), // +X 右面
  new THREE.MeshStandardMaterial({ color: 0x4444ff }), // -X 左面
  new THREE.MeshStandardMaterial({ color: 0x44ff44 }), // +Y 顶面
  new THREE.MeshStandardMaterial({ color: 0xffaa00 }), // -Y 底面
  new THREE.MeshStandardMaterial({ color: 0xff44ff }), // +Z 前面
  new THREE.MeshStandardMaterial({ color: 0x44ffff }), // -Z 后面
];
const mesh = new THREE.Mesh(new THREE.BoxGeometry(3, 3, 3), materials);
```

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
