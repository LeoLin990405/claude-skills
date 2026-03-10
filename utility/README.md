<p align="center">
  <img src="https://img.shields.io/badge/Claude%20Code-Skill-blue?style=for-the-badge" alt="Claude Code Skill">
  <img src="https://img.shields.io/badge/Skills-6-green?style=for-the-badge" alt="Skills">
  <img src="https://img.shields.io/badge/Developer-Toolkit-607D8B?style=for-the-badge" alt="Developer Toolkit">
</p>

<h1 align="center">Developer Toolkit</h1>

<p align="center">
  <strong>Complete Developer Toolkit for Claude Code</strong>
  <br>
  <em>6 specialized skills, 3 templates — covering skill creation, MCP building, docs, testing, and more</em>
</p>

<p align="center">
  <a href="#skills">Skills</a> •
  <a href="#templates">Templates</a> •
  <a href="#quick-start">Quick Start</a>
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

**Developer Toolkit** is a complete developer toolkit organized by domain. It provides 6 specialized skills with actionable workflows, frameworks, and executable templates for common developer tasks.

### What Changed (v2.0)

| Before (v1) | After (v2) |
|-------------|------------|
| Flat skill list | **Grouped by domain** (Development Tools, Knowledge Base, Communications, Testing, Research) |
| No routing | **Intent-based routing** to the right skill |
| No templates | **3 executable templates** (MCP server spec, skill spec, test plan) |
| Skills only | **Workflow layer** on top of existing skills |

---

## Skills

| # | Group | Skill | What It Covers |
|---|-------|-------|---------------|
| 1 | Development Tools | [skill-creator](skills/skill-creator/SKILL.md) | Skill creation guide, SKILL.md format, best practices |
| 2 | Development Tools | [mcp-builder](skills/mcp-builder/SKILL.md) | MCP server creation, FastMCP/TypeScript SDK, tools, resources |
| 3 | Knowledge Base | [anthropic-docs](skills/anthropic-docs/SKILL.md) | Anthropic documentation, Claude API, model selection, Claude Code |
| 4 | Communications | [internal-comms](skills/internal-comms/SKILL.md) | Status reports, leadership updates, newsletters, incident reports |
| 5 | Testing | [webapp-testing](skills/webapp-testing/SKILL.md) | Playwright web app testing, screenshots, browser logs, UI debugging |
| 6 | Research | [history-note-processor](skills/history-note-processor/SKILL.md) | Four-step deep reading, YAML frontmatter, Mermaid diagrams |

---

## Templates

Ready-to-use templates for common developer tasks:

| Template | Use Case |
|----------|----------|
| [mcp-server-spec](templates/mcp-server-spec.md) | Specify an MCP server: tools, resources, prompts, auth, deployment |
| [skill-spec](templates/skill-spec.md) | Specify a new skill: name, triggers, workflow, resources, testing |
| [test-plan](templates/test-plan.md) | Plan web app testing: scenarios, expected results, environment setup |

---

## Quick Start

### Installation

```bash
cd ~/.claude/skills
git clone https://github.com/LeoLin990405/claude-utility-skills.git
```

### Usage

```bash
# The toolkit auto-routes based on your request:
"Create a new skill"              -> skill-creator + skill-spec template
"Build an MCP server"             -> mcp-builder + mcp-server-spec template
"Test my web app"                 -> webapp-testing + test-plan template
"Write a status report"           -> internal-comms
"Look up Anthropic API docs"      -> anthropic-docs

# Or access skills directly:
"Use the mcp-builder skill"       -> mcp-builder
"Show me the test plan template"  -> templates/test-plan
```

---

## 中文

### 概述

**Developer Toolkit** 是一个完整的开发者工具集，按领域组织。提供 6 个专业技能和 3 个可执行模板，覆盖技能创建、MCP 服务器构建、文档查询、测试等常见开发任务。

### 技能

| 分组 | 技能 | 覆盖范围 |
|------|------|---------|
| 开发工具 | skill-creator | 技能创建指南、SKILL.md 格式、最佳实践 |
| 开发工具 | mcp-builder | MCP 服务器创建、FastMCP/TypeScript SDK |
| 知识库 | anthropic-docs | Anthropic 文档、Claude API、模型选择 |
| 通讯 | internal-comms | 状态报告、领导更新、通讯、事件报告 |
| 测试 | webapp-testing | Playwright Web 应用测试、截图、浏览器日志 |
| 研究 | history-note-processor | 四步深度阅读法、YAML、Mermaid 图表 |

### 模板

| 模板 | 用途 |
|------|------|
| mcp-server-spec | MCP 服务器规格：工具、资源、认证、部署 |
| skill-spec | 技能规格：名称、触发器、工作流、测试 |
| test-plan | 测试计划：场景、预期结果、环境配置 |

### 安装

```bash
cd ~/.claude/skills
git clone https://github.com/LeoLin990405/claude-utility-skills.git
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
