---
id: use-small-discrete-outcome-encoding-for-uncertainty-recall
title: Use a small discrete-outcome encoding to support uncertainty recall
bibliography: references.bib
description: For short-term recall of uncertainty from a single reported experiment,
  prefer a small discrete-outcome encoding on uncertainty displays to improve fidelity
  and address weak memory for distribution shape among statistically novice readers.
labels:
- purpose:refine
- basis:empirical
- scope:single-result
- lever:encoding
- operator:uncertainty
- density:sparse
- quality:fidelity
- literacy:novice
---

## Small discrete-outcome uncertainty display <!-- role: advice -->

Use a small discrete-outcome encoding instead of a smooth continuous probability curve when readers need to remember a shown uncertainty distribution. For example, present about 20 discrete replication outcomes rather than one continuous density when displaying the sampling distribution from a single experiment.

## Why small discrete displays aid recall <!-- role: reason -->

A small set of discrete outcomes can be remembered as a shape. That made the shown uncertainty distribution easier to reproduce later in a graphical recall task, even after an intervening task.

**Mechanism:** Discrete outcomes compress the distribution into a limited visual pattern that readers can store and reproduce more easily than a continuous curve.

**Evidence:** Participants who viewed uncertainty as a small discrete-outcome display recalled the shown sampling distribution more accurately in the graphical recall task than participants who viewed a continuous display; the paper notes that many readers appeared to remember the discrete shape directly [@hullmanImaginingReplicationsGraphical2018].

**Notes:** The same clear advantage did not appear on the text probability recall task, so the benefit may be tied to remembering graphical shape rather than fully translating its meaning.

## Use when graphical recall is the goal <!-- role: context -->

- **User Goal:** Remember the uncertainty shown for one reported experiment.
- **Task:** Graphically reproduce a previously shown uncertainty distribution.
- **Data:** One sampling distribution associated with a single experiment.
- **Chart Setting:** A display where uncertainty can be shown as a limited set of discrete outcomes.
- **Audience:** Readers with limited statistics training.
- **Success Criterion:** More accurate redraws of the shown distribution.

## Do not use it for new-study estimation <!-- role: exceptions -->

**Break it when:** Readers must estimate the uncertainty of a new study rather than recall one already shown. **Why:** Discrete displays reduced accuracy on the transfer task.

## Costs of using discrete outcomes <!-- role: costs -->

**Sacrifice:** You give up some precision and expressiveness compared with a continuous distribution.
**Risk:** Some readers may remember the shape without understanding what the individual outcomes mean.
**Mitigation:** Use this encoding when graphical recall of the shown distribution matters more than transfer to a new estimate.

## Common encoding failure <!-- role: mistakes -->

**Mistake:** Use a smooth continuous uncertainty curve in a recall-focused view. **Why it fails:** Continuous conditions produced less accurate graphical recall than small discrete-outcome displays.

## How to test the recall benefit <!-- role: check -->

**Failure Sign:** Readers cannot redraw the shown uncertainty distribution after a short delay or intervening task.
**Quick Check:** Compare a small discrete-outcome version against a continuous version and ask readers to redraw the distribution later.
**Stronger Test:** Score the redraws against the shown distribution and compare error across the two encodings.

## What to change <!-- role: fix -->

- Replace the continuous uncertainty curve with a discrete-outcome display.
- Keep the discrete-outcome count small rather than increasing the number of outcomes.
- Use the discrete version only on views where recall of the shown graphical distribution is the priority.
- Switch back to a continuous encoding if the same view must support new-study estimation.
