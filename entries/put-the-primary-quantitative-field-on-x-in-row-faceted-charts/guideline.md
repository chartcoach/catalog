---
id: put-the-primary-quantitative-field-on-x-in-row-faceted-charts
title: Put the primary quantitative field on the x-axis in row-faceted charts
bibliography: references.bib
description: For row-faceted point plots, use the x-axis for the primary quantitative
  field to improve readability and mitigate slow, misaligned cross-panel lookups for
  readers comparing values across vertically stacked panels.
labels:
- purpose:refine
- basis:empirical
- structure:small-multiples
- lever:encoding
- component:axis:use
- measure:multi
- quality:readability
---

## Swap the primary value onto the horizontal axis <!-- role: advice -->

Place the primary quantitative field on x rather than y when categories are split into stacked row facets. For example, in a trellis of vertically arranged panels, use a shared horizontal scale for the quantity readers must read or compare instead of forcing separate y-axis lookups in each panel.

## Why the horizontal axis works better in row facets <!-- role: reason -->

Row faceting changes how readers compare values. A shared horizontal axis aligns lookups across panels and avoids the extra burden of reading vertically separated y scales, which can also require scrolling to find the axis.

**Mechanism:** Horizontal alignment across vertically stacked panels makes cross-panel reading easier than repeated y-axis lookups.

**Evidence:** Within row-faceted charts, putting the primary quantitative field on x produced faster completion for read-value and compare-values tasks and better accuracy for find-maximum than putting that same field on y [@kimAssessingEffectsTask2018].

## Use when categories are stacked in rows <!-- role: context -->

- **User Goal:** Read or compare values across multiple faceted categories.
- **Task:** Cross-panel lookup or comparison.
- **Data:** A categorical field split into vertically ordered subplots and a primary quantitative field that can be assigned to either axis.
- **Chart Setting:** Row faceting with shared scales across panels.
- **Success Criterion:** Faster cross-panel reading with fewer errors.

## Do not use outside the tested row-facet condition <!-- role: exceptions -->

**Break it when:** The chart is not faceted into rows. **Why:** The reported advantage comes from vertically stacked panels; the paper does not generalize it to all other layouts.

## What this costs <!-- role: costs -->

**Sacrifice:** Another field must move off x.
**Risk:** A careless swap can protect the primary field but weaken a second task-critical field.
**Mitigation:** Keep the primary field on x and move the less critical field to y or another channel.

## Common failure around this move <!-- role: mistakes -->

**Mistake:** Put the primary quantitative field on y in a row-faceted chart. **Why it fails:** Readers must compare unaligned y lookups across panels and may need to scroll to find the axis.

## How to test the choice <!-- role: check -->

**Failure Sign:** Readers scroll to the bottom to find the scale or struggle to compare values across panels.
**Quick Check:** Compare the current row-faceted chart against the same chart with x and y swapped.
**Stronger Test:** Time one read-value or compare-values question on both versions and keep the faster version if accuracy does not drop.

## What to change <!-- role: fix -->

- Swap x and y so the primary quantitative field uses x.
- Keep the categorical split as row facets.
- Preserve shared horizontal scales across the stacked panels.
