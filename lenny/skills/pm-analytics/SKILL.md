---
name: pm-analytics
description: Measurement and operations workflow - metrics, financial modeling, data-driven decisions, platform ops, and design systems
triggers:
  - metrics
  - financial model
  - dashboard
  - data-driven
  - analytics
  - KPI
  - unit economics
  - cohort analysis
  - platform
  - design system
  - tech debt
  - product operations
  - AI evaluation
  - evals
---

# PM Analytics: Measure What Matters

Analytics turns intuition into evidence. This module covers metrics design, financial modeling, data-driven decision-making, and the operational infrastructure that keeps products healthy.

## When to Use This Module

- Defining metrics for a new product/feature
- Building financial models or unit economics
- Setting up dashboards and review cadences
- Evaluating technical investments (platform, tech debt)
- Running data-informed product reviews

## Workflow Overview

```
Define Metrics → Build Dashboards → Review Cadence → Financial Model → Platform Health → Iterate
```

## Skills

### 1. Product Operations

**Context**: Product ops builds the systems that make product teams effective — data pipelines, review cadences, tooling, and processes.

**Framework — Product Ops Pillars**:
1. **Data infrastructure**: Ensure teams can self-serve data (event tracking, dashboards, analysis tools)
2. **Review cadence**: Weekly metrics review, monthly business review, quarterly strategy review
3. **Process standardization**: Templates, launch processes, feedback loops
4. **Tooling**: Evaluate and maintain product tools (analytics, A/B testing, feature flags)
5. **Knowledge management**: Document decisions, experiments, learnings

### 2. Metrics Tree Methodology

**Context**: A metrics tree connects your north star to actionable team-level metrics. It's the translation layer between strategy and execution.

**Framework — Building a Metrics Tree**:
1. **North Star** (top): The one metric that captures core value (see [pm-strategy](../pm-strategy/SKILL.md))
2. **Input Metrics** (level 2): 3-5 metrics that mathematically or causally drive the north star
3. **Team Metrics** (level 3): Metrics each team owns and can directly influence
4. **Leading Indicators** (level 4): Early signals that team metrics will move

**Example**:
```
North Star: Weekly Active Users
├── New Users (Acquisition team)
│   ├── Signups
│   └── Signup-to-activation rate
├── Returning Users (Engagement team)
│   ├── D7 retention
│   └── Feature adoption rate
└── Resurrected Users (Lifecycle team)
    ├── Reactivation email CTR
    └── Winback conversion rate
```

**Template**: See [metrics-dashboard](../../templates/metrics-dashboard.md)

### 3. Financial Modeling

**Context**: PMs need financial literacy to make business cases, evaluate pricing, and communicate with leadership.

**Framework — PM Financial Model**:
1. **Revenue model**: How do you make money? (subscription, transaction, ads, marketplace take-rate)
2. **Unit economics**: CAC, LTV, LTV/CAC ratio, payback period, gross margin
3. **Cohort projections**: Revenue by signup cohort over time
4. **Scenario analysis**: Best/base/worst case with key variable sensitivities
5. **TAM/SAM/SOM**: Top-down market sizing + bottom-up reality check

**Key Formulas**:
- LTV = ARPU × (1 / Churn Rate)
- CAC Payback = CAC / (ARPU × Gross Margin)
- LTV/CAC > 3x is healthy
- Rule of 40: Growth Rate + Profit Margin > 40% (SaaS benchmark)

**Template**: See [financial-model-spec](../../templates/financial-model-spec.md)

**For spreadsheet creation**: Use the xlsx skill at `../../office/skills/xlsx/SKILL.md` for formula construction, formatting standards, and Excel best practices.

### 4. Data-Driven Decision Making

**Context**: Data informs decisions; it doesn't make them. Know when to use data and when to use judgment.

**Framework — Data-Decision Spectrum**:
| Signal Strength | Approach |
|----------------|----------|
| Strong data (A/B test, large sample) | Let data decide |
| Moderate data (analytics, surveys) | Data-informed, judgment calls on ties |
| Weak data (anecdotes, small sample) | Use as input, decide on principles |
| No data (new market, novel product) | Conviction + fast iteration |

**Data Review Cadence**:
- **Daily**: Core metrics dashboard (anomaly detection)
- **Weekly**: Team metrics review (progress against OKRs)
- **Monthly**: Business review (revenue, growth, retention cohorts)
- **Quarterly**: Strategy review (are we working on the right things?)

### 5. Technical Roadmaps

**Context**: PMs must balance feature work with technical investment. Ignoring tech debt compounds until it blocks everything.

**Framework — Tech Investment Portfolio**:
1. **Features** (60-70%): User-facing capabilities that drive metrics
2. **Tech debt** (15-20%): Performance, reliability, maintainability improvements
3. **Platform** (10-15%): Shared infrastructure that accelerates future feature work
4. **Exploration** (5-10%): Prototypes, spikes, research

**Tech Debt Prioritization**:
- Prioritize debt that slows down the highest-priority feature work
- Measure in "developer time tax" — how many hours per week does this cost?
- Create a tech debt backlog with estimated ROI (hours saved / hours to fix)

### 6. Managing Tech Debt

**Context**: Tech debt is a business decision, not an engineering failure. Manage it like financial debt — take it on deliberately, pay it down strategically.

**Framework**:
1. **Categorize**: Is it deliberate (speed trade-off) or accidental (unknown at the time)?
2. **Quantify**: How much does it cost per sprint in velocity? In incidents?
3. **Prioritize**: Address debt that blocks upcoming feature work first
4. **Allocate**: Reserve 15-20% of sprint capacity for debt reduction
5. **Track**: Maintain a debt register with interest rate (growing cost over time)

### 7. Platform & Infrastructure

**Context**: When 3+ teams need the same capability, it's time to invest in platform.

**Framework — Platform Decision Matrix**:
- Build platform when: multiple teams blocked, shared pattern emerging, total cost of separate implementations > platform cost
- Don't build platform when: only one team needs it, requirements are too different, premature abstraction

### 8. Design Systems

**Context**: Design systems are a product, not a project. They reduce per-feature cost and improve consistency.

**Framework**:
1. Start with an audit of existing patterns (buttons, forms, typography, colors)
2. Define tokens: spacing, color palette, typography scale
3. Build components: start with the 10 most-used components
4. Document: usage guidelines, do/don't examples
5. Maintain: designate an owner, accept contributions via PR review

### 9. AI Evaluation (Evals)

**Context**: AI products require different measurement. Traditional A/B testing is necessary but not sufficient.

**Framework — Eval Design for AI Products**:
1. **Define quality dimensions**: Accuracy, relevance, safety, latency, cost
2. **Build eval sets**: Curated input/output pairs with human-labeled quality scores
3. **Automate measurement**: Run evals on every model change (CI for models)
4. **Track regression**: Alert when quality drops below threshold
5. **Human-in-the-loop**: Sample outputs for human review at regular intervals

## Module Checklist

- [ ] North star metric defined with input metrics tree
- [ ] Dashboard built with daily/weekly/monthly views
- [ ] Review cadence established
- [ ] Unit economics calculated (CAC, LTV, payback)
- [ ] Tech debt backlog maintained with ROI estimates
- [ ] Data review happening on cadence

## Related Modules

- For metric goal-setting: [pm-strategy](../pm-strategy/SKILL.md)
- For growth metrics: [pm-growth](../pm-growth/SKILL.md)
- For financial spreadsheet execution: xlsx skill at `../../office/skills/xlsx/SKILL.md`
