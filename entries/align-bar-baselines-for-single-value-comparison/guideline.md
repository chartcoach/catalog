---
id: align-bar-baselines-for-single-value-comparison
title: Align bar baselines for single-value comparison
bibliography: references.bib
description: For compare tasks on single-value bar displays, use aligned position
  encoding on bar charts to improve fidelity and mitigate imprecise single-value judgments
  for readers making direct value comparisons.
labels:
- purpose:refine
- basis:empirical
- task:compare
- scope:single-result
- chart:bar
- quality:fidelity
- lever:encoding
- operator:difference
- channel:position:use
---

## Align bar baselines <!-- role: advice -->

Keep compared bar values on a shared baseline so readers judge position instead of isolated length. For example, use standard bars with a common baseline and avoid making readers compare misaligned bar segments such as parts of a stacked bar.

## Why aligned baselines work for single values <!-- role: reason -->

When two values share a baseline, the reader can compare the tops by position, which is more precise than comparing separated lengths. When the bars are misaligned, the comparison shifts toward length and precision drops.

**Mechanism:** A shared baseline turns the task into a position comparison. Misalignment removes that position cue and forces a less precise extent judgment.

**Evidence:** In 1vs1 comparisons, normal bar graphs were as precise as dot plots and much more precise than misaligned bar graphs, indicating that aligned bars supported position-based reading while misaligned bars did not [@yuanPerceptualProxiesExtracting2019].

## Use when single values are the comparison target <!-- role: context -->

- **User Goal:** Decide which of two individual values is larger.
- **Task:** Direct value comparison.
- **Data:** One quantitative value per compared item.
- **Chart Setting:** Bar charts where the compared values can be placed on a common baseline.
- **Success Criterion:** More precise single-value judgments.

## Do not rely on this for multi-value mean judgments <!-- role: exceptions -->

**Break it when:** The reader must compare averages across multiple values rather than two individual values. **Why:** In the experiments, aligned bars were not more precise than misaligned bars for multi-value average comparisons.

## Tradeoffs of aligned baselines <!-- role: costs -->

**Sacrifice:** You give up using separated bar segments as the main comparison target.
**Risk:** Applying this rule to group-average judgments will not fix the harder problem of extracting means from many bars.
**Mitigation:** Use a display that supports the mean task directly instead of assuming alignment alone is enough.

## Common baseline mistake <!-- role: mistakes -->

**Mistake:** Keeping the compared values on different baselines and expecting readers to compare them as precisely as aligned bars. **Why it fails:** The task becomes a length comparison instead of a position comparison.

## How to check baseline alignment <!-- role: check -->

**Failure Sign:** The two values being compared start from different vertical offsets.
**Quick Check:** Ask whether the compared tops can be read against the same baseline without mentally shifting one bar.
**Stronger Test:** Make an aligned version of the same two-value display and compare whether judgments become easier or more precise.

## How to fix misaligned single-value bars <!-- role: fix -->

- Move the compared values onto a common baseline.
- Redraw stacked or offset segments as separate aligned bars when the task is precise single-value comparison.
- If precise comparison is critical, replace the compared segments with points on a shared scale.
