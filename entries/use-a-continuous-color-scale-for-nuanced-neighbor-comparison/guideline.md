---
id: use-a-continuous-color-scale-for-nuanced-neighbor-comparison
title: Use a continuous color scale for nuanced neighbor comparison
bibliography: references.bib
description: For overview comparison of nearby regional values, prefer a continuous
  color scale over discrete steps on a choropleth to improve fidelity and mitigate
  lost nuance when neighboring values fall into the same class for readers who can
  use tooltips.
labels:
- purpose:refine
- basis:heuristic
- chart:choropleth
- quality:fidelity
- lever:encoding
- reading-mode:overview
- component:tooltip:use
- data:geospatial
---

## Continuous color scaling <!-- role: advice -->

Use a continuous color scale when readers need to compare neighboring regions more finely than a small set of classes allows. For example, let adjacent values take slightly different shades and use tooltips to reveal the exact number instead of forcing both regions into the same discrete step.

## Why continuous scales preserve local nuance <!-- role: reason -->

Classed colors simplify the map, but they also erase differences inside each class.

**Mechanism:** A continuous scale preserves shade differences between nearby values, which helps readers compare adjacent regions more finely. Tooltips can carry the exact values that the overview color cannot show.

**Evidence:** The post says discrete steps are good when readers should immediately see the value range, but that continuous scales keep nuance for comparing neighboring regions and can rely on tooltips for exact values [@muth_choroplethmaps_2018].

## Use when nearby differences matter <!-- role: context -->

- **User Goal:** Compare neighboring regions with more nuance.
- **Task:** Scan local differences across the map.
- **Data:** Ordered regional values with meaningful near-neighbor variation.
- **Chart Setting:** The map can use tooltips for exact values.
- **Audience:** Readers doing overview comparison, not immediate bin lookup.
- **Success Criterion:** Different nearby values remain visually distinguishable.

## Do not use when range bins are the message <!-- role: exceptions -->

**Break it when:** Readers mainly need to know which broad value range each region falls into at a glance. **Why:** The post says discrete steps are a good choice for immediate range reading.

## Costs of removing classes <!-- role: costs -->

**Sacrifice:** You lose instant range classification.
**Risk:** Readers may need the tooltip to recover exact values.
**Mitigation:** Keep tooltips enabled so the exact value is still available on demand.

## Common classing failure <!-- role: mistakes -->

**Mistake:** Use a small set of discrete steps when neighboring regions with different values need fine comparison. **Why it fails:** Different values collapse into one color shade and the local contrast disappears.

## Compare continuous and discrete drafts <!-- role: check -->

**Failure Sign:** Adjacent regions with different values share one class color.
**Quick Check:** Put a continuous draft beside the discrete-step draft and inspect neighboring regions you want readers to compare.
**Stronger Test:** If the discrete version hides differences that matter to the story, keep the continuous scale.

## Edit the scale for local nuance <!-- role: fix -->

- Switch the choropleth from discrete steps to a continuous color scale.
- Keep tooltips on so readers can still retrieve exact values.
- Recheck the adjacent regions that were collapsing into one class.
- Return to discrete steps only if broad range membership is the main message.
