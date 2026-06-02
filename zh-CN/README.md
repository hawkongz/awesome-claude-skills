<div align="center">
  <h1>Awesome Claude Code Skills</h1>
  <p>我日常使用 Claude Code 编程、写文档、学习中积累的好用 Skill 清单。<br>直接告诉 Claude Code 这些名字，它就能自动安装。</p>

  [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](../LICENSE)
  [![Platform](https://img.shields.io/badge/Platform-Claude%20Code-blue)](https://code.claude.com)
  [![Stars](https://img.shields.io/github/stars/hawkongz/awesome-claude-skills)](https://github.com/hawkongz/awesome-claude-skills)

  <p><strong>Language:</strong> <a href="../README.md">English</a> | <a href="README.md">简体中文</a></p>
</div>

---

## 📋 目录

- [开发流程](#-开发流程)
- [文档处理](#-文档处理)
- [前端设计](#-前端设计)
- [测试](#-测试)
- [集成扩展](#-集成扩展)
- [效率工具](#-效率工具)
- [学习辅助](#-学习辅助)
- [快速安装全部](#-快速安装全部)

---

## 🔧 开发流程

### Superpowers
一套完整的开发流程套件，覆盖从需求到交付：头脑风暴 → 计划 → 执行 → TDD → 调试 → 代码审查 → 验证 → 收尾，14 个 skill 协同工作。

触发条件：写代码、修 bug、做功能、提 PR 时自动介入。

- ⭐⭐⭐⭐⭐ · 所有人

---

## 📄 文档处理

### docx
创建、读取、编辑 Word 文档。支持目录、页眉页脚、批注、替换图片等。
- ⭐⭐⭐⭐⭐ · 写报告/方案的人

### pdf
PDF 全功能：读取、合并、拆分、旋转、水印、OCR 识别、表单填写。
- ⭐⭐⭐⭐⭐ · 处理 PDF 资料的人

### mineru-pdf
高精度 PDF 内容解析。提取公式（可编译 LaTeX）、图片（含 bbox 坐标 + 图注）、表格，正确处理双栏排版和扫描件。与官方 pdf skill 互补。

触发条件：`/mineru-pdf`，提到 "MinerU"、"解析这篇论文"、"提取 PDF 的公式" 等。

- ⭐⭐⭐⭐⭐ · 学术科研人员、处理公式密集或扫描件 PDF 的人
- [github.com/hawkongz/mineru-pdf](https://github.com/hawkongz/mineru-pdf)

### pptx
创建和编辑 PPT 演示文稿——读取内容、修改样式、替换图片、合并拆分、基于模板创建。适合"改已有 PPT"的场景。是一个灵活通用的 PPTX 工具箱。
- ⭐⭐⭐⭐ · 做汇报/分享的人

### ppt-master
AI 驱动的高质量 PPT 生成。支持 PDF/Word/Markdown/网页等多种格式输入，三角色协作（策略师 → 图片师 → 执行师），SVG→DrawingML 管线生成原生可编辑 PPTX，内置 20+ 专业模板。适合"从素材从零生成精美幻灯片"的场景。

触发条件："生成PPT"、"做PPT"、"create presentation"、"make slides"。

- ⭐⭐⭐⭐⭐ · 追求专业设计质量的 PPT 制作者
- [github.com/hugohe3/ppt-master](https://github.com/hugohe3/ppt-master)

> **pptx vs ppt-master**：`pptx` 是通用 PPTX 工具箱——读取、编辑、合并、改模板，适合"修改已有 PPT"。`ppt-master` 专注于**从任意文档从零生成专业演示文稿**，设计质量和风格一致性更好，适合"给我素材、帮我做出彩的 PPT"。改/修已有 PPT 用 `pptx`，从素材生成精美幻灯片用 `ppt-master`。
>
> **⚠️ 触发冲突**：两者都对"做PPT""生成PPT"等词触发。建议在 settings.json 中把不常用的那个设为手动调用，避免每次都要选：
> ```json
> "skillOverrides": {
>   "pptx": "user-invocable-only"
> }
> ```
> 这样日常说"做PPT"→ 自动走 `ppt-master`，需要编辑已有文件时用 `/pptx` 显式调用官方 pptx skill。

### xlsx
表格处理：创建、编辑、公式计算、图表、数据清洗、格式转换。
- ⭐⭐⭐⭐ · 处理数据表格的人

---

## 🎨 前端设计

### frontend-design
高质量前端界面设计。生成有创意、不"AI 味"的 UI 代码。

触发条件：提到"设计网页"、"做个页面"、"前端组件"、"美化 UI" 等。

- ⭐⭐⭐⭐⭐ · 前端开发者

### ui-ux-pro-max
UI/UX 设计智囊。50+ 风格、161 调色板、57 字体搭配、99 UX 指南，覆盖 React/Next.js/Vue/SwiftUI/Flutter/Tailwind 等。

触发条件：提到"UI 设计"、"UX 优化"、"配色"、"字体搭配"、"组件样式" 等。

- ⭐⭐⭐⭐⭐ · 做界面的人

---

## 🧪 测试

### webapp-testing
用 Playwright 自动化测试本地 Web 应用。截图、调试 UI、查看浏览器日志。

触发条件：提到"测试页面"、"截屏"、"浏览器调试"、"端到端测试" 等。

- ⭐⭐⭐⭐ · Web 开发者

---

## 🔌 集成扩展

### mcp-builder
构建 MCP 服务器的完整指南。Python（FastMCP）和 Node/TypeScript 都支持。

触发条件：提到"构建 MCP"、"对接 API"、"给 Claude 接工具" 等。

- ⭐⭐⭐ · 想给 Claude 接外部 API 的人

### skill-creator
创建、修改和优化 Claude Code skill。覆盖完整开发周期：起草 → 测试 → 审查 → 改进 → 打包。

触发条件：提到"创建 skill"、"写个 skill"、"做个新 skill"、"优化 skill" 等。

- ⭐⭐⭐⭐ · Skill 开发者

### find-skills
搜索和发现新 Skill。当你想要某个功能但不确定有没有现成 Skill 时用它。

触发条件：提到"有没有 XX 的 skill"、"怎么装 XX"、"找个 skill" 等。

- ⭐⭐⭐⭐⭐ · 所有人

---

## ⚡ 效率工具

### CodeGraph
语义级代码地图。给 Claude Code 提供代码全局视野，避免反复搜索文件。成本降低 ~35%，工具调用减少 ~70%，100% 本地运行。

安装后在项目目录运行 `codegraph init -i` 启用，之后 Claude Code 在该项目中自动获得代码全局感知能力。

- ⭐⭐⭐⭐⭐ · 在大型项目中用 Claude Code 的人
- [github.com/colbymchenry/codegraph](https://github.com/colbymchenry/codegraph)

### deepseek-eyes
让不支持原生识图的模型（如 DeepSeek）也能"看懂"图片。通过阿里云百炼的 Qwen 视觉模型分析图片，返回中文描述。

触发条件：发送图片、提到"分析这张图"、"图片里有什么" 等。

- ⭐⭐⭐⭐ · 用 DeepSeek 等非多模态模型的人
- [github.com/hawkongz/deepseek-eyes](https://github.com/hawkongz/deepseek-eyes)

---

## 📚 学习辅助

### codebase-to-course
将任意代码库转换为精美的交互式单页 HTML 课程。用滚动导航、动画可视化、嵌入式测验和代码对照讲解，教非技术人员理解代码原理。

触发条件：提到"把这个做成课程"、"讲解代码库"、"交互式教程"、"从代码学习" 等。

- ⭐⭐⭐⭐ · 教学和代码库作者

### understand-anything
将任意代码库或知识库转换为交互式知识图谱。可视化文件/函数/类依赖关系，自然语言问答，Diff 影响分析，架构分层展示。5 个 Agent 流水线，结合静态分析（tree-sitter）和 LLM 语义理解。

触发条件：`/understand`、"知识图谱"、"看懂这个项目"、"架构概览"、`/understand-knowledge`（分析 Markdown 知识库）。

- ⭐⭐⭐⭐⭐ · 接手新项目的开发者
- [github.com/Lum1104/Understand-Anything](https://github.com/Lum1104/Understand-Anything)

---

## 📦 快速安装全部

在 Claude Code 对话中说：

```
请帮我安装以下 skill：
Superpowers、docx、pdf、pptx、xlsx、frontend-design、
ui-ux-pro-max、webapp-testing、mcp-builder、
skill-creator、find-skills、codebase-to-course、understand-anything

CodeGraph：https://github.com/colbymchenry/codegraph
deepseek-eyes：https://github.com/hawkongz/deepseek-eyes（模型无识图功能才需要）
mineru-pdf：https://github.com/hawkongz/mineru-pdf（复杂 PDF 高精度解析）
ppt-master：https://github.com/hugohe3/ppt-master（AI 驱动高质量 PPT 生成，支持多种文档输入）
```

---

## 👤 作者

[@hawkongz](https://github.com/hawkongz)

---

> 持续更新中 · 最后更新 2026-06-02
