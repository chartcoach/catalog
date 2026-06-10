---
id: use-continuous-uncertainty-encoding-for-new-study-estimates
title: Use a continuous uncertainty encoding for new-study estimates
bibliography: references.bib
description: For estimating replication uncertainty for a new reported experiment,
  prefer a continuous encoding on interactive uncertainty displays to improve fidelity
  and address misestimation from small discrete-outcome views for statistically novice
  readers.
labels:
- purpose:refine
- basis:empirical
- scope:single-result
- lever:encoding
- operator:uncertainty
- quality:fidelity
- literacy:novice
---

## Continuous uncertainty encoding for transfer <!-- role: advice -->

Use a continuous uncertainty encoding when readers must estimate what a new study's replications would look like. For example, use a smooth probability curve rather than a display of about 20 discrete outcomes when readers draw or inspect the distribution of replicated effects for another experiment.

## Why continuous encoding helps new estimates <!-- role: reason -->

Continuous encoding avoided the transfer penalty seen with discrete-outcome displays. The paper suggests that some readers may not have understood the meaning of individual discrete outcomes well enough to use them in a new estimation task.

**Mechanism:** A continuous display better supports judging overall location and spread for a new prediction instead of relying on memorized discrete shape.

**Evidence:** In the transfer task, discrete uncertainty displays led to worse accuracy than continuous displays when participants estimated uncertainty for a new experiment [@hullmanImaginingReplicationsGraphical2018].

**Notes:** The discrete advantage in this paper was limited to graphical recall of a distribution that had already been shown.

## Use when readers must estimate a second study <!-- role: context -->

- **User Goal:** Estimate replication uncertainty for a new experiment.
- **Task:** Transfer what was learned from one uncertainty display to a second experimental result.
- **Data:** A single new experiment summarized with sample statistics.
- **Chart Setting:** An interactive uncertainty display used for estimation or prediction.
- **Audience:** Readers with limited statistics training.
- **Success Criterion:** More accurate predicted distributions for the new study.

## Do not use it when recall is the priority <!-- role: exceptions -->

**Break it when:** The main goal is short-term graphical recall of the uncertainty already shown for one study. **Why:** Small discrete-outcome displays were better for that recall task.

## Costs of choosing continuous encoding <!-- role: costs -->

**Sacrifice:** You lose the graphical memorability benefit that came with small discrete-outcome displays.
**Risk:** A continuous display may be harder to remember exactly after a delay.
**Mitigation:** Reserve continuous encoding for estimation and transfer tasks rather than recall-focused summaries.

## Common transfer failure <!-- role: mistakes -->

**Mistake:** Reuse a small discrete-outcome uncertainty display because it was memorable in an earlier view. **Why it fails:** That memorability did not translate into better accuracy when readers estimated uncertainty for a new study.

## How to test the encoding choice <!-- role: check -->

**Failure Sign:** Readers misestimate the location or spread of the uncertainty distribution for a second study.
**Quick Check:** Compare continuous and small discrete-outcome versions on a second-study estimation task.
**Stronger Test:** Score readers' predicted distributions against the target replication prediction distribution and compare the two encodings.

## What to change <!-- role: fix -->

- Replace the discrete-outcome uncertainty view with a continuous distribution view in the transfer step.
- Use the continuous version for any drawing interface that collects a new-study uncertainty estimate.
- Keep the continuous encoding through the full new-study estimation task rather than switching formats midstream.
- If the view is only for later graphical recall, move that recall-focused version back to a small discrete-outcome display.
