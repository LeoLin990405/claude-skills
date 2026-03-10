---
name: developer-toolkit
description: Complete developer toolkit - 6 specialized skills, 3 templates. Covers skill creation, MCP server building, documentation, testing, communications, and research.
version: 2.0.0
triggers:
  - developer toolkit
  - dev tools
  - skill creator
  - create skill
  - build skill
  - MCP server
  - MCP builder
  - build MCP
  - anthropic docs
  - anthropic API
  - claude API
  - claude code
  - webapp testing
  - playwright
  - test web app
  - internal comms
  - status report
  - history notes
  - note processing
  - test plan
  - skill spec
  - mcp spec
---

# Developer Toolkit

A complete developer toolkit organized by domain. Each skill is an actionable workflow with frameworks, templates, and best practices.

## Routing Guide

| User Intent | Skill | Quick Templates |
|---|---|---|
| Create a new skill, update skill format, SKILL.md best practices | [skill-creator](skills/skill-creator/SKILL.md) | [skill-spec](templates/skill-spec.md) |
| Build an MCP server, define tools/resources, FastMCP or TypeScript SDK | [mcp-builder](skills/mcp-builder/SKILL.md) | [mcp-server-spec](templates/mcp-server-spec.md) |
| Anthropic docs, Claude API, model selection, Claude Code features | [anthropic-docs](skills/anthropic-docs/SKILL.md) | -- |
| Write status reports, leadership updates, newsletters, incident reports | [internal-comms](skills/internal-comms/SKILL.md) | -- |
| Test web apps, Playwright, screenshots, browser debugging | [webapp-testing](skills/webapp-testing/SKILL.md) | [test-plan](templates/test-plan.md) |
| Process history notes, Gemini exports, academic research notes | [history-note-processor](skills/history-note-processor/SKILL.md) | -- |
| "I need a [template]" | Serve directly from [templates/](templates/) | -- |

## Quick Actions

Common developer tasks with direct template links:

- **"Create a new skill"** -> Load [skill-creator](skills/skill-creator/SKILL.md) + [skill-spec](templates/skill-spec.md)
- **"Build an MCP server"** -> Load [mcp-builder](skills/mcp-builder/SKILL.md) + [mcp-server-spec](templates/mcp-server-spec.md)
- **"Test my web app"** -> Load [webapp-testing](skills/webapp-testing/SKILL.md) + [test-plan](templates/test-plan.md)
- **"Write a status report"** -> Load [internal-comms](skills/internal-comms/SKILL.md)
- **"Look up Anthropic API docs"** -> Load [anthropic-docs](skills/anthropic-docs/SKILL.md)
- **"Process my history notes"** -> Load [history-note-processor](skills/history-note-processor/SKILL.md)

## Skill Index

| # | Group | Skill | Scope |
|---|-------|-------|-------|
| 1 | **Development Tools** | [skill-creator](skills/skill-creator/SKILL.md) | Skill creation guide, SKILL.md format, best practices, templates |
| 2 | **Development Tools** | [mcp-builder](skills/mcp-builder/SKILL.md) | MCP server creation, FastMCP/TypeScript SDK, tool definitions, resources |
| 3 | **Knowledge Base** | [anthropic-docs](skills/anthropic-docs/SKILL.md) | Anthropic documentation, Claude API, model selection, Claude Code |
| 4 | **Communications** | [internal-comms](skills/internal-comms/SKILL.md) | Status reports, leadership updates, newsletters, incident reports, FAQs |
| 5 | **Testing** | [webapp-testing](skills/webapp-testing/SKILL.md) | Playwright-based web app testing, screenshots, browser logs, UI debugging |
| 6 | **Research** | [history-note-processor](skills/history-note-processor/SKILL.md) | Four-step deep reading methodology, YAML frontmatter, Mermaid diagrams |

## Templates

| Template | Use Case |
|----------|----------|
| [mcp-server-spec](templates/mcp-server-spec.md) | Specify an MCP server: tools, resources, prompts, auth, deployment |
| [skill-spec](templates/skill-spec.md) | Specify a new skill: name, triggers, workflow, resources, testing |
| [test-plan](templates/test-plan.md) | Plan web app testing: scenarios, expected results, environment setup |
