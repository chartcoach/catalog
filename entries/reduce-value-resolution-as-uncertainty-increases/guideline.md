---
id: reduce-value-resolution-as-uncertainty-increases
title: Reduce value resolution as uncertainty increases
bibliography: references.bib
description: For decision tasks on bivariate color maps that combine value and uncertainty,
  use value-suppressing quantization on uncertain regions to improve uncertainty-aware
  choices and mitigate overinterpretation of noisy data for decision-makers.
labels:
- purpose:refine
- basis:empirical
- task:compare
- quality:trust:use
- lever:encoding
- operator:uncertainty
- audience:decision-maker
- reading-mode:overview
---

## Suppress value detail in high-uncertainty regions <!-- role: advice -->

Allocate more distinct value colors where uncertainty is low and fewer where uncertainty is high. For example, use a tree-like bivariate palette that preserves many low-uncertainty value bins but collapses the highest-uncertainty cases toward a common light or gray mark instead of keeping equal value resolution across the whole legend.

## Why suppressing uncertain values changes decisions <!-- role: reason -->

When high-uncertainty marks still show many distinct values, readers can overread noisy differences. Suppressing value detail in those regions makes uncertainty hard to ignore and shifts attention toward comparisons that are better supported.

**Mechanism:** Value suppression limits fine-grained distinctions exactly where the data are least reliable, which encourages more cautious choices and discourages strong conclusions in noisy regions.

**Evidence:** In the paper's prediction experiment, value-suppressing palettes led participants to avoid very high-uncertainty choices and to accept slightly worse nominal value rather than act on the riskiest regions, compared with traditional bivariate maps [@correllValueSuppressingUncertaintyPalettes2018].

## Use when uncertainty should downweight decisions <!-- role: context -->

- **User Goal:** Choose among locations or alternatives while accounting for both payoff and uncertainty.
- **Task:** Risk-sensitive comparison or selection.
- **Data:** Quantitative values with associated uncertainty, including regions with meaningfully high uncertainty.
- **Chart Setting:** A discrete superimposed bivariate color map whose legend can assign fewer outputs to high-uncertainty cases.
- **Audience:** Decision-makers or general readers asked to act on uncertain information.
- **Success Criterion:** More cautious choices and fewer strong judgments based on the noisiest data.

## Do not use when uncertain values must stay distinguishable <!-- role: exceptions -->

- **Break it when:** The task depends on preserving rare, highly uncertain possibilities such as long-tail risks or black-swan outcomes. **Why:** Suppression intentionally downweights uncertain values.
- **Break it when:** The task requires more, not less, discrimination at high uncertainty, such as filtering out outliers in uncertain data. **Why:** The palette removes fine distinctions where uncertainty is high.

## What you give up with value suppression <!-- role: costs -->

**Sacrifice:** You give up fine-grained differentiation among uncertain values.
**Risk:** Important differences in high-uncertainty regions can be hidden if those regions still matter to the task.
**Mitigation:** Use suppression only when uncertainty should explicitly reduce analytical weight.

## Common failures around uncertainty suppression <!-- role: mistakes -->

- **Mistake:** Keep equal value resolution at every uncertainty level. **Why it fails:** Readers still see distinct value differences in regions where the signal is least reliable.
- **Mistake:** Change only the legend shape to a wedge without actually reducing the number of high-uncertainty bins. **Why it fails:** The paper found no significant performance or decision change from wedge versus square legends by themselves.

## Check whether high-uncertainty regions are still overread <!-- role: check -->

**Failure Sign:** The noisiest regions still contain many distinct value colors, or reviewers keep selecting them because of their nominal value alone.
**Quick Check:** Compare the current equal-resolution palette with a suppressed palette on one decision task that requires weighting uncertainty.
**Stronger Test:** Inspect whether decisions in the revised chart avoid the highest-uncertainty regions without simply shifting all choices to the safest few cells.

## Edit the palette to downweight noisy regions <!-- role: fix -->

- Merge the highest uncertainty levels into fewer value bins.
- Add a top uncertainty level that collapses to one common output regardless of value.
- Rebuild the legend so the available value categories narrow as uncertainty increases.
- Do not rely on legend shape alone; change the underlying quantization.
