---
id: place-the-most-important-segment-at-the-bottom-of-the-stack
title: Place the most important segment at the bottom of the stack
bibliography: references.bib
description: For part-to-whole comparison in stacked column charts, use stack order
  to place the most important segment on the shared baseline to improve readability
  and mitigate hard comparisons of floating segments for readers comparing one key
  part across totals.
labels:
- purpose:refine
- basis:heuristic
- chart:bar
- operator:part-whole
- quality:readability
- lever:scale-order
---

## Reorder the stack around the shared baseline <!-- role: advice -->

Move the most important segment to the bottom of each stacked column. For example, keep the key category touching the baseline in every column, and use color on that same category if it also needs extra emphasis.

## Why the bottom segment is easiest to compare <!-- role: reason -->

Only the segment that starts from the common baseline can be compared directly across columns. Segments higher in the stack start from different positions and are harder to read against each other.

**Mechanism:** Putting the key segment on the baseline gives it the clearest common reference point across all columns.

**Evidence:** The post recommends bringing the most important value to the bottom of the chart because readers can compare values more easily when they share the same baseline, and pairing that move with color to make the value stand out [@muth_stacked_columns_2018].

## Use when one segment matters most <!-- role: context -->

- **User Goal:** Compare one part across several totals.
- **Task:** Make the main segment easy to compare across columns.
- **Data:** Part-to-whole data already shown as stacked columns.
- **Chart Setting:** One category is more important than the others.
- **Audience:** Readers need to spot the key part quickly.
- **Success Criterion:** The main segment can be compared directly across the columns.

## Do not use when another segment is the real focus <!-- role: exceptions -->

**Break it when:** The segment at the bottom is not the one readers need to compare most. **Why:** The shared baseline would be helping the wrong part.

## What you give up <!-- role: costs -->

**Sacrifice:** You optimize comparison for one segment more than for the others.
**Risk:** Other segments remain harder to compare because they still float above changing baselines.
**Mitigation:** Reserve the bottom position for the segment that carries the main message.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Putting the key segment in the middle or at the top of the stack. **Why it fails:** The segment then starts from different baselines in each column and becomes harder to compare.

## Test the ordering <!-- role: check -->

**Failure Sign:** The category you talk about most does not touch the baseline in every column.
**Quick Check:** Scan the bottoms of all columns; if the key category is not consistently there, reorder the stack.
**Stronger Test:** Compare the key segment across two columns without reading labels; if the start positions differ, it is not on the shared baseline.

## Revise the design <!-- role: fix -->

- Reorder the stacks so the key category starts at zero in every column.
- Keep that same category at the bottom across the whole chart.
- Use color to reinforce the same category after the order change.
