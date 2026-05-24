# Claude Code 好用的 Skill 推荐清单：从开发到部署全流程提效

## 目录

- [前言](#前言)
- [Superpowers：开发流程全家桶](#superpowers开发流程全家桶)
- [文档处理四件套](#文档处理四件套)
- [前端设计双雄](#前端设计双雄)
- [CodeGraph：代码语义地图](#codegraph代码语义地图)
- [deepseek-eyes：让 DeepSeek 看懂图片](#deepseek-eyes让-deepseek-看懂图片)
- [安装方式](#安装方式)
- [小结](#小结)

## 前言

用了几个月 Claude Code，陆陆续续装了不少 Skill。有些是官方自带的，有些是社区推荐的，有些是自己写的。踩过坑也挖到过宝。整理一份清单出来，希望能帮你省下筛选的时间。

每个 Skill 只需要把名字告诉 Claude Code，它就能自动搜索和安装，不用手动输入任何命令。

## Superpowers：开发流程全家桶

`obra/superpowers` 是目前最完整的开发流程 Skill 套件，14 个 Skill 覆盖从需求到交付的全过程：

头脑风暴 → 编写计划 → 执行计划 → 子代理并行推进 → TDD 红绿重构 → 系统化调试 → 代码审查 → 完成验证 → 分支收尾。

装上之后最大的变化是编码节奏变稳了。以前经常"写到一半发现方向不对"，现在 `brainstorming` 在动手前强制理清需求，`systematic-debugging` 让你遇到 bug 先走流程而不是凭直觉乱改。

## 文档处理四件套

`docx`、`pdf`、`pptx`、`xlsx` 这四个来自 `anthropics/skills`，覆盖了日常文档处理的全部场景：

- **docx**：创建和编辑 Word 文档，支持目录、批注、替换图片、格式排版
- **pdf**：读取、合并、拆分、旋转、水印、OCR 识别、表单填写
- **pptx**：创建和编辑 PPT，支持模板、演讲者备注、合并拆分
- **xlsx**：表格处理，公式计算、图表、数据清洗、格式转换

以前写周报要切出去开 Word，做数据统计要打开 Excel，现在全部在对话里完成。

## 前端设计双雄

**frontend-design** 是 Claude Code 官方自带的，生成的前端代码没有那种"一眼 AI"的廉价感。

**ui-ux-pro-max** 则是社区爆款（180K+ 安装量），内置 50+ 设计风格、161 调色板、57 字体搭配、99 UX 指南，覆盖 React、Next.js、Vue、SwiftUI、Flutter、Tailwind、shadcn/ui 等十个技术栈。提到"配色"、"字体搭配"、"组件样式"就会自动触发。

## CodeGraph：代码语义地图

CodeGraph 不是 Skill，而是一个独立的 MCP 工具。它给 Claude Code 提供项目的语义级代码地图——哪些文件调用了哪些函数、模块之间的依赖关系——让 AI 不用反复搜索文件就能精准定位代码。

实际效果：工具调用减少约 70%，成本降低约 35%，100% 本地运行。大型项目中感知很明显——以前 Claude 要 grep 好几次才能找到目标，现在一步到位。

安装后在项目目录运行 `codegraph init -i` 即可。

项目地址：[github.com/colbymchenry/codegraph](https://github.com/colbymchenry/codegraph)

## deepseek-eyes：让 DeepSeek 看懂图片

这是我自己的项目。DeepSeek 虽然强，但不支持原生识图——发张截图给它是看不到的。deepseek-eyes 解决了这个问题：

图片 → eyes.py → 阿里云百炼 Qwen 视觉模型 → 中文描述 → 喂回主模型

阿里云百炼新用户有 100 万 token 免费额度（90 天有效），零成本上手。

项目地址：[github.com/20kiki/deepseek-eyes](https://github.com/20kiki/deepseek-eyes)

## 安装方式

在 Claude Code 对话中直接说：

```
请帮我安装以下 skill：
Superpowers、docx、pdf、pptx、xlsx、
ui-ux-pro-max、webapp-testing、mcp-builder、
find-skills
（frontend-design 和 skill-creator 官方自带，无需装）

CodeGraph：github.com/colbymchenry/codegraph
deepseek-eyes：github.com/20kiki/deepseek-eyes
```

## 小结

这套清单是我日常编程、写文档、做前端实际验证过的。不是搬运文档，每个都用了至少几周到几个月。如果你有自己觉得好用的 Skill，也欢迎提 PR 补充。

完整清单：[github.com/20kiki/awesome-claude-skills](https://github.com/20kiki/awesome-claude-skills)
