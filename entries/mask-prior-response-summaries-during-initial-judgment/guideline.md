---
id: mask-prior-response-summaries-during-initial-judgment
title: Mask prior-response summaries during initial visual judgments
bibliography: references.bib
description: For individual graphical perception tasks in social visualization systems,
  avoid prior-response annotations on chart views to prevent judgment error and mitigate
  biased information cascades for viewers making objective estimates.
labels:
- purpose:refine
- basis:empirical
- quality:fidelity
- lever:interaction-access
- component:annotation:avoid
---

## Hide prior-response overlays <!-- role: advice -->

Hide prior-response overlays while viewers make an initial estimate. For example, do not place a histogram of previous answers beside a chart when the viewer's job is to judge a proportion or estimate a linear association.

## Why hiding the overlay improves accuracy <!-- role: reason -->

Visible prior answers act as social proof during perceptual judgment. When that visible summary is off target, readers shift their own estimate toward it instead of relying only on the chart.

**Mechanism:** A displayed social summary changes the center that readers treat as plausible. A summary that is farther from the true answer pulls estimates farther away and increases error.

**Evidence:** Across proportion-judgment and linear-association tasks, showing a histogram of previous answers changed estimates in the direction of the shown distribution. The farther social signal produced higher error than the closer social signal, and the paper concludes that biased social signals can reduce perceptual accuracy and should sometimes be masked [@hullmanImpactSocialInformation2011].

**Notes:** The paper also finds that aggregate social signals are not automatically better than unaided judgments, because systematic bias can make many users wrong in the same direction.

## Use when the chart includes visible prior answers <!-- role: context -->

- **User Goal:** Make an individual estimate from a chart before discussion.
- **Task:** Judge an objective visual quantity such as a proportion or a linear association.
- **Data:** Quantitative values with a known correct answer.
- **Chart Setting:** A social or collaborative chart view can display a histogram or similar summary of previous answers next to the chart.
- **Audience:** Viewers submit their own estimate independently.
- **Success Criterion:** Lower estimation error on the individual judgment.

## Do not use when the social summary is already validated for this task <!-- role: exceptions -->

**Break it when:** Prior testing shows that the displayed social summary is less biased for the same task than viewers' unaided judgments. **Why:** The study found that a closer social signal produced lower error than a farther one.

## Tradeoffs of hiding the overlay <!-- role: costs -->

**Sacrifice:** You give up any benefit from a well-calibrated social summary.
**Risk:** Removing the summary can also remove a cue that helps viewers coordinate around a correct answer when the signal is accurate.
**Mitigation:** Keep the summary suppressed unless testing shows that it improves accuracy for that exact task.

## Common failure mode: assuming the crowd summary is harmless <!-- role: mistakes -->

**Mistake:** Adding a previous-answer summary because the average response looks like collective intelligence. **Why it fails:** When viewers share a systematic bias, the displayed aggregate can be wrong in the same direction and can pull later viewers away from the truth.

## How to test whether the overlay is distorting judgment <!-- role: check -->

**Failure Sign:** Answers cluster around the displayed social center instead of the chart evidence.
**Quick Check:** Compare the same chart with and without the prior-response summary; the overlay fails if estimates move toward the shown summary without reducing error.
**Stronger Test:** Seed two versions of the same chart with different prior-response summaries and check whether the version with the farther summary produces larger error.

## What to change <!-- role: fix -->

- Remove the prior-response summary from the chart used for the initial estimate.
- Suppress the summary on tasks where pilot tests show higher error than a no-social version.
- Keep the summary only when you have validated that it improves accuracy for that same judgment task.
