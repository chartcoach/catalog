---
id: annotate-forecast-and-inference-boundaries
title: Annotate forecast and inference boundaries explicitly
bibliography: references.bib
description: For explanatory narrative visualization that includes forecasts or inferential
  limits, use text annotation on chart regions or captions to improve trust and mitigate
  overconfident reading for readers interpreting uncertain values.
labels:
- purpose:refine
- basis:empirical
- quality:trust:use
- lever:text-annotation
- operator:uncertainty
- communication:credibility
- component:annotation:use
---

## Uncertainty annotations <!-- role: advice -->

Mark the point where observed data ends and uncertain values begin. For example, label a forecast region, note inferential limits such as margins of error or confidence intervals, or add a short note of doubt when the conclusion is tentative.

## Why uncertainty annotations work <!-- role: reason -->

Uncertainty annotations stop readers from treating estimated or extrapolated values as equally observed and equally certain. They make the chart's evidential limits visible at the place where misreading would otherwise happen.

**Mechanism:** Explicit uncertainty notes tell readers where the chart changes from observed data to extrapolation or inference, which prevents a false sense of certainty.

**Evidence:** The paper identifies representations of uncertainty as a recurring provenance technique in narrative visualization, especially through textual means such as confidence-interval descriptions, forecast or "leap-of-faith" labels, and expressions of doubt about conclusions. It also argues that these textual methods are common because visual uncertainty codes may not be commonly understood by non-experts [@hullmanVisualizationRhetoricFraming2011].

**Notes:** The paper discusses textual uncertainty annotation more directly than visual uncertainty encoding.

## Use when uncertain values are present <!-- role: context -->

- **User Goal:** Judge a trend or claim without overstating confidence.
- **Task:** Read a forecast, estimate, extrapolation, or inference-based conclusion.
- **Data:** Observed data is mixed with predicted, extrapolated, or inferentially limited values.
- **Chart Setting:** Narrative visualization with room for labels, notes, or a caption.
- **Audience:** Readers who may not share expert conventions for reading visual uncertainty.
- **Success Criterion:** A reader can point to where certainty changes and describe the limitation.

## Do not add uncertainty notes without uncertainty <!-- role: exceptions -->

**Break it when:** The chart contains only directly observed values and makes no extrapolation or inferential claim. **Why:** There is no uncertain boundary to disclose.

## Costs of uncertainty annotations <!-- role: costs -->

**Sacrifice:** You give up some visual simplicity.
**Risk:** If the note is vague, readers may still read the uncertain region as firm evidence.
**Mitigation:** Place the note at the boundary itself, not only in distant surrounding text.

## Common uncertainty annotation mistake <!-- role: mistakes -->

**Mistake:** Leaving forecast or inferred values visually continuous with observed data and adding no boundary note. **Why it fails:** Readers can easily treat the entire line or region as equally grounded in observed data.

## Check uncertainty disclosure <!-- role: check -->

**Failure Sign:** The chart includes estimated or forecasted values, but a reviewer cannot identify where they begin.
**Quick Check:** Ask a reviewer to point to the exact place where observed data ends.
**Stronger Test:** Ask the reviewer to explain one uncertainty limit after a ten-second scan of the chart.

## Fix missing uncertainty disclosure <!-- role: fix -->

- Add a direct label where extrapolated or forecasted values begin.
- Add a short note describing the inferential limit, such as margin of error or confidence interval.
- Add a brief cautionary note when the conclusion is tentative rather than definitive.
