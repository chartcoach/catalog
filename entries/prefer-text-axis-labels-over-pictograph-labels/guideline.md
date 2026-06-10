---
id: prefer-text-axis-labels-over-pictograph-labels
title: Use text axis labels instead of pictograph labels for brief recall tasks
bibliography: references.bib
description: For brief recall tasks, prefer text labels on chart axes to improve memory
  fidelity and address weaker category-to-value encoding for viewers reading short,
  unambiguous category names.
labels:
- purpose:refine
- basis:empirical
- task:retrieve
- chart:bar
- quality:fidelity
- lever:text-annotation
- component:axis:use
- channel:text:use
---

## Axis label format <!-- role: advice -->

Keep axis category labels in text when viewers must remember values after a brief glance. For example, place short words under the bars instead of replacing those labels with pictographs, even if later prompts or surrounding graphics use icons.

## Why text labels helped memory here <!-- role: reason -->

Short text labels can be recognized quickly and linked to a value with little extra decoding. Icon labels add another interpretation step and can weaken the connection between category and value during brief exposure.

**Mechanism:** Text axis labels make it easier to encode which category goes with which number when the chart disappears and the reader must recall the values from memory.

**Evidence:** Across chart types, pictographs used as x-axis labels increased recall error, while changing the response prompt between text and pictographs made no reliable difference [@harozISOTYPEVisualizationWorking2015].

## Use when labels must be encoded quickly <!-- role: context -->

- **User Goal:** Remember which value belongs to each category.
- **Task:** Brief-glance recall after the chart is removed.
- **Data:** Quantitative values with category names that can be shown as short words.
- **Chart Setting:** The x-axis labels could be rendered either as text or as pictographs.
- **Audience:** Viewers reading short, unambiguous category labels.
- **Success Criterion:** Lower recall error for category-value matches.

## Do not generalize beyond short readable labels <!-- role: exceptions -->

**Break it when:** The category cannot be expressed as succinct, easy-to-read text. **Why:** The reported text advantage was observed with short readable labels, and the study did not test longer or more complex wording.

## Tradeoffs of using text labels <!-- role: costs -->

**Sacrifice:** You give up some visual illustration in the axis.
**Risk:** The chart may feel less pictorial.
**Mitigation:** Keep imagery in the data marks if you need it, but leave the axis labels as text.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Replacing every axis label with an icon to match the subject matter. **Why it fails:** The icon label is harder to encode quickly than the short text label it replaces.

## How to test it <!-- role: check -->

**Failure Sign:** Viewers remember the numbers but confuse which category each number belonged to.
**Quick Check:** Compare a text-labeled version against an icon-labeled version in a brief-glance recall task.
**Stronger Test:** Randomize the recall order of categories and compare average absolute error across the two label styles.

## What to change <!-- role: fix -->

- Restore text words on the axis where categories are named.
- Shorten category wording so the text remains quick to read.
- Remove pictograph labels from the axis rather than duplicating the category in both icon and word form.
