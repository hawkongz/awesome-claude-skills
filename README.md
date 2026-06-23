<div align="center">
  <h1>Awesome Claude Code Skills</h1>
  <p>My curated list of great skills for coding, writing, and learning with Claude Code.<br>Just tell Claude Code these names and it will install them automatically.</p>

  [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
  [![Platform](https://img.shields.io/badge/Platform-Claude%20Code-blue)](https://code.claude.com)
  [![Stars](https://img.shields.io/github/stars/hawkongz/awesome-claude-skills)](https://github.com/hawkongz/awesome-claude-skills)

  <p><strong>Language:</strong> <a href="README.md">English</a> | <a href="zh-CN/README.md">简体中文</a></p>
</div>

---

## 📋 Table of Contents

- [Development Workflow](#-development-workflow)
- [Document Processing](#-document-processing)
- [Frontend Design](#-frontend-design)
- [Testing](#-testing)
- [Integration & Extensions](#-integration--extensions)
- [Productivity Tools](#-productivity-tools)
- [Learning Aid](#-learning-aid)
- [Install All at Once](#-install-all-at-once)

---

## 🔧 Development Workflow

### Superpowers
A complete development workflow suite covering the full cycle: brainstorm → plan → execute → TDD → debug → code review → verify → ship. 14 skills working together.

Triggers: writing code, fixing bugs, building features, opening PRs.

- ⭐⭐⭐⭐⭐ · Everyone

---

## 📄 Document Processing

### docx
Create, read, and edit Word documents. Supports table of contents, headers, footers, tracked changes, image replacement, and more.
- ⭐⭐⭐⭐⭐ · Report and proposal writers

### pdf
Full PDF toolkit: read, merge, split, rotate, watermark, OCR, form filling.
- ⭐⭐⭐⭐⭐ · Anyone working with PDFs

### mineru-pdf
High-accuracy PDF content extraction for complex documents. Extracts formulas (compilable LaTeX), images (with bbox + captions), tables, and handles multi-column layouts and scanned PDFs. Complements the official pdf skill.

Triggers: `/mineru-pdf`, "MinerU", "parse this paper", "extract formulas from PDF".

- ⭐⭐⭐⭐⭐ · Academic researchers, anyone dealing with formula-heavy or scanned PDFs
- [github.com/hawkongz/mineru-pdf](https://github.com/hawkongz/mineru-pdf)

### pptx
Create and edit PowerPoint presentations — read content, modify styles, replace images, merge/split, template-based creation. A general-purpose PPTX toolbox best suited for editing existing files.
- ⭐⭐⭐⭐ · Presenters and knowledge sharers

### ppt-master
AI-driven PPT generation from any source document (PDF/DOCX/Markdown/URL). Uses multi-role collaboration (Strategist → Image Generator → Executor) and SVG→DrawingML pipeline to produce natively editable PPTX with 20+ professional templates. Best for creating polished decks from raw materials.

Triggers: "create PPT", "make presentation", "generate slides", "生成PPT", "做PPT".

- ⭐⭐⭐⭐⭐ · PPT creators who want professional design quality
- [github.com/hugohe3/ppt-master](https://github.com/hugohe3/ppt-master)

> **pptx vs ppt-master**: `pptx` is a general-purpose PPTX toolbox — read, edit, merge, template tweaks. `ppt-master` specializes in **generating professional decks from scratch** from source documents, with higher design quality and style consistency. Use `pptx` when editing existing files; use `ppt-master` when creating a polished presentation from raw materials.
>
> **⚠️ Trigger conflict**: Both skills respond to "create PPT", "make presentation", etc. To avoid choosing every time, set the less-frequently-used one to manual-only in settings.json:
> ```json
> "skillOverrides": {
>   "pptx": "user-invocable-only"
> }
> ```
> This way "make a PPT" → auto-routes to `ppt-master`; when you need to edit an existing file, explicitly invoke via `/pptx`.

### xlsx
Spreadsheet processing: create, edit, formulas, charts, data cleaning, format conversion.
- ⭐⭐⭐⭐ · Data and spreadsheet users

---

## 🎨 Frontend Design

### frontend-design
Production-grade frontend interfaces with high design quality. Avoids generic "AI aesthetic" code.

Triggers: "design a webpage", "build a page", "frontend component", "beautify UI".

- ⭐⭐⭐⭐⭐ · Frontend developers

### ui-ux-pro-max
UI/UX design intelligence. 50+ styles, 161 color palettes, 57 font pairings, 99 UX guidelines across React/Next.js/Vue/SwiftUI/Flutter/Tailwind and more.

Triggers: "UI design", "UX improvement", "color palette", "font pairing", "component styling".

- ⭐⭐⭐⭐⭐ · UI builders

---

## 🧪 Testing

### webapp-testing
Automated browser testing with Playwright. Screenshots, UI debugging, browser log inspection.

Triggers: "test the page", "screenshot", "browser debug", "e2e test".

- ⭐⭐⭐⭐ · Web developers

---

## 🔌 Integration & Extensions

### mcp-builder
Complete guide for building MCP servers. Supports Python (FastMCP) and Node/TypeScript.

Triggers: "build an MCP", "connect API", "add tools to Claude".

- ⭐⭐⭐ · API integration builders

### skill-creator
Create, modify, and optimize Claude Code skills. Supports the full development cycle: draft → test → review → improve → package.

Triggers: "create a skill", "make a new skill", "write a skill", "improve this skill".

- ⭐⭐⭐⭐ · Skill developers

### find-skills
Search and discover new skills. Use when you want a capability but unsure if a skill exists.

Triggers: "is there a skill for X", "how to install X", "find a skill".

- ⭐⭐⭐⭐⭐ · Everyone

### runapi-cli
Run AI image, video, music/audio, speech, and LLM model API jobs through the RunAPI CLI from Claude Code, Codex, and similar agents.

Triggers: "generate an image with RunAPI", "create AI video", "make music", "run a model API job".

- ⭐⭐⭐⭐ · Builders using model APIs in agent workflows
- [github.com/runapi-ai/cli-skill](https://github.com/runapi-ai/cli-skill)

---

## ⚡ Productivity Tools

### CodeGraph
Semantic code maps for Claude Code. Provides global code awareness, reducing tool calls by ~70% and costs by ~35%. Runs 100% locally.

After install, run `codegraph init -i` in your project directory.

- ⭐⭐⭐⭐⭐ · Large project developers
- [github.com/colbymchenry/codegraph](https://github.com/colbymchenry/codegraph)

### deepseek-eyes
Enables non-vision models (like DeepSeek) to understand images. Routes images through Alibaba Cloud's Qwen vision models, returning Chinese descriptions.

Triggers: sharing images, "analyze this picture", "what's in this image".

- ⭐⭐⭐⭐ · DeepSeek and non-multimodal model users
- [github.com/hawkongz/deepseek-eyes](https://github.com/hawkongz/deepseek-eyes)

---

## 📚 Learning Aid

### codebase-to-course
Turn any codebase into a beautiful, interactive single-page HTML course. Teaches how the code works with scroll-based navigation, animated visualizations, embedded quizzes, and code-with-plain-English translations.

Triggers: "turn this into a course", "explain this codebase", "teach this code", "interactive tutorial from code".

- ⭐⭐⭐⭐ · Educators and codebase authors

### understand-anything
Turn any codebase or knowledge base into an interactive knowledge graph. Visual file/function/class dependency explorer, natural language Q&A, diff impact analysis, and architecture layer visualization. 5-agent pipeline combining static analysis (tree-sitter) with LLM semantic understanding.

Triggers: `/understand`, "knowledge graph", "understand this codebase", "architecture overview", `/understand-knowledge` for markdown wikis.

- ⭐⭐⭐⭐⭐ · Developers onboarding to new projects
- [github.com/Lum1104/Understand-Anything](https://github.com/Lum1104/Understand-Anything)

---

## 📦 Install All at Once

Paste this in Claude Code:

```
Please install these skills:
Superpowers, docx, pdf, pptx, xlsx, frontend-design,
ui-ux-pro-max, webapp-testing, mcp-builder,
skill-creator, find-skills, codebase-to-course, understand-anything

CodeGraph: https://github.com/colbymchenry/codegraph
deepseek-eyes: https://github.com/hawkongz/deepseek-eyes (only needed if your model lacks vision)
mineru-pdf: https://github.com/hawkongz/mineru-pdf (high-accuracy PDF extraction for complex documents)
ppt-master: https://github.com/hugohe3/ppt-master (AI-driven PPT generation from any source document)
```

---

## 👤 Author

[@hawkongz](https://github.com/hawkongz)

---

> Updated 2026-06-02
