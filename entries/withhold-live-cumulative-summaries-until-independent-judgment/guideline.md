---
id: withhold-live-cumulative-summaries-until-independent-judgment
title: Withhold live cumulative summaries until independent judgments are complete
bibliography: references.bib
description: For sequential judgment workflows in social visualization systems, avoid
  live cumulative annotations on chart views to prevent information cascades and mitigate
  first-response bias for viewers making objective estimates.
labels:
- purpose:refine
- basis:empirical
- time:ordered-time
- quality:fidelity
- lever:interaction-access
- component:annotation:avoid
- communication:workflow
---

## Withhold live cumulative summaries <!-- role: advice -->

Withhold live cumulative summaries until viewers have made their own judgment. For example, do not let person n+1 see the running histogram built from people 1 through n while estimating a proportion or a linear association.

## Why early exposure creates cascades <!-- role: reason -->

Once early answers are visible, they become the seed that later viewers can follow. In this study, even a small visible seed could shape later judgments.

**Mechanism:** Sequentially visible summaries create an information cascade. The first visible answers establish a direction that later readers reuse, so error can propagate through the sequence.

**Evidence:** In the iterated experiment, the shown histogram mean strongly influenced the next person's answer. Initial conditions affected later judgments, while the number of prior responses n was not significant, so a summary based on a few people influenced later viewers about as much as one based on many [@hullmanImpactSocialInformation2011].

**Notes:** Low sample counts are not a safe threshold by themselves.

## Use when judgments arrive one person at a time <!-- role: context -->

- **User Goal:** Gather many individual judgments without earlier answers biasing later ones.
- **Task:** Objective estimation answered sequentially.
- **Data:** Quantitative values with responses submitted over time.
- **Chart Setting:** A live social interface updates a visible histogram or similar aggregate as new answers arrive.
- **Audience:** Later viewers can see earlier viewers' estimates before submitting their own.
- **Success Criterion:** Stable accuracy regardless of the first few responses.

## Do not use when answers are collected independently first <!-- role: exceptions -->

**Break it when:** Responses are collected independently and the aggregate is revealed only after the individual answer is complete. **Why:** The cascade condition in the study requires person n+1 to see the judgments from the first n people before answering.

## Tradeoffs of delaying the summary <!-- role: costs -->

**Sacrifice:** You lose live social feedback during the estimation step.
**Risk:** Delaying the summary can reduce the immediate sense of community activity.
**Mitigation:** Reveal the aggregate after independent submission rather than during the judgment itself.

## Common failure mode: trusting small-n summaries <!-- role: mistakes -->

**Mistake:** Leaving the running summary visible because only a few earlier users have contributed. **Why it fails:** The study found that the first visible judgments already set the stage for later answers.

## How to test for an early-seed cascade <!-- role: check -->

**Failure Sign:** Later answers depend on how the first few visible responses were seeded.
**Quick Check:** Seed the same chart with two different early cumulative summaries and compare later judgments.
**Stronger Test:** Compare a live sequential condition against a batch-collected independent condition and inspect whether the live condition inherits the initial seed.

## What to change <!-- role: fix -->

- Stop showing the public cumulative summary until the user has submitted an answer.
- Collect a batch of independent responses before publishing any aggregate.
- Remove the live cumulative summary from the estimation view when independent collection is not possible.
