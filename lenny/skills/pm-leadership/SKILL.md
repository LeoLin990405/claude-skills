---
name: pm-leadership
description: Leadership workflow - product taste, coaching, AI strategy, organizational design, energy management, career growth, fundraising, and systems thinking
triggers:
  - leadership
  - coaching
  - product taste
  - organizational design
  - org design
  - AI strategy
  - LLM
  - energy management
  - fundraising
  - pivoting
  - imposter syndrome
  - productivity
  - vibe coding
  - dogfooding
  - career growth
---

# PM Leadership: Think Bigger, Lead Better

Leadership is about making the right decisions under uncertainty, developing others, and maintaining the judgment and energy to do it sustainably. This module covers senior PM skills, AI strategy, and personal effectiveness.

## When to Use This Module

- Developing product intuition and taste
- Coaching other PMs or new managers
- Building AI/LLM strategy for your product
- Designing organizational structure
- Managing your energy and career growth
- Preparing for fundraising or pivoting

## Skills

### Product Craft

#### 1. Developing Product Taste

**Context**: Taste is pattern recognition refined by experience. It's knowing what "good" feels like before you can articulate why.

**Framework — Building Taste**:
1. **Study great products**: Use 50+ products deeply. Note what delights and what frustrates.
2. **Study failures**: Why did products fail? What signals were missed?
3. **Ship and learn**: Taste improves with reps. Ship, measure, reflect.
4. **Cross-pollinate**: Borrow patterns from non-tech fields (architecture, restaurant design, game design)
5. **Develop strong opinions, loosely held**: Have a point of view, but update it with data

**Taste Tests**:
- Can you identify what makes a product feel "right" vs "off"?
- Can you predict which features will be used and which won't?
- Can you simplify a complex feature while retaining its value?

#### 2. Dogfooding

**Context**: Using your own product is the fastest way to find friction. If you don't use it daily, your judgment is secondhand.

**Framework**:
1. Use the product for real tasks (not just testing)
2. Note every moment of friction, confusion, or delight
3. File bugs and improvement ideas immediately (don't rely on memory)
4. Share findings in a team channel — make dogfooding a team sport
5. Prioritize fixes for the most embarrassing issues

#### 3. Vibe Coding

**Context**: Using AI tools (Claude, Copilot, Cursor) to prototype and validate ideas at the speed of thought.

**Framework**:
1. Start with the user problem, not the technology
2. Prototype in hours, not weeks — AI accelerates the build-measure-learn loop
3. Test the prototype with real users before investing in production code
4. Know the limits: AI-generated code needs review for security, edge cases, and maintainability
5. PMs who can prototype have a superpower — they can validate without waiting for eng cycles

### AI & Technology Strategy

#### 4. AI Product Strategy

**Context**: AI is reshaping every product category. PMs need a framework for when and how to apply AI.

**Framework — AI Opportunity Assessment**:
1. **User need**: What task is tedious, repetitive, or requires expertise users don't have?
2. **Data advantage**: Do you have unique data that makes your AI better than generic solutions?
3. **Error tolerance**: What's the cost of AI being wrong? (low for suggestions, high for medical/financial)
4. **Evaluation**: Can you measure quality automatically? If not, AI is hard to improve.
5. **Build vs integrate**: Use APIs for commoditized AI (transcription, summarization). Build models for core differentiators.

#### 5. Building with LLMs

**Framework**:
1. **Start with prompts**: Before fine-tuning, see how far prompting gets you
2. **Eval-driven development**: Build evals before building features (see [pm-analytics](../pm-analytics/SKILL.md))
3. **Design for uncertainty**: LLM outputs are probabilistic — build UX that handles variability
4. **Guardrails**: Content filtering, output validation, fallback to deterministic logic
5. **Cost optimization**: Cache, batch, use smaller models where quality allows
6. **Stay current**: Model capabilities change quarterly — reassess what's possible regularly

#### 6. Evaluating New Technology

**Framework — Technology Adoption Checklist**:
1. Does this solve a real user problem better than current solution?
2. Is the technology mature enough for production? (or just demo-ready?)
3. What's the switching cost if it doesn't work?
4. Do we have the team to build and maintain it?
5. What's our unfair advantage using this tech? (if everyone can use it, it's table stakes)

#### 7. Platform Strategy

**Framework**:
1. **Platform = infrastructure others build on**: APIs, SDKs, marketplaces
2. **When to platform**: When your ecosystem creates more value than you can alone
3. **Platform incentives**: Make it easier to build on you than to build alone
4. **Governance**: Rules for what partners can/can't do (protect users, maintain quality)
5. **Metrics**: Number of active developers, API calls, ecosystem GMV

### People & Organization

#### 8. Coaching Product Managers

