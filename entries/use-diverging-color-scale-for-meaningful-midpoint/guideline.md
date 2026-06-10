---
id: use-diverging-color-scale-for-meaningful-midpoint
title: Use a diverging color scale when the data have a meaningful midpoint
bibliography: references.bib
description: For comparison in quantitative color-encoded charts, use a diverging
  color scale on data with a meaningful midpoint to improve insight and address one-directional
  magnitude readings for readers interpreting values above and below that midpoint.
labels:
- purpose:refine
- basis:heuristic
- task:compare
- data:quantitative
- quality:insight
- lever:encoding
- polish:palette
- aesthetic:color:use
---

## Center the color scale on a meaningful midpoint <!-- role: advice -->

Use a diverging color scale when the quantitative data have a meaningful middle value. For example, center the scale on zero, 50%, the average or median, an agreed threshold such as a poverty line, or a target such as a revenue goal.

## Why a meaningful midpoint helps <!-- role: reason -->

A diverging scale makes the middle color carry meaning instead of acting as a decorative center. Readers can then see whether values fall above or below a reference value, not just where they sit on a single low-to-high ramp.

**Mechanism:** The split palette turns the midpoint into an explicit benchmark and makes both sides of that benchmark visible.

**Evidence:** The article recommends diverging colors when there is a meaningful middle value and names zero, 50%, the average or median, an agreed threshold, and a target as valid centers [@muth_diverging_vs_sequential_2021].

## Use when the midpoint is part of the message <!-- role: context -->

- **User Goal:** Show whether values are above or below a reference value.
- **Task:** Compare values by side of midpoint and by distance from it.
- **Data:** Quantitative values with an explicit middle such as zero, 50%, median, threshold, or target.
- **Chart Setting:** A chart or map already using a quantitative color scale.
- **Audience:** Readers need to interpret the center as a real benchmark.
- **Success Criterion:** Readers can state what the center color means and tell which values fall on each side.

## Do not use when the middle is arbitrary <!-- role: exceptions -->

**Break it when:** The data do not have a meaningful middle value and are better read as a one-directional low-to-high range. **Why:** A diverging center would impose a split the data do not justify.

## Costs of adding a midpoint split <!-- role: costs -->

**Sacrifice:** You give up some immediate light-to-dark simplicity.\
**Risk:** Readers may wonder what the middle color means if the center is weak or unexplained.\
**Mitigation:** Use a midpoint readers can name and recognize.

## Common midpoint failure <!-- role: mistakes -->

**Mistake:** Centering a diverging scale on an arbitrary middle that is not a real benchmark. **Why it fails:** Readers infer an above-versus-below meaning that the data do not support.

## Check that the midpoint is real <!-- role: check -->

**Failure Sign:** Reviewers cannot explain what the middle color stands for.\
**Quick Check:** Ask, “What exact value is the midpoint?” If it is not a named benchmark such as zero, 50%, median, threshold, or target, do not use diverging.\
**Stronger Test:** Compare a sequential version; if the diverging center adds no interpretable above/below meaning, keep the sequential scale.

## Fix an arbitrary diverging center <!-- role: fix -->

- Set the center of the scale to an explicit benchmark.
- Replace the diverging scale with a sequential light-to-dark scale if no benchmark exists.
- Preview both sequential and diverging versions and keep the one whose midpoint has a clear meaning.
