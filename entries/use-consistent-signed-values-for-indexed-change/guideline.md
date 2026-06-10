---
id: use-consistent-signed-values-for-indexed-change
title: Use signed values consistently for indexed change
bibliography: references.bib
description: For explaining ordered-time values indexed to a reference timepoint,
  use signed value formatting on the y-axis and in tooltips of an indexed chart to
  improve readability and mitigate mistaken readings of direction for general audiences.
labels:
- purpose:refine
- basis:heuristic
- time:ordered-time
- operator:difference
- quality:readability
- lever:text-annotation
- component:axis:use
- component:tooltip:use
- audience:general-public
---

## Repeat signed change formatting <!-- role: advice -->

Format every displayed value as change from the reference point, and keep that sign consistent across the y-axis and tooltips. For example, show “−11%” instead of plain “11” on the axis and in tooltip readouts when a historical value sits below the reference value.

## Why repeated signed values reinforce the chart’s meaning <!-- role: reason -->

Consistent signed formatting keeps readers in the same frame wherever they look. The number reads as distance from the reference point each time, instead of flipping between an indexed comparison and an unsigned standalone quantity.

**Mechanism:** Repeating the same signed framing on the axis and in tooltips reinforces direction and prevents readers from dropping the reference-point interpretation when they inspect individual values.

**Evidence:** The source recommends “repeating these concepts in symbolic terms” by putting the whole y-axis and every tooltip value in terms of a negative percentage, such as showing “−11%” instead of plain “11” [@mintzer_y_axis_2024].

## Use when the chart shows values below a reference point <!-- role: context -->

- **User Goal:** Emphasize that the current value is the high point and earlier values are below that benchmark.
- **Task:** Help readers read the direction of indexed difference at each timepoint.
- **Data:** A time series indexed to a reference period, with historical values shown as negative relative change.
- **Chart Setting:** The chart prints values both on the y-axis and in tooltip readouts.
- **Audience:** Readers who do not immediately understand the index.
- **Success Criterion:** Readers interpret sample values as being below or at the reference point rather than as standalone rates.

## Do not use on non-indexed values <!-- role: exceptions -->

**Break it when:** The chart is not showing change from a reference point. **Why:** A repeated negative percentage or signed change format would misstate direct values.

## Trade off brevity for consistency <!-- role: costs -->

**Sacrifice:** Axis labels and tooltip numbers become less compact.
**Risk:** If only the axis or only the tooltip uses signed change formatting, readers see two different framings for the same quantity.
**Mitigation:** Apply the same signed format everywhere the indexed value is printed.

## Common formatting mismatch <!-- role: mistakes -->

**Mistake:** Mixing signed and unsigned versions of the same indexed value across the axis and tooltip. **Why it fails:** Readers lose the directional cue that tells them the value is below the reference point.

## Check whether value formatting stays in one frame <!-- role: check -->

**Failure Sign:** A tooltip shows a plain positive number while the axis describes negative distance from the reference point, or vice versa.
**Quick Check:** Inspect one historical point and compare its y-axis label format to its tooltip format.
**Stronger Test:** Ask a reviewer whether a sample printed value is above or below the reference point without letting them rely on surrounding text.

## Align the printed values <!-- role: fix -->

- Add signed change formatting to the y-axis labels.
- Apply the same signed format to tooltip values.
- Remove unsigned duplicates of the same indexed quantity.
