---
id: remove-gratuitous-third-dimensions
title: Remove gratuitous third dimensions
bibliography: references.bib
description: For explanatory charts where values must be decoded accurately, avoid
  decorative depth encoding on the visual representation to prevent perceptual obscuring
  and address hard-to-judge positions for readers making visual comparisons.
labels:
- purpose:refine
- basis:empirical
- quality:fidelity:use
- lever:encoding
---

## Depth encoding <!-- role: advice -->

Remove third-dimensional depth cues when depth does not encode data. For example, do not add 3D perspective that makes marks harder to size, compare, or place on an axis without adding new information.

## Why flat encoding works better here <!-- role: reason -->

Decorative depth changes what readers can judge. It adds perceptual noise, distorts apparent size and position, and makes a simple readout harder than it needs to be.

**Mechanism:** When depth is decorative rather than data-bearing, it interferes with size and position judgments instead of contributing information.

**Evidence:** The paper identifies gratuitous third dimension as a mapping-rhetoric technique that obscures information at a perceptual level. It also describes related non-essential sizing transformations as obscuring when they make elements too small, too large, or hard to judge accurately [@hullmanVisualizationRhetoricFraming2011].

**Notes:** The paper treats obscuring as a rhetorical move, not only as an accidental error.

## Use when accurate value reading matters <!-- role: context -->

- **User Goal:** Compare values or read positions accurately.
- **Task:** Decode a chart rather than experience it as visual metaphor or noise.
- **Data:** The plotted values can already be shown in two dimensions.
- **Chart Setting:** Static or interactive chart where 3D depth does not carry a separate variable.
- **Audience:** Readers relying on visual comparison of size or position.
- **Success Criterion:** Readers can judge value differences without perceptual distortion from depth.

## Do not flatten the chart when obscuring is the intended rhetorical effect <!-- role: exceptions -->

**Break it when:** The intended rhetorical effect is to obscure or create visual confusion rather than support accurate decoding. **Why:** The paper explicitly treats obscuring and visual noise as rhetorical strategies.

## Costs of removing decorative depth <!-- role: costs -->

**Sacrifice:** You give up a dramatic stylistic effect.
**Risk:** Flattening can reduce a metaphorical or theatrical presentation cue.
**Mitigation:** Keep any intended message in explicit labels or other direct mappings instead of depth.

## Common depth-encoding mistake <!-- role: mistakes -->

**Mistake:** Adding 3D perspective for style when it does not encode a variable. **Why it fails:** The extra depth changes apparent size and position while contributing no new data.

## Check whether depth is decorative <!-- role: check -->

**Failure Sign:** The chart uses perspective or depth, but no variable is mapped to that depth.
**Quick Check:** Ask whether removing the third dimension would remove any data.
**Stronger Test:** If flattening the chart leaves the same data but makes marks easier to compare, the depth was gratuitous.

## Fix gratuitous depth <!-- role: fix -->

- Flatten the chart to a two-dimensional view.
- Remove perspective and other decorative depth cues that shift apparent position.
- Resize marks if the current styling makes them too small or too large to judge accurately.
