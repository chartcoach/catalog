---
id: use-standard-uncertainty-display-with-text-explanation
title: Use a standard uncertainty display and explain it in text
bibliography: references.bib
description: For communicating uncertain estimates, use explicit uncertainty encoding
  with textual explanation on charts that display statistical confidence or uncertainty
  to improve accessibility and mitigate ambiguous interpretation for readers who need
  unambiguous chart reading.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:text-annotation
- operator:uncertainty
- component:annotation:use
- needs:cognitive
---

## Pair uncertainty marks with text <!-- role: advice -->

Use a standard uncertainty display and state in text what uncertainty it shows whenever a chart includes statistical confidence or uncertainty. For example, pair error bars, a violin plot, or gradient shading with text that explains the confidence interval or uncertainty range being shown.

## Why explicit uncertainty explanations help <!-- role: reason -->

Uncertainty marks are easy to misread when viewers must infer their meaning from appearance alone. An explicit text explanation gives viewers a direct interpretation rule and reduces ambiguity when they read uncertain results.

**Mechanism:** Standard visual uncertainty conventions signal that an estimate is not exact, and a textual explanation tells viewers what the uncertainty display represents.

**Evidence:** Chartability states that statistical confidence and uncertainty must be clearly and unambiguously communicated and that confidence intervals should use clear conventions with textual explanation [@elavskyHowAccessibleMy2022]. Research cited in the item reports that clear uncertainty conventions such as error bars, violin plots, or gradient shading combined with textual explanations improve understanding and decision-making [@fernandes_uncertainty_displays_2018].

**Notes:** The source notes that some uncertainty contexts remain difficult and that the best communication choice may not always be obvious from a cognitive accessibility or ethical standpoint.

## Use when uncertainty is shown <!-- role: context -->

- **User Goal:** Interpret or act on a result that includes statistical uncertainty.
- **Data:** The chart includes a confidence interval or another explicit uncertainty representation.
- **Chart Setting:** Uncertainty is already shown visually or needs to be added to the chart.
- **Audience:** Readers need an unambiguous explanation, including readers with cognitive accessibility needs.
- **Success Criterion:** Readers can identify that uncertainty is present and what the uncertainty display means without guessing.

## Skip when uncertainty is absent <!-- role: exceptions -->

**Break it when:** The chart does not show any statistical confidence or uncertainty. **Why:** This guideline is specifically about making uncertainty explicit and does not apply when no uncertainty is presented.

## Tradeoffs of adding uncertainty explanation <!-- role: costs -->

**Sacrifice:** The chart needs additional visual or textual content.
**Risk:** A visual uncertainty mark can still be ambiguous if the explanation is missing or unclear.
**Mitigation:** Keep the uncertainty display conventional and state directly in text what the display represents.

## Common uncertainty communication failures <!-- role: mistakes -->

- **Mistake:** Showing a confidence interval without any textual explanation. **Why it fails:** Readers must infer what the interval means, so the uncertainty is not communicated unambiguously.
- **Mistake:** Using an uncertainty display that does not follow a clear convention. **Why it fails:** Readers may not recognize the mark as uncertainty or may misread its meaning.

## Check whether uncertainty is explicit <!-- role: check -->

**Failure Sign:** The chart contains a confidence interval or uncertainty mark, but no nearby text explains what it represents.
**Quick Check:** Scan the chart text and look for a direct statement naming the confidence interval or uncertainty being shown.
**Stronger Test:** Ask a reviewer to identify the uncertainty display and explain what it means using only the chart; if they cannot do so unambiguously, fail the chart.

## Revise the uncertainty display <!-- role: fix -->

- Add text near the chart that explicitly names the confidence interval or uncertainty being shown.
- Replace an unclear custom uncertainty mark with a clear conventional uncertainty display.
- Keep the uncertainty mark and add a short explanation that states what range or confidence information the mark represents.
