<p align="center">
  <img src="https://img.shields.io/badge/Claude%20Code-Skill-blue?style=for-the-badge" alt="Claude Code Skill">
  <img src="https://img.shields.io/badge/Skills-7-green?style=for-the-badge" alt="Skills">
  <img src="https://img.shields.io/badge/Design-Toolkit-E91E63?style=for-the-badge" alt="Design Toolkit">
</p>

<h1 align="center">Design Toolkit</h1>

<p align="center">
  <strong>Complete Design Toolkit for Claude Code</strong>
  <br>
  <em>4 workflow modules, 7 specialized skills, 3 templates — covering the full design lifecycle</em>
</p>

<p align="center">
  <a href="#modules">Modules</a> •
  <a href="#templates">Templates</a> •
  <a href="#workflow">Workflow</a> •
  <a href="#quick-start">Quick Start</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Claude%20Code-CLI-8A2BE2?logo=anthropic&logoColor=white" alt="Claude Code">
  <img src="https://img.shields.io/badge/p5.js-ED225D?logo=p5.js&logoColor=white" alt="p5.js">
  <img src="https://img.shields.io/badge/React-61DAFB?logo=react&logoColor=black" alt="React">
  <img src="https://img.shields.io/badge/License-MIT-yellow" alt="License">
</p>

**English** | [中文](#中文)

---

## Overview

**Design Toolkit** is a complete design toolkit organized by workflow phase. It groups 7 specialized design skills into 4 actionable workflow modules with templates, checklists, and a design-system foundation.

### What Changed (v2.0)

| Before (v1) | After (v2) |
|-------------|------------|
| 7 scattered skills | **4 workflow modules** |
| Flat directory listing | **Intent-based routing** |
| No templates | **3 reusable templates** |
| No design-system guidance | **Design-system module** for cross-skill consistency |

---

## Modules

| # | Module | Skills | What It Covers |
|---|--------|--------|---------------|
| 1 | [design-generative](skills/design-generative/SKILL.md) | 2 | Algorithmic art (p5.js), animated GIFs, motion design |
| 2 | [design-visual](skills/design-visual/SKILL.md) | 2 | Canvas compositions, posters, brand assets, visual identity |
| 3 | [design-frontend](skills/design-frontend/SKILL.md) | 3 | Frontend UI, React web artifacts, theming with 10 presets |
| 4 | [design-system](skills/design-system/SKILL.md) | — | Design tokens, component docs, accessibility, consistency |

---

## Templates

Ready-to-use templates for common design tasks:

| Template | Use Case |
|----------|----------|
| [design-brief](templates/design-brief.md) | Define project objectives, audience, constraints, and references |
| [style-guide](templates/style-guide.md) | Document colors, typography, spacing, and component patterns |
| [design-review-checklist](templates/design-review-checklist.md) | Review visual hierarchy, consistency, accessibility, performance |

---

## Workflow

Design projects flow through four phases:

```
Concept → Design → Implement → Polish
```

| Phase | What Happens | Modules |
|-------|-------------|---------|
| **Concept** | Define brief, set constraints, choose tools | design-system |
| **Design** | Create visuals, apply brand, compose layout | design-visual, design-generative |
| **Implement** | Build components, apply themes, generate assets | design-frontend, design-generative |
| **Polish** | Review, ensure consistency, check accessibility | design-system |

---

## Quick Start

### Installation

```bash
cd ~/.claude/skills
git clone https://github.com/LeoLin990405/claude-design-skills.git
```

### Usage

```bash
# The toolkit auto-routes based on your request:
"Create generative art"           → design-generative → algorithmic-art
"Design a poster"                 → design-visual → canvas-design
"Build a themed UI"               → design-frontend → theme-factory
"Create a React artifact"         → design-frontend → web-artifacts-builder
"Make a Slack GIF"                → design-generative → slack-gif-creator

# Or access modules directly:
"Use the frontend design module"  → design-frontend
"Set up a design system"          → design-system
```

---

## 中文

### 概述

**Design Toolkit** 是一个完整的设计工具集，按工作流阶段组织。将 7 个专业设计技能整合为 4 个可执行的工作流模块，包含模板、检查清单和设计系统基础。

### 模块

| 模块 | 技能数 | 覆盖范围 |
|------|--------|---------|
| design-generative | 2 | 算法艺术（p5.js）、动画 GIF、动效设计 |
| design-visual | 2 | Canvas 构图、海报、品牌资产、视觉识别 |
| design-frontend | 3 | 前端 UI、React Web Artifacts、主题化 |
| design-system | — | 设计令牌、组件文档、无障碍、一致性 |

### 模板

| 模板 | 用途 |
|------|------|
| [design-brief](templates/design-brief.md) | 定义项目目标、受众、约束和参考 |
| [style-guide](templates/style-guide.md) | 记录颜色、字体、间距和组件规范 |
| [design-review-checklist](templates/design-review-checklist.md) | 审查视觉层次、一致性、无障碍、性能 |

### 安装

```bash
cd ~/.claude/skills
git clone https://github.com/LeoLin990405/claude-design-skills.git
```

### 使用方法

```bash
# 创建生成艺术
"Create generative art"           → design-generative → algorithmic-art

# 设计海报
"Design a poster"                 → design-visual → canvas-design

# 构建主题化 UI
"Build a themed UI"               → design-frontend → theme-factory

# 创建 React artifact
"Create a React artifact"         → design-frontend → web-artifacts-builder
```

---

## Contributors

- **Leo** ([@LeoLin990405](https://github.com/LeoLin990405)) - Project Lead
- **Claude** (Anthropic Claude) - Content Generation

## License

MIT License - see [LICENSE](LICENSE) for details.

---

<p align="center">
  <sub>Built with collaboration between human and AI</sub>
</p>
