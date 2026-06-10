---
id: use-directional-words-instead-of-values-on-color-keys
title: Use directional words instead of numeric values when only the gradient direction
  matters
bibliography: references.bib
description: For overview reading in quantitative color keys, use directional words
  on legends with metrics that need heavy explanation when the message is relative
  more-or-less change to improve readability and mitigate distracting units for readers
  who only need the general idea.
labels:
- purpose:refine
- basis:heuristic
- data:quantitative
- quality:readability
- lever:text-annotation
- component:legend:use
- reading-mode:overview
- needs:low-domain-knowledge
---

## Directional labels <!-- role: advice -->

Replace numeric values with directional words when the reader only needs the direction of the gradient. For example, label the key with endpoints such as “less” and “more” or “worse” and “better” instead of printing the full metric values and units.

## General direction can be enough <!-- role: reason -->

Some metrics take too much explanation to help in a legend. When readers only need to know which areas are lower or higher, directional words communicate the message faster than technical values.

**Mechanism:** Directional labels remove distracting units and focus the key on the core interpretation the reader needs.

**Evidence:** The post says that values and units can be omitted entirely in favor of a general “less/more” or “worse/better” when the metric needs lots of explanation, may confuse readers, and does not add useful understanding, while also noting that static visualizations should err toward showing more values if exact reading matters. [@muth_color_keys_2023]

## Use when the legend's job is only directional <!-- role: context -->

- **User Goal:** Grasp which areas or values are lower or higher.
- **Data:** Quantitative color scale based on a metric that is hard to explain or not useful to decode exactly.
- **Chart Setting:** The chart message is relative intensity, and exact numeric reading is not the main task.
- **Audience:** Readers may not have much domain knowledge about the metric itself.
- **Success Criterion:** Readers get the general idea without being slowed by technical units.

## Do not use when exact values must be read from the key <!-- role: exceptions -->

**Break it when:** Readers need exact values, especially in a static visualization. **Why:** A general directional label removes numeric information they may need to interpret the chart.

## Cost of simplifying the scale text <!-- role: costs -->

**Sacrifice:** You give up precise numeric interpretation in the key itself.\
**Risk:** The simplification can go too far when the chart requires exact numeric reading.\
**Mitigation:** Keep numeric labels when exact value lookup is part of the task.

## Common overtechnical legend failure <!-- role: mistakes -->

**Mistake:** Keep technical values and units in the key when they add confusion but not insight. **Why it fails:** The legend gets harder to read without helping readers understand the chart better.

## Quick review for directional sufficiency <!-- role: check -->

**Failure Sign:** The key is full of technical units, but the chart message is simply high versus low.\
**Quick Check:** Ask whether replacing the numbers with “less/more” changes the interpretation readers need.\
**Stronger Test:** Confirm that exact values are either unnecessary or available somewhere else in the experience.

## Concrete edits for overtechnical keys <!-- role: fix -->

- Replace numeric endpoints with directional words such as “less” and “more.”
- Remove units that do not add useful understanding.
- Keep the legend focused on the gradient direction rather than the metric definition.
