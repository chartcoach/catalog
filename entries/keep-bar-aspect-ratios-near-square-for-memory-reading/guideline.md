---
id: keep-bar-aspect-ratios-near-square-for-memory-reading
title: Keep bar aspect ratios near square for memory-based value reading
bibliography: references.bib
description: For exact recall of bar values across separated views, prefer near-square
  mark aspect ratios on bar charts to improve recall fidelity and mitigate overestimation
  of wide bars and underestimation of tall bars for viewers making memory-based readings.
labels:
- purpose:refine
- basis:empirical
- task:retrieve
- chart:bar
- quality:fidelity
- lever:encoding
- reading-mode:exact
---

## Bar aspect ratio <!-- role: advice -->

Keep bar aspect ratios near square when readers must remember bar-top positions after the chart disappears. For example, in a bar chart avoid very wide bars that are later recalled too high and very tall bars that are later recalled too low; square bars showed no systematic bias.

## Why near-square bars work <!-- role: reason -->

Bar-top position was not remembered independently of the bar's shape. Memory for the mark was pulled toward a prototypical square, so wide bars were recalled as higher and tall bars were recalled as lower.

**Mechanism:** A bar's incidental width:height ratio changes the remembered top position even when position is the intended encoding. Keeping the mark closer to square reduces this shape-driven pull and preserves more accurate value recall.

**Evidence:** Across three experiments, wide bars were overestimated, tall bars were underestimated, square bars were not systematically biased, and the same aspect-ratio pattern remained when area was controlled or varied, showing that aspect ratio rather than area drove the bias [@cejaTruthSquareAspect2021].

**Notes:** Tall bars also produced larger absolute error and variability than square or wide bars.

## When to use near-square bars <!-- role: context -->

- **User Goal:** Remember or report an exact bar value after a short delay.
- **Task:** Reproduce or compare bar-top positions from a previous view.
- **Data:** Quantitative values encoded by vertical position in bars.
- **Chart Setting:** The original bar will not stay visible during the judgment, and the layout can make bars very wide or very tall.
- **Audience:** Viewers making memory-based readings.
- **Success Criterion:** Minimize systematic overestimation of wide bars and underestimation of tall bars.

## When not to rely on this rule alone <!-- role: exceptions -->

**Break it when:** The original bar remains simultaneously visible during the comparison or tracing response. **Why:** The tested wide-versus-tall memory-bias pattern did not persist under direct concurrent perception.

## Tradeoffs of controlling bar aspect ratio <!-- role: costs -->

**Sacrifice:** This rule limits freedom to stretch bars into very wide or very tall shapes as a layout choice.\
**Risk:** Applying the same correction outside bar charts assumes the same effect without direct test.\
**Mitigation:** Use this rule directly for bar charts and treat other mark types as separate review cases.

## Common aspect-ratio mistakes <!-- role: mistakes -->

**Mistake:** Changing bar area while leaving the bars distinctly wide or tall. **Why it fails:** Area did not account for the bias pattern; wide bars still skewed high and tall bars still skewed low.

## How to check for aspect-ratio bias risk <!-- role: check -->

**Failure Sign:** Bars are visibly elongated and the reader must recall them from a prior view.\
**Quick Check:** Inspect the width:height ratios of the bars; if they are clearly wide or clearly tall, expect directional recall bias.\
**Stronger Test:** Hide the chart briefly and ask reviewers to reproduce a bar's top position; systematic positive error on wide bars or negative error on tall bars indicates the problem.

## How to fix elongated bars <!-- role: fix -->

- Reduce extreme width:height ratios so the bars are closer to square.
- Resize the chart region or reallocate panel space when the current layout creates very wide or very tall bars.
- Avoid using elongated bars for tasks that require exact value recall after the chart disappears.
- If exact comparison must happen across views, keep a visible reference bar onscreen instead of relying only on memory.
