---
name: pm-growth
description: Growth workflow - product-market fit, growth loops, pricing, retention, activation, behavioral design, and experimentation
triggers:
  - growth
  - PMF
  - product-market fit
  - growth loops
  - pricing
  - retention
  - engagement
  - activation
  - onboarding
  - A/B test
  - experiment
  - behavioral design
  - marketplace
---

# PM Growth: Grow the Product

Growth is the discipline of systematically increasing the value a product delivers and captures. It starts with PMF and compounds through loops, not one-off campaigns.

## When to Use This Module

- Measuring or validating product-market fit
- Designing growth loops and activation funnels
- Setting pricing strategy
- Improving retention and engagement
- Designing and prioritizing experiments

## Workflow Overview

```
Measure PMF → Design Growth Model → Optimize Activation → Build Loops → Retain → Monetize
```

## Skills

### 1. Measuring Product-Market Fit

**Context**: PMF is not a binary event. It's a spectrum you measure and push toward.

**Framework — Sean Ellis Test**:
- Survey users: "How would you feel if you could no longer use [product]?"
- **Very disappointed** responses:
  - <25% → No PMF. Go back to discovery.
  - 25-40% → Getting close. Double down on what resonates.
  - >40% → PMF achieved. Time to grow.

**Complementary Signals**:
- Organic word-of-mouth (users tell others without prompting)
- Retention curve flattens (cohorts stabilize, not decay to zero)
- Users complain when it's down (they depend on it)
- Pull > push (inbound demand exceeds outbound effort)

**Anti-patterns**:
- Declaring PMF based on vanity metrics (signups, downloads)
- Equating revenue with PMF (enterprise contracts ≠ product love)
- Moving to growth before PMF (scaling a leaky bucket)

### 2. Designing Growth Loops

**Context**: Loops are self-reinforcing cycles where output of one step becomes input to the next. They compound; channels don't.

**Framework — Growth Loop Design**:
1. **Identify the loop**: New user → [gets value] → [shares/creates] → [attracts new user]
2. **Map the steps**: Each step has a conversion rate you can measure and optimize
3. **Find the fuel**: What makes the loop spin faster? (content, invites, SEO, data network effects)
4. **Remove friction**: Every unnecessary step in the loop is a leak

**Common Loop Types**:
| Loop | Example | Fuel |
|------|---------|------|
| Viral | User invites → friend joins → friend invites | Social value |
| Content | User creates → Google indexes → searcher finds → searcher creates | SEO + UGC |
| Paid | Revenue → ad spend → new user → revenue | Unit economics |
| Data network | More users → better product → more users | Data quality |

### 3. Pricing Strategy

**Context**: Pricing is the most underleveraged growth lever. A 1% improvement in pricing yields more than a 1% improvement in acquisition.

**Framework — Pricing Design**:
1. **Value metric**: What unit reflects value delivered? (seats, messages, storage, transactions)
2. **Willingness to pay**: Survey users with Van Westendorp or Gabor-Granger
3. **Competitive anchoring**: Price relative to alternatives, not your costs
4. **Packaging**: 3 tiers is the sweet spot — Starter / Pro / Enterprise
5. **Iteration**: Review pricing annually. Most startups underprice.

**Pricing Principles**:
- Charge for value, not features
- Free plans should be a growth loop input, not charity
- Usage-based pricing aligns incentives (you grow when they grow)
- Annual discounts improve cash flow and reduce churn

### 4. Retention & Engagement

**Context**: Retention is the foundation of all growth. No loop works if users don't come back.

**Framework — Retention Analysis**:
1. **Define your retention event**: What action = "active"? (not just login)
2. **Cohort analysis**: Group users by signup week, plot % active over time
3. **Find the magic number**: What behavior in week 1 predicts long-term retention? (e.g., "users who create 3+ documents in week 1 retain at 2x")
4. **Build habits**: Use the Hook Model (Trigger → Action → Variable Reward → Investment)
5. **Reactivation**: For churned users, identify the trigger that brings them back

**Retention Benchmarks** (monthly):
- Consumer social: 25%+ good, 50%+ great
- Consumer SaaS: 40%+ good, 60%+ great
- B2B SaaS: 60%+ good, 80%+ great

