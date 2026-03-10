---
name: design-toolkit
description: Complete design toolkit - 4 workflow modules, 7 specialized skills, 3 templates. Covers the full design lifecycle from concept to polished output.
version: 2.0.0
triggers:
  - design
  - visual design
  - generative art
  - algorithmic art
  - canvas design
  - brand guidelines
  - theme
  - frontend design
  - web artifacts
  - UI design
  - design system
  - style guide
  - typography
  - color palette
  - GIF
  - motion design
  - p5.js
  - React component
  - design tokens
---

# Design Toolkit

A complete design toolkit organized by workflow phase. Each module groups related design skills into actionable workflows with checklists and linked templates.

## Routing Guide

| User Intent | Module | Quick Templates |
|---|---|---|
| Generative art, algorithmic visuals, animated GIFs, motion design | [design-generative](skills/design-generative/SKILL.md) | — |
| Posters, visual compositions, brand assets, brand guidelines | [design-visual](skills/design-visual/SKILL.md) | [design-brief](templates/design-brief.md), [style-guide](templates/style-guide.md) |
| Frontend UI, web components, React artifacts, theming | [design-frontend](skills/design-frontend/SKILL.md) | [design-brief](templates/design-brief.md) |
| Design tokens, component libraries, cross-skill consistency | [design-system](skills/design-system/SKILL.md) | [style-guide](templates/style-guide.md), [design-review-checklist](templates/design-review-checklist.md) |
| "I need a [template]" | Serve directly from [templates/](templates/) | — |

## Quick Actions

Common design tasks with direct module links:

- **"Create generative art"** → Load [design-generative](skills/design-generative/SKILL.md) → [algorithmic-art](skills/algorithmic-art/SKILL.md)
- **"Design a poster"** → Load [design-visual](skills/design-visual/SKILL.md) → [canvas-design](skills/canvas-design/SKILL.md)
- **"Apply brand guidelines"** → Load [design-visual](skills/design-visual/SKILL.md) → [brand-guidelines](skills/brand-guidelines/SKILL.md)
- **"Build a themed UI"** → Load [design-frontend](skills/design-frontend/SKILL.md) → [theme-factory](skills/theme-factory/SKILL.md)
- **"Create a React artifact"** → Load [design-frontend](skills/design-frontend/SKILL.md) → [web-artifacts-builder](skills/web-artifacts-builder/SKILL.md)
- **"Make a Slack GIF"** → Load [design-generative](skills/design-generative/SKILL.md) → [slack-gif-creator](skills/slack-gif-creator/SKILL.md)
- **"Set up a design system"** → Load [design-system](skills/design-system/SKILL.md) + [style-guide](templates/style-guide.md)
- **"Review my design"** → Load [design-review-checklist](templates/design-review-checklist.md)

## Modules

| # | Module | Skills | Scope |
|---|--------|--------|-------|
| 1 | **design-generative** | 2 | Algorithmic art (p5.js), animated GIFs, motion design, procedural visuals |
| 2 | **design-visual** | 2 | Canvas compositions, posters, brand assets, brand guidelines, visual identity |
| 3 | **design-frontend** | 3 | Frontend UI, React web artifacts, theming with 10 presets, responsive layouts |
| 4 | **design-system** | — | Design tokens, component documentation, cross-skill consistency, accessibility |

## Workflow Overview

Design projects typically flow through four phases. Each phase maps to one or more modules:

```
Concept          Design           Implement         Polish
───────          ──────           ─────────         ──────
Define brief     Create visuals   Build components  Review & refine
Set constraints  Apply brand      Apply themes      Check accessibility
Choose tools     Compose layout   Generate assets   Validate consistency
    │                │                │                  │
    ▼                ▼                ▼                  ▼
[design-brief]   [visual]         [frontend]        [design-review]
[style-guide]    [generative]     [generative]      [design-system]
```

### Phase-to-Module Mapping

| Phase | Modules | Templates |
|-------|---------|-----------|
| **Concept** — Define objectives, audience, constraints | design-system | [design-brief](templates/design-brief.md), [style-guide](templates/style-guide.md) |
| **Design** — Create visual assets, compositions, art | design-visual, design-generative | — |
| **Implement** — Build UI components, web artifacts, themes | design-frontend, design-generative | — |
| **Polish** — Review, ensure consistency, accessibility | design-system | [design-review-checklist](templates/design-review-checklist.md) |

## Source

Skills curated from professional design practice, covering generative art, visual design, frontend engineering, and design systems.
