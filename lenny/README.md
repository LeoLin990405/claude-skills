<p align="center">
  <img src="https://img.shields.io/badge/Claude%20Code-Skill-blue?style=for-the-badge" alt="Claude Code Skill">
  <img src="https://img.shields.io/badge/Skills-88-green?style=for-the-badge" alt="Skills">
  <img src="https://img.shields.io/badge/PM-Toolkit-orange?style=for-the-badge" alt="PM Toolkit">
</p>

<h1 align="center">PM Toolkit</h1>

<p align="center">
  <strong>Complete Product Management Toolkit for Claude Code</strong>
  <br>
  <em>8 workflow modules, 88 skills, 10 executable templates — covering the full PM lifecycle</em>
</p>

<p align="center">
  <a href="#-modules">Modules</a> •
  <a href="#-templates">Templates</a> •
  <a href="#-playbooks">Playbooks</a> •
  <a href="#-quick-start">Quick Start</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Claude%20Code-CLI-8A2BE2?logo=anthropic&logoColor=white" alt="Claude Code">
  <img src="https://img.shields.io/badge/Lenny's-Podcast-FF6B6B?logo=podcast&logoColor=white" alt="Lenny's Podcast">
  <img src="https://img.shields.io/badge/License-MIT-yellow" alt="License">
</p>

**English** | [中文](#中文)

---

## Overview

**PM Toolkit** is a complete product management toolkit organized by workflow phase. It evolved from 86 Lenny's Podcast skills into 8 actionable workflow modules with executable templates, frameworks, and checklists.

### What Changed (v2.0)

| Before (v1) | After (v2) |
|-------------|------------|
| 16 knowledge categories | **8 workflow modules** |
| Advice-level bullet points | **Actionable frameworks with anti-patterns** |
| No templates | **10 executable templates** |
| Domain-organized | **Lifecycle-organized** |

---

## Modules

| # | Module | Skills | What It Covers |
|---|--------|--------|---------------|
| 1 | [pm-discovery](skills/pm-discovery/SKILL.md) | 7 | Problem definition, user research, competitive analysis, JTBD |
| 2 | [pm-strategy](skills/pm-strategy/SKILL.md) | 8 | Vision, north star, OKRs, roadmap, PRD, prioritization |
| 3 | [pm-execution](skills/pm-execution/SKILL.md) | 10 | Shipping, timelines, decisions, meetings, retros |
| 4 | [pm-growth](skills/pm-growth/SKILL.md) | 8 | PMF, growth loops, pricing, retention, experiments |
| 5 | [pm-analytics](skills/pm-analytics/SKILL.md) | 8 | Metrics, financial modeling, data-driven decisions, platform |
| 6 | [pm-communication](skills/pm-communication/SKILL.md) | 9 | Presentations, writing, stakeholders, brand, content |
| 7 | [pm-team](skills/pm-team/SKILL.md) | 22 | Hiring, 1:1s, culture, delegation, sales team |
| 8 | [pm-leadership](skills/pm-leadership/SKILL.md) | 16 | Coaching, product taste, AI strategy, org design, career |

---

## Templates

Ready-to-use templates for common PM tasks:

| Template | Use Case |
|----------|----------|
| [prd-template](templates/prd-template.md) | Write a product requirements document |
| [okr-template](templates/okr-template.md) | Set quarterly OKRs |
| [user-interview-script](templates/user-interview-script.md) | Conduct user research interviews |
| [competitive-analysis](templates/competitive-analysis.md) | Analyze competitive landscape |
| [launch-checklist](templates/launch-checklist.md) | Plan and execute a product launch |
| [retro-template](templates/retro-template.md) | Run retrospectives and post-mortems |
| [metrics-dashboard](templates/metrics-dashboard.md) | Design a metrics dashboard |
| [one-on-one-template](templates/one-on-one-template.md) | Run effective 1:1 meetings |
| [decision-doc-template](templates/decision-doc-template.md) | Make and document decisions |
| [financial-model-spec](templates/financial-model-spec.md) | Build financial models and unit economics |

---

## Playbooks

Role-based workflow sequences — see [pm-playbooks](skills/pm-playbooks/SKILL.md):

| Playbook | Workflow Sequence |
|----------|------------------|
| **Startup Founder** | discovery → strategy → execution → growth → team → leadership |
| **Product Manager** | discovery → strategy → execution → communication → leadership |
| **First-Time Manager** | team → communication → execution → leadership |
| **Growth Leader** | growth → discovery → analytics → communication → leadership |
| **Engineering Manager** | execution → analytics → team → communication |
| **Sales Leader** | team → communication → strategy → growth |
| **AI Builder** | leadership → strategy → discovery → growth → execution |
| **Executive** | communication → leadership → strategy → execution |
| **Career Growth** | leadership → communication → team |

---

## Quick Start

### Installation

```bash
cd ~/.claude/skills
git clone https://github.com/LeoLin990405/claude-lenny-skills.git
```

### Usage

```bash
# The toolkit auto-routes based on your request:
"Help me write a PRD"              → pm-strategy + prd-template
"Prepare user interviews"          → pm-discovery + interview-script
"Set OKRs for Q2"                  → pm-strategy + okr-template
"Run a retro"                      → pm-execution + retro-template
"Build a financial model"          → pm-analytics + financial-model-spec

# Or access modules directly:
"Use the PM growth module"         → pm-growth
"Show me the founder playbook"     → pm-playbooks
```

---

## 中文

### 概述

**PM Toolkit** 是一个完整的产品管理工具集，按工作流阶段组织。从 86 个 Lenny's Podcast 技能进化为 8 个可执行的工作流模块，包含模板、框架和检查清单。

### 模块

| 模块 | 技能数 | 覆盖范围 |
|------|--------|---------|
| pm-discovery | 7 | 问题定义、用户研究、竞品分析 |
| pm-strategy | 8 | 愿景、北极星指标、OKR、路线图、PRD |
| pm-execution | 10 | 发布、时间线、决策、会议、复盘 |
| pm-growth | 8 | PMF、增长飞轮、定价、留存、实验 |
| pm-analytics | 8 | 指标、财务建模、数据驱动决策 |
| pm-communication | 9 | 演示、写作、利益相关者、品牌 |
| pm-team | 22 | 招聘、1:1、文化、委派、销售团队 |
| pm-leadership | 16 | 教练、产品品味、AI 战略、组织设计 |

### 安装

```bash
cd ~/.claude/skills
git clone https://github.com/LeoLin990405/claude-lenny-skills.git
```

---

## Contributors

- **Leo** ([@LeoLin990405](https://github.com/LeoLin990405)) - Project Lead
- **Claude** (Anthropic Claude) - Content Generation

## Acknowledgements

- **[Lenny Rachitsky](https://www.lennyspodcast.com/)** - For the incredible podcast and PM wisdom

## License

MIT License - see [LICENSE](LICENSE) for details.

---

<p align="center">
  <sub>Built with collaboration between human and AI</sub>
</p>
