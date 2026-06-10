---
id: integrate-very-high-ratio-values-with-the-full-range
title: Integrate very high ratio values with the full 100% range
bibliography: references.bib
description: "For exact reading of high part-to-whole values, use integrated full-range\
  \ encoding on bar charts to improve fidelity and mitigate underestimation of large\
  \ values for readers judging values near the top of a 0\u2013100% scale."
labels:
- purpose:refine
- basis:empirical
- task:retrieve
- chart:bar
- quality:fidelity:use
- lever:encoding
- operator:part-whole
- reading-mode:exact
---

## Add the full-range endpoint for very high values <!-- role: advice -->

Integrate a very high proportion with its 0–100% whole when accurate reading of the large value matters more than neutral midpoint reading. For example, use a stacked bar instead of a lone bar when the key value is near the top of the scale, such as around 95%, so the 100% endpoint becomes an extra reference.

## Why the full range helps at the top end <!-- role: reason -->

Large stand-alone values tend to be read low. A visible endpoint gives readers a second anchor, so a very high value can be judged as a small distance from 100% instead of only as a long distance from 0%.

**Mechanism:** In a stacked bar, a value such as 95% can be interpreted from the top endpoint as well as from the bottom baseline, which reduces the underestimation seen for large stand-alone magnitudes.

**Evidence:** The paper found that smaller values were overestimated and larger values were underestimated, while integrated context lowered overall unsigned error. It specifically recommends stacked bars when the important values are high, noting that a value like 95% benefits from the visible 100% endpoint [@mccolemanNoMarkIsland2021].

**Notes:** This is a precision tradeoff, not a universal preference for stacked bars.

## Use when high values are the critical readout <!-- role: context -->

- **User Goal:** Read a high percentage accurately.
- **Task:** Exact single-value reading or recall near the upper end of a 0–100% scale.
- **Data:** One part-to-whole value close to 100%.
- **Chart Setting:** A bar chart where the value can be shown alone or as part of a full stacked 100% bar.
- **Success Criterion:** Reduce underestimation of large values.

## Do not use when midpoint neutrality is the priority <!-- role: exceptions -->

**Break it when:** The important values lie around 50%, or small differences across 50% must remain unbiased. **Why:** Integrated context introduces a midpoint repulsion effect that can push values below 50% lower and values above 50% higher.

## Costs of adding the full range <!-- role: costs -->

**Sacrifice:** You give up neutral reading around the midpoint.
**Risk:** A stacked whole can exaggerate differences for values on opposite sides of 50%.
**Mitigation:** Reserve the integrated form for very high ratios or for cases where lower overall error matters more than midpoint neutrality.

## Common high-value encoding mistake <!-- role: mistakes -->

**Mistake:** Leaving a very high ratio as a lone bar when exact reading near 100% matters. **Why it fails:** Large stand-alone values are systematically prone to underestimation.

## Check whether a high value needs the full range <!-- role: check -->

**Failure Sign:** Important values are near the top of the scale and readers tend to read them low.
**Quick Check:** Compare a lone-bar version and a stacked-to-100% version for the same high values.
**Stronger Test:** Test sample values near the top of the scale and keep the version with lower absolute error.

## Fix underestimation of very high values <!-- role: fix -->

- Stack the value to a visible 100% whole instead of showing it as a lone bar.
- Make the full-range endpoint visible so the top of the bar can serve as an additional reference.
- If the critical values move toward 50%, switch back to a stand-alone bar.
