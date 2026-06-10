---
id: prefer-vertically-stacked-small-multiples-over-superposed-bars-for-set-comparisons
title: Prefer vertically stacked small multiples over superposed bars for set comparisons
bibliography: references.bib
description: For grouped set comparison under brief viewing, prefer vertically stacked
  layout structure on static bar charts to improve fidelity and mitigate low-precision
  overlap-based judgments for viewers comparing overall mean or range.
labels:
- purpose:select
- basis:empirical
- task:compare
- chart:bar
- structure:small-multiples:use
- structure:single-view:avoid
- quality:fidelity:use
- lever:layout-structure
---

## Use stacked panels for set comparison <!-- role: advice -->

Choose a vertically stacked small-multiple arrangement when a bar chart must compare two sets by their overall mean or range. For example, place the two bar-chart sets in separate stacked panels instead of overlaying both sets in one shared chart space distinguished by color.

## Why stacked panels work better here <!-- role: reason -->

Set-level comparisons are more precise when each dataset is visually separated into its own panel instead of competing inside one shared chart space. In the tested bar charts, the stacked arrangement preserved comparable bar lengths while avoiding the lower-precision reading produced by the superposed arrangement.

**Mechanism:** Separating the two sets into stacked panels supports whole-set comparison, while overlaying both sets in one chart space makes the comparison depend on a less precise shared-space readout.

**Evidence:** A graphical-perception review records this study as ranking the stacked bar arrangement above the superposed arrangement for aggregate comparison by JND, with a significant pairwise advantage, and it records the same stacked-to-superposed ordering for determine-range in the extracted results [@zengReviewCollationGraphical2023; @jardinePerceptualProxiesVisual2020].

**Notes:** The extracted evidence is strongest for aggregate comparison. The same ordering was recorded for determine-range, but no pairwise significance was retained in the structured extraction.

## Use when these conditions all hold <!-- role: context -->

- **User Goal:** Decide which of two value sets is larger overall.
- **Task:** Compare set mean or compare set range.
- **Data:** Two quantitative sets shown as bars.
- **Chart Setting:** Static bar charts with an arrangement choice between separated panels and one shared chart space.
- **Success Criterion:** More precise judgments when the between-set difference is small.

## Do not use when these conditions hold <!-- role: exceptions -->

**Break it when:** The reader must compare item-to-item changes rather than whole-set summaries. **Why:** The paper explicitly states that other comparison tasks showed different best arrangements, so the stacked choice should not be treated as a universal comparison layout.

## Tradeoffs of stacked panels <!-- role: costs -->

**Sacrifice:** You give up the single shared chart space of an overlay.
**Risk:** If one chart must serve several different comparison tasks, optimizing the layout for mean or range judgments can hurt other tasks.
**Mitigation:** Use a task-specific view, or separate the summary-comparison view from any item-level comparison view.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Overlay both bar sets in one chart space for mean or range comparison. **Why it fails:** The superposed arrangement was the lowest-ranked option in the extracted JND ordering for both tasks.

## How to check the layout choice <!-- role: check -->

**Failure Sign:** Reviewers can only answer correctly when the difference between the two sets is made obviously large in the overlaid version.
**Quick Check:** Make a stacked and a superposed version with the same data and compare which version still supports the correct set choice after only a brief look.
**Stronger Test:** Reduce the between-set difference and keep the arrangement that still supports correct judgments at the smaller difference.

## What to change <!-- role: fix -->

- Move the second dataset out of the shared chart space and into a panel stacked above or below the first.
- Keep both views as matching bar charts rather than encoding the second set as an overlaid series in the same plot.
- If the current overlay was chosen to support another task, create a separate stacked comparison view for mean or range judgments.