### 5. User Onboarding

**Context**: Activation is the steepest drop in the funnel. Most products lose 60-80% of users before they experience core value.

**Framework — Time to Value (TTV)**:
1. Define the "aha moment" — the first time the user gets real value
2. Map every step from signup to aha moment
3. Remove every step that isn't absolutely necessary
4. For necessary steps, make them progressive (don't front-load all setup)
5. Measure: % of signups reaching aha moment within [time window]

**Onboarding Patterns**:
- **Product-led**: Empty states that teach, interactive tutorials, sample data
- **Human-assisted**: Onboarding calls, white-glove setup (high ACV products)
- **Community-led**: Templates, starter kits, community forums

### 6. Behavioral Product Design

**Context**: Products that align with human psychology grow faster. This isn't manipulation — it's reducing friction and increasing value perception.

**Framework — BJ Fogg Behavior Model** (B = MAP):
- **Motivation**: Does the user want to do this? (pain/pleasure, hope/fear, social acceptance)
- **Ability**: Is it easy enough? (time, money, effort, cognitive load)
- **Prompt**: Is there a clear trigger? (notification, visual cue, habit stack)
- All three must be present simultaneously. If behavior isn't happening, diagnose which is missing.

**Design Principles**:
- Reduce cognitive load (fewer choices = more action)
- Show social proof at decision points
- Default to the behavior you want (opt-out > opt-in)
- Celebrate milestones (progress bars, streaks, congratulations)

### 7. Launch Marketing

**Context**: A launch is a growth event, not a PR event. Plan for sustained impact, not a one-day spike.

**Framework — Launch Phases**:
1. **Pre-launch** (4 weeks): Build waitlist, seed content, brief press
2. **Launch week**: Product Hunt, HN, social, email blast, press hits
3. **Sustain** (4 weeks post): Content marketing, case studies, SEO
4. **Iterate**: Measure CAC from launch activities, double down on winners

**Anti-patterns**:
- All energy on launch day, nothing after
- Launching before the product is good enough (first impression = lasting impression)
- Not measuring which launch channel drove actual retention (not just signups)

### 8. Marketplace Liquidity Management

**Context**: Two-sided marketplaces have a cold-start problem. Neither side has value without the other.

**Framework — Marketplace Growth Playbook**:
1. **Pick a side**: Start by subsidizing supply or demand (usually supply)
2. **Geo-concentrate**: Launch in one city/market until it works, then expand
3. **Constrain to create liquidity**: Narrow the market until supply/demand ratio feels abundant
4. **Cross-side network effects**: More supply → better matches → more demand → more supply
5. **Measure liquidity**: Search-to-fill rate, time-to-match, utilization rate

## Experimentation Framework

### Designing Experiments

1. **Hypothesis**: "If we [change], then [metric] will [improve by X%] because [reason]"
2. **Metrics**: Primary metric + guardrail metrics (make sure you don't break something else)
3. **Sample size**: Calculate power analysis before running (avoid peeking)
4. **Duration**: Run for full business cycles (min 1 week for B2C, 2 weeks for B2B)
5. **Decision criteria**: Pre-commit — "We ship if primary metric improves ≥X% with p<0.05"

### Experiment Prioritization (ICE)

- **Impact**: How much will this move the metric? (1-10)
- **Confidence**: How sure are you it will work? (1-10)
- **Ease**: How fast can you run it? (1-10)
- Score = I × C × E. Run highest-scoring experiments first.

## Module Checklist

- [ ] PMF measured (Sean Ellis test or retention curve)
- [ ] Primary growth loop identified and mapped
- [ ] Activation funnel measured (signup → aha moment conversion)
- [ ] Retention cohorts analyzed
- [ ] Pricing reviewed against value delivered
- [ ] Experiment backlog prioritized with ICE

## Related Modules

- For discovery pre-PMF: [pm-discovery](../pm-discovery/SKILL.md)
- For metrics and dashboards: [pm-analytics](../pm-analytics/SKILL.md)
- For launch execution: [pm-execution](../pm-execution/SKILL.md)
