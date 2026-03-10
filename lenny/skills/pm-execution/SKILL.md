---
name: pm-execution
description: Build-and-ship workflow - shipping products, managing timelines, decisions, meetings, retros, and cross-functional collaboration
triggers:
  - shipping
  - launch
  - timeline
  - cross-functional
  - collaboration
  - decision
  - meeting
  - retro
  - retrospective
  - post-mortem
  - trade-offs
  - design review
---

# PM Execution: Ship with Quality and Speed

Execution is where strategy meets reality. This module covers the full build-to-launch cycle: decisions, coordination, delivery, and learning from the outcome.

## When to Use This Module

- Kicking off a new project with eng and design
- Managing delivery timelines and dependencies
- Making go/no-go decisions
- Running meetings, retros, or post-mortems
- Resolving cross-functional conflicts

## Workflow Overview

```
Kickoff → Build (decisions + coordination) → QA → Launch → Retro → Learn
```

## Skills

### 1. Shipping Products

**Context**: The #1 job of a PM is to ship. Shipping is a muscle — the more you do it, the better you get.

**Framework — Ship Cadence**:
1. **Define "done"** before starting (launch criteria, not feature list)
2. **Break into milestones**: 1-2 week chunks with demoable output
3. **Daily standups**: 15 min, blockers only — not status updates
4. **Weekly demo**: Show working software to stakeholders
5. **Launch readiness review**: 1 week before launch, run the [launch checklist](../../templates/launch-checklist.md)

**Anti-patterns**:
- "Almost done" for 3 weeks
- No launch criteria defined upfront
- Launching on Friday

### 2. Managing Timelines

**Context**: Timelines slip. Good PMs plan for it.

**Framework — Timeline Management**:
1. Get engineering estimates, then add 30% buffer (first-time features: 50%)
2. Track to milestones, not to final date — early slip detection
3. When behind: cut scope first, extend timeline second, add people never
4. Communicate timeline changes immediately — no surprises
5. Use a shared tracker visible to all stakeholders

### 3. Cross-functional Collaboration

**Context**: PMs don't build anything. They align people who do.

**Framework — RACI for Every Project**:
- **Responsible**: Who does the work?
- **Accountable**: Who makes the final call? (only one person)
- **Consulted**: Who provides input before the decision?
- **Informed**: Who needs to know after the decision?

**Collaboration Rules**:
1. Establish RACI at kickoff — ambiguity causes conflict later
2. Over-communicate at boundaries (PM↔eng, eng↔design, product↔marketing)
3. Write things down — verbal agreements evaporate
4. Resolve conflicts by going back to the user problem and data

### 4. Running Decision Processes

**Context**: The speed and quality of decisions determines the speed and quality of everything else.

**Framework — Decision Velocity**:
1. **Type 1 decisions** (irreversible): Deliberate, get input, document reasoning
2. **Type 2 decisions** (reversible): Decide fast, course-correct later
3. Most decisions are Type 2 — default to speed
4. For Type 1: Use [decision-doc template](../../templates/decision-doc-template.md)
5. Set a decision deadline. No deadline = no decision.

**Decision Meeting Protocol**:
1. Send context doc 24h before (never present the problem for the first time in the meeting)
2. In the meeting: clarify questions (10 min) → debate options (20 min) → decide (5 min)
3. Document: what was decided, who's responsible, by when
4. Send write-up within 1 hour

### 5. Evaluating Trade-offs

**Context**: Every product decision is a trade-off. Make them explicit.

**Framework — Trade-off Matrix**:
1. List the options (usually 2-3)
2. Define criteria (user impact, eng effort, risk, strategic alignment)
3. Weight criteria by importance
4. Score each option
5. Discuss the highest-scored option — does it feel right? If not, examine which criterion is wrong.

**Common PM Trade-offs**:
- Speed vs quality (default: ship smaller with quality)
- Revenue vs user experience (default: UX, unless existential)
- Platform vs product (default: product, unless 3+ teams blocked)
- Build vs buy (default: buy, unless core differentiator)

### 6. Running Effective Meetings

**Context**: Meetings are expensive. A 1-hour meeting with 8 people costs 8 hours of productivity.

**Framework — Meeting Hygiene**:
1. Every meeting has an **owner**, an **agenda**, and a **desired outcome**
2. Default to 25 minutes (not 30) or 50 minutes (not 60) — give people buffer
3. Start with the decision or question, not background (people read faster than you present)
4. End every meeting with: decisions made, action items, owners, deadlines
5. If no agenda → cancel. If no decision needed → make it an email.

**Meeting Types**:
| Type | Purpose | Frequency | Duration |
|------|---------|-----------|----------|
| Standup | Unblock | Daily | 15 min |
| Sprint planning | Align on work | Biweekly | 60 min |
| Design review | Evaluate solutions | As needed | 30 min |
| Decision meeting | Make a call | As needed | 25 min |
| Demo | Show progress | Weekly | 30 min |
| Retro | Learn | End of cycle | 60 min |

### 7. Post-mortems & Retrospectives

**Context**: Retros turn failures into institutional knowledge. Skip them and you repeat mistakes.

**Framework — Blameless Post-mortem**:
1. **Timeline**: What happened, in chronological order (facts only)
2. **Impact**: Who was affected and how much?
3. **Root cause**: 5 Whys analysis until you find the systemic issue
4. **Action items**: Specific, owned, with deadlines — max 3 (more = none get done)
5. **Follow-up**: Review action item completion in 2 weeks

**Template**: See [retro-template](../../templates/retro-template.md)

**Anti-patterns**:
- Blaming individuals (blame the system, not the person)
- Action items without owners
- Never reviewing whether action items were completed

### 8. Planning Under Uncertainty

**Context**: You don't have perfect information. Plan anyway.

**Framework — Scenario Planning**:
1. Identify the 2-3 biggest unknowns
2. Define best case, base case, worst case for each
3. Build plans that work across scenarios (robust) vs plans optimized for one scenario (fragile)
4. Set tripwires: "If X happens by date Y, we switch to plan B"
5. Revisit scenarios monthly — update as you learn

### 9. Running Design Reviews

**Context**: Design reviews align product, design, and engineering on the solution before building.

**Framework**:
1. Designer presents the problem (not the solution) first — 2 min
2. Walk through the user flow — 10 min
3. Feedback round: each reviewer gives feedback on stickies/comments, then discuss — 15 min
4. Distinguish "must fix" from "nice to have" from "personal preference"
5. Decision: ship as-is, iterate, or rethink

### 10. Design Engineering

**Context**: The intersection of design and engineering — where polish and performance meet.

**Principles**:
1. Design and engineering should review together, not in sequence
2. Prototype in code early — static mocks miss interaction details
3. Define the experience budget: load time, animation FPS, interaction latency
4. Invest in design systems to reduce per-feature design cost

## Module Checklist

- [ ] Kickoff complete with RACI defined
- [ ] Milestones set with 2-week check-ins
- [ ] Decision process agreed (who decides what)
- [ ] Launch criteria defined and shared
- [ ] Launch checklist reviewed 1 week before ship
- [ ] Post-launch retro scheduled

## Related Modules

- Previous step: [pm-strategy](../pm-strategy/SKILL.md) — what are we building?
- For growth post-launch: [pm-growth](../pm-growth/SKILL.md)
- For stakeholder communication: [pm-communication](../pm-communication/SKILL.md)
