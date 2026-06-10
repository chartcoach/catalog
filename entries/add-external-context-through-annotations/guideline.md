---
id: add-external-context-through-annotations
title: Add external context through annotations
bibliography: references.bib
description: For contextualizing a news topic, use additive text annotation on a narrative
  visualization to improve insight and address missing external background for readers
  seeking perspective beyond the plotted values.
labels:
- purpose:refine
- basis:empirical
- lever:text-annotation
- component:annotation:use
- communication:context
- quality:insight
---

## Additive context annotations <!-- role: advice -->

Add annotations that introduce external background when the chart's job is to provide context around a news topic. For example, annotate a time point with a related event, historical note, or linked article title instead of only labeling the highest or lowest value already visible in the chart.

## Why additive context annotations work <!-- role: reason -->

Additive annotations change the chart from a display of values into a contextual entry point. They give readers background, perspective, or related events that are not already encoded in the marks.

**Mechanism:** External-information annotations help readers connect the displayed data to relevant events and history instead of forcing them to infer meaning from the line or bars alone.

**Evidence:** In the paper's analysis of 136 professional news visualizations, additive annotations appeared more often than observational annotations, and this prevalence directly informed the system's focus on additive context messages [@hullmanContextifierAutomaticGeneration2013].

**Notes:** Observational annotations still matter when the intent is to highlight comparisons, extremes, or outliers already present in the display.

## Where additive context annotations apply <!-- role: context -->

- **User Goal:** Gain background or perspective beyond the current article.
- **Data:** Plotted values paired with related external text, events, or articles.
- **Chart Setting:** Narrative news visualization with text callouts attached to the visual display.
- **Audience:** Readers consuming online news and seeking added context.
- **Success Criterion:** The annotations add outside information rather than merely restating what the marks already show.

## When additive context annotations fail <!-- role: exceptions -->

**Break it when:** The reader mainly needs help noticing comparisons, extremes, or outliers already visible in the chart. **Why:** Observational annotations are the better fit when the message should come from the visualized data itself.

## Tradeoffs of additive context annotations <!-- role: costs -->

**Sacrifice:** You use annotation space for outside background instead of direct commentary on the chart's own extrema and trends.\
**Risk:** External notes alone can miss visually important turning points in the data.\
**Mitigation:** Pair additive messages with selection that still accounts for visually salient dates or values.

## Common mistakes with additive context annotations <!-- role: mistakes -->

**Mistake:** Using annotations that only restate visible peaks, troughs, or low points when the goal is to add context. **Why it fails:** The chart still lacks the external background the reader came for.

## Check whether additive context annotations are present <!-- role: check -->

**Failure Sign:** The annotations can be fully understood without any information beyond the plotted marks.\
**Quick Check:** Inspect each annotation and ask whether it introduces a related event, perspective, or background fact not already encoded visually.\
**Stronger Test:** Classify annotations as additive versus observational and confirm that the intended context notes are additive.

## Fix additive context annotations <!-- role: fix -->

- Rewrite context notes so they mention related events, history, or perspective external to the plotted values.
- Replace some extrema-only callouts with article-title or event-summary annotations tied to relevant dates.
- Keep observational notes only where the purpose is to highlight a visible comparison or outlier.
