---
name: pm-discovery
description: Problem discovery workflow - user research, competitive analysis, problem definition, and Jobs-to-Be-Done
triggers:
  - user research
  - user interview
  - competitive analysis
  - problem definition
  - discovery
  - survey
  - usability testing
  - jobs to be done
  - JTBD
  - working backwards
---

# PM Discovery: Find the Right Problem

Discovery is about building conviction that you're solving a real problem for real people. Skip this and you risk building something nobody wants.

## When to Use This Module

- Starting a new product or feature
- Validating assumptions before committing resources
- Exploring a new market or user segment
- Investigating why a metric is underperforming
- Re-evaluating product direction after a miss

## Workflow Overview

```
1. Define the Problem Space → 2. Research Users → 3. Map the Landscape → 4. Synthesize → 5. Validate
```

## Skills

### 1. Problem Definition

**Context**: Before any research, articulate what you're trying to learn and why it matters.

**Framework — Problem Statement Canvas**:
1. **Who** has this problem? (specific user segment, not "everyone")
2. **What** is the current pain? (observable behavior, not assumed frustration)
3. **When/where** does it occur? (context and frequency)
4. **Why** does it matter now? (market timing, business impact)
5. **How** do they solve it today? (existing workarounds = proof of pain)

**Anti-patterns**:
- Defining the problem as the absence of your solution ("users need a dashboard")
- Too broad ("improve user experience")
- Skipping straight to solutions

**Signals of success**: You can explain the problem to a stranger in 30 seconds and they say "yes, I have that problem too."

### 2. Conducting User Interviews

**Context**: Interviews uncover motivations, workflows, and pain points that surveys miss.

**Framework — The Mom Test** (Rob Fitzpatrick):
1. Ask about their life, not your idea
2. Ask about specifics in the past, not hypotheticals about the future
3. Talk less, listen more — aim for 80/20 listen/talk ratio
4. Ask "tell me about the last time you..." not "would you use...?"
5. Follow the emotion — when they get animated, dig deeper

**Process**:
1. Recruit 5-8 participants per segment (diminishing returns after 8)
2. Prepare a guide, not a script — see [user-interview-script template](../../templates/user-interview-script.md)
3. Record with permission; take notes on observations, not just words
4. Debrief within 24 hours while context is fresh
5. Synthesize patterns across interviews, not individual anecdotes

**Anti-patterns**:
- Leading questions ("Don't you think X would be better?")
- Asking people to predict their future behavior
- Only interviewing power users

### 3. Designing Surveys

**Context**: Surveys validate at scale what interviews surface qualitatively.

**Framework — Survey Design Checklist**:
1. Start with your hypothesis — what decision will this data inform?
2. Keep it under 5 minutes (12-15 questions max)
3. Use closed-ended questions for measurement, open-ended for discovery
4. Randomize answer order to reduce bias
5. Pilot with 5 people before full launch
6. Target sample size: 100+ for directional, 400+ for statistical significance

**Question Types by Purpose**:
- **Segmentation**: Role, company size, frequency of use
- **Severity**: "How disappointed would you be if you could no longer use X?" (Sean Ellis PMF test)
- **Priority**: Force-rank features or problems (MaxDiff preferred over rating scales)
- **Satisfaction**: CSAT, NPS, or CES depending on what you're measuring

### 4. Usability Testing

**Context**: Watch real users attempt real tasks. What they do matters more than what they say.

**Framework — 5-Second Test + Task Completion**:
1. **5-second test**: Show the screen for 5 seconds, ask what they remember → tests clarity
2. **Task completion**: Give specific tasks ("find the billing page and update your plan") → tests usability
3. **Think-aloud protocol**: Ask them to narrate their thought process as they navigate
4. Measure: task success rate, time on task, error rate, satisfaction
5. Test with 5 users — catches ~85% of usability issues (Nielsen)

**Anti-patterns**:
- Helping them when they get stuck ("oh, you just click here")
- Testing with colleagues instead of real users
- Only testing the happy path

### 5. Competitive Analysis

**Context**: Understanding the landscape helps you find gaps and avoid building table-stakes features.

**Framework — Four Lenses of Competition**:
1. **Direct competitors**: Same solution, same market
2. **Indirect competitors**: Different solution, same problem
3. **Substitutes**: Workarounds users cobble together (spreadsheets, emails, manual processes)
4. **Potential entrants**: Adjacent players who could move into your space

**Process**:
1. Map competitors on a 2x2 (pick the two axes that matter most for your market)
2. Build a feature comparison matrix — see [competitive-analysis template](../../templates/competitive-analysis.md)
3. Identify positioning gaps (where no competitor is strong)
4. Analyze their go-to-market, not just features (pricing, distribution, brand)
5. Update quarterly — competitive landscape changes fast

### 6. Analyzing User Feedback

**Context**: You're drowning in feedback from support tickets, reviews, social media, and sales calls. Turn noise into signal.

**Framework — Feedback Taxonomy**:
1. **Collect**: Aggregate all sources into one place (spreadsheet, Productboard, etc.)
2. **Tag**: Categorize by theme, user segment, and severity
3. **Quantify**: Count frequency per theme — the loudest voice isn't always the biggest problem
4. **Prioritize**: Cross-reference with business metrics (retention impact, revenue impact)
5. **Close the loop**: Tell users what you did with their feedback

**Anti-patterns**:
- Building features for the loudest customer
- Treating all feedback as equally important
- Never closing the loop

### 7. Working Backwards (Amazon Method)

**Context**: Start from the customer experience and work backward to requirements.

**Framework — Press Release / FAQ**:
1. Write a mock press release announcing the finished product (1 page max)
2. Include: headline, subheadline, problem summary, solution summary, customer quote, CTA
3. Write an FAQ section answering: Who is this for? What does it cost? How is it different?
4. If you can't write a compelling press release, the product vision isn't clear enough
5. Use this document as the north star through development

## Discovery Sprint (5-Day Process)

For time-boxed discovery on a specific problem:

| Day | Activity | Output |
|-----|----------|--------|
| Mon | Problem framing + stakeholder interviews | Problem Statement Canvas |
| Tue | User interviews (4-6) | Interview synthesis notes |
| Wed | Competitive analysis + market sizing | Landscape map + TAM estimate |
| Thu | Solution brainstorm + concept testing | 2-3 concepts with user feedback |
| Fri | Synthesis + recommendation | Go/no-go recommendation with evidence |

## Module Checklist

- [ ] Problem statement written and reviewed by team
- [ ] 5+ user interviews conducted and synthesized
- [ ] Competitive landscape mapped (direct + indirect + substitutes)
- [ ] Key user segments identified and prioritized
- [ ] Go/no-go decision made with evidence

## Related Modules

- Next step: [pm-strategy](../pm-strategy/SKILL.md) — turn validated problems into vision and roadmap
- For quantitative validation: [pm-analytics](../pm-analytics/SKILL.md)
- For growth-specific research: [pm-growth](../pm-growth/SKILL.md)
