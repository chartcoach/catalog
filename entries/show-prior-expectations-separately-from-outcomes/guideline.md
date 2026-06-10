---
id: show-prior-expectations-separately-from-outcomes
title: Show prior expectations separately from outcomes
bibliography: references.bib
description: For retrospective evaluation over ordered time, use explicit ex ante
  expectation annotation on temporal charts to improve fidelity and mitigate hindsight
  for reviewers.
labels:
- purpose:refine
- basis:empirical
- time:ordered-time
- data:temporal
- quality:fidelity
- lever:text-annotation
- component:annotation:use
- audience:reviewer
---

## Expectation layer <!-- role: advice -->

Display prior expectations as a separate visible value or series from the realized outcome in retrospective charts. For example, on a timeline or line chart, add the earlier forecast, estimate, or contemporaneous belief next to the final realized value instead of showing only the realized result.

## Why separating expectations from outcomes works <!-- role: reason -->

Once the outcome is known, readers tend to see the past as more predictable than it was. A visible ex ante layer preserves the earlier information state so the chart does not collapse judgment into the final result.

**Mechanism:** Separating what was believed before the event from what actually happened reduces hindsight and supports fairer evaluation of past decisions.

**Evidence:** The source describes hindsight bias as a tendency to exaggerate what was known before, shows that outcome information gets overused when judging decisions after the fact, and argues that this leads to excessive penalties for bad outcomes and insufficient penalties for lucky good outcomes [@camererCurseKnowledgeEconomic1989].

**Notes:** This applies to postmortems, performance evaluation, and any chart used to judge a past choice after its result is known.

## When to use an expectation layer <!-- role: context -->

- **User Goal:** Evaluate a past decision or explain an event after the outcome is already known.
- **Data:** You have both a contemporaneous expectation and the realized outcome.
- **Chart Setting:** The chart is retrospective, such as a postmortem, review, or after-the-fact explanation.
- **Audience:** Reviewers are judging past choices with the benefit of outcome knowledge.
- **Success Criterion:** A reader can identify both what was known before and what actually happened.

## When not to use an expectation layer <!-- role: exceptions -->

**Break it when:** No contemporaneous expectation, forecast, or earlier information state is available to display. **Why:** The guideline depends on separating an ex ante view from the realized outcome.

## Costs of an expectation layer <!-- role: costs -->

**Sacrifice:** You spend chart space on a second displayed value or series.\
**Risk:** If the prior expectation and the outcome are merged back into one summary, hindsight returns.\
**Mitigation:** Keep the prior expectation and the realized outcome as distinct displayed elements.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Showing only the realized outcome in a retrospective chart. **Why it fails:** Readers then judge the past with outcome knowledge alone and infer that the result was more predictable than it was.

## How to test an expectation layer <!-- role: check -->

**Failure Sign:** Reviewers can point to the final outcome but cannot point to what was believed before it occurred.\
**Quick Check:** Ask a reviewer to identify, from the chart alone, both the ex ante expectation and the realized outcome.\
**Stronger Test:** Ask whether the chart lets them judge the earlier decision without collapsing it into the final result.

## What to change <!-- role: fix -->

- Add the earlier forecast, estimate, or prior belief as a separate plotted value or series.
- Add an annotation that marks when that prior expectation was formed.
- Keep the realized outcome as its own distinct displayed element.
- If the chart currently shows only the final result, add a companion expectation layer before using it for retrospective judgment.
