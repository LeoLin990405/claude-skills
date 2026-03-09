<p align="center">
  <img src="https://img.shields.io/badge/Claude%20Code-Skill-blue?style=for-the-badge" alt="Claude Code Skill">
  <img src="https://img.shields.io/badge/Skills-6-green?style=for-the-badge" alt="Skills">
  <img src="https://img.shields.io/badge/Utility-Tools-607D8B?style=for-the-badge" alt="Utility">
</p>

<h1 align="center">Claude Utility Skills</h1>

<p align="center">
  <strong>Utility and Specialized Domain Skills for Claude Code</strong>
  <br>
  <em>Skill creation, MCP building, documentation, testing, and more</em>
</p>

<p align="center">
  <a href="#-features">Features</a> •
  <a href="#-quick-start">Quick Start</a> •
  <a href="#-skills">Skills</a> •
  <a href="#-usage">Usage</a> •
  <a href="#-guides">Guides</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Claude%20Code-CLI-8A2BE2?logo=anthropic&logoColor=white" alt="Claude Code">
  <img src="https://img.shields.io/badge/MCP-Protocol-00BCD4?logo=protocol&logoColor=white" alt="MCP">
  <img src="https://img.shields.io/badge/Playwright-2EAD33?logo=playwright&logoColor=white" alt="Playwright">
  <img src="https://img.shields.io/badge/License-MIT-yellow" alt="License">
</p>

**English** | [中文](#中文)

---

## Overview

**Claude Utility Skills** provides utility tools and specialized domain knowledge for various tasks, from creating new skills to building MCP servers.

### Why Utility Skills?

| Challenge | Solution |
|-----------|----------|
| Creating new skills | **Skill Creator** with templates and best practices |
| Building MCP servers | **MCP Builder** with setup guides |
| Finding Anthropic docs | **Anthropic Docs** knowledge base |
| Testing web apps | **Webapp Testing** with Playwright |

---

## Features

| Feature | Description |
|---------|-------------|
| **Skill Creator** | Templates, best practices, SKILL.md format |
| **MCP Builder** | Server setup, tool definitions, resources |
| **Anthropic Docs** | API reference, SDK usage, best practices |
| **History Notes** | Four-step methodology, YAML, Mermaid |
| **Internal Comms** | Communication templates |
| **Webapp Testing** | Playwright-based testing |

---

## Quick Start

### Installation

```bash
cd ~/.claude/skills
git clone https://github.com/LeoLin990405/claude-utility-skills.git
```

### Verify Installation

```bash
ls ~/.claude/skills/claude-utility-skills/SKILL.md
```

---

## Skills

| Skill | Command | Description |
|-------|---------|-------------|
| `skill-creator` | `/skill-creator` | Guide for creating skills |
| `mcp-builder` | `/mcp-builder` | MCP server creation guide |
| `anthropic-docs` | `/anthropic-docs` | Anthropic documentation |
| `history-note-processor` | `/history-note-processor` | History note processing |
| `internal-comms` | `/internal-comms` | Internal communications |
| `webapp-testing` | `/webapp-testing` | Web application testing |

---

## Guides

### Skill Creator

```yaml
# SKILL.md format
---
name: my-skill
description: Brief description
triggers:
  - keyword1
  - keyword2
---
# Instructions here...
```

### MCP Builder

```python
# FastMCP server example
from fastmcp import FastMCP

mcp = FastMCP("my-server")

@mcp.tool()
def my_tool(param: str) -> str:
    return f"Result: {param}"
```

### Webapp Testing

```python
# Playwright testing
from playwright.sync_api import sync_playwright

with sync_playwright() as p:
    browser = p.chromium.launch()
    page = browser.new_page()
    page.goto("http://localhost:3000")
```

---

## Usage

```bash
# Create new skills
/skill-creator

# Build MCP servers
/mcp-builder

# Access Anthropic docs
/anthropic-docs

# Test web applications
/webapp-testing
```

---

## 中文

### 概述

**Claude Utility Skills** 提供实用工具和各种任务的专业领域知识，从创建新技能到构建 MCP 服务器。

### 包含的技能

| 技能 | 命令 | 描述 |
|------|------|------|
| `skill-creator` | `/skill-creator` | 技能创建指南 |
| `mcp-builder` | `/mcp-builder` | MCP 服务器创建指南 |
| `anthropic-docs` | `/anthropic-docs` | Anthropic 文档知识库 |
| `history-note-processor` | `/history-note-processor` | 历史笔记处理 |
| `internal-comms` | `/internal-comms` | 内部通讯模板 |
| `webapp-testing` | `/webapp-testing` | Web 应用测试 |

### 功能特性

| 功能 | 描述 |
|------|------|
| **技能创建器** | 模板、最佳实践、SKILL.md 格式 |
| **MCP 构建器** | 服务器设置、工具定义、资源处理 |
| **Anthropic 文档** | API 参考、SDK 用法、最佳实践 |
| **历史笔记** | 四步方法论、YAML frontmatter、Mermaid 图表 |

### 安装

```bash
cd ~/.claude/skills
git clone https://github.com/LeoLin990405/claude-utility-skills.git
```

### 使用方法

```bash
# 创建新技能
/skill-creator

# 构建 MCP 服务器
/mcp-builder

# 访问 Anthropic 文档
/anthropic-docs

# 测试 Web 应用
/webapp-testing
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
