---
id: calibrate-hue-spacing-to-line-thickness
title: Calibrate hue spacing to line thickness
bibliography: references.bib
description: For color-difference reading in static charts, use hue spacing calibrated
  to line thickness on line charts to improve fidelity and mitigate point-based underuse
  of available color range for viewers reading web-based visualizations.
labels:
- purpose:refine
- basis:empirical
- chart:line
- quality:fidelity:use
- lever:encoding
- channel:color-hue:use
- aesthetic:color:use
---

## Use line-aware hue thresholds <!-- role: advice -->

Set hue spacing from line thickness rather than from point-based color thresholds. For example, allow long line strokes to use tighter color spacing than equally thick points, but still widen the spacing as lines get thinner.

## Why thin lines need their own hue thresholds <!-- role: reason -->

Long line strokes make color differences easier to see than equally thick point marks, but thin lines still lose discriminability as thickness shrinks. A line-specific threshold preserves distinguishability without wasting as much palette range as a point-based rule.

**Mechanism:** Color differences on lines vary inversely with line thickness, and long asymmetric strokes are more discriminable than equally thick points.

**Evidence:** The knowledge collation records this source as experimental evidence about color-hue encodings on line marks, and the paper reports that line color differences shrink with thickness while remaining more discriminable than equally thick scatterplot points [@zengReviewCollationGraphical2023; @szafirModelingColorDifference2018].

**Notes:** The source describes line thickness as less sensitive to size variation than point diameter.

## Use when the line is the primary colored mark <!-- role: context -->

- **User Goal:** Keep differently colored lines distinguishable while preserving as much useful color range as possible.
- **Data:** Color is already assigned to line marks, and the minimum rendered line thickness is known or can be bounded.
- **Chart Setting:** Static line charts with long strokes as the primary colored elements on standard web or desktop displays.
- **Audience:** Viewers comparing rendered line colors rather than isolated swatches.
- **Success Criterion:** The thinnest important lines remain distinguishable from neighboring line colors.

## Do not use this as-is for short line segments <!-- role: exceptions -->

**Break it when:** Most of the important marks are short line segments rather than long strokes. **Why:** The source states that for short lines below the asymptotic edge ratio, the bar model is a closer approximation.

## Tradeoffs of line-aware hue spacing <!-- role: costs -->

**Sacrifice:** More conservative spacing for thin lines reduces how many distinct color steps fit into the palette.
**Risk:** Reusing one spacing across very different line thicknesses can still fail at the thinnest lines.
**Mitigation:** Check the thinnest rendered lines and widen spacing only where the line view actually needs it.

## Common failure with line colors <!-- role: mistakes -->

**Mistake:** Reusing point-based color spacing for line charts. **Why it fails:** It underuses available color range on long lines and still does not account for the loss of discriminability on very thin lines.

## Check the thinnest rendered lines <!-- role: check -->

**Failure Sign:** Neighboring line colors collapse on the thinnest visible strokes.
**Quick Check:** Compare the thinnest rendered lines directly instead of judging the palette on large swatches.
**Stronger Test:** Compute the threshold from the minimum line thickness and verify that neighboring line colors still exceed it.

## Fix the line-color spacing <!-- role: fix -->

- Widen the hue spacing as line thickness decreases.
- Increase line thickness if the required color separation cannot be achieved.
- Use a line-specific threshold instead of a point-based threshold when choosing or refining the palette.
- If many important marks are short segments, validate them with a more conservative threshold before finalizing the chart.
