---
id: animate-individual-draws-for-uncertain-ordering-comparisons
title: Animate individual draws for uncertain ordering comparisons
bibliography: references.bib
description: For comparison tasks on a few uncertain quantitative variables, use animated
  individual draws on uncertainty displays to improve ordering-estimate fidelity and
  mitigate misreading of variable-order reliability for readers without specialized
  statistical training.
labels:
- purpose:refine
- basis:empirical
- task:compare
- quality:fidelity
- lever:interaction-access
- operator:uncertainty
- measure:multi
- group-cardinality:few
- temporal-pattern:dynamic
---

## Animated individual draws <!-- role: advice -->

Use animated individual draws rather than static uncertainty summaries when viewers must estimate how often one quantity exceeds another across a small set of variables. For example, replace error bars or violin plots with a HOP-style animation when readers need an out-of-100 judgment for comparisons such as one variable exceeding another or one variable exceeding both of two others.

## Why animated draws work for ordering judgments <!-- role: reason -->

Animated individual draws turn an abstract probability comparison into repeated concrete outcomes that viewers can count or visually integrate. That reduces the need to infer a joint distribution from static intervals or density shapes.

**Mechanism:** One draw per frame lets viewers judge a direct outcome like “is B larger than A in this case?” instead of translating overlap or area into a probability estimate.

**Evidence:** In the experiment, animated HOPs produced much lower mean absolute error than both error bars and violin plots for all bivariate ordering tasks and for the trivariate “B larger than both others” task, including a correlated bivariate case [@hullmanHypotheticalOutcomePlots2015].

## Use when ordering reliability is the question <!-- role: context -->

- **User Goal:** Judge how reliable an ordering is across uncertain quantities.
- **Task:** Estimate how often one variable is larger than another, or larger than both of two others.
- **Data:** Two or three quantitative distributions; the variables may be independent or correlated.
- **Chart Setting:** The display is communicating uncertainty and can use either a static summary or an animated sequence of draws.
- **Audience:** Lay or otherwise untrained readers.
- **Success Criterion:** Lower absolute error in out-of-100 judgments about ordering frequency.

## Do not use when the job is a single-variable mean readout <!-- role: exceptions -->

**Break it when:** The viewer’s job is to estimate the mean of one high-variance distribution. **Why:** The study found animated draws worse than static summaries for that univariate mean task.

## Costs of animated draws <!-- role: costs -->

**Sacrifice:** Viewers must integrate information across multiple frames instead of reading one static summary.
**Risk:** A finite number of viewed frames introduces sampling imprecision.
**Mitigation:** Reserve animated draws for small-set ordering questions, where the study found clear accuracy gains.

## Common failure mode with static summaries <!-- role: mistakes -->

**Mistake:** Use error bars or violin plots and still ask viewers to estimate how often one uncertain value exceeds another. **Why it fails:** Readers made very large errors on these ordering questions and sometimes gave implausible answers even when the higher-mean variable should usually be larger.

## Check ordering accuracy directly <!-- role: check -->

**Failure Sign:** Readers give widely scattered ordering-frequency estimates or answer below 50% when the higher-mean variable should usually be larger.
**Quick Check:** Show the same two- or three-variable comparison in a HOP-style version and a static-summary version, then ask for an out-of-100 estimate of the ordering frequency.
**Stronger Test:** Compute absolute error against the known probability and keep the version with the smaller error.

## Switch the uncertainty display to animated draws <!-- role: fix -->

- Replace the static uncertainty summary with an animation that shows one draw per frame.
- Swap error bars for the animated draw sequence when the question is “how often is B larger than A?”
- Swap violin plots for the animated draw sequence when the question is “how often is one variable the largest?”
- Keep the axis mapping fixed across frames so viewers can compare positions from frame to frame.
