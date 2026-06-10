---
id: use-unclassed-color-scales-for-continuous-patterns
title: Use an unclassed color scale to show continuous patterns
bibliography: references.bib
description: For overview reading of continuous values, use an unclassed color scale
  on quantitative choropleth maps to improve fidelity and mitigate oversimplified
  regional differences for readers scanning general spatial patterns.
labels:
- purpose:refine
- basis:heuristic
- chart:choropleth
- data:quantitative
- quality:fidelity
- lever:encoding
- reading-mode:overview
---

## Keep the gradient continuous <!-- role: advice -->

Use an unclassed color scale when the goal is to show continuous overall pattern and subtle spatial differences. For example, keep every numeric value on the gradient when you want readers to see outliers, smooth versus abrupt transitions, or whether one area differs slightly from its neighbors.

## Preserve nuance across the map <!-- role: reason -->

A classed map collapses nearby values into shared bins. An unclassed map keeps those differences visible, which gives a more exact view of the underlying data.

**Mechanism:** Continuous color makes small value differences, local contrasts, and transition shapes visible instead of hiding them inside a few broad brackets.

**Evidence:** The article describes unclassed choropleths as the most exact representation of the data model and recommends them when the goal is a general pattern or a nuanced view rather than a predefined bracket [@muth_classed_vs_unclassed_2021].

## Use when subtle differences matter <!-- role: context -->

- **User Goal:** Show the overall spatial pattern without forcing values into a few bins.
- **Task:** Scan for broad gradients, local contrasts, outliers, or transition shapes.
- **Data:** Continuous quantitative values where small differences between regions are meaningful.
- **Chart Setting:** A choropleth map that readers will inspect for regional variation.
- **Success Criterion:** Subtle variation remains visible across neighboring regions and across the whole map.

## Do not use when readers must see brackets or ranges first <!-- role: exceptions -->

**Break it when:** The map's main job is to show predefined brackets or let readers read value ranges confidently. **Why:** Classed scales make bracket membership and range reading easier.

## Accept weaker range reading <!-- role: costs -->

**Sacrifice:** Readers get nuance, but they lose easy value-range reading.
**Risk:** Exact values remain guesses from the color alone.
**Mitigation:** Improve the legend if readers also need to estimate values from the map.

## Avoid unnecessary binning <!-- role: mistakes -->

**Mistake:** Sorting continuous values into a few classes when the goal is the overall pattern. **Why it fails:** Different regions collapse into the same color and meaningful local variation disappears.

## Check whether classification hides pattern <!-- role: check -->

**Failure Sign:** Large same-color areas hide visible variation in the underlying values.
**Quick Check:** Compare classed and unclassed versions and see whether relevant outliers or neighboring differences disappear after binning.
**Stronger Test:** Inspect whether transitions that should look smooth or abrupt become unreadable once classes are added.

## Remove the artificial bins <!-- role: fix -->

- Replace the stepped color scale with a continuous gradient.
- Remove class boundaries that are not part of the message.
- Recheck neighboring regions and outliers on the unclassed version before finalizing.