**Framework — GROW Model**:
1. **Goal**: What do they want to achieve?
2. **Reality**: Where are they now? What's the gap?
3. **Options**: What could they do? (let them generate options, don't prescribe)
4. **Will**: What will they commit to doing? By when?

**Coaching Principles**:
- Ask questions more than give answers
- Focus on frameworks they can reuse, not solutions to one problem
- Give feedback on decisions, not just outcomes (good decision + bad outcome ≠ bad decision)
- Match challenge level to growth edge — stretch, don't break

#### 9. Organizational Design

**Context**: How you structure teams determines what products you can build. Conway's Law is real.

**Framework**:
1. **Team topology**: Align teams to user problems, not technical layers
2. **Two-pizza teams**: 5-8 people who own a clear outcome
3. **Clear ownership**: Every metric and surface has exactly one team responsible
4. **Interface contracts**: Teams interact through APIs, docs, and review processes — not ad hoc
5. **Reorg criteria**: Reorg when teams are consistently blocked by other teams, not for new leader preference

#### 10. Energy Management

**Context**: Productivity is a function of energy, not time. Manage energy and time follows.

**Framework — Energy Audit**:
1. **Track for 1 week**: Rate your energy (1-5) every 2 hours. Note what you're doing.
2. **Identify**: What gives energy? What drains it?
3. **Restructure**: Put high-judgment work in high-energy periods. Admin in low-energy periods.
4. **Protect**: Block focus time. Say no to meetings that don't need you.
5. **Recover**: Sleep, exercise, and breaks aren't optional — they're infrastructure.

### Career & Growth

#### 11. Startup Ideation

**Framework**:
1. Start with problems you've personally experienced
2. Validate demand before building (pre-sell, waitlists, landing page tests)
3. Look for broken markets: high prices, terrible UX, regulatory change
4. Talk to 50 potential customers before writing a line of code
5. Founder-market fit: Why are you uniquely qualified to solve this?

#### 12. Managing Imposter Syndrome

**Framework**:
1. **Recognize**: Everyone has it. Senior leaders just manage it better.
2. **Evidence journal**: Keep a log of wins, positive feedback, and completed challenges
3. **Reframe**: "I don't know everything" → "I'm learning and growing"
4. **Talk about it**: Normalize with peers. You'll find you're not alone.
5. **Action bias**: Imposter syndrome paralyzes. Counter it by doing, not thinking.

#### 13. Personal Productivity

**Framework — PM Productivity Stack**:
1. **Weekly planning**: Sunday evening, plan the 3 most important things for the week
2. **Daily top 3**: Each morning, identify the 3 things that must get done today
3. **Time blocking**: Calendar = your resource allocation. If it's not blocked, it doesn't happen.
4. **Batch communications**: Check email/Slack 3x per day, not continuously
5. **Weekly review**: Friday afternoon, review what got done, what didn't, and why

#### 14. Organizational Transformation

**Context**: Changing how an org works is harder than changing what it builds.

**Framework**:
1. **Burning platform**: People change when the cost of not changing exceeds the cost of changing
2. **Coalition**: Build a group of influential supporters before announcing
3. **Quick wins**: Deliver visible results in 30-60 days to build momentum
4. **Sustain**: New processes need 3-6 months of active reinforcement before they stick
5. **Measure**: Define what "transformed" looks like in metrics, not feelings

### Startup Leadership

#### 15. Fundraising Strategy

**Framework**:
1. **Timing**: Raise when you have momentum (metrics up, not when you're desperate)
2. **Materials**: Deck (10-15 slides), data room, financial model
3. **Targeting**: 50-80 investors, prioritize by stage fit and sector expertise
4. **Process**: Run a tight process (3-4 weeks), create urgency through parallel conversations
5. **Terms**: Optimize for valuation AND investor quality (board member, network, brand)

#### 16. Startup Pivoting

**Framework — Pivot Decision**:
1. **Evidence**: PMF signals absent after 6-12 months of focused effort
2. **Partial pivot**: Change the solution, keep the problem (most common)
3. **Full pivot**: Change the problem and the solution (rare, high risk)
4. **Pivot ≠ give up**: Pivoting is redirecting, not failing
5. **Speed**: Once you decide to pivot, move fast. Lingering between old and new is the worst position.

## Module Checklist

- [ ] Product taste: using 10+ competing/adjacent products regularly
- [ ] AI strategy documented (build/buy/integrate decisions)
- [ ] 1:1 coaching framework in use with direct reports
- [ ] Energy audit completed, calendar restructured
- [ ] Weekly planning ritual established

## Related Modules

- For team building: [pm-team](../pm-team/SKILL.md)
- For strategy: [pm-strategy](../pm-strategy/SKILL.md)
- For communication: [pm-communication](../pm-communication/SKILL.md)
