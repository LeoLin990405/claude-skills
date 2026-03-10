<p align="center">
  <img src="https://img.shields.io/badge/Claude%20Code-Skill-blue?style=for-the-badge" alt="Claude Code Skill">
  <img src="https://img.shields.io/badge/Skills-14-green?style=for-the-badge" alt="Skills">
  <img src="https://img.shields.io/badge/Multi--AI-Coordination-orange?style=for-the-badge" alt="Multi-AI Coordination">
</p>

<h1 align="center">Multi-AI Coordination Toolkit</h1>

<p align="center">
  <strong>Route tasks to 9 AI providers, orchestrate parallel workflows, synthesize results</strong>
  <br>
  <em>14 skills, 4 orchestration patterns, 3 executable templates</em>
</p>

<p align="center">
  <a href="#modules">Modules</a> •
  <a href="#templates">Templates</a> •
  <a href="#orchestration-patterns">Patterns</a> •
  <a href="#quick-start">Quick Start</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Claude%20Code-CLI-8A2BE2?logo=anthropic&logoColor=white" alt="Claude Code">
  <img src="https://img.shields.io/badge/WezTerm-Terminal-4E9A06?logo=wezterm&logoColor=white" alt="WezTerm">
  <img src="https://img.shields.io/badge/License-MIT-yellow" alt="License">
</p>

**English** | [中文](#中文)

---

## Overview

**Multi-AI Coordination Toolkit** enables Claude Code to delegate tasks to 9 AI providers running in separate terminal sessions. Beyond simple delegation, it provides orchestration patterns and templates for parallel fan-out, consensus voting, sequential pipelines, and specialist routing.

### What Changed (v2.0)

| Before (v1) | After (v2) |
|-------------|------------|
| Flat list of 14 skills | **Organized by function**: delegation, monitoring, workflows |
| No orchestration guidance | **4 orchestration patterns** with step-by-step instructions |
| No templates | **3 executable templates** for common multi-AI workflows |
| Skills-only | **Router SKILL.md** auto-routes based on user intent |

---

## Modules

### Delegation (9 providers)

| Provider | Command | Best For |
|----------|---------|----------|
| [Codex](skills/cask/SKILL.md) | `/cask <msg>` | Code generation, refactoring, PR review |
| [Gemini](skills/gask/SKILL.md) | `/gask <msg>` | Long-context analysis, research, multimodal |
| [OpenCode](skills/oask/SKILL.md) | `/oask <msg>` | Code analysis, debugging, architecture |
| [DeepSeek](skills/dskask/SKILL.md) | `/dskask <msg>` | Reasoning, math, algorithms |
| [iFlow](skills/iask/SKILL.md) | `/iask <msg>` | Workflow automation, integrations |
| [Kimi](skills/kask/SKILL.md) | `/kask <msg>` | Long documents, Chinese-language tasks |
| [Qwen](skills/qask/SKILL.md) | `/qask <msg>` | Multilingual, general-purpose analysis |
| [Droid](skills/dask/SKILL.md) | `/dask <msg>` | Mobile/Android development |
| [Generic](skills/ask/SKILL.md) | `/ask <provider> <msg>` | Any provider by name |

### Monitoring

| Skill | Command | Description |
|-------|---------|-------------|
| [pend](skills/pend/SKILL.md) | `/pend <provider>` | Fetch latest reply from a provider |
| [ping](skills/ping/SKILL.md) | `/ping <provider>` | Check provider connectivity |

### Workflows

| Skill | Command | Description |
|-------|---------|-------------|
| [all-plan](skills/all-plan/SKILL.md) | `/all-plan` | Multi-AI collaborative planning |
| [stem-modeling](skills/stem-modeling/SKILL.md) | `/stem-modeling` | STEM academic modeling |
| [ccb-launcher](skills/ccb-launcher/SKILL.md) | `/ccb-launcher` | CCB environment management |

---

## Templates

Ready-to-use templates for common multi-AI workflows:

| Template | Use Case |
|----------|----------|
| [parallel-review](templates/parallel-review.md) | Send code review to multiple providers in parallel, then synthesize |
| [consensus-decision](templates/consensus-decision.md) | Get multiple AI opinions on a design/architecture decision |
| [research-delegation](templates/research-delegation.md) | Delegate research tasks to specialized providers |

---

## Orchestration Patterns

For advanced multi-AI coordination, see [orchestration/patterns.md](orchestration/patterns.md):

| Pattern | When to Use |
|---------|-------------|
| **Parallel Fan-Out** | Same task to N providers, synthesize results |
| **Sequential Pipeline** | Chain providers: output of one feeds the next |
| **Consensus Voting** | Multiple providers vote on a decision |
| **Specialist Routing** | Route sub-tasks to the best-fit provider |

---

## Quick Start

### Installation

```bash
cd ~/.claude/skills
git clone https://github.com/LeoLin990405/claude-ccb-skills.git
```

### Usage

```bash
# The toolkit auto-routes based on your request:
"Review this code with Gemini and Codex"  --> parallel fan-out + parallel-review template
"Get opinions on this architecture"       --> consensus-decision template
"Ask DeepSeek to solve this algorithm"    --> /dskask

# Direct provider delegation:
/gask "analyze this codebase"
/cask "review this PR"

# Check results:
/pend gemini
/ping codex
```

---

## 中文

### 概述

**多 AI 协调工具集** 让 Claude Code 能够将任务委托给 9 个独立终端会话中运行的 AI 服务商。除了简单委托外，还提供编排模式和模板，支持并行扇出、共识投票、顺序流水线和专家路由。

### 模块

| 类别 | 技能数 | 覆盖范围 |
|------|--------|---------|
| 委托 | 9 | Codex、Gemini、OpenCode、DeepSeek、iFlow、Kimi、Qwen、Droid、通用 |
| 监控 | 2 | 获取回复 (pend)、连接检查 (ping) |
| 工作流 | 3 | 多 AI 规划、STEM 建模、环境管理 |

### 模板

| 模板 | 用途 |
|------|------|
| parallel-review | 并行代码审查，多服务商同时审查后综合结果 |
| consensus-decision | 多 AI 共识决策，获取多方意见后投票 |
| research-delegation | 研究任务委托，按专长分配给最合适的服务商 |

### 编排模式

| 模式 | 适用场景 |
|------|---------|
| 并行扇出 | 同一任务发给多个服务商，综合结果 |
| 顺序流水线 | 链式调用，前一个的输出作为下一个的输入 |
| 共识投票 | 多个服务商投票决定 |
| 专家路由 | 按子任务特点分配给最擅长的服务商 |

### 安装

```bash
cd ~/.claude/skills
git clone https://github.com/LeoLin990405/claude-ccb-skills.git
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
