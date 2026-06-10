---
id: describe-visually-apparent-relationships-in-text
title: Describe visually apparent relationships in text
bibliography: references.bib
description: For interpretation of chart-level findings, use text annotation on charts
  with visually apparent trends, clusters, patterns, outliers, or significant statistical
  findings to improve accessibility and mitigate purely visual inference for screen-reader
  users.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:text-annotation
- component:annotation:use
- needs:screen-reader
- access:screen-reader:use
- reading-mode:overview
---

## Describe apparent relationships in text <!-- role: advice -->

Add text that explicitly names visually apparent relationships and findings instead of leaving them only in the marks. For example, add a chart-level summary that states a trend, cluster, pattern, or outlier, and add a text callout for a statistically or visually important region so the same finding is available to screen readers.

## Why relationship text reduces inference work <!-- role: reason -->

High-level chart meaning often lives in relationships between marks rather than in any single value. When those relationships are stated in text, readers can reach the intended finding directly instead of reconstructing it through serial point reading.

**Mechanism:** Text exposes chart-level semantics such as trends, clusters, patterns, outliers, and significant findings that are otherwise only visually apparent, reducing cognitive and functional labor for nonvisual access.

**Evidence:** Chartability requires visually apparent trends, clusters, patterns, outliers, and significant findings to be described through text at minimum, and the paper shows a scatterplot callout that exposes an outlier cluster summary instead of forcing piece-by-piece screen-reader navigation [@elavskyHowAccessibleMy2022]. W3C's understanding of Info and Relationships says relationships conveyed visually should also be available in a programmatically determinable form rather than being left only in appearance [@w3c_understanding_info].

**Notes:** Sonification or tactile output can supplement this text, but the minimum supported requirement here is a textual description of the relationship.

## Use when important relationships are carried by appearance <!-- role: context -->

- **User Goal:** Understand the chart's main finding or important area without relying on sight alone.
- **Data:** The chart contains a trend, cluster, pattern, outlier, or significant statistical relationship that is visually apparent.
- **Chart Setting:** The chart is dense, complex, or interactive enough that point-by-point reading would be tedious, and a summary or callout can be attached to the whole chart or a highlighted region.
- **Audience:** People using screen readers or other nonvisual access methods.
- **Success Criterion:** The key relationship can be identified from text at minimum, without traversing every mark.

## Do not apply it as invented interpretation <!-- role: exceptions -->

**Break it when:** The chart does not communicate any higher-level trend, cluster, pattern, outlier, or significant finding beyond the raw values already provided. **Why:** This rule is for exposing relationships that the visualization is already using to communicate meaning, not for adding unsupported interpretation.

## Costs of relationship text <!-- role: costs -->

**Sacrifice:** You add visible and nonvisual text that must be authored and kept aligned with the chart.
**Risk:** A vague summary or a list of raw values still leaves the relationship hidden.
**Mitigation:** Name the specific relationship directly, such as the trend direction, the outlier region, or the important cluster.

## Common failure modes <!-- role: mistakes -->

- **Mistake:** Expose only individual values or a table and expect readers to infer the trend, cluster, or outlier themselves. **Why it fails:** The higher-level relationship remains unavailable without extra cognitive work and tedious navigation.
- **Mistake:** Treat a one-to-one audio or tactile rendering as sufficient without naming the relationship in text. **Why it fails:** The marks may be mirrored, but the semantic relationship between them is still not explicitly described.

## How to test it <!-- role: check -->

**Failure Sign:** The chart has an obvious trend, cluster, pattern, outlier, or highlighted statistical finding, but the available text names only the chart or the raw values.
**Quick Check:** Ask what a sighted reader would notice first, then look for text that states that relationship explicitly.
**Stronger Test:** Review the chart through text or screen-reader access only and verify that you can identify the important area without traversing every mark one by one.

## What to change <!-- role: fix -->

- Add a chart-level text summary that states the main trend, cluster, pattern, outlier, or significant finding.
- Add a text callout on the statistically or visually important region.
- Expose that summary or callout to screen readers, not only visually on the chart.
- If the experience already supports multisensory output, supplement the text by exposing the same relationship through sonification or tactile output.
