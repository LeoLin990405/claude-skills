---
name: design-frontend
description: Frontend design module - UI components, React web artifacts, and theming with 10 preset themes
triggers:
  - frontend
  - UI design
  - web design
  - React
  - web artifact
  - component
  - theme
  - theming
  - responsive
  - layout
  - shadcn
  - Tailwind
---

# Design Frontend: Web UI and Theming

Frontend design bridges visual design and working code. This module covers UI component design, multi-component React artifact construction, and theme application — everything needed to go from mockup to functional, styled web output.

## When to Use This Module

- Designing UI components (buttons, forms, cards, navigation)
- Building complete React web artifacts with multiple components
- Applying pre-built themes or creating custom theme systems
- Creating responsive layouts for web applications
- Theming an existing project with a cohesive visual style

## Workflow Overview

```
1. Define UI Requirements → 2. Choose Theme → 3. Design Components → 4. Build Artifact → 5. Polish
```

For theming: start at step 2 with **theme-factory**, then apply to components.
For UI components: start at step 3 with **frontend-design**.
For full artifacts: use all three skills in sequence.

## Skills

### 1. Frontend Design

**Skill**: [frontend-design](../frontend-design/SKILL.md)

Design frontend interfaces with modern patterns — component architecture, responsive layouts, interaction design, and accessibility. Covers the design thinking behind UI, not just implementation.

**Key capabilities**:
- Component-based UI architecture
- Responsive design patterns and breakpoint strategy
- Interaction design (hover, focus, active, disabled states)
- Accessibility-first design (ARIA, keyboard nav, screen readers)
- Layout systems (flexbox, grid, container queries)

### 2. Web Artifacts Builder

**Skill**: [web-artifacts-builder](../web-artifacts-builder/SKILL.md)

Construct multi-component React artifacts with bundling and deployment scripts. Handles project scaffolding, component organization, and build pipeline.

**Key capabilities**:
- React project scaffolding with sensible defaults
- Multi-component artifact assembly
- shadcn/ui component integration
- Build scripts for bundling and deployment
- Component composition patterns

**Assets**:
- `web-artifacts-builder/scripts/init-artifact.sh` — Project scaffolding
- `web-artifacts-builder/scripts/bundle-artifact.sh` — Build pipeline
- `web-artifacts-builder/scripts/shadcn-components.tar.gz` — Pre-built components

### 3. Theme Factory

**Skill**: [theme-factory](../theme-factory/SKILL.md)

Apply and customize visual themes from a library of 10 preset themes. Each theme is a complete design system with colors, typography, spacing, and component styles.

**Key capabilities**:
- 10 preset themes (Nord, Dracula, Catppuccin, Tokyo Night, and more)
- Custom theme generation from any color palette
- CSS custom properties for runtime theming
- Dark/light mode support
- Theme showcase PDF for visual comparison

**Assets**:
- `theme-factory/themes/` — 10 theme definition files
- `theme-factory/theme-showcase.pdf` — Visual theme catalog

**Available Themes**:

| Theme | Style | Best For |
|-------|-------|----------|
| Arctic Frost | Cool, minimal | Developer tools, dashboards |
| Botanical Garden | Green, organic | Health, sustainability |
| Desert Rose | Warm, earthy | Lifestyle, editorial |
| Forest Canopy | Deep green | Nature, outdoors |
| Golden Hour | Warm amber | Photography, creative |
| Midnight Galaxy | Dark, cosmic | Entertainment, media |
| Modern Minimalist | Clean, neutral | SaaS, productivity |
| Ocean Depths | Deep blue | Finance, enterprise |
| Sunset Boulevard | Vibrant warm | Social, community |
| Tech Innovation | Electric, sharp | Tech startups, AI |

## Combining the Skills

For a themed web application:
1. Browse **theme-factory** to select a theme (or define custom)
2. Use **frontend-design** to plan component architecture and layouts
3. Use **web-artifacts-builder** to scaffold, build, and bundle the artifact
4. Apply the selected theme via CSS custom properties

For a quick themed component:
1. Pick a theme from **theme-factory**
2. Build directly with **frontend-design** using theme tokens

## Module Checklist

- [ ] UI requirements documented (components needed, interactions, states)
- [ ] Theme selected or custom palette defined
- [ ] Responsive breakpoints planned (mobile, tablet, desktop)
- [ ] Component states designed (default, hover, focus, active, disabled, error)
- [ ] Accessibility verified (contrast, keyboard nav, screen reader)
- [ ] Build pipeline tested (init, develop, bundle)
- [ ] Design reviewed using [design-review-checklist](../../templates/design-review-checklist.md)

## Related Modules

- For visual assets to embed: [design-visual](../design-visual/SKILL.md) — posters, illustrations
- For generative backgrounds or animations: [design-generative](../design-generative/SKILL.md)
- For design tokens and documentation: [design-system](../design-system/SKILL.md)
