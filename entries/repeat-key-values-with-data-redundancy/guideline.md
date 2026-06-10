---
id: repeat-key-values-with-data-redundancy
title: Repeat key values with data redundancy
bibliography: references.bib
description: For exact reading and recall of quantitative values, use repeated quantitative
  encodings on the chart to improve insight and address missed values for readers
  interpreting the figure directly.
labels:
- purpose:refine
- basis:empirical
- task:retrieve
- data:quantitative
- quality:insight
- lever:encoding
- operator:lookup
- reading-mode:exact
- component:label:use
---

## Add a second cue for the same values <!-- role: advice -->

Repeat important quantitative values in more than one encoding on the chart. For example, place numbers on bars or pie sectors, or use an additional channel such as color, size, or opacity only when it repeats a value that is already shown elsewhere in the visualization.

## Why data redundancy works <!-- role: reason -->

Readers describe charts better when the numbers or magnitudes are available through more than one cue. Repeating the same value reduces the chance that the viewer notices the structure of the chart but misses the quantitative content.

**Mechanism:** A second quantitative cue gives the viewer another way to encode and retrieve the same value, which supports later description of the chart.

**Evidence:** Visualizations with data redundancy had higher average description quality than those without it, and the top third of visualizations by description quality contained data redundancy much more often than the bottom third [@borkinMemorabilityVisualizationRecognition2016].

## Use when the chart presents quantitative values that can be restated <!-- role: context -->

- **User Goal:** Help viewers notice and later recall exact values or magnitudes.
- **Task:** Exact reading and recall.
- **Data:** Quantitative values already appear in the visualization and can be repeated without changing their meaning.
- **Chart Setting:** The figure is intended to communicate values directly, not only a qualitative takeaway.
- **Success Criterion:** Reviewers can later report key values, not just the direction of the trend.

## Do not use this when the chart's need is message repetition rather than value repetition <!-- role: exceptions -->

**Break it when:** The main goal is to restate a qualitative conclusion rather than to repeat the same numeric values. **Why:** The paper treats message redundancy and data redundancy as different interventions.

## Tradeoffs of data redundancy <!-- role: costs -->

**Sacrifice:** You reduce visual simplicity by adding another cue for the same values.\
**Risk:** Extra labels or channels can feel busy if they do not repeat the same data.\
**Mitigation:** Use the extra cue only for the same values already encoded by the chart.

## Common data redundancy failure <!-- role: mistakes -->

**Mistake:** Adding labels or visual channels that introduce different information instead of repeating the same values. **Why it fails:** The viewer gets more material to parse but no redundant support for the target values.

## Check whether the values are repeated <!-- role: check -->

**Failure Sign:** Reviewers can name the chart type and trend but cannot report key values.\
**Quick Check:** Inspect whether the important numeric values are available in more than one form, such as a mark plus a direct label.\
**Stronger Test:** Ask a reviewer to report key values after a short viewing; if they recall only the overall shape, add a redundant quantitative cue.

## Fix value repetition <!-- role: fix -->

- Add direct numeric labels to the key marks, such as bars or pie sectors.
- Add one extra quantitative channel only when it repeats a value already shown by position, length, or another existing encoding.
- Choose the repeated cue that makes the same values visible without changing what they mean.
