---
id: label-only-distinct-steps-on-dense-quantitative-color-keys
title: Label only distinct steps on dense quantitative color keys
bibliography: references.bib
description: For overview and lookup in dense quantitative color keys, use a subset
  of labels on legends with many classes or highly interpolated colors to improve
  readability and mitigate overlap and false precision for readers scanning magnitudes.
labels:
- purpose:refine
- basis:heuristic
- data:quantitative
- quality:readability
- lever:text-annotation
- component:legend:use
- density:dense
- reading-mode:overview
---

## Sparse value labels <!-- role: advice -->

Label only the steps that readers can usefully distinguish on a dense quantitative color key. For example, on a classed scale with many obvious class borders, label every other class instead of all of them, and on a highly interpolated scale, do not label two adjacent colors that look almost the same.

## Fewer labels keep the scale readable <!-- role: reason -->

A dense key with a number on every step becomes busy and discouraging to read. Labels work best when they mark colors or class boundaries that readers can actually tell apart.

**Mechanism:** Reducing labels lowers visual clutter and keeps attention on meaningful thresholds instead of impossible fine distinctions.

**Evidence:** The post says that showing values for all classes is often not the best choice when there are many classes, recommends skipping every other class when borders are obvious, and says to label only visibly distinct colors rather than near-identical ones in highly interpolated scales. [@muth_color_keys_2023]

## Use when the key is crowded with steps <!-- role: context -->

- **User Goal:** Understand the rough magnitude pattern without wrestling with a crowded legend.
- **Data:** Quantitative color scale with many classes or many interpolated subdivisions.
- **Chart Setting:** The current key looks busy, or adjacent colors are not visually distinct enough to justify separate labels.
- **Audience:** Readers are scanning for approximate ranges rather than decoding every possible step.
- **Success Criterion:** The key stays readable while still supporting the intended magnitude reading.

## Do not use when exact numeric reading is required from the key <!-- role: exceptions -->

**Break it when:** Readers need exact values from a static visualization. **Why:** A static chart cannot rely on tooltips, so removing too many numeric labels can take away needed precision.

## Precision tradeoff of fewer labels <!-- role: costs -->

**Sacrifice:** You give up some exactness at a glance.\
**Risk:** Removing too many labels can hide useful thresholds.\
**Mitigation:** Keep labels for the distinct and important steps readers truly need.

## Common overlabeling failure <!-- role: mistakes -->

**Mistake:** Label every class or label near-identical adjacent colors separately. **Why it fails:** The key becomes busy without adding readable distinctions.

## Quick review for overlabeling <!-- role: check -->

**Failure Sign:** Labels overlap, crowd together, or sit on colors that look nearly identical.\
**Quick Check:** Remove alternating labels and see whether the legend still communicates the intended pattern.\
**Stronger Test:** Ask whether a reader can still identify the useful ranges without reading every step.

## Concrete edits for dense numeric keys <!-- role: fix -->

- Remove every other label when class borders are already obvious.
- Keep labels only on steps that are visibly distinct.
- Delete labels on adjacent colors that readers cannot reliably tell apart.
