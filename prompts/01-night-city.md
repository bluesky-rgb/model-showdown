# 01 · 程序化夜景城市（Three.js）

## Prompt

```
Build a single self-contained HTML file using Three.js (from a CDN, no other external assets). Create a procedurally generated city at night: varied skyscrapers with lit windows, streets with cars whose headlights and taillights move along the roads, and a smooth day-to-night cycle. Add a cinematic camera that flies through the city automatically, and let me switch to free-fly mode with the mouse and keyboard. Everything must be generated in code. It should run at 60fps in a normal browser.
```

## 考察点
- Three.js 场景组织与性能（实例化渲染、draw call 控制）
- 程序化生成（建筑、窗户、道路、车流）
- 昼夜循环的光照与天空过渡
- 自动电影镜头 + 自由飞行双模式交互
