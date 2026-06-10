---
id: place-primary-quantitative-field-on-x-axis-in-row-faceted-point-plots
title: Place the primary quantitative field on the x-axis in row-faceted point plots
bibliography: references.bib
description: For exact lookup and maximum search, prefer x-axis assignment for the
  primary quantitative field on row-faceted point plots to improve fidelity and mitigate
  slow misaligned cross-panel comparisons for readers scanning multiple panels.
labels:
- purpose:refine
- basis:empirical
- quality:fidelity:use
- lever:encoding
- operator:lookup
- reading-mode:exact
- structure:small-multiples
- channel:position:use
---

## Put the primary field on the x-axis across row facets <!-- role: advice -->

Place the primary quantitative field on the x-axis when categories are split into row facets and readers must read values or find maxima. For example, in a row-faceted point plot, swap the primary and secondary quantitative fields so the main field uses the common horizontal axis rather than the y-axis.

## Why x-axis assignment works better in row facets <!-- role: reason -->

The horizontal axis stays aligned across stacked panels, while the y-axis requires harder cross-panel lookups and can force the reader to scroll to the bottom to see the needed scale. That made the x-assigned version faster or more accurate in the studied row-faceted tasks.

**Mechanism:** A shared horizontal scale supports easier panel-to-panel comparison than repeated vertical lookups in stacked facets.

**Evidence:** Within the row-faceted designs, the version with the primary quantitative field on x was faster for read-value and compare-values tasks and more accurate for find-maximum than the transposed version with the primary field on y [@zengReviewCollationGraphical2023; @kimAssessingEffectsTask2018].

**Notes:** This finding was reported for row facets specifically.

## Use when the facet layout is already fixed <!-- role: context -->

- **User Goal:** Read exact values, compare individual values, or find the group containing the maximum value.
- **Task:** Lookup, pairwise comparison, or maximum search.
- **Data:** One categorical field split into row facets plus two quantitative fields.
- **Chart Setting:** A row-faceted point plot is already chosen and the main quantitative field can be assigned to either x or y.
- **Success Criterion:** Faster or more accurate reading across stacked panels.

## Do not generalize beyond the studied facet setup <!-- role: exceptions -->

**Break it when:** The layout is not row-faceted or the task is not one of the studied lookup or maximum tasks. **Why:** The reported advantage was specific to row facets and was not established as a general x-over-y rule for other layouts or tasks.

## What you give up <!-- role: costs -->

**Sacrifice:** The secondary quantitative field must take the y-axis.
**Risk:** Leaving the primary field on y preserves the slower, harder cross-panel lookup pattern.
**Mitigation:** Treat axis assignment as part of the facet design, not as a neutral swap.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Keep the primary quantitative field on the y-axis in stacked row facets when readers must compare across panels. **Why it fails:** The repeated vertical lookups are less aligned and slower than reading from the shared horizontal axis.

## Check the axis assignment directly <!-- role: check -->

**Failure Sign:** Readers must compare y positions across stacked panels or scroll to find the primary scale.
**Quick Check:** Transpose the two quantitative axes and compare one read-value question and one maximum-search question.
**Stronger Test:** Measure time and error for the x-assigned and y-assigned versions on a small set of row-faceted tasks.

## Swap the axes inside the facets <!-- role: fix -->

- Move the primary quantitative field from y to x.
- Move the secondary quantitative field to y.
- Keep the category field on row facets while re-testing the same tasks.
