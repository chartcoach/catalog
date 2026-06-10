---
id: encode-primary-quantity-with-size-for-summary-point-tasks
title: Encode the primary quantitative field with size for grouped summary tasks in
  point plots
bibliography: references.bib
description: For grouped summary tasks, use size encoding for the primary quantitative
  field on categorical point plots to improve fidelity and mitigate weaker group-level
  judgments from position-only encodings for readers comparing maxima or averages
  across categories.
labels:
- purpose:refine
- basis:empirical
- lever:encoding
- channel:area:use
- scope:grouped-result
- reading-mode:overview
- measure:multi
- quality:fidelity
---

## Size the primary quantitative field for group summaries <!-- role: advice -->

Use point size for the primary quantitative field when the job is to judge grouped summaries rather than exact single-point values. For example, in a categorical point plot used to find which group contains the highest value or which group has the larger average, encode the primary quantity with size instead of a positional axis.

## Why size helps with summary reading <!-- role: reason -->

Summary tasks ask readers to judge a set of marks, not decode one exact value at a time. Size supported those grouped judgments well in the tested point plots.

**Mechanism:** Size can support ensemble reading of a group of marks, which helps when readers need to judge maxima or averages across categories.

**Evidence:** For summary tasks, dot plots with the primary quantitative field encoded by size outperformed other dot-plot encodings that used position for that same primary field [@kimAssessingEffectsTask2018].

## Use when the reader must compare groups, not points <!-- role: context -->

- **User Goal:** Decide which category has the highest value or the larger average.
- **Task:** Group-level summary comparison across categories.
- **Data:** One categorical field and a primary quantitative field shown with points.
- **Chart Setting:** A categorical point plot where the primary quantity could be assigned either to size or to position.
- **Success Criterion:** Lower error on summary judgments.

## Do not use when exact point lookup is required <!-- role: exceptions -->

**Break it when:** Readers must read an individual value or compare two specific points exactly. **Why:** Position was the stronger choice for those value tasks.

## What this costs <!-- role: costs -->

**Sacrifice:** Exact value reading of individual marks becomes less direct.
**Risk:** The same chart becomes a poor fit if the task shifts from overview judgment to exact lookup.
**Mitigation:** Keep size for summary views and switch back to position when the task becomes exact point reading.

## Common failure around this move <!-- role: mistakes -->

**Mistake:** Keep the primary quantitative field on position in a categorical point plot that is mainly used for average or maximum judgments. **Why it fails:** The study found that size-based encodings performed better for those summary tasks.

## How to test the choice <!-- role: check -->

**Failure Sign:** Readers struggle more with “which group is larger” or “which group contains the maximum” than with point-level lookup.
**Quick Check:** Compare the current plot against a version that moves the primary quantity from position to size.
**Stronger Test:** Ask one maximum-finding question and one average-comparison question on both versions and keep the lower-error version.

## What to change <!-- role: fix -->

- Move the primary quantitative field from position to size.
- Keep the category on x or y so groups remain easy to identify.
- Reserve this size-based encoding for summary views rather than exact value views.
