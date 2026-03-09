<p align="center">
  <img src="https://img.shields.io/badge/Claude%20Code-Skill-blue?style=for-the-badge" alt="Claude Code Skill">
  <img src="https://img.shields.io/badge/Skills-14-green?style=for-the-badge" alt="Skills">
  <img src="https://img.shields.io/badge/Multi--AI-Collaboration-orange?style=for-the-badge" alt="Multi-AI">
</p>

<h1 align="center">Claude CCB Skills</h1>

<p align="center">
  <strong>Multi-AI Collaboration Toolkit for Claude Code</strong>
  <br>
  <em>Async delegation, provider management, and distributed AI workflows</em>
</p>

<p align="center">
  <a href="#-features">Features</a> •
  <a href="#-quick-start">Quick Start</a> •
  <a href="#-skills">Skills</a> •
  <a href="#-usage">Usage</a> •
  <a href="#-requirements">Requirements</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Claude%20Code-CLI-8A2BE2?logo=anthropic&logoColor=white" alt="Claude Code">
  <img src="https://img.shields.io/badge/WezTerm-Terminal-4E9A06?logo=wezterm&logoColor=white" alt="WezTerm">
  <img src="https://img.shields.io/badge/License-MIT-yellow" alt="License">
</p>

**English** | [中文](#中文)

---

## Overview

**Claude CCB Skills** is a multi-AI collaboration toolkit that enables Claude Code to delegate tasks to other AI assistants (Codex, Gemini, OpenCode, iFlow, Kimi, Qwen, DeepSeek, Droid) running in separate terminal sessions.

### Why CCB Skills?

| Challenge | Solution |
|-----------|----------|
| Single AI limitations | **Multi-AI collaboration** for diverse perspectives |
| Synchronous blocking | **Async delegation** - continue working while waiting |
| Manual provider switching | **Unified commands** - consistent `*ask` / `*ping` interface |
| No visibility into AI status | **Provider monitoring** - health checks and connectivity |

---

## Features

| Feature | Description |
|---------|-------------|
| **Async Delegation** | Send tasks to providers without blocking |
| **9 AI Providers** | Claude, Codex, Gemini, OpenCode, DeepSeek, iFlow, Kimi, Qwen, Droid |
| **Unified Commands** | Consistent `*ask` / `*ping` / `*pend` interface |
| **Collaborative Planning** | Multi-AI planning with `all-plan` |
| **STEM Modeling** | Distributed academic modeling |
| **CCB Launcher** | Environment management and setup |

---

## Quick Start

### Installation

```bash
cd ~/.claude/skills
git clone https://github.com/LeoLin990405/claude-ccb-skills.git
```

### Verify Installation

```bash
ls ~/.claude/skills/claude-ccb-skills/SKILL.md
```

---

## Skills

| Skill | Command | Description |
|-------|---------|-------------|
| `ask` | `/ask <provider> <msg>` | Generic async delegation |
| `cask` | `/cask <msg>` | Delegate to Codex |
| `gask` | `/gask <msg>` | Delegate to Gemini |
| `oask` | `/oask <msg>` | Delegate to OpenCode |
| `iask` | `/iask <msg>` | Delegate to iFlow |
| `kask` | `/kask <msg>` | Delegate to Kimi |
| `qask` | `/qask <msg>` | Delegate to Qwen |
| `dskask` | `/dskask <msg>` | Delegate to DeepSeek |
| `dask` | `/dask <msg>` | Delegate to Droid |
| `ping` | `/ping <provider>` | Check provider connectivity |
| `pend` | `/pend <provider>` | Fetch latest reply |
| `ccb-launcher` | `/ccb-launcher` | CCB environment management |
| `all-plan` | `/all-plan` | Multi-AI collaborative planning |
| `stem-modeling` | `/stem-modeling` | STEM academic modeling |

---

## Usage

```bash
# Delegate to Gemini
/gask "analyze this code"

# Delegate to Codex
/cask "review this PR"

# Check provider status
/ping codex

# Fetch latest reply
/pend gemini
```

---

## Requirements

- Claude Code CLI
- WezTerm or tmux for multi-session management
- Respective AI CLI tools installed (codex, gemini-cli, etc.)

---

## 中文

### 概述

**Claude CCB Skills** 是一个多 AI 协作工具集，允许 Claude Code 将任务委托给在独立终端会话中运行的其他 AI 助手。

### 包含的技能

| 技能 | 命令 | 描述 |
|------|------|------|
| `ask` | `/ask <provider> <msg>` | 通用异步委托 |
| `cask` | `/cask <msg>` | 委托给 Codex |
| `gask` | `/gask <msg>` | 委托给 Gemini |
| `oask` | `/oask <msg>` | 委托给 OpenCode |
| `iask` | `/iask <msg>` | 委托给 iFlow |
| `kask` | `/kask <msg>` | 委托给 Kimi |
| `qask` | `/qask <msg>` | 委托给 Qwen |
| `dskask` | `/dskask <msg>` | 委托给 DeepSeek |
| `dask` | `/dask <msg>` | 委托给 Droid |
| `ping` | `/ping <provider>` | 检查 provider 连接 |
| `pend` | `/pend <provider>` | 获取最新回复 |
| `ccb-launcher` | `/ccb-launcher` | CCB 环境管理 |
| `all-plan` | `/all-plan` | 多 AI 协作规划 |
| `stem-modeling` | `/stem-modeling` | STEM 学术建模 |

### 安装

```bash
cd ~/.claude/skills
git clone https://github.com/LeoLin990405/claude-ccb-skills.git
```

### 使用方法

```bash
# 委托给 Gemini
/gask "分析这段代码"

# 委托给 Codex
/cask "审查这个 PR"

# 检查 provider 状态
/ping codex
```

### 依赖

- Claude Code CLI
- WezTerm 或 tmux（多会话管理）
- 相应的 AI CLI 工具（codex、gemini-cli 等）

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
