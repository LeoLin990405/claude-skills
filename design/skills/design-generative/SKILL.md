---
name: design-generative
description: Generative and motion design module - algorithmic art with p5.js and animated GIF creation for Slack and web
triggers:
  - generative art
  - algorithmic art
  - p5.js
  - flow field
  - particle system
  - procedural
  - GIF
  - animated GIF
  - Slack GIF
  - motion design
---

# Design Generative: Algorithmic Art and Motion

Generative design produces visuals through code and algorithms rather than manual drawing. This module covers static generative art (p5.js) and animated output (GIF creation), giving you a complete pipeline from procedural concept to deliverable motion asset.

## When to Use This Module

- Creating algorithmic or procedural artwork (flow fields, particle systems, fractals)
- Building animated GIFs for Slack, social media, or web headers
- Generating unique visual patterns with seeded randomness
- Producing motion design assets from code
- Exploring creative coding as a design tool

## Workflow Overview

```
1. Define Parameters → 2. Write Algorithm → 3. Generate Frames → 4. Export (Static or Animated)
```

For static art: steps 1-2, then export PNG/SVG via **algorithmic-art**.
For motion: steps 1-4, composing frames into optimized GIF via **slack-gif-creator**.

## Skills

### 1. Algorithmic Art (p5.js)

**Skill**: [algorithmic-art](../algorithmic-art/SKILL.md)

Create generative artwork using p5.js with flow fields, particle systems, Perlin noise, and seeded randomness. Includes a generator template and HTML viewer for rapid iteration.

**Key capabilities**:
- Flow fields and vector-based compositions
- Particle systems with physics simulation
- Perlin noise landscapes and organic textures
- Seeded randomness for reproducible outputs
- Canvas export to PNG

**Assets**:
- `algorithmic-art/templates/generator_template.js` — Starter sketch
- `algorithmic-art/templates/viewer.html` — Browser preview

### 2. Slack GIF Creator

**Skill**: [slack-gif-creator](../slack-gif-creator/SKILL.md)

Build optimized animated GIFs for Slack and web use. Includes a Python pipeline with easing functions, frame composition, and GIF assembly with file-size optimization.

**Key capabilities**:
- Frame-by-frame composition with programmatic control
- Easing functions (ease-in, ease-out, bounce, elastic)
- GIF optimization for Slack's 500KB limit
- Color palette reduction and dithering
- Validation for dimensions and file size

**Assets**:
- `slack-gif-creator/core/gif_builder.py` — Main GIF assembly
- `slack-gif-creator/core/frame_composer.py` — Frame generation
- `slack-gif-creator/core/easing.py` — Easing functions library
- `slack-gif-creator/core/validators.py` — Output validation

## Combining the Skills

For animated generative art:
1. Use **algorithmic-art** to design the visual algorithm in p5.js
2. Export individual frames (vary a parameter across frames)
3. Use **slack-gif-creator** to compose frames into an optimized GIF

For static generative art:
1. Use **algorithmic-art** directly — design, iterate, export PNG

## Module Checklist

- [ ] Visual concept defined (pattern type, color palette, dimensions)
- [ ] Algorithm produces consistent output with seed control
- [ ] Output reviewed for visual quality and aesthetic intent
- [ ] If animated: frame count and timing validated
- [ ] If animated: file size within target (< 500KB for Slack, < 1MB for web)
- [ ] Final asset exported in correct format and dimensions

## Related Modules

- For brand-aligned generative art: [design-visual](../design-visual/SKILL.md) — apply brand colors and guidelines
- For embedding in web UI: [design-frontend](../design-frontend/SKILL.md) — integrate into React components
- For design tokens and consistency: [design-system](../design-system/SKILL.md)
