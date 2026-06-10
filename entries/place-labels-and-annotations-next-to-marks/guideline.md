---
id: place-labels-and-annotations-next-to-marks
title: Place labels and annotations next to the marks they explain
bibliography: references.bib
description: For lookup and explanation tasks, use nearby labels and annotations on
  charts to improve readability and mitigate back-and-forth legend or text lookup
  for readers scanning a single display.
labels:
- purpose:refine
- basis:empirical
- quality:readability:use
- lever:text-annotation
- operator:lookup
- component:label:use
- component:legend:avoid
- polish:annotation
---

## Move text to the mark <!-- role: advice -->

Put text next to the data element it refers to. For example, label slices directly instead of making readers match colors to a separate legend, and place explanatory callouts beside the highlighted line segment rather than in distant bullets.

## Why nearby text works <!-- role: reason -->

Readers should not have to hold a color, name, or verbal claim in memory while searching elsewhere in the figure. Nearby labels and annotations reduce extra eye movements and working-memory load.

**Mechanism:** When the label or explanation sits beside the mark, readers can identify and interpret the target in one place instead of switching back and forth between separated parts of the display.

**Evidence:** The paper argues that legends hurt performance because they require maintaining features in memory, shows a directly labeled pie example as easier to use than a legend-based version, and recommends placing verbal information near the visual information of interest [@zacksDesigningGraphsDecisionMakers2020].

## Use when readers must match text to marks <!-- role: context -->

- **User Goal:** Identify named categories or understand a highlighted claim.
- **Task:** Lookup or explanation.
- **Data:** Mark identities depend on labels, colors, or callouts.
- **Chart Setting:** A separate legend or distant explanatory text is present.
- **Audience:** Readers scanning quickly through one display.
- **Success Criterion:** Readers answer lookup questions without repeated back-and-forth glances.

## Do not use when callouts would overwhelm the chart <!-- role: exceptions -->

**Break it when:** Many items would need labels or callouts at once. **Why:** Only a very limited number of things can be called out with language without overwhelming the viewer.

## Trade space for less lookup pain <!-- role: costs -->

**Sacrifice:** Nearby text uses space around the marks.
**Risk:** Too many labels can clutter the chart and compete with the data.
**Mitigation:** Label the marks or claims readers must identify directly, not every possible detail.

## Avoid remote lookup aids <!-- role: mistakes -->

**Mistake:** Keeping a color legend or side bullets even when the viewer must map each text item back to specific marks. **Why it fails:** The viewer must repeatedly store information in memory and search the chart again.

## Check whether the reader must look away <!-- role: check -->

**Failure Sign:** Readers keep jumping between legend, bullets, and plot before answering.
**Quick Check:** Ask someone to answer a named-item question; if they must remember a color or phrase while scanning elsewhere in the chart, the text is too far away.
**Stronger Test:** Compare the current version with a directly labeled version on the same question and see which one readers answer more smoothly.

## Bring the words to the data <!-- role: fix -->

- Move category names onto the slices, bars, lines, or points they identify.
- Move explanatory text next to the highlighted region or comparison.
- Remove a separate legend when direct labeling can replace it.
