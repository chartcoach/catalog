---
id: combine-small-pie-slices-into-an-others-category
title: Group small pie slices into an others category
bibliography: references.bib
description: For pie charts with many small slices, use grouped slices on the chart
  to improve readability and mitigate clutter from tiny wedges and many labels for
  readers.
labels:
- purpose:refine
- basis:heuristic
- chart:pie-donut
- lever:encoding
- group-cardinality:many
- quality:readability
- polish:declutter
---

## Group tiny wedges into one slice <!-- role: advice -->

Combine several small slices into one larger slice such as "others." For example, group the smallest categories when the pie looks busy and the labels start multiplying.

## Why grouping small slices helps pies <!-- role: reason -->

A pie chart becomes easier to read when the wedges are larger and fewer labels compete for space. Grouping tiny slices cleans up the chart and turns many hard-to-read wedges into one readable segment.

**Mechanism:** The grouped slice reduces the number of tiny wedges and labels, which simplifies the chart's overall look.

**Evidence:** The source recommends grouping slices together in one bigger slice, such as "others," to clean up the chart, and notes that bigger slices are easier to read and require fewer labels [@muth_pie_charts_2018].

## Use when the pie has many tiny slices <!-- role: context -->

- **User Goal:** Clean up a busy pie chart.
- **Data:** One total split into many small categories.
- **Chart Setting:** A pie chart already has several tiny wedges and many labels.
- **Success Criterion:** The chart has fewer labels and larger, easier-to-read slices.

## Do not use when the slices are already easy to read individually <!-- role: exceptions -->

**Break it when:** The slices are already large enough to read and label one by one. **Why:** The cleanup benefit is smaller when tiny wedges are not a problem.

## Tradeoffs of grouping small slices <!-- role: costs -->

**Sacrifice:** You stop showing every small category as its own separate wedge.
**Risk:** Leaving every tiny slice separate keeps the pie cluttered.
**Mitigation:** Combine only the smaller slices into one grouped slice such as "others."

## Common clutter mistake in pies <!-- role: mistakes -->

**Mistake:** Keeping many tiny slices separate in the pie chart. **Why it fails:** The chart stays cluttered and harder to read.

## Check whether the pie needs grouping <!-- role: check -->

**Failure Sign:** The pie has many tiny wedges and a long set of labels.
**Quick Check:** Look for several slices that are so small they mainly add clutter.
**Stronger Test:** Compare the current pie with a version that groups the smallest slices into "others" and keep the cleaner draft.

## Fix a cluttered pie chart <!-- role: fix -->

- Identify the smallest slices in the pie chart.
- Combine those small slices into one larger slice labeled "others."
- Recheck the chart and keep the grouped version if it produces larger slices and fewer labels.
