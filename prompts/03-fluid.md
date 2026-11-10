# 03 · GPU 实时流体模拟（WebGL）

## Prompt

```
Create a single HTML file with an interactive real-time fluid simulation on the GPU (WebGL). I can drag the mouse to stir colorful dye through the fluid, and there are on-screen sliders for viscosity, vorticity, and color. Add a mode where solid objects I draw act as obstacles the fluid flows around. Make it look beautiful and run smoothly.
```

## 考察点
- Stable Fluids 求解器的 GPU 实现（平流、散度、压力投影、涡度约束）
- 粘度 / 涡度 / 颜色控件是否真实生效
- 障碍物边界条件（流体是否绕流、有无泄漏）
- 视觉表现（配色、光晕、障碍物质感）与流畅度
