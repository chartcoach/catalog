---
id: prefer-position-over-area-for-quantitative-values
title: Prefer position over area for quantitative values
bibliography: references.bib
description: For exact quantitative comparison, prefer position encoding on quantitative
  displays to improve reading accuracy and mitigate imprecise size judgments for viewers
  interpreting static graphics.
labels:
- purpose:refine
- basis:empirical
- task:compare
- data:quantitative
- quality:fidelity:use
- lever:encoding
- channel:position:use
- channel:area:avoid
- reading-mode:exact
---

## Prioritize position for quantitative values <!-- role: advice -->

Map quantitative values to position before area when accuracy matters. For example, use a scatter plot with x and y position for two numeric measures instead of encoding one of those measures by bubble area, because the position version supports more accurate reading.

## Why position beats area for exact reading <!-- role: reason -->

Position gives readers a direct spatial comparison against an axis, while area requires judging relative sizes of marks. That makes small differences harder to read accurately when the same numbers could instead be placed on an axis.

**Mechanism:** Position reduces the perceptual work needed to compare quantitative values, so readers can recover magnitudes more accurately than when they must infer values from mark size.

**Evidence:** The paper ranks position above area for quantitative perception and uses a scatter plot versus an area/position design to show that the position-based design is more effective for the same price/mileage data [@mackinlayAutomatingDesignGraphical1986].

## Use when exact numeric reading matters <!-- role: context -->

- **User Goal:** Read or compare quantitative values accurately.
- **Task:** Compare magnitudes from the chart rather than just notice a rough pattern.
- **Data:** Two quantitative measures can be plotted directly on axes.
- **Chart Setting:** The same values could be encoded either by axis position or by mark area.
- **Success Criterion:** Readers can judge relative values accurately from the display.

## Do not force this when position is already reserved for more important values <!-- role: exceptions -->

**Break it when:** A multivariate display already uses the best positional channels for more important quantitative relations. **Why:** The paper explicitly allows lower-ranked channels such as area for less important information when the more accurate channels are needed elsewhere.

## Tradeoffs of remapping area to position <!-- role: costs -->

**Sacrifice:** You use up scarce positional channels that might be needed for another measure.
**Risk:** Forcing every quantitative field onto position can make a multivariate design impossible.
**Mitigation:** Keep the most important quantitative values on position and demote less important ones to lower-ranked channels only when necessary.

## Common failure mode with area encoding <!-- role: mistakes -->

**Mistake:** Encode a quantitatively important measure by mark area even though an axis position is available. **Why it fails:** Readers must estimate size instead of reading position, which lowers quantitative accuracy.

## Check the encoding choice directly <!-- role: check -->

**Failure Sign:** One important quantitative field is shown by bubble size while a comparable design could place it on an axis.
**Quick Check:** Sketch the same display once with area and once with position for that field; if exact reading is easier in the positional version, keep the positional encoding.
**Stronger Test:** Ask whether a reader can recover the ordering and spacing of values from the axis without estimating mark size.

## Fix the encoding assignment <!-- role: fix -->

- Move the quantitatively important field from area to an x or y axis.
- Keep area only for a less important quantitative field after the higher-priority fields already occupy the available axes.
- Redraw the display as a scatter plot when two quantitative measures can be placed directly on axes.
