---
id: use-stacked-bars-for-repeated-share-breakdowns
title: Use stacked bars for repeated share breakdowns
bibliography: references.bib
description: For comparing repeated share breakdowns across groups or time, prefer
  stacked bar charts over multiple pie or donut charts to improve readability and
  mitigate hard-to-compare repeated proportions for general audiences.
labels:
- purpose:select
- basis:heuristic
- chart:bar:use
- chart:pie-donut:avoid
- operator:part-whole
- measure:multi
- lever:chart-family
- quality:readability
---

## Stacked bars for repeated shares <!-- role: advice -->

Use stacked bars when the same share breakdown repeats across several groups or time points. For example, show survey response distributions or repeated percentage splits in stacked bars instead of lining up multiple pies or donuts.

## Why stacked bars scale better across repeated share views <!-- role: reason -->

Repeated circle charts make readers re-learn the same part-to-whole structure over and over. Stacked bars keep the repeated comparison in one compact form.

**Mechanism:** A row or column of stacked bars lets readers scan repeated percentage splits more efficiently than comparing many separate circles.

**Evidence:** Multiple pies, donuts, and waffles can show several dimensions side by side, but stacked bar charts are presented as a likely best option for repeated share displays such as survey results because they are space-efficient [@muth_chart_types_guide_2025].

## Use when the same proportions repeat across groups or time <!-- role: context -->

- **User Goal:** Compare how the same share breakdown differs across categories or dates.
- **Task:** Scan repeated proportions efficiently.
- **Data:** Multiple groups or time points, each split into the same set of percentage categories.
- **Chart Setting:** A display where space efficiency matters.
- **Audience:** A mainstream audience.
- **Success Criterion:** Readers can compare several repeated share breakdowns without scanning separate circular charts.

## Do not use when there is only one overall share breakdown <!-- role: exceptions -->

**Break it when:** You are only showing a single share breakdown and do not need repeated comparison across groups or dates. **Why:** The extra structure of repeated stacked bars is not needed for a one-off share view.

## Costs of switching to stacked bars <!-- role: costs -->

**Sacrifice:** You lose the more eye-catching repeated circle format.\
**Risk:** If there is only one breakdown to show, the switch adds structure you do not need.\
**Mitigation:** Use stacked bars specifically for repeated share displays.

## Common failure with repeated share charts <!-- role: mistakes -->

**Mistake:** Repeat pies or donuts for each group or year when readers need to compare the whole set. **Why it fails:** Separate circle sections are harder to scan across many repeated views and take more space.

## Check whether the repeated shares need a more compact comparison form <!-- role: check -->

**Failure Sign:** The display repeats many pies or donuts for the same set of share categories.\
**Quick Check:** Compare the repeated circular version with a stacked-bar version; if the stacked bars fit more cleanly and make cross-group scanning easier, keep the stacked bars.\
**Stronger Test:** Ask whether a reader can compare several groups in one pass without jumping between separate circles.

## Fix the repeated share display <!-- role: fix -->

- Replace each repeated pie or donut with a stacked bar.
- Align the repeated share breakdowns in one stacked-bar chart.
- Use the stacked-bar form when survey-style or repeated percentage splits need compact comparison.
