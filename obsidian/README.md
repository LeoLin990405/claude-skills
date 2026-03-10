<p align="center">
  <img src="https://img.shields.io/badge/Claude%20Code-Skill-blue?style=for-the-badge" alt="Claude Code Skill">
  <img src="https://img.shields.io/badge/Skills-3-green?style=for-the-badge" alt="Skills">
  <img src="https://img.shields.io/badge/Templates-4-orange?style=for-the-badge" alt="Templates">
  <img src="https://img.shields.io/badge/Obsidian-KM--Toolkit-7C3AED?style=for-the-badge" alt="Obsidian">
</p>

<h1 align="center">Knowledge Management Toolkit</h1>

<p align="center">
  <strong>Complete Obsidian Knowledge Management Toolkit for Claude Code</strong>
  <br>
  <em>3 format skills, 4 workflow templates — covering the full knowledge lifecycle</em>
</p>

<p align="center">
  <a href="#-skills">Skills</a> •
  <a href="#-templates">Templates</a> •
  <a href="#-workflow">Workflow</a> •
  <a href="#-quick-start">Quick Start</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Claude%20Code-CLI-8A2BE2?logo=anthropic&logoColor=white" alt="Claude Code">
  <img src="https://img.shields.io/badge/Obsidian-7C3AED?logo=obsidian&logoColor=white" alt="Obsidian">
  <img src="https://img.shields.io/badge/License-MIT-yellow" alt="License">
</p>

**English** | [中文](#中文)

---

## Overview

**Knowledge Management Toolkit** is a complete Obsidian toolkit organized by the knowledge lifecycle. It combines three format reference skills with workflow templates covering capture, organization, connection, and visualization.

### What Changed (v2.0)

| Before (v1) | After (v2) |
|-------------|------------|
| 3 standalone format references | **3 skills + workflow routing layer** |
| No templates | **4 ready-to-use templates** |
| Format-organized | **Lifecycle-organized** (capture → organize → connect → visualize) |
| Manual skill selection | **Auto-routing** by user intent |

---

## Skills

| # | Skill | What It Covers |
|---|-------|---------------|
| 1 | [obsidian-markdown](skills/obsidian-markdown/SKILL.md) | Wikilinks, embeds, callouts, properties, Obsidian Flavored Markdown |
| 2 | [obsidian-bases](skills/obsidian-bases/SKILL.md) | Database views, filters, sorts, formulas, aggregations |
| 3 | [json-canvas](skills/json-canvas/SKILL.md) | JSON Canvas spec, nodes, edges, groups, spatial layout |

---

## Templates

Ready-to-use templates for common knowledge management tasks:

| Template | Format | Use Case |
|----------|--------|----------|
| [daily-note](templates/daily-note.md) | Markdown | Daily journal with tasks, notes, and reflections |
| [project-tracker](templates/project-tracker.base) | Bases | Track projects by status, priority, due date, tags |
| [research-canvas](templates/research-canvas.canvas) | Canvas | Map research from topic to findings |
| [meeting-note](templates/meeting-note.md) | Markdown | Meeting notes with attendees, decisions, action items |

---

## Workflow

The knowledge lifecycle in Obsidian:

```
Capture → Organize → Connect → Visualize
```

| Phase | Activity | Skills & Templates |
|---|---|---|
| **Capture** | Daily notes, meeting notes, fleeting ideas | obsidian-markdown + daily-note, meeting-note |
| **Organize** | Properties, tags, database views, status tracking | obsidian-bases + project-tracker |
| **Connect** | Wikilinks, backlinks, block references, transclusion | obsidian-markdown |
| **Visualize** | Canvas maps, spatial layouts, node grouping | json-canvas + research-canvas |

---

## Quick Start

### Installation

```bash
cd ~/.claude/skills
git clone https://github.com/LeoLin990405/claude-skills.git
```

### Usage

```bash
# The toolkit auto-routes based on your request:
"Create a daily note for today"        → obsidian-markdown + daily-note
"Set up a project tracker"             → obsidian-bases + project-tracker
"Map out my research on X"             → json-canvas + research-canvas
"Take notes for this meeting"          → obsidian-markdown + meeting-note

# Or access skills directly:
"Use obsidian-markdown"                → obsidian-markdown
"Show me how Bases work"               → obsidian-bases
"Help me edit a canvas file"           → json-canvas
```

---

## 中文

### 概述

**知识管理工具集** 是一个完整的 Obsidian 知识管理工具集，按知识生命周期组织。将三个格式参考技能与工作流模板相结合，覆盖捕获、组织、连接和可视化全流程。

### 技能

| 技能 | 覆盖范围 |
|------|---------|
| obsidian-markdown | Wikilinks、嵌入、Callouts、属性、Obsidian 风格 Markdown |
| obsidian-bases | 数据库视图、筛选、排序、公式、聚合 |
| json-canvas | JSON Canvas 规范、节点、连线、分组、空间布局 |

### 模板

| 模板 | 格式 | 用途 |
|------|------|------|
| daily-note | Markdown | 每日笔记：任务、记录、反思 |
| project-tracker | Bases | 项目跟踪：状态、优先级、截止日期 |
| research-canvas | Canvas | 研究地图：主题 → 问题 → 来源 → 发现 |
| meeting-note | Markdown | 会议记录：参会者、讨论、决策、行动 |

### 工作流

```
捕获 → 组织 → 连接 → 可视化
```

### 安装

```bash
cd ~/.claude/skills
git clone https://github.com/LeoLin990405/claude-skills.git
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
