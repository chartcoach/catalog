---
id: anchor-date-specific-annotations-to-single-data-points
title: Anchor date-specific annotations to single data points
bibliography: references.bib
description: For date-specific context over ordered time, use single-datum text annotation
  on annotated line charts to improve insight and address ambiguous message-to-mark
  mapping for readers scanning historical events.
labels:
- purpose:refine
- basis:empirical
- time:ordered-time
- chart:line
- lever:text-annotation
- component:annotation:use
- quality:insight
---

## Single-point annotation anchors <!-- role: advice -->

Anchor a context annotation to one exact data point when the message refers to a specific dated event or observation. For example, point the callout to one date on a line graph rather than placing the same message as a region note or a whole-view caption.

## Why single-point annotation anchors work <!-- role: reason -->

A single-point anchor tells the reader exactly which observation the note explains. This reduces ambiguity about what date or value the text refers to.

**Mechanism:** Precise anchoring makes the annotation-to-mark mapping explicit, so the reader does not have to infer which moment in the series the message belongs to.

**Evidence:** In the paper's sample of 136 professional news visualizations, single-datum anchors were the most common annotation scope, appearing more often than group-or-region and entire-view anchors, and this finding directly motivated the system's initial focus on single-point annotations [@hullmanContextifierAutomaticGeneration2013].

**Notes:** Broader anchors still make sense when the message truly applies to a region or the entire view.

## Where single-point annotation anchors apply <!-- role: context -->

- **User Goal:** Connect a specific event or article to one exact point in the plotted history.
- **Data:** Ordered-time observations that can be matched to individual dates or weeks.
- **Chart Setting:** Annotated line graph or similar time-indexed news graphic.
- **Audience:** Readers skimming annotations quickly inside a news interface.
- **Success Criterion:** Each annotation clearly points to one exact observation.

## When single-point annotation anchors fail <!-- role: exceptions -->

**Break it when:** The message summarizes a group of values, a time span, or the entire view. **Why:** Region and whole-view anchors are the appropriate scopes for broader messages.

## Tradeoffs of single-point annotation anchors <!-- role: costs -->

**Sacrifice:** You give up some ability to summarize an interval or the full graphic with one annotation.\
**Risk:** Too many point notes can exceed the available space in the chart.\
**Mitigation:** Reserve broader anchors for messages that actually describe a region or the whole view.

## Common mistakes with single-point annotation anchors <!-- role: mistakes -->

**Mistake:** Placing a date-specific message as a region note or general caption. **Why it fails:** The reader must infer which exact observation the note is meant to explain.

## Check whether single-point annotation anchors are correct <!-- role: check -->

**Failure Sign:** A reader cannot tell which exact date or value an annotation refers to.\
**Quick Check:** Verify that each point-specific callout touches or clearly points to one observation.\
**Stronger Test:** Label each annotation as single datum, group-or-region, or entire view and confirm that the chosen anchor matches the message scope.

## Fix single-point annotation anchors <!-- role: fix -->

- Move the callout so it points to the exact date or mark the message describes.
- Split a mixed broad-and-specific note into separate point annotations when it refers to multiple distinct dates.
- Convert the annotation to a region or whole-view note only when the text truly summarizes that broader scope.
