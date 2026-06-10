---
id: encode-uncertain-time-predictions-as-a-low-density-quantile-dotplot
title: Encode uncertain time predictions as a low-density quantile dotplot
bibliography: references.bib
description: For quick repeated threshold decisions, use a discrete frequency encoding
  on uncertain time-to-event predictions to improve fidelity and address oversimplified
  interval summaries for non-expert users.
labels:
- purpose:refine
- basis:empirical
- chart:dotplot:use
- quality:fidelity:use
- lever:encoding
- operator:uncertainty
- density:sparse
---

## Discrete outcome uncertainty encoding <!-- role: advice -->

Encode the predictive distribution as a low-density quantile dotplot when users need to judge several possible cutoff times from an uncertain time prediction. For example, place 20 or 50 equally likely dots on the time axis instead of only showing an interval summary; the 50-dot version was the best-performing display in the study.

## Why discrete outcome encoding works <!-- role: reason -->

A low-density quantile dotplot lets readers estimate threshold chances by counting visible outcomes instead of inferring probability from area or from one preselected interval. That makes the display easier to adapt to changing tradeoffs and helps people learn a more consistent decision strategy over repeated use.

**Mechanism:** The dotplot exposes the distribution shape while keeping the probability readout close to a count of equally likely outcomes, which supports quick interval estimation and repeated calibration.

**Evidence:** In the incentivized transit decision experiment, the 50-dot quantile dotplot reached about 97% of optimal expected payoff by the final trial and about a 3 percentage point within-subject standard deviation, roughly 5 points better and 4 points more consistent than the no-uncertainty control; both low-density dotplot variants were among the best-performing displays and outperformed interval displays [@fernandesUncertaintyDisplaysUsing2018].

## Use when repeated threshold choices depend on uncertain arrival time <!-- role: context -->

- **User Goal:** Choose when to act so as to balance waiting against missing an uncertain event.
- **Task:** Judge the chance that an event will occur before or after several candidate times.
- **Data:** A predictive distribution over a future time-to-event.
- **Chart Setting:** A glanceable, space-constrained display that will be used repeatedly.
- **Audience:** Non-experts making in-the-moment decisions.
- **Success Criterion:** Decisions stay close to optimal and become more consistent over repeated use.

## Do not use when one fixed interval is enough <!-- role: exceptions -->

**Break it when:** One fixed probability interval is already known to represent the best decision across situations. **Why:** The main benefit of the dotplot is letting readers adapt to different thresholds instead of being locked to one summary interval.

## Tradeoffs of discrete outcome encoding <!-- role: costs -->

**Sacrifice:** A dotplot shows more of the distribution than a single interval summary.
**Risk:** Extra detail can be unnecessary when users only need one fixed threshold.
**Mitigation:** Keep the dotplot low density, such as 20 or 50 outcomes.

## Common failure with discrete outcome encoding <!-- role: mistakes -->

**Mistake:** Using only an interval summary when readers need to inspect several possible cutoff times. **Why it fails:** The reader cannot flex the display to different risk tradeoffs as the costs of waiting and missing change.

## Check whether the dotplot supports threshold reading <!-- role: check -->

**Failure Sign:** A reviewer cannot quickly tell the chance of the event occurring after two or three candidate times.
**Quick Check:** Pick several times on the axis and verify that the probability after each time can be estimated by visible counting of equally likely dots.
**Stronger Test:** Compare the dotplot against an interval-only version on repeated decision trials and inspect both mean expected/optimal payoff and within-user variability.

## Fix interval-only summaries <!-- role: fix -->

- Replace the interval-only summary with 20 or 50 equally likely dots positioned on the existing time axis.
- Keep the dotplot low density rather than packing in more outcomes.
- If the current display shows only a most-probable time, replace that lone summary with the dot distribution on the same axis.
