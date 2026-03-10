---
name: design-system
description: Design system module - design tokens, component documentation, cross-skill consistency, and accessibility standards
triggers:
  - design system
  - design tokens
  - component library
  - style guide
  - documentation
  - consistency
  - accessibility
  - WCAG
  - design ops
---

# Design System: Tokens, Standards, and Consistency

A design system is the single source of truth that keeps all design output consistent — across skills, across projects, across time. This module provides the methodology for building and maintaining design systems, from atomic tokens to component documentation.

## When to Use This Module

- Starting a new project that will span multiple design skills
- Establishing design tokens (colors, spacing, typography) shared across artifacts
- Documenting component patterns for reuse
- Auditing existing designs for consistency and accessibility
- Bridging the gap between visual design and frontend implementation

## Workflow Overview

```
1. Audit Current State → 2. Define Tokens → 3. Document Components → 4. Review & Enforce
```

## Skills

This module does not wrap existing sub-skills. It provides the connective methodology that makes all other modules work together.

### 1. Design Token Architecture

Design tokens are the atomic values that feed every other design decision.

**Token Hierarchy**:
```
Global Tokens          → Alias Tokens           → Component Tokens
─────────────           ─────────────            ─────────────────
color.blue.500          color.primary            button.background
space.16                space.md                 card.padding
font.size.16            font.size.body           input.font-size
radius.8                radius.md                badge.border-radius
```

**Defining Tokens**:
1. **Inventory**: List every unique color, size, font, spacing, radius, shadow, and duration in the current design
2. **Normalize**: Group similar values — if you have `#3B82F6` and `#3B83F7`, pick one
3. **Name**: Use a semantic naming convention (purpose-based, not value-based)
4. **Format**: Store tokens in a format consumable by all skills:
   - CSS custom properties for web (theme-factory, frontend-design, web-artifacts-builder)
   - JSON for programmatic use (algorithmic-art, slack-gif-creator)
   - Markdown for documentation (brand-guidelines, style-guide template)

**Template**: Use the [style-guide template](../../templates/style-guide.md) to document tokens.

### 2. Component Documentation

Components are reusable patterns built from tokens.

**Component Spec Format**:
For each component, document:

1. **Purpose**: What this component does and when to use it
2. **Anatomy**: Visual breakdown of constituent parts
3. **Variants**: All supported variations (size, color, state)
4. **States**: Default, hover, focus, active, disabled, error, loading
5. **Tokens Used**: Which design tokens this component consumes
6. **Accessibility**: ARIA roles, keyboard interactions, screen reader behavior
7. **Do / Don't**: Usage guidelines with examples

**Component Maturity Scale**:

| Level | Name | Criteria |
|-------|------|----------|
| 0 | **Concept** | Identified need, no implementation |
| 1 | **Draft** | Single implementation, not reviewed |
| 2 | **Ready** | Reviewed, documented, accessible |
| 3 | **Stable** | Used in 2+ contexts, battle-tested |

### 3. Cross-Skill Consistency

When using multiple design skills in one project, consistency breaks without intentional coordination.

**Consistency Checklist**:
- [ ] Single color palette shared across all outputs (canvas, web, generative)
- [ ] Typography choices are compatible (canvas-design fonts available in web context)
- [ ] Spacing scale is consistent between visual mockups and frontend code
- [ ] Brand guidelines are applied uniformly (if applicable)
- [ ] Motion parameters (easing, duration) match between GIF and web animations

**Integration Points**:

| Skill A | Skill B | What to Align |
|---------|---------|--------------|
| canvas-design | frontend-design | Colors, fonts, spacing |
| algorithmic-art | theme-factory | Color palette, visual density |
| brand-guidelines | all other skills | Full brand constraints |
| slack-gif-creator | theme-factory | Colors, motion easing |
| theme-factory | web-artifacts-builder | CSS custom properties, component styles |

### 4. Accessibility Standards

Every design output should meet minimum accessibility standards.

**WCAG AA Checklist** (applicable across all modules):

**Perceivable**:
- [ ] Text contrast ratio 4.5:1 (normal) / 3:1 (large)
- [ ] Non-text contrast ratio 3:1 (icons, borders, focus rings)
- [ ] Color is never the sole indicator of meaning
- [ ] Images have alt text; decorative images are marked as such

**Operable** (web outputs):
- [ ] All interactive elements reachable via keyboard
- [ ] Focus order matches visual order
- [ ] Focus indicators are visible (not just browser default)
- [ ] No keyboard traps

**Understandable**:
- [ ] Language is clear and concise
- [ ] Error messages explain the problem and suggest a fix
- [ ] Interactive patterns are consistent and predictable

**Robust**:
- [ ] Semantic HTML used (not just divs and spans)
- [ ] ARIA attributes used correctly (and only when needed)
- [ ] Output works across major browsers / screen readers

### 5. Design System Governance

Keeping the system alive requires process.

**Contribution Workflow**:
1. Identify a new pattern or token need
2. Check if existing tokens/components solve it (avoid duplication)
3. If new: propose addition with rationale
4. Review: does it fit the existing system? Is it reusable?
5. Document: add to style guide, update component docs
6. Communicate: inform team of the addition

**Audit Cadence**:
- **Per project**: Run [design-review-checklist](../../templates/design-review-checklist.md) before shipping
- **Quarterly**: Audit token usage — remove unused, consolidate duplicates
- **When adding a skill**: Verify new skill's defaults align with system tokens

## Module Checklist

- [ ] Design tokens defined (colors, typography, spacing, radius, shadows)
- [ ] Tokens documented in [style-guide](../../templates/style-guide.md) format
- [ ] Component patterns documented with variants and states
- [ ] Accessibility standards reviewed (WCAG AA minimum)
- [ ] Cross-skill consistency verified (shared palette, fonts, spacing)
- [ ] Design review process established

## Related Modules

- For visual asset creation: [design-visual](../design-visual/SKILL.md)
- For frontend implementation: [design-frontend](../design-frontend/SKILL.md)
- For generative assets: [design-generative](../design-generative/SKILL.md)
