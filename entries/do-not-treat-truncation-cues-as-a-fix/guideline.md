---
id: do-not-treat-truncation-cues-as-a-fix
title: Do not treat truncation cues as a fix for a non-zero y-axis
bibliography: references.bib
description: For truncated quantitative bar charts where readers should judge effect
  size without added emphasis, avoid using broken-axis or gradient continuation cues
  as the fix for a non-zero y-axis to prevent exaggerated perceived effect size and
  address false confidence that disclosure alone removes the distortion for readers
  comparing small differences.
labels:
- purpose:refine
- basis:empirical
- chart:bar
- lever:scale-order
- component:axis
- quality:fidelity:use
---

## Treat truncation cues as disclosure, not correction <!-- role: advice -->

Do not use a broken-axis mark or a gradient-bottom bar as the fix for a truncated y-axis. For example, broken-axis bars and gradient-bottom bars produced perceived-severity inflation similar to standard truncated bars, so keep those cues only as disclosure and separately reconsider the axis range.

## Why truncation cues do not remove the exaggeration <!-- role: reason -->

A visible cue can tell readers that the axis has been cut, but it does not stop the marks from looking visually amplified. Readers still react to the exaggerated bar heights before any cue can fully neutralize that impression.

**Mechanism:** Subjective effect-size judgments remain driven by the visual magnification created by truncation, so disclosure of the cut axis does not by itself debias the chart.

**Evidence:** In experiments comparing standard truncated bars, broken-axis bars, and gradient-bottom bars, the alternative designs did not significantly reduce perceived severity relative to ordinary truncated bars; the review paper records this study as empirical graphical-perception evidence for recommendation systems and critique rules [@correllTruncatingYAxisThreat2020; @zengReviewCollationGraphical2023].

## Use when all are true <!-- role: context -->

- **User Goal:** Show small differences in a bar chart without making them feel larger than intended.
- **Task:** Compare the importance or severity of differences between bar values.
- **Data:** Quantitative values displayed as bar heights with a non-zero y-axis start.
- **Chart Setting:** A static truncated bar chart that uses a broken axis or gradient continuation cue.
- **Success Criterion:** The cue helps disclose truncation without being mistaken for a correction of truncation bias.

## Do not use when any are true <!-- role: exceptions -->

**Break it when:** The axis is not truncated. **Why:** The paper notes that broken-axis and continuation cues are inappropriate without truncation and should collapse back to a standard bar chart.

## Costs of relying on truncation cues <!-- role: costs -->

**Sacrifice:** You add extra chart treatment without gaining a reliable reduction in perceived-severity inflation.\
**Risk:** Reviewers may assume the chart has been debiased simply because the truncation is visibly marked.\
**Mitigation:** Use the cue only to disclose the cut axis, then separately justify whether truncation is warranted at all.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Adding a broken-axis mark or gradient cue and assuming the chart is no longer misleading. **Why it fails:** The study found similar perceived-severity inflation across standard truncated, broken-axis, and gradient designs.

## Check whether the cue actually helps <!-- role: check -->

**Failure Sign:** The broken-axis or gradient version feels just as dramatic as the ordinary truncated bar chart.\
**Quick Check:** Compare the indicated version directly against the standard truncated version and ask whether effect severity still feels the same.\
**Stronger Test:** Ask a reviewer to rate perceived severity across the standard, broken-axis, and gradient versions; if the ratings stay similar, the cue is not solving the problem.

## Fix the chart after the cue fails <!-- role: fix -->

- Restore a 0-baseline when the inflated effect is not intentional.
- Keep the broken-axis or gradient treatment only as disclosure, not as the main correction.
- Re-evaluate whether the narrower y-axis range is the right framing for the message.
- If truncation remains necessary, review the truncated chart against a 0-baseline alternative before publishing.
