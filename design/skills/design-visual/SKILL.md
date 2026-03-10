---
name: design-visual
description: Static visual design module - canvas compositions, posters, brand assets, and brand guidelines
triggers:
  - visual design
  - poster
  - canvas
  - brand
  - brand guidelines
  - brand assets
  - visual identity
  - composition
  - layout
  - print design
---

# Design Visual: Static Composition and Brand

Visual design is the craft of arranging elements — color, type, shape, space — to communicate clearly and beautifully. This module covers canvas-based compositions (posters, illustrations, infographics) and brand identity (guidelines, assets, visual standards).

## When to Use This Module

- Designing posters, covers, banners, or visual compositions
- Creating or applying brand guidelines to design work
- Building visual assets that must align with an established identity
- Producing print-ready or high-resolution static artwork
- Defining the visual language for a new project or product

## Workflow Overview

```
1. Review Brand → 2. Set Up Canvas → 3. Compose Layout → 4. Refine Details → 5. Export
```

If brand guidelines exist, start at step 1 with **brand-guidelines**.
If this is freeform visual work, start at step 2 with **canvas-design**.

## Skills

### 1. Canvas Design

**Skill**: [canvas-design](../canvas-design/SKILL.md)

Create visual compositions using the Canvas API with a rich font library. Supports posters, data visualizations, abstract art, and typographic layouts.

**Key capabilities**:
- High-resolution canvas rendering (PNG, PDF)
- 40+ bundled fonts (serif, sans-serif, mono, display)
- Typographic composition and layout systems
- Grid-based and freeform composition
- Design philosophy guidance (balance, contrast, hierarchy)

**Assets**:
- `canvas-design/canvas-fonts/` — 40+ font files (TTF) with licenses
- See the full font catalog in the skill for pairing recommendations

### 2. Brand Guidelines

**Skill**: [brand-guidelines](../brand-guidelines/SKILL.md)

Reference and apply Anthropic brand guidelines including color palette, typography rules, logo usage, and visual tone. Use this as a constraint layer on top of any other design skill.

**Key capabilities**:
- Official color palette with usage rules
- Typography standards and font hierarchy
- Logo usage guidelines (spacing, sizing, placement)
- Visual tone and personality direction
- Do's and don'ts for brand representation

## Combining the Skills

For brand-aligned visual work:
1. Load **brand-guidelines** to understand color, type, and tone constraints
2. Use **canvas-design** to compose the actual visual
3. Cross-check against brand rules before finalizing

For freeform visual work:
1. Use **canvas-design** directly with your own palette and fonts
2. Optionally create a project-specific style guide using [style-guide template](../../templates/style-guide.md)

## Module Checklist

- [ ] Brand guidelines reviewed (if applicable)
- [ ] Canvas dimensions and format defined (PNG / PDF / resolution)
- [ ] Color palette selected and documented
- [ ] Typography choices made (heading + body fonts, sizes)
- [ ] Composition follows visual hierarchy principles
- [ ] Design reviewed using [design-review-checklist](../../templates/design-review-checklist.md)
- [ ] Final asset exported at correct resolution and format

## Related Modules

- For generative patterns and textures: [design-generative](../design-generative/SKILL.md)
- For implementing visuals as web UI: [design-frontend](../design-frontend/SKILL.md)
- For documenting visual standards: [design-system](../design-system/SKILL.md)
