# 中国象棋 (Xiangqi)

纯前端中国象棋游戏，单文件 HTML，零依赖，打开即玩。

## 玩法与功能

- **人机对战**：AI 可选执红或执黑，搜索深度可调
- **人人对战**：本地双人轮流走棋
- **悔棋**：撤销上一手（人机模式回退到你的回合），快捷键 `Ctrl+Z`
- **棋局导入/导出**：JSON 格式保存与恢复局面
- 走棋记录、回合提示、胜负判定（含绝杀检测）

## AI 实现

- Negamax + Alpha-Beta 剪枝
- 静止搜索（Quiescence Search）防止水平线效应
- 差值剪枝：静态评估追不上 alpha 的着法直接跳过
- 子力价值评估 + 可调搜索深度

## 运行

直接用浏览器打开 `index.html` 即可，无需安装任何东西。

也可以访问 [GitHub Pages](https://jiangpedro.github.io/xiangqi/) 在线玩（需在仓库 Settings → Pages 中启用）。

## 技术栈

- HTML5 Canvas 绘制棋盘与棋子
- 原生 JavaScript（无任何第三方库）
- 单文件，约 30 KB

## License

MIT
