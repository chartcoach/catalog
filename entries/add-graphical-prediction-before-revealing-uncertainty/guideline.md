---
id: add-graphical-prediction-before-revealing-uncertainty
title: Add a graphical prediction step before revealing uncertainty
bibliography: references.bib
description: For uncertainty estimation from a single reported experiment, use a prediction-before-reveal
  interaction on interactive uncertainty displays to improve fidelity and address
  weak transfer from one experiment to judgments about another for statistically novice
  readers.
labels:
- purpose:refine
- basis:empirical
- scope:single-result
- lever:interaction-access
- operator:uncertainty
- quality:fidelity
- literacy:novice
- communication:workflow
---

## Prediction-before-reveal interaction <!-- role: advice -->

Add a graphical prediction step before revealing the uncertainty distribution. For example, let readers sketch the distribution of replicated effects with an interactive drawing surface, then reveal the true sampling distribution against their sketch.

## Why prediction-first helps transfer <!-- role: reason -->

A prediction step makes readers commit to an uncertainty model before they see the answer. Seeing the gap between their sketch and the shown distribution can focus attention on what replication uncertainty means, which supports later estimates for a new experiment.

**Mechanism:** Prediction turns the uncertainty view into an active comparison between the reader's expectation and the displayed distribution.

**Evidence:** In the controlled study, participants who graphically predicted uncertainty before seeing the true distribution made more accurate uncertainty estimates for a new experiment than participants who only viewed the distribution; the same clear advantage did not appear for recall alone [@hullmanImaginingReplicationsGraphical2018].

## Use when transfer to a new study matters <!-- role: context -->

- **User Goal:** Estimate the uncertainty of a new experiment after seeing one example.
- **Task:** Transfer what was learned from one uncertainty display to another experimental result.
- **Data:** A single reported experiment summarized with sample statistics such as mean, standard deviation, and sample size.
- **Chart Setting:** An interactive uncertainty view that can collect a user-drawn distribution before showing the true distribution.
- **Audience:** Readers with limited statistics training.
- **Success Criterion:** More accurate predicted distributions for a later study.

## Do not use it as a recall-only intervention <!-- role: exceptions -->

**Break it when:** The only success criterion is short-term recall of the exact shown distribution. **Why:** The study did not show a clear recall advantage from graphical prediction by itself.

## Costs of adding the prediction step <!-- role: costs -->

**Sacrifice:** You add an interaction step before showing the answer.
**Risk:** The benefit varies across readers rather than helping everyone equally.
**Mitigation:** Keep the step only if it improves later uncertainty judgments, not just immediate engagement.

## Common workflow failure <!-- role: mistakes -->

**Mistake:** Show only the true uncertainty distribution, or replace the sketch step with formula-based rule training. **Why it fails:** Those alternatives did not match the transfer improvement seen with graphical prediction.

## How to test the prediction step <!-- role: check -->

**Failure Sign:** After seeing one study, readers still draw poor uncertainty estimates for a second study.
**Quick Check:** Compare a version with the prediction step against the same display without it and inspect second-study prediction accuracy.
**Stronger Test:** Score the second-study drawings against the target replication prediction distribution and compare error across conditions.

## What to change <!-- role: fix -->

- Add a required sketch-before-reveal step to the uncertainty view.
- Reveal the true distribution immediately after the sketch so readers can compare their prediction with the shown answer.
- Use the same graphical distribution format for the prediction step and the revealed uncertainty view.
- Replace or supplement formula-only instruction with the graphical prediction step.
