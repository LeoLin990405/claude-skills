<p align="center">
  <img src="https://img.shields.io/badge/Claude%20Code-Skill-blue?style=for-the-badge" alt="Claude Code Skill">
  <img src="https://img.shields.io/badge/Skills-3-green?style=for-the-badge" alt="Skills">
  <img src="https://img.shields.io/badge/Obsidian-Note--Taking-7C3AED?style=for-the-badge" alt="Obsidian">
</p>

<h1 align="center">Claude Obsidian Skills</h1>

<p align="center">
  <strong>Obsidian Note-Taking Toolkit for Claude Code</strong>
  <br>
  <em>Obsidian Flavored Markdown, Bases database views, and JSON Canvas editing</em>
</p>

<p align="center">
  <a href="#-features">Features</a> •
  <a href="#-quick-start">Quick Start</a> •
  <a href="#-skills">Skills</a> •
  <a href="#-usage">Usage</a> •
  <a href="#-syntax">Syntax</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Claude%20Code-CLI-8A2BE2?logo=anthropic&logoColor=white" alt="Claude Code">
  <img src="https://img.shields.io/badge/Obsidian-7C3AED?logo=obsidian&logoColor=white" alt="Obsidian">
  <img src="https://img.shields.io/badge/License-MIT-yellow" alt="License">
</p>

**English** | [中文](#中文)

---

## Overview

**Claude Obsidian Skills** enables Claude Code to work with Obsidian-specific formats, including wikilinks, callouts, properties, and the new Bases feature.

### Why Obsidian Skills?

| Challenge | Solution |
|-----------|----------|
| Standard Markdown limitations | **Obsidian Flavored Markdown** with wikilinks, embeds |
| No database views | **Bases** for database-like note organization |
| Text-only notes | **JSON Canvas** for visual note connections |
| Manual formatting | **Auto-formatting** with Obsidian syntax |

---

## Features

| Feature | Description |
|---------|-------------|
| **Wikilinks** | `[[note]]` and `[[note\|alias]]` syntax |
| **Embeds** | `![[image]]` and `![[note]]` transclusion |
| **Callouts** | `> [!note]`, `> [!warning]`, etc. |
| **Properties** | YAML frontmatter with tags, aliases |
| **Bases** | Database views with filters, sorts, formulas |
| **Canvas** | Visual node connections and grouping |

---

## Quick Start

### Installation

```bash
cd ~/.claude/skills
git clone https://github.com/LeoLin990405/claude-obsidian-skills.git
```

### Verify Installation

```bash
ls ~/.claude/skills/claude-obsidian-skills/SKILL.md
```

---

## Skills

| Skill | Command | Description |
|-------|---------|-------------|
| `obsidian-markdown` | `/obsidian-markdown` | Obsidian Flavored Markdown |
| `obsidian-bases` | `/obsidian-bases` | Database views with filters |
| `json-canvas` | `/json-canvas` | Visual canvas editing |

---

## Syntax

### Wikilinks

```markdown
[[Note Name]]           # Basic link
[[Note Name|Display]]   # Aliased link
[[Note Name#Heading]]   # Heading link
[[Note Name#^block-id]] # Block link
```

### Embeds

```markdown
![[image.png]]          # Image embed
![[note]]               # Note transclusion
![[note#heading]]       # Section embed
```

### Callouts

```markdown
> [!note] Title
> Content here

> [!warning] Warning
> Important message

> [!tip]+ Collapsible
> Hidden by default
```

### Properties (Frontmatter)

```yaml
---
title: My Note
tags: [tag1, tag2]
aliases: [alias1]
created: 2024-01-01
---
```

---

## Usage

```bash
# Create Obsidian-style notes
/obsidian-markdown

# Work with Bases database views
/obsidian-bases

# Edit canvas files
/json-canvas
```

---

## 中文

### 概述

**Claude Obsidian Skills** 使 Claude Code 能够处理 Obsidian 特有格式，包括 wikilinks、callouts、properties 和新的 Bases 功能。

### 包含的技能

| 技能 | 命令 | 描述 |
|------|------|------|
| `obsidian-markdown` | `/obsidian-markdown` | Obsidian 风格 Markdown |
| `obsidian-bases` | `/obsidian-bases` | 数据库视图 |
| `json-canvas` | `/json-canvas` | 可视化画布编辑 |

### 语法示例

#### Wikilinks

```markdown
[[笔记名称]]            # 基本链接
[[笔记名称|显示文本]]   # 别名链接
[[笔记名称#标题]]       # 标题链接
```

#### 嵌入

```markdown
![[图片.png]]           # 图片嵌入
![[笔记]]               # 笔记嵌入
```

#### Callouts

```markdown
> [!note] 标题
> 内容

> [!warning] 警告
> 重要信息
```

### 安装

```bash
cd ~/.claude/skills
git clone https://github.com/LeoLin990405/claude-obsidian-skills.git
```

### 使用方法

```bash
# 创建 Obsidian 风格笔记
/obsidian-markdown

# 使用 Bases 数据库视图
/obsidian-bases

# 编辑 canvas 文件
/json-canvas
```

---

## Contributors

- **Leo** ([@LeoLin990405](https://github.com/LeoLin990405)) - Project Lead
- **Claude** (Anthropic Claude Opus 4.5) - Content Generation

## License

MIT License - see [LICENSE](LICENSE) for details.

---

<p align="center">
  <sub>Built with collaboration between human and AI</sub>
</p>
