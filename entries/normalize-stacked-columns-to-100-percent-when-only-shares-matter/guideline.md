---
id: normalize-stacked-columns-to-100-percent-when-only-shares-matter
title: Normalize stacked columns to 100% when only shares matter
bibliography: references.bib
description: For part-to-whole comparison in stacked column charts, use percentage
  normalization when relative part size matters more than absolute totals to improve
  readability and mitigate misplaced attention to total height for readers comparing
  shares.
labels:
- purpose:refine
- basis:heuristic
- chart:bar
- operator:part-whole
- measure:multi
- quality:readability
- lever:encoding
---

## Normalize the stack to percentages <!-- role: advice -->

Convert stacked columns to percentages so every column sums to 100% when relative part size matters more than absolute size. For example, normalize the stacks when totals are not of interest, and use the top baseline for the second most important category if that comparison matters.

## Why equal-height totals help share comparison <!-- role: reason -->

When every column has the same height, readers can compare proportions instead of first separating proportion from total size. The normalized chart also creates a second shared edge at the top.

**Mechanism:** Percentage normalization removes total-height variation, which shifts attention to relative part size and adds a top baseline for another important category.

**Evidence:** The post recommends stacking percentages so every total sums to 100% when relative size is more important than absolute size and totals are not of interest, noting that this also creates a second baseline at the top of the chart [@muth_stacked_columns_2018].

**Notes:** The top baseline can help with the second most important category.

## Use when relative size is the point <!-- role: context -->

- **User Goal:** Compare shares across several totals.
- **Task:** Read relative size instead of absolute total size.
- **Data:** Part-to-whole values that can be expressed as percentages.
- **Chart Setting:** A stacked column chart is already chosen.
- **Audience:** Readers should focus on proportions, not on which total is bigger.
- **Success Criterion:** Every column sums to 100% and share comparison becomes easier.

## Do not use when total size matters too <!-- role: exceptions -->

**Break it when:** The absolute size of each total is important to the reader. **Why:** A 100% stack removes that total-size information.

## What you give up <!-- role: costs -->

**Sacrifice:** You give up direct comparison of the total sizes.
**Risk:** Readers cannot tell which total is larger once every column has the same height.
**Mitigation:** Keep raw stacked columns when total magnitude is part of the message.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Normalizing to 100% when the reader needs both the shares and the total sizes. **Why it fails:** The chart makes all totals look equal.

## Test the normalization choice <!-- role: check -->

**Failure Sign:** The chart is meant to compare shares, but readers keep reading total height as if it matters.
**Quick Check:** Ask whether every total should sum to 100%; if yes, normalize the columns.
**Stronger Test:** Check whether the message still works after removing total-size differences; if it does, 100% stacking fits better.

## Revise the design <!-- role: fix -->

- Convert the stacked values to percentages so each column sums to 100%.
- Keep the focus on relative share size rather than total height.
- Place the second most important category at the top if the new top baseline helps that comparison.
