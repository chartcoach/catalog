---
id: include-only-parts-of-the-whole-in-a-stacked-column-chart
title: Include only parts of the whole in a stacked column chart
bibliography: references.bib
description: For part-to-whole composition in stacked column charts, use only component
  parts in the stack to improve fidelity and mitigate double-counting or incomplete
  totals for readers interpreting the whole.
labels:
- purpose:refine
- basis:heuristic
- chart:bar
- operator:part-whole
- quality:fidelity
- lever:encoding
---

## Keep the stack to component parts <!-- role: advice -->

Build each stacked column from the complete set of component parts and nothing else. For example, include every part of the whole in the stack and remove any separate total segment.

## Why the stack must contain only parts <!-- role: reason -->

A stacked column chart represents a whole made from component parts. If a part is missing or the total is added as another segment, the whole no longer reads correctly.

**Mechanism:** Restricting the stack to mutually exclusive parts preserves the part-to-whole meaning of the chart.

**Evidence:** The post says stacked column charts should include all parts of the total and only parts of the total, and explicitly says not to include the total in the chart [@muth_stacked_columns_2018].

## Use when the chart is showing a whole and its parts <!-- role: context -->

- **User Goal:** Show how each total is composed.
- **Task:** Preserve a correct part-to-whole structure.
- **Data:** Components that sum to a whole.
- **Chart Setting:** A stacked column chart is already being used.
- **Audience:** Readers should be able to trust that each stack represents one full whole.
- **Success Criterion:** Each column is made only from the full set of parts.

## Do not use when one value is a total rather than a part <!-- role: exceptions -->

**Break it when:** One of the values is the total itself rather than a component part. **Why:** The total does not belong as another stacked segment.

## What you give up <!-- role: costs -->

**Sacrifice:** You give up showing the total as an internal segment of the stack.
**Risk:** Leaving out a part or adding the total breaks the logic of the whole.
**Mitigation:** Keep the stack limited to the component categories that make up the total.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Plotting the total alongside its parts in the same stacked column. **Why it fails:** The whole gets counted again inside itself.

## Test the part-to-whole structure <!-- role: check -->

**Failure Sign:** A segment is labeled as the total or sum.
**Quick Check:** Add the segments in a column; if they already equal the whole, the total must not appear as another segment.
**Stronger Test:** Verify that each segment is a distinct part of the same total and that no component is missing.

## Revise the design <!-- role: fix -->

- Remove any total segment from the stack.
- Add any missing component parts needed to complete the whole.
- Keep each stacked segment as one part of the total and nothing more.
