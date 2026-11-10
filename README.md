# Opus 5.5 vs Fable 5.2 · 单文件 Demo 对比

同一组三个提示词，分别交给 Claude Opus 5.5 和 Claude Fable 5.2，各自一次性产出单个 HTML 文件。所有内容都由代码生成，没有图片或音频素材（城市场景只从 CDN 加载 Three.js）。

## 在线查看

开启 GitHub Pages 后：

- 首页：`https://<你的用户名>.github.io/<仓库名>/`
- 并排对比：`https://<你的用户名>.github.io/<仓库名>/compare.html?t=01`（`t=02` 赛车，`t=03` 流体）

对比页横屏时左右并排、竖屏时上下排列，点「隐藏」可以去掉工具条直接录屏。

## 测试

| # | 测试 | 提示词 | Opus 5.5 | Fable 5.2 |
|---|---|---|---|---|
| 01 | 程序化夜景城市（Three.js） | [prompt](prompts/01-night-city.md) | [demo](opus-5.5/01-night-city.html) | [demo](fable-5.2/01-night-city.html) |
| 02 | 俯视角街机赛车 | [prompt](prompts/02-racing-game.md) | [demo](opus-5.5/02-racing-game.html) | [demo](fable-5.2/02-racing-game.html) |
| 03 | GPU 实时流体模拟（WebGL） | [prompt](prompts/03-fluid.md) | [demo](opus-5.5/03-fluid.html) | [demo](fable-5.2/03-fluid.html) |

## 目录结构

```
.
├── index.html          # 画廊首页
├── compare.html        # 同屏并排对比（录屏用）
├── prompts/            # 三个提示词原文 + 考察点
├── opus-5.5/           # Opus 5.5 的三个结果
└── fable-5.2/          # Fable 5.2 的三个结果
```

## 测试说明

- 每个提示词只发送一次，结果是模型在那一轮回复里交付的文件（模型可以在回复过程中自己运行、检查和修正），人没有手动改过代码。
- 浏览器：<填写>；设备：<填写>。
