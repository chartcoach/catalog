---
id: avoid-full-range-context-for-midpoint-values
title: Avoid full-range context when values near 50% must be read without bias
bibliography: references.bib
description: For exact single-value reading of part-to-whole data, avoid full-range
  contextual encoding on bar or dot charts to prevent midpoint bias and mitigate systematic
  underestimation below 50% and overestimation above 50% for readers judging values
  near the middle of the scale.
labels:
- purpose:refine
- basis:empirical
- task:retrieve
- quality:fidelity:use
- lever:encoding
- operator:part-whole
- reading-mode:exact
---

## Reduce full-range context near midpoints <!-- role: advice -->

Avoid integrating a target mark with a visible 0–100% whole when readers must read a value near 50% without bias. For example, use a stand-alone bar instead of a stacked bar, or keep a dot separate from the axis rather than placing it directly on the axis, when the important values sit around 50%.

## Why full-range context biases midpoint values <!-- role: reason -->

Visible whole-range context creates an implicit halfway category. Readers then remember values as farther from that category boundary than they were, which shifts values below 50% downward and values above 50% upward.

**Mechanism:** A visible 0–100% frame helps people estimate magnitude, but it also creates a salient 50% boundary that repels remembered values away from the midpoint.

**Evidence:** Across the paper’s bar and dot experiments, integrated context reduced overall unsigned error but produced a consistent signed-error pattern around 50%: values from 25–49% were underestimated and values from 51–75% were overestimated. The paper explicitly recommends avoiding stacked bars for nearly equal values around 50/50 when precision is critical [@mccolemanNoMarkIsland2021].

**Notes:** The midpoint bias was strongest in the integrated conditions.

## Use when exact midpoint reading matters <!-- role: context -->

- **User Goal:** Read or remember one proportion without systematic bias.
- **Task:** Exact value reading or reproduction, especially for values that sit on opposite sides of 50%.
- **Data:** Single part-to-whole values on a 0–100% scale.
- **Chart Setting:** The mark would otherwise be shown with a visible whole, such as a stacked bar, a reference bar, or a dot placed directly on an axis.
- **Success Criterion:** Minimize systematic underestimation below 50% and overestimation above 50%.

## Do not use when overall error matters more than midpoint neutrality <!-- role: exceptions -->

**Break it when:** Overall unsigned error across the full range matters more than unbiased reading around 50%, or the important values are very high proportions near 100%. **Why:** The added whole-range context lowered overall error, and the paper notes that it can help with very high values.

## Costs of removing full-range context <!-- role: costs -->

**Sacrifice:** You give up some of the accuracy benefit that comes from a visible 0% and 100% frame.
**Risk:** Stand-alone values can have more overall error, especially at large magnitudes.
**Mitigation:** Apply reduced context mainly when the key values cluster around 50% or cross that midpoint.

## Common midpoint-context mistake <!-- role: mistakes -->

**Mistake:** Keeping a stacked bar or axis-integrated mark for a near-even comparison such as 48% versus 52%. **Why it fails:** The visible whole can push the lower value down and the higher value up, making the difference look larger than it is.

## Check midpoint bias risk <!-- role: check -->

**Failure Sign:** Critical values fall in the 25–49% or 51–75% range and are shown with a visible whole.
**Quick Check:** Make a stand-alone version of the same values and compare it with the integrated version before finalizing the chart.
**Stronger Test:** Show sample values just below and above 50% briefly and ask people to redraw them; watch for underestimation below 50% and overestimation above 50%.

## Fix midpoint bias by separating the mark from the whole <!-- role: fix -->

- Unstack the focal value so it is shown as a stand-alone bar rather than as a segment of a stacked bar.
- Remove full-range integration from the focal mark, such as drawing the dot away from the axis instead of directly on it.
- Keep the reduced-context version for values whose interpretation depends on a neutral read around 50%.
