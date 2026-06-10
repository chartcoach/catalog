---
id: choose-annotations-from-visually-salient-time-points
title: Choose annotations from visually salient time points
bibliography: references.bib
description: For explaining visible movement over ordered time, use visual-saliency-based
  text annotation on stock line charts to improve insight and mitigate callouts that
  miss peaks, troughs, and sharp changes for readers interpreting company performance.
labels:
- purpose:refine
- basis:empirical
- task:trend
- time:ordered-time
- chart:line
- lever:text-annotation
- component:annotation:use
- quality:insight
---

## Visually salient annotation selection <!-- role: advice -->

Choose annotation dates from visually salient points in the time series when the chart must explain trends and oscillations. For example, annotate weeks containing global peaks or troughs and the largest changes in closing price or traded volume, then choose a representative article for each selected week.

## Why visually salient annotation selection works <!-- role: reason -->

Readers naturally attend to sharp turns, extrema, and unusual changes in a line. Putting annotations there makes the text feel explanatory rather than arbitrary.

**Mechanism:** Saliency-based selection places messages where the chart already attracts attention, helping readers connect visible rises, falls, and spikes to explanatory context.

**Evidence:** In the paper's evaluation, visual-saliency-selected annotations were rated significantly better than both random and relevance-only annotations at explaining trends and oscillations in stock performance [@hullmanContextifierAutomaticGeneration2013].

## Where visually salient annotation selection applies <!-- role: context -->

- **User Goal:** Explain trends and oscillations in company stock performance.
- **Data:** Ordered closing-price data with traded-volume data over the same period.
- **Chart Setting:** Annotated stock line chart with callouts attached to specific weeks or dates.
- **Audience:** Readers interpreting what caused visible rises, falls, and spikes.
- **Success Criterion:** Annotations land on visually notable turning points or abrupt changes.

## When visually salient annotation selection fails <!-- role: exceptions -->

**Break it when:** The main goal is topical background around the current article rather than explanation of the visible stock movement. **Why:** Relevance-based selection better optimizes how on-topic the annotations feel.

## Tradeoffs of visually salient annotation selection <!-- role: costs -->

**Sacrifice:** You may give up some topical match to the current article.\
**Risk:** Saliency-only selection can surface visually dramatic weeks that are less relevant to the article being read.\
**Mitigation:** Combine saliency with linguistic relevance when both explanation and topicality matter.

## Common mistakes with visually salient annotation selection <!-- role: mistakes -->

**Mistake:** Choosing articles from visually ordinary weeks while leaving major peaks, troughs, or sharp changes unannotated. **Why it fails:** The annotations do not help explain the movements the reader is already trying to interpret.

## Check whether visually salient annotation selection is working <!-- role: check -->

**Failure Sign:** Large peaks, troughs, or abrupt changes remain unannotated.\
**Quick Check:** Compare annotation locations against the global maxima and minima and the largest absolute changes in price or volume.\
**Stronger Test:** Create a saliency ranking of weeks and verify that the chosen annotations come from the top-ranked weeks.

## Fix visually salient annotation selection <!-- role: fix -->

- Detect global peaks and troughs in closing price and traded volume.
- Compute absolute change from the previous time point for price and volume.
- Aggregate those saliency signals by week and annotate the top-ranked weeks.
- Choose a representative article from each selected week instead of picking arbitrary related articles.
