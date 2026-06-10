---
id: make-the-effect-of-a-complex-action-visible
title: Make the effect of a complex action visible
bibliography: references.bib
description: For ordered-time explanatory animations, use explicit state-change cues
  on dynamic process displays to improve fidelity and address ambiguous action meaning
  for viewers learning cause-and-effect steps.
labels:
- purpose:refine
- basis:empirical
- time:ordered-time
- temporal-pattern:dynamic
- quality:fidelity:use
- lever:encoding
---

## Show the resulting state <!-- role: advice -->

Animate the result of a complex action, not just the motion that leads into it. For example, show two elements combine into a new state, add a visible reaction when an external input strikes a complex, or show the changed structure after the action.

## Why visible effects matter <!-- role: reason -->

Motion alone does not always tell viewers what changed. When the outcome of the action is visible, the animation explains the process instead of only showing movement.

**Mechanism:** A visible state change clarifies cause and effect. Viewers can connect the incoming action to a resulting condition rather than guessing what the motion meant.

**Evidence:** The paper found that complex actions were poorly recalled when the animation did not show their effect, and recall improved after the redesign made the combined state, reaction, separation, and repaired structure explicit [@faradayDesigningEffectiveMultimedia1997].

## Use when the action changes state or relation <!-- role: context -->

- **User Goal:** Understand what changed and why during a process step.
- **Data:** A step involves a transformation, reaction, or non-obvious relation.
- **Chart Setting:** A dynamic display currently shows motion or impact without a clear visible result.
- **Audience:** Viewers may not be able to infer the process from motion alone.
- **Success Criterion:** Viewers can state the effect of the action, not just describe where motion occurred.

## Do not add reaction effects to already clear simple actions <!-- role: exceptions -->

**Break it when:** The action is simple and already clear from the motion with a speech cue. **Why:** The source reports that simple actions such as attaching or detaching were improved by speech cueing, while the need for added visual effect arose with more complex steps.

## What explicit effects cost <!-- role: costs -->

**Sacrifice:** You give up some visual economy.
**Risk:** Extra effects can add competing motion.
**Mitigation:** Reserve reaction or state-change cues for the step that actually needs explanation.

## Common action-encoding misuse <!-- role: mistakes -->

**Mistake:** Animating only the approach or impact of one element on another and never showing the changed state. **Why it fails:** Viewers may remember the motion but infer the wrong cause, target, or result.

## How to test whether the effect is visible <!-- role: check -->

**Failure Sign:** Viewers can describe where motion went but cannot say what changed after it.
**Quick Check:** Inspect each complex animated step and ask whether the resulting state is visibly shown on screen.
**Stronger Test:** Show the step once and ask viewers what effect the action had.

## What to change <!-- role: fix -->

- Add a visible changed state after the action.
- Add a brief reaction cue at the moment of impact or combination.
- Show the before-and-after structure so the transformation is explicit.
- Separate combined elements again if that separation is part of the explained effect.
