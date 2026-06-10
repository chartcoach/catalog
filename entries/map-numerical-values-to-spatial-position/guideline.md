---
id: map-numerical-values-to-spatial-position
title: Map numerical values to spatial position when accurate reading matters
bibliography: references.bib
description: For compare tasks on quantitative charts, prefer spatial position encoding
  to improve fidelity and mitigate inaccurate magnitude decoding from angle, area,
  volume, and color saturation for readers interpreting numbers.
labels:
- purpose:refine
- basis:empirical
- task:compare
- data:quantitative
- quality:fidelity
- lever:encoding
- channel:position:use
- channel:angle:avoid
---

## Position encoding <!-- role: advice -->

Make spatial position the primary channel for numerical values when readers must compare magnitudes accurately. For example, use bar charts, line charts, or scatter plots for the main numeric readout instead of relying on pie-slice angles, bubble areas, 3D volumes, or color saturation to carry the comparison.

## Why position improves numeric reading <!-- role: reason -->

Aligned position reduces the amount of visual estimation readers must do. Readers can compare values more directly when they judge where marks fall in space rather than inferring magnitude from less precise channels such as angle or filled size.

**Mechanism:** Position supports more accurate magnitude decoding, so small differences and rank changes are easier to read correctly.

**Evidence:** The paper reports graphical perception experiments showing that spatial position leads to the most accurate decoding of numerical data and is generally preferable to angle, one-dimensional length, two-dimensional area, three-dimensional volume, and color saturation; it also notes that common charts such as bar charts, line charts, and scatter plots use position encodings for this reason [@heerTourVisualizationZoo2010].

**Notes:** The paper also states that graphical-perception guidance should be balanced with interaction design and aesthetics.

## Where this applies <!-- role: context -->

- **User Goal:** Compare numeric magnitudes or see which values are larger or smaller.
- **Task:** Read or compare quantitative values directly from the display.
- **Data:** Numerical values are the main message.
- **Chart Setting:** You can choose the primary visual channel that carries magnitude.
- **Audience:** Readers need to decode numbers from marks rather than from accompanying text.
- **Success Criterion:** Small numeric differences can be judged accurately.

## When not to force this rule <!-- role: exceptions -->

**Break it when:** Accurate numeric decoding is not the primary priority and interaction design or aesthetics are the stronger constraint. **Why:** The paper says perceptual accuracy guidance must be balanced with those other design goals.

## Tradeoffs of prioritizing position <!-- role: costs -->

**Sacrifice:** You give up some stylistic freedom in how the main numeric variable is encoded.\
**Risk:** A design that optimizes only for perceptual accuracy can under-serve interaction or aesthetic goals.\
**Mitigation:** Keep position as the main quantitative readout, then balance the rest of the design with interaction and aesthetic choices.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Letting angle, area, volume, or color saturation carry the main numeric comparison. **Why it fails:** Those channels are less accurate for decoding magnitude, so readers must estimate more and compare less precisely.

## How to check the chart <!-- role: check -->

**Failure Sign:** The chart asks readers to compare sizes, angles, or saturation levels instead of aligned locations.\
**Quick Check:** Ask what a reader must visually judge to compare two values; if the answer is angle, area, volume, or saturation, the chart misses the rule.\
**Stronger Test:** Mock up a version with the same data mapped to aligned position and see whether the key comparisons become more direct.

## How to fix it <!-- role: fix -->

- Move the main quantitative scale onto a shared spatial axis.
- Replace angle-based or area-based numeric comparisons with bars, points, or lines positioned against a scale.
- Demote color saturation or 3D size to a secondary role instead of using it as the primary magnitude encoding.
