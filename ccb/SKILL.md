---
name: coordination-toolkit
description: Multi-AI coordination toolkit — route tasks to 9 providers, orchestrate parallel workflows, synthesize results. Covers single delegation, multi-provider fan-out, consensus, and specialist routing.
version: 2.0.0
triggers:
  - multi-AI
  - coordination
  - delegate
  - ask provider
  - ask codex
  - ask gemini
  - ask opencode
  - ask deepseek
  - ask kimi
  - ask qwen
  - ask iflow
  - ask droid
  - parallel review
  - consensus
  - fan-out
  - ping
  - pend
  - ccb
  - all-plan
  - stem modeling
---

# Multi-AI Coordination Toolkit

Route tasks to AI providers, orchestrate multi-provider workflows, and synthesize results.

## Routing Guide

| User Intent | Route To | Quick Templates |
|---|---|---|
| Delegate a task to one provider | Provider-specific skill below | -- |
| Get multiple AIs to review/analyze in parallel | [all-plan](skills/all-plan/SKILL.md) | [parallel-review](templates/parallel-review.md) |
| Get consensus from multiple providers on a decision | [all-plan](skills/all-plan/SKILL.md) | [consensus-decision](templates/consensus-decision.md) |
| Delegate a research task to the best-fit provider | Provider-specific skill below | [research-delegation](templates/research-delegation.md) |
| Check if a provider finished | [pend](skills/pend/SKILL.md) | -- |
| Check provider connectivity | [ping](skills/ping/SKILL.md) | -- |
| STEM academic modeling | [stem-modeling](skills/stem-modeling/SKILL.md) | -- |
| Set up CCB environment | [ccb-launcher](skills/ccb-launcher/SKILL.md) | -- |
| Learn orchestration patterns | [patterns](orchestration/patterns.md) | -- |

## Provider Index

| Provider | Command | Best For |
|----------|---------|----------|
| **Codex** | `/cask <msg>` | Code generation, refactoring, PR review |
| **Gemini** | `/gask <msg>` | Long-context analysis, research synthesis, multimodal |
| **OpenCode** | `/oask <msg>` | Code analysis, debugging, architecture review |
| **DeepSeek** | `/dskask <msg>` | Reasoning-heavy tasks, math, algorithms |
| **iFlow** | `/iask <msg>` | Workflow automation, integration tasks |
| **Kimi** | `/kask <msg>` | Long document processing, Chinese-language tasks |
| **Qwen** | `/qask <msg>` | Multilingual tasks, general-purpose analysis |
| **Droid** | `/dask <msg>` | Mobile/Android development, platform-specific tasks |
| **Generic** | `/ask <provider> <msg>` | Any provider by name |

## Quick Actions

Common coordination tasks with direct links:

- **"Review this code with multiple AIs"** --> Fan out with [parallel-review](templates/parallel-review.md), collect with `/pend`
- **"Get opinions on this architecture"** --> Use [consensus-decision](templates/consensus-decision.md) pattern
- **"Research this topic thoroughly"** --> Delegate with [research-delegation](templates/research-delegation.md)
- **"Ask Gemini to analyze this"** --> `/gask "analyze ..."`
- **"Ask Codex to review this PR"** --> `/cask "review ..."`
- **"Check if Codex is done"** --> `/pend codex`
- **"Is Gemini running?"** --> `/ping gemini`
- **"Plan across all providers"** --> `/all-plan`

## Orchestration Patterns

For advanced multi-AI workflows, see [orchestration/patterns.md](orchestration/patterns.md):

| Pattern | When to Use |
|---------|-------------|
| **Parallel Fan-Out** | Same task to multiple providers, synthesize results |
| **Sequential Pipeline** | Chain providers: one's output feeds the next |
| **Consensus Voting** | Multiple providers vote on a decision |
| **Specialist Routing** | Route sub-tasks to the best-fit provider |

## Skills Index

### Delegation (9 skills)

| Skill | Description |
|-------|-------------|
| [ask](skills/ask/SKILL.md) | Generic async delegation to any provider |
| [cask](skills/cask/SKILL.md) | Delegate to Codex |
| [gask](skills/gask/SKILL.md) | Delegate to Gemini |
| [oask](skills/oask/SKILL.md) | Delegate to OpenCode |
| [dskask](skills/dskask/SKILL.md) | Delegate to DeepSeek |
| [iask](skills/iask/SKILL.md) | Delegate to iFlow |
| [kask](skills/kask/SKILL.md) | Delegate to Kimi |
| [qask](skills/qask/SKILL.md) | Delegate to Qwen |
| [dask](skills/dask/SKILL.md) | Delegate to Droid |

### Monitoring (2 skills)

| Skill | Description |
|-------|-------------|
| [pend](skills/pend/SKILL.md) | Fetch latest reply from a provider |
| [ping](skills/ping/SKILL.md) | Check provider connectivity |

### Workflows (3 skills)

| Skill | Description |
|-------|-------------|
| [all-plan](skills/all-plan/SKILL.md) | Multi-AI collaborative planning |
| [stem-modeling](skills/stem-modeling/SKILL.md) | STEM academic modeling |
| [ccb-launcher](skills/ccb-launcher/SKILL.md) | CCB environment management |

## Templates

| Template | Purpose |
|----------|---------|
| [parallel-review](templates/parallel-review.md) | Delegate code review to multiple providers in parallel |
| [consensus-decision](templates/consensus-decision.md) | Get multiple AI opinions on a design decision |
| [research-delegation](templates/research-delegation.md) | Delegate research tasks to specialized providers |
