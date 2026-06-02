# Claude Code 必备 Skill 清单：17 个亲测好用的效率技能包，一键安装全部

## Skill 清单

### 开发流程

**Superpowers** ⭐⭐⭐⭐⭐

一套完整的开发流程套件，14 个 skill 协同工作，覆盖从需求到交付的全周期：

```
头脑风暴 → 计划 → 执行 → TDD → 调试 → 代码审查 → 验证 → 收尾
```

写代码、修 bug、做功能、提 PR 时自动介入。适合所有人。

### 文档处理

**docx** ⭐⭐⭐⭐⭐

Word 文档全功能处理。创建、读取、编辑，支持目录生成、页眉页脚、批注修订、图片替换。写报告和方案的人必备。

**pdf** ⭐⭐⭐⭐⭐

PDF 工具箱：读取内容、合并拆分页面、旋转方向、添加水印、OCR 文字识别、表单填写。经常处理 PDF 资料的人非常实用。

**mineru-pdf** ⭐⭐⭐⭐⭐

高精度 PDF 内容解析，与官方 pdf skill 互补。专门处理复杂 PDF：提取公式（可编译 LaTeX）、图片（含坐标 + 图注）、表格，正确处理双栏排版和扫描件 OCR。学术论文、含公式的 PDF、扫描件都不在话下。

> 项目地址：[github.com/hawkongz/mineru-pdf](https://github.com/hawkongz/mineru-pdf)

**pptx** ⭐⭐⭐⭐

创建和编辑 PowerPoint 演示文稿。支持模板应用、布局调整、演讲者备注、多文件合并拆分。适合经常做汇报和分享的人。

**ppt-master** ⭐⭐⭐⭐⭐

AI 驱动的高质量 PPT 生成。支持 PDF、Word、Markdown、网页等多种格式输入，三角色协作（策略师 → 图片师 → 执行师），SVG→DrawingML 管线生成原生可编辑 PPTX，内置 20+ 专业模板。适合从素材从零生成精美幻灯片的场景。

> 项目地址：[github.com/hugohe3/ppt-master](https://github.com/hugohe3/ppt-master)

**xlsx** ⭐⭐⭐⭐

表格数据处理：创建工作表、编辑单元格、公式计算、生成图表、数据清洗、格式转换。处理数据表格的人会经常用到。

### 前端设计

**frontend-design** ⭐⭐⭐⭐⭐

生成高质量前端界面代码。避免千篇一律的「AI 风格」，产出有创意、有设计感的 UI。提到"设计网页"、"做个页面"、"前端组件"、"美化 UI" 时自动触发。

**ui-ux-pro-max** ⭐⭐⭐⭐⭐

UI/UX 设计智囊。内置 50+ 设计风格、161 套配色方案、57 组字体搭配、99 条 UX 指南，覆盖 React、Next.js、Vue、SwiftUI、Flutter、Tailwind、shadcn/ui 等主流技术栈。提到配色、字体、组件样式时自动介入。

### 测试

**webapp-testing** ⭐⭐⭐⭐

基于 Playwright 的自动化浏览器测试。可以对本地 Web 应用截图、调试 UI、检查浏览器日志。适合 Web 开发者做端到端测试。

### 集成扩展

**mcp-builder** ⭐⭐⭐

构建 MCP（Model Context Protocol）服务器的完整指南。支持 Python（FastMCP）和 Node.js/TypeScript。想把外部 API 接入 Claude 时用它。

**skill-creator** ⭐⭐⭐⭐

创建和优化自定义 Skill。覆盖完整开发周期：起草 → 测试 → 审查 → 改进 → 打包。想做自己的 Skill 或者修改现有 Skill 的时候用。

**find-skills** ⭐⭐⭐⭐⭐

搜索和发现新的 Skill。不确定有没有现成的 Skill 能解决你的问题？用它搜一下，省得自己造轮子。

### 效率工具

**CodeGraph** ⭐⭐⭐⭐⭐

语义级代码地图。给 Claude Code 提供代码全局视野，避免反复搜索文件读取内容。实测工具调用次数减少约 70%，token 成本下降约 35%，100% 本地运行。大型项目中效果尤为明显。

安装后在项目目录运行 `codegraph init -i` 即可启用。

> 项目地址：[github.com/colbymchenry/codegraph](https://github.com/colbymchenry/codegraph)

**deepseek-eyes** ⭐⭐⭐⭐

让不支持原生识图能力的模型（如 DeepSeek）也能「看懂」图片。背后通过阿里云百炼的 Qwen 视觉模型分析图片，返回中文描述。发送图片或提到「分析这张图」「图片里有什么」时自动调用。

> 项目地址：[github.com/hawkongz/deepseek-eyes](https://github.com/hawkongz/deepseek-eyes)

### 学习辅助

**codebase-to-course** ⭐⭐⭐⭐

将任意代码库转换为精美的交互式单页 HTML 课程。带滚动导航、动画可视化、嵌入式测验和代码对照讲解。适合想用代码库做教学材料的人，或者想快速理解一个陌生项目的开发者。

**understand-anything** ⭐⭐⭐⭐⭐

将任意代码库或知识库转换为交互式知识图谱。可视化文件、函数、类的依赖关系，支持自然语言问答、Diff 影响分析、架构分层展示。5 个 Agent 流水线结合静态分析和 LLM 语义理解，接手新项目时快速摸清架构。

> 项目地址：[github.com/Lum1104/Understand-Anything](https://github.com/Lum1104/Understand-Anything)

## 一键安装

在 Claude Code 对话中粘贴以下内容：

```bash
请帮我安装以下 skill：
Superpowers、docx、pdf、pptx、xlsx、frontend-design、
ui-ux-pro-max、webapp-testing、mcp-builder、
skill-creator、find-skills、codebase-to-course、understand-anything

CodeGraph：https://github.com/colbymchenry/codegraph
deepseek-eyes：https://github.com/hawkongz/deepseek-eyes（模型无识图功能才需要）
mineru-pdf：https://github.com/hawkongz/mineru-pdf（复杂 PDF 高精度解析）
ppt-master：https://github.com/hugohe3/ppt-master（AI 驱动 PPT 生成）
```

## 项目地址

🔗 [github.com/hawkongz/awesome-claude-skills](https://github.com/hawkongz/awesome-claude-skills)

中英双语 README，会根据使用体验持续更新。如果对你有帮助，欢迎 Star ⭐
