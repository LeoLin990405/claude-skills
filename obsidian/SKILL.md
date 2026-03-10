---
name: knowledge-toolkit
description: Knowledge management toolkit for Obsidian — 3 format skills, 4 workflow templates. Covers the full knowledge lifecycle from capture to visualization.
version: 2.0.0
triggers:
  - knowledge management
  - obsidian
  - note-taking
  - daily note
  - meeting note
  - project tracker
  - research
  - canvas
  - markdown
  - wikilinks
  - callouts
  - bases
  - database
  - visual mapping
  - zettelkasten
  - PKM
  - second brain
---

# Knowledge Management Toolkit

A complete Obsidian knowledge management toolkit. Three format reference skills plus workflow templates covering the full knowledge lifecycle: capture, organize, connect, visualize.

## Routing Guide

| User Intent | Skill | Quick Templates |
|---|---|---|
| Note-taking, markdown, wikilinks, callouts, embeds, properties | [obsidian-markdown](skills/obsidian-markdown/SKILL.md) | [daily-note](templates/daily-note.md), [meeting-note](templates/meeting-note.md) |
| Databases, tracking, tables, filters, formulas, status views | [obsidian-bases](skills/obsidian-bases/SKILL.md) | [project-tracker](templates/project-tracker.base) |
| Visual mapping, spatial layout, node connections, brainstorming | [json-canvas](skills/json-canvas/SKILL.md) | [research-canvas](templates/research-canvas.canvas) |
| "I need a [template]" | Serve directly from [templates/](templates/) | — |

## Quick Actions

Common knowledge management tasks with direct template links:

- **"Create a daily note"** → Load [obsidian-markdown](skills/obsidian-markdown/SKILL.md) + [daily-note](templates/daily-note.md)
- **"Set up a project tracker"** → Load [obsidian-bases](skills/obsidian-bases/SKILL.md) + [project-tracker](templates/project-tracker.base)
- **"Map out a research topic"** → Load [json-canvas](skills/json-canvas/SKILL.md) + [research-canvas](templates/research-canvas.canvas)
- **"Take meeting notes"** → Load [obsidian-markdown](skills/obsidian-markdown/SKILL.md) + [meeting-note](templates/meeting-note.md)
- **"Build a knowledge base"** → Load [obsidian-markdown](skills/obsidian-markdown/SKILL.md) for format, [obsidian-bases](skills/obsidian-bases/SKILL.md) for indexing
- **"Create a visual overview"** → Load [json-canvas](skills/json-canvas/SKILL.md) + [research-canvas](templates/research-canvas.canvas)

## Workflow Overview

The knowledge lifecycle in Obsidian follows four phases:

```
Capture → Organize → Connect → Visualize
```

| Phase | Activity | Skills & Templates |
|---|---|---|
| **Capture** | Daily notes, meeting notes, fleeting ideas | obsidian-markdown + daily-note, meeting-note |
| **Organize** | Properties, tags, database views, status tracking | obsidian-bases + project-tracker |
| **Connect** | Wikilinks, backlinks, block references, transclusion | obsidian-markdown |
| **Visualize** | Canvas maps, spatial layouts, node grouping | json-canvas + research-canvas |

## Skills

| # | Skill | Scope |
|---|-------|-------|
| 1 | **obsidian-markdown** | Wikilinks, embeds, callouts, properties, frontmatter, Obsidian Flavored Markdown |
| 2 | **obsidian-bases** | Database views, filters, sorts, formulas, aggregations, YAML schema |
| 3 | **json-canvas** | JSON Canvas spec, nodes, edges, groups, colors, spatial layout |

## Templates

| Template | Format | Use Case |
|----------|--------|----------|
| [daily-note](templates/daily-note.md) | Markdown | Daily journal with tasks, notes, and reflections |
| [project-tracker](templates/project-tracker.base) | Bases | Track projects by status, priority, due date, tags |
| [research-canvas](templates/research-canvas.canvas) | Canvas | Map research from central topic to findings |
| [meeting-note](templates/meeting-note.md) | Markdown | Meeting notes with attendees, decisions, actions |
