---
id: encode-threshold-probability-cumulatively-instead-of-as-density-area
title: Encode threshold probability cumulatively instead of as density area
bibliography: references.bib
description: For threshold uncertainty judgments at a timepoint, use cumulative position
  encoding on predictive distributions to improve fidelity and address area-based
  probability estimation for non-expert decision-makers.
labels:
- purpose:refine
- basis:empirical
- quality:fidelity:use
- lever:encoding
- operator:uncertainty
- channel:position:use
- channel:area:avoid
- reading-mode:lookup
---

## Cumulative threshold encoding <!-- role: advice -->

Encode threshold probability cumulatively when readers need to know whether an event will happen by or after a chosen time. For example, use a complementary cumulative distribution plot instead of a probability density plot so the chance remaining after time *t* is a direct lookup rather than an area estimate.

## Why cumulative threshold encoding works <!-- role: reason -->

A cumulative encoding turns the threshold question into a position read rather than an area-ratio judgment. That aligns the display with the user's decision question and improves consistency when people repeatedly act on the forecast.

**Mechanism:** The complementary cumulative form maps each candidate time directly to the probability still remaining after that time, so the reader does not need to infer threshold chance from the area under a density curve.

**Evidence:** In the experiment, the complementary CDF performed nearly as well as the best quantile dotplot and better than PDFs and interval plots on both mean decision quality and consistency; the design was chosen because it matched the key decision question of how delaying until a given time changes the chance of still catching the event [@fernandesUncertaintyDisplaysUsing2018].

## Use when the main question is chance by or after a chosen time <!-- role: context -->

- **User Goal:** Decide whether delaying to a chosen time is still safe.
- **Task:** Look up the probability that the event has not yet occurred at a specific threshold time.
- **Data:** A predictive distribution over future event time.
- **Chart Setting:** A compact predictive display for quick repeated decisions.
- **Audience:** Non-experts who need a direct probability readout.
- **Success Criterion:** Readers can read threshold chance directly and make more consistent choices.

## Do not use when threshold probability is not the target readout <!-- role: exceptions -->

**Break it when:** The display's main readout is not a threshold chance at a chosen time, or the reader mainly needs some other summary such as the mean. **Why:** The cumulative encoding was selected for a threshold question and is less natural when a different summary is the primary target.

## Tradeoffs of cumulative threshold encoding <!-- role: costs -->

**Sacrifice:** A cumulative plot is less direct than a density plot for showing the local peak of the distribution.
**Risk:** Readers who want the most probable value rather than a threshold chance may find the display less intuitive.
**Mitigation:** Use the complementary form when the operative question is the probability remaining after a chosen time.

## Common failure with cumulative threshold encoding <!-- role: mistakes -->

**Mistake:** Using a density plot when the reader's task is to estimate the chance after a chosen time. **Why it fails:** The reader must infer threshold probability from area, which was a worse basis for decisions in the study.

## Check whether the plot supports direct threshold lookup <!-- role: check -->

**Failure Sign:** To answer "what is the chance after time *t*?" a reviewer has to estimate an area instead of reading a value at *t*.
**Quick Check:** Pick a candidate time and verify that the remaining chance is a direct vertical lookup from the plot.
**Stronger Test:** Compare the cumulative version against a density-area version on repeated decision trials and inspect both mean expected/optimal payoff and decision variance.

## Fix density-area threshold displays <!-- role: fix -->

- Replace the density-area encoding with a complementary cumulative probability plot on the same time axis.
- Redraw the display so the value at time *t* directly represents the probability still remaining after *t*.
- Use the complementary cumulative form when the decision is explicitly about the chance of still catching the event after delaying.
