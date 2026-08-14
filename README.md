# 🏀 Michael.Kai.com

> **张海源 Michael 的个人网站** — 单文件 · 零依赖 · 纯前端
> **Michael's personal website** — single-file · zero-dependency · pure frontend

**🌐 线上地址 / Live: https://michael.kai.com/**
（备用镜像 / Backup mirror: https://james-kobe-curry.github.io/Michael.Kai.com/）

深色科技风 + 篮球主题的个人展示站：一键切换的中英双语、可拖拽投篮的完整彩蛋系统、NBA 2K 风格六维雷达图……所有代码都在一个 `index.html` 里，双击即可打开，无需构建、无需服务器。

A dark-tech themed personal portfolio with a basketball twist: bilingual zh/en in one click, a fully playable basketball shooting easter egg, an NBA 2K-style attribute radar… Everything lives in a single `index.html` — double-click to open, no build step, no server required.

---

## ✨ 功能亮点 / Features

- **单文件架构**：内联 CSS/JS，零框架零依赖（含 Web Audio、SVG 均手写）
- **6 大板块**：首页 / 关于我 / 技能 / 项目 / 荣誉 / 联系（Hash 路由，刷新不丢页面、可分享链接）
- **中英双语**：一键切换 + localStorage 记忆；标签页标题同步
- **🏀 投篮彩蛋**（可玩！）：
  - 拖动篮球定位 + 双击出手，瞄准虚线为**重力抛物线弧**（与真实弹道逐点一致）
  - 距离 ≥550px 记三分（`THREE_DIST` 常量可调）；命中率随距离线性衰减：贴脸 100% → 最远 30%
  - MISS! / SCORE! / THREE POINTS! 爆炸播报 + 粒子特效；命中篮网晃动、未中砸筐弹出
  - 计分板持久化（刷新不掉分）、🔥 连击徽章、命中率面板、最近 5 球历史、10/20/30/40/50/75/100 分里程碑播报
  - WebAudio 合成音效（出手嗖 / 打铁哐 / 空心唰 / 三分蜂鸣器），导航栏 🔊 开关
- **🎯 NBA 2K 属性雷达图**：悬停显示各维度数值；技能分类带熟练度条
- **🏆 荣誉陈列室**：NBA 风格奖杯图标（金属渐变 + 玻璃容器）
- **🎁 隐藏彩蛋**：双击任意 "Michael" 大字签名 或 键盘连按 `M V P` → 全场彩带庆祝
- **🎨 视觉系统**：玻璃质感容器、渐变描边图标、球场线条背景、流光跑马灯、卡片 3D 悬停、深色滚动条

## 🚀 快速开始 / Quick Start

**方式一（最简单）**：直接双击打开 `index.html`

**方式二（本地服务）**：

```bash
cd Michael.Kai.com
python -m http.server 8765
# 浏览器访问 http://localhost:8765
```

部署到任意静态托管（GitHub Pages / Vercel / Netlify）只需上传整个目录。换云服务器/正式域名等进阶部署方案见 [部署方案.md](部署方案.md)。

## 📁 文件结构 / Project Structure

```
Michael.Kai.com/
├── index.html           # 全部页面结构 + 样式 + 逻辑（单文件核心）
├── avatar.png           # 关于我页头像
├── avatar1.png          # 导航栏头像 + 标签页图标（favicon）
├── basketball.png       # 投篮彩蛋篮球（Fluent 3D emoji）
├── 张海源_简历.pdf      # 「下载简历」按钮附件
└── README.md
```

## 🛠 技术栈 / Tech Stack

- 原生 **HTML / CSS / JavaScript**（ES6+）
- 手写 **SVG**（雷达图、篮筐、奖杯图标、球场线条）
- **Web Audio API**（程序化合成音效，零音频文件）
- `localStorage`（语言/计分/音效记忆）+ Hash 路由
- 无任何第三方依赖 / No third-party dependencies

## ⚙️ 可调参数 / Tunables

代码内搜索以下常量即可调整：`THREE_DIST`（三分线距离）、`GRAVITY`（投篮重力）、`hitPct()`（命中率曲线）、`RADAR_VALUES`（六维属性值）、`GITHUB_URL`、`BASKETBALL`（球员档案卡）。

## 👤 作者 / Author

**张海源 Michael** — AI 全栈开发实习生 · 上海海洋大学

- GitHub: [@james-kobe-curry](https://github.com/james-kobe-curry)
- 本项目: [Michael.Kai.com](https://github.com/james-kobe-curry/Michael.Kai.com)

---

© 2026 Michael · Built with 🏀
