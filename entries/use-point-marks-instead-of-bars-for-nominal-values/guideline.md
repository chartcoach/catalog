---
id: use-point-marks-instead-of-bars-for-nominal-values
title: Use point marks instead of bars for nominal values
bibliography: references.bib
description: For categorical lookup on charts with nominal values, prefer point-mark
  charts over bar charts to prevent false ordering cues and address misleading length
  comparisons for readers interpreting unordered categories.
labels:
- purpose:select
- basis:empirical
- data:categorical
- chart:dotplot:use
- chart:bar:avoid
- quality:fidelity:use
- lever:chart-family
---

## Replace bars with points for nominal categories <!-- role: advice -->

Use point marks rather than bar length when the encoded values are nominal and unordered. For example, replace a bar chart with a plot chart that places a point at each category position, so the display does not suggest that one category is longer, larger, or better than another.

## Why bars misstate nominal data <!-- role: reason -->

Bars carry length, and length invites readers to interpret order or magnitude. That implication is harmless for ordered or quantitative values, but it is wrong for a nominal set.

**Mechanism:** Point marks show membership in a category without adding a length comparison that the data do not support.

**Evidence:** The paper gives an example where a bar chart incorrectly implies ordering for a nationality relation and contrasts it with a plot chart as the correct way to encode a nominal domain set [@mackinlayAutomatingDesignGraphical1986].

## Use when the value set has no inherent order <!-- role: context -->

- **User Goal:** Show which category each item belongs to without implying rank.
- **Task:** Read nominal categories correctly.
- **Data:** The encoded domain is nominal rather than ordered or quantitative.
- **Chart Setting:** A bar chart is a candidate only because it is familiar, not because the values have magnitude.
- **Success Criterion:** Readers do not infer a false ordering from the display.

## Use bars only when the values are ordered or quantitative <!-- role: exceptions -->

**Break it when:** The encoded values form an ordered or quantitative set. **Why:** Then length can legitimately encode the ordering or magnitude.

## Tradeoffs of removing bars <!-- role: costs -->

**Sacrifice:** You give up a length cue that can support ordered comparisons.
**Risk:** A point-based display no longer provides magnitude judgments, which is correct here but may disappoint readers expecting bar lengths.
**Mitigation:** Reserve bars for data that truly have order or quantity.

## Common nominal-data failure <!-- role: mistakes -->

**Mistake:** Draw bars for nominal categories and rely on the reader to ignore the lengths. **Why it fails:** The lengths still suggest an ordering relationship that is not in the data.

## Check whether the chart implies an order that does not exist <!-- role: check -->

**Failure Sign:** The viewer can describe one nominal category as longer, larger, or better than another from the marks alone.
**Quick Check:** Compare a bar version and a point-mark version; if only the bar version creates a visible ranking, keep the point-mark version.
**Stronger Test:** Ask whether any mark length in the chart encodes a magnitude that the data do not actually contain.

## Remove the misleading length cue <!-- role: fix -->

- Replace the bars with points positioned at the category values.
- Keep the category labels on the axes and let the point positions carry the relation.
- Reserve bar length for ordered or quantitative values only.
