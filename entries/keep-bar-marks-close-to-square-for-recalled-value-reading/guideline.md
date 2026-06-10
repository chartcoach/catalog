---
id: keep-bar-marks-close-to-square-for-recalled-value-reading
title: Keep bar marks close to square when readers must recall single values
bibliography: references.bib
description: For retrieve-value tasks involving recalled single values, prefer square
  bar aspect ratios on bar charts to improve fidelity and mitigate systematic overestimation
  and underestimation for viewers comparing values across separate views.
labels:
- purpose:refine
- basis:empirical
- task:retrieve
- scope:single-result
- chart:bar
- reading-mode:exact
- quality:fidelity
- lever:encoding
---

## Square bar aspect ratios <!-- role: advice -->

Make single bar marks close to square when readers must recall a value from memory. For example, revise a bar chart so the target bar is near a 1:1 aspect ratio instead of very wide or very tall, because wide bars were remembered too high, tall bars were remembered too low, and square bars showed no systematic bias.

## Why square-like bars work for recalled values <!-- role: reason -->

Remembered bar height is not read from position alone. The bar's aspect ratio shifts the recalled top edge toward a more square-like shape, which changes the reproduced value upward for wide bars and downward for tall bars.

**Mechanism:** Square bar marks reduce the incidental shape cue that distorts remembered height, so recalled values stay closer to the encoded value.

**Evidence:** In controlled bar-chart experiments for single-value retrieval, wide aspect ratios were significantly overestimated, tall aspect ratios were significantly underestimated, square aspect ratios showed no systematic bias, and the bias pattern was present in memory-based responses rather than concurrent tracing of a visible bar [@zengReviewCollationGraphical2023; @cejaTruthSquareAspect2021].

**Notes:** Changing bar area alone did not account for the bias pattern.

## Use when delayed or cross-view recall matters <!-- role: context -->

- **User Goal:** Recall or compare a single bar value after the original bar is no longer visible.
- **Task:** Retrieve an exact value from a single bar.
- **Data:** One quantitative value encoded by a rectangular bar mark.
- **Chart Setting:** The value will be judged across separate views, separate graphs, or after a brief delay.
- **Audience:** Readers who must remember individual bar values.
- **Success Criterion:** Minimize signed error in recalled bar height.

## Do not use when the source bar stays visible <!-- role: exceptions -->

**Break it when:** Readers can match the response directly against the original bar while that original bar remains visible on screen. **Why:** The wide-versus-tall recall bias pattern did not persist in the tracing condition, so memory-based aspect-ratio distortion is not the main failure there.

## Tradeoffs of enforcing square-like bars <!-- role: costs -->

**Sacrifice:** You give up freedom to use very wide or very tall bars for the target value.
**Risk:** Applying this rule blindly to direct on-screen matching can target the wrong problem.
**Mitigation:** Reserve the change for bars that will be read from memory, across time, or across separate views.

## Common failures when adjusting bar shape <!-- role: mistakes -->

- **Mistake:** Leaving target bars very wide or very tall because position is assumed to stay precise on its own. **Why it fails:** The incidental aspect ratio changes the remembered top position.
- **Mistake:** Trying to fix the problem by changing bar area without correcting aspect ratio. **Why it fails:** The tested bias pattern tracked aspect ratio, not area alone.

## How to check for aspect-ratio recall bias <!-- role: check -->

**Failure Sign:** Wide bars are remembered as higher than they were, or tall bars are remembered as lower than they were.
**Quick Check:** Inspect any bar used for delayed or cross-view reading and flag it if it is much wider than tall or much taller than wide.
**Stronger Test:** Show the chart briefly, hide it, ask a reviewer to place the bar top from memory, then repeat with a square-bar version and compare signed error.

## How to fix the chart <!-- role: fix -->

- Resize the plot region or adjust bar width so the target bar moves closer to a 1:1 aspect ratio.
- Replace very wide target bars with square-like bars when recalled values run high.
- Replace very tall target bars with square-like bars when recalled values run low.
- If the chart will be read across separate views, test a square-bar variant before finalizing it.
