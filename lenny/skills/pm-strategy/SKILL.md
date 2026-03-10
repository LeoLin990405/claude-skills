---
name: pm-strategy
description: Strategic planning workflow - vision, north star metrics, OKRs, roadmap, PRD, specs, and prioritization frameworks
triggers:
  - product vision
  - north star metric
  - roadmap
  - OKR
  - goals
  - PRD
  - product requirements
  - specs
  - prioritization
  - RICE
  - scoping
  - product strategy
---

# PM Strategy: Define Where to Go and How to Get There

Strategy translates validated problems into a clear plan. It answers: what are we building, why, in what order, and how will we know it worked?

## When to Use This Module

- Defining or refreshing product vision
- Planning quarterly/annual roadmaps
- Writing PRDs for new features
- Setting OKRs and success metrics
- Deciding what to build next (prioritization)

## Workflow Overview

```
Vision → North Star Metric → OKRs → Roadmap → PRD → Specs → Build
```

## Skills

### 1. Defining Product Vision

**Context**: Vision is the destination. Without it, roadmaps become feature shopping lists.

**Framework — Vision Stack**:
1. **Mission**: Why does this product exist? (1 sentence, timeless)
2. **Vision**: What does the world look like if we succeed? (1 paragraph, 3-5 year horizon)
3. **Principles**: What trade-offs do we make? (3-5 opinionated statements: "we choose X over Y")
4. **Current strategy**: How are we getting there this year? (2-3 strategic bets)

**Test**: Can every team member recite the vision unprompted? If not, it's not clear enough.

**Anti-patterns**:
- Vision so generic it could apply to any company
- Changing vision quarterly (that's strategy, not vision)
- Vision without principles = no decision-making framework

### 2. Writing North Star Metrics

**Context**: One metric that captures the core value your product delivers to users.

**Framework — North Star Metric Design**:
1. It measures **value delivered to users**, not revenue (revenue is a lagging indicator)
2. It's a **leading indicator** of business success
3. Every team can influence it
4. It has a **clear unit** and **measurement frequency**

**Examples**:
- Airbnb: Nights booked
- Spotify: Time spent listening
- Slack: Messages sent in channels with 2+ participants
- Notion: Weekly active editors

**Supporting Metrics**: Break the north star into 3-5 input metrics that teams can directly move. Build a metrics tree: North Star → Input Metrics → Team Metrics.

### 3. Setting OKRs & Goals

**Context**: OKRs connect strategy to execution. Objectives say where to go; Key Results say how to measure progress.

**Framework — OKR Writing Rules**:
1. **Objective**: Qualitative, inspiring, time-bound ("Make onboarding effortless for new users in Q2")
2. **Key Results**: 2-4 per objective, quantitative, measurable, ambitious but possible
3. Use "from X to Y" format for KRs ("Increase activation rate from 40% to 60%")
4. 70% completion = healthy ambition. 100% = sandbagging.
5. Weekly check-ins, monthly scoring, quarterly retro

**Template**: See [okr-template](../../templates/okr-template.md)

**Anti-patterns**:
- KRs that are tasks, not outcomes ("Launch feature X" is a task, not a KR)
- Too many OKRs (3 objectives max per team per quarter)
- No scoring cadence — OKRs without check-ins are just wish lists

### 4. Prioritizing Roadmap

**Context**: You will always have more ideas than capacity. Prioritization is the core PM skill.

**Framework Options**:

**RICE** (Reach × Impact × Confidence / Effort):
- Reach: How many users will this affect per quarter?
- Impact: How much will it move the target metric? (3=massive, 2=high, 1=medium, 0.5=low, 0.25=minimal)
- Confidence: How sure are you? (100%=high, 80%=medium, 50%=low)
- Effort: Person-months of work

**ICE** (Impact × Confidence × Ease): Simpler, better for early-stage teams.

**Kano Model** (for feature-type decisions):
- **Must-have**: Absence causes dissatisfaction; presence doesn't delight
- **Performance**: More is better (linear satisfaction)
- **Delighter**: Unexpected features that create disproportionate satisfaction

**Process**:
1. Score all candidates with your chosen framework
2. Stack-rank by score
3. Sanity-check the top 10 with stakeholders — does it feel right?
4. Cut mercilessly — if you have 20 items, you're not prioritized
5. Revisit monthly, not daily

### 5. Writing PRDs

**Context**: The PRD is the contract between product, engineering, and design. It says what to build and why, not how.

**Framework — PRD Sections**:
1. **Problem**: What user problem are we solving? (link to discovery evidence)
2. **Goal**: What metric will move and by how much?
3. **User stories**: As a [user], I want [action], so that [outcome]
4. **Scope**: What's in v1? What's explicitly out?
5. **Design**: Link to mocks/wireframes
6. **Success metrics**: How will we measure success post-launch?
7. **Open questions**: What don't we know yet?
8. **Timeline**: Target dates and milestones

**Template**: See [prd-template](../../templates/prd-template.md)

**Anti-patterns**:
- PRD as spec (describing UI pixel by pixel)
- No success metrics
- PRD written after development starts

### 6. Writing Specs & Designs

**Context**: Specs translate the PRD's "what" into engineering's "how."

**Framework**:
1. **Technical approach**: Architecture decisions, data model changes, API contracts
2. **Edge cases**: What happens when [X fails / user does Y / data is missing]?
3. **Dependencies**: What other teams or systems are involved?
4. **Migration plan**: How do existing users transition?
5. **Rollout plan**: Feature flags, percentage rollout, rollback criteria

### 7. Scoping & Cutting

**Context**: The most underrated PM skill. Shipping 80% of the value in 20% of the time.

**Framework — Scope Cutting Checklist**:
1. For each feature in the PRD, ask: "Would we launch without this?"
2. If yes → cut it to v2
3. Look for the "cupcake" — the smallest thing that delivers the core value
4. Time-box, don't feature-box: "What can we ship in 2 weeks?" beats "When will all 12 features be done?"
5. Cut scope, not quality. Never ship broken; ship less.

**Anti-patterns**:
- "Just one more feature" syndrome
- Cutting quality (tests, error handling) instead of scope
- Not communicating cuts to stakeholders

### 8. Systems Thinking

**Context**: Products exist in systems — users, competitors, markets, internal teams. Understanding second-order effects prevents surprises.

**Framework — Systems Mapping**:
1. Draw the key actors (users, teams, partners, competitors)
2. Draw the flows between them (data, money, value, attention)
3. Identify feedback loops (reinforcing and balancing)
4. Ask: "If we change X, what happens to Y?" for each change
5. Look for leverage points — small changes with outsized impact

## Module Checklist

- [ ] Product vision documented and shared
- [ ] North star metric defined with input metrics tree
- [ ] OKRs set for the quarter (≤3 objectives, 2-4 KRs each)
- [ ] Roadmap prioritized with RICE/ICE scores
- [ ] PRD written and reviewed by eng + design
- [ ] Scope cut to MVP

## Related Modules

- Previous step: [pm-discovery](../pm-discovery/SKILL.md) — validate the problem first
- Next step: [pm-execution](../pm-execution/SKILL.md) — ship what you planned
- Metrics depth: [pm-analytics](../pm-analytics/SKILL.md)
