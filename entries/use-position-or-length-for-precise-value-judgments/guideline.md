---
id: use-position-or-length-for-precise-value-judgments
title: Use position or length when readers need precise value judgments
bibliography: references.bib
description: For exact quantitative reading, use position or length encoding on quantitative
  charts to improve fidelity and mitigate imprecise value estimation for readers making
  precise judgments.
labels:
- purpose:refine
- basis:empirical
- data:quantitative
- quality:fidelity:use
- lever:encoding
- reading-mode:exact
- channel:position:use
- channel:area:avoid
---

## Choose the exact encoding <!-- role: advice -->

Encode quantitative values with position or length when readers must read values accurately. For example, use bar length, line position, or scatterplot position instead of bubble area or color intensity when the task is to judge values or ratios precisely.

## Why exact channels work <!-- role: reason -->

Some visual channels support much more accurate reading than others. Position and length give readers a tighter mapping from mark to value, while area and intensity are better for broad pattern sensing than for exact judgment.

**Mechanism:** Position and length reduce estimation error when readers compare or read values, so the chart supports exact judgments instead of rough impressions.

**Evidence:** The paper summarizes empirical rankings of visual features showing that position is most precise, length is also strong, and area and intensity are less precise for quantitative judgments, while noting that area and intensity remain useful for big-picture overview tasks [@zacksDesigningGraphsDecisionMakers2020].

## Use when exact value reading matters <!-- role: context -->

- **User Goal:** Read values accurately or judge ratios between values.
- **Task:** Exact reading of magnitude.
- **Data:** Quantitative values encoded visually.
- **Chart Setting:** The same values could be encoded by position, length, area, or intensity.
- **Audience:** Readers who need accurate numeric interpretation.
- **Success Criterion:** Readers make precise value judgments with low error.

## Do not use when overview is enough <!-- role: exceptions -->

**Break it when:** The goal is rapid overview of a large array rather than precise reading of individual values. **Why:** Area and intensity can still make broad patterns immediately visible for big-picture scanning.

## Weigh overview against precision <!-- role: costs -->

**Sacrifice:** Broad spatial patterns may feel less immediate than in a color-coded overview.
**Risk:** For dense displays, replacing overview shading with exact encodings can make the chart less glanceable.
**Mitigation:** Keep area or intensity for overview views, and reserve position or length for exact readout.

## Watch for imprecise magnitude channels <!-- role: mistakes -->

**Mistake:** Leaving magnitude in bubble size or color intensity while asking readers to make exact numeric or ratio judgments. **Why it fails:** Those channels support less precise estimates than position and length.

## Test the encoding choice <!-- role: check -->

**Failure Sign:** Readers hesitate or disagree on simple value or ratio judgments.
**Quick Check:** Ask someone to estimate the relation between two marks; if the values are encoded by area or intensity, sketch a position- or length-based version and compare the responses.
**Stronger Test:** Create a quick alternate version using a common position or length scale and see whether answers become more accurate and consistent.

## Replace weak channels with exact ones <!-- role: fix -->

- Replace area encoding with aligned bars, dots, or points on a common scale.
- Replace intensity readout with position or length when exact judgment matters.
- Keep intensity or area only for overview displays where precise value reading is not the goal.
