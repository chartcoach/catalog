---
id: provide-playback-controls-for-long-or-looping-animations
title: Provide playback controls for long or looping animations
bibliography: references.bib
description: For dynamic chart explanations and state transitions, use playback controls
  on animated visualizations to improve accessibility and mitigate uncontrolled long-running
  or looping motion for motion-sensitive or high-cognitive-load viewing contexts.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:interaction-access
- temporal-pattern:dynamic
- access:motion-safe:use
---

## Playback controls for long animations <!-- role: advice -->

Add pause, stop, and start controls to chart animations that run longer than 2 seconds or loop. For example, give video-style or explanatory chart animations a way to pause or stop, and give data-state transition animations that last more than 2 seconds a way to start over.

## Why playback controls help <!-- role: reason -->

Long-running motion forces users to consume changing content at the animation's pace. Playback controls let users interrupt, stop, or restart that change so they can manage motion and review the sequence.

**Mechanism:** User-controlled playback reduces forced continuous motion and lets readers revisit an animated state transition instead of waiting for the sequence to run again.

**Evidence:** Chartability requires pause, stop, and start controls for longer video-style or explanatory animations, requires pause or stop for animations lasting more than 2 seconds or looping, and requires a way to start over for data-state transitions longer than 2 seconds. The linked inclusive design guidance also recommends letting users pause, stop, or adjust long-running animations to reduce motion sickness and cognitive load [@elavskyHowAccessibleMy2022; @inclusivedesignprinciples_give_control].

**Notes:** The trigger is the animation's duration or repetition: more than 2 seconds, any loop, or a data-state transition longer than 2 seconds.

## When this applies <!-- role: context -->

- **User Goal:** Follow an animated explanation or inspect a changing chart state at their own pace.
- **Chart Setting:** The visualization includes a video-style animation, an explanatory animation, or an animated transition in the state of the data.
- **Audience:** Users may need control over motion because continuous animation can increase motion sickness or cognitive load.
- **Success Criterion:** Any long or looping animation can be paused or stopped, and any long data-state transition can be started again.

## When not to apply this rule <!-- role: exceptions -->

**Break it when:** The animation lasts 2 seconds or less, does not loop, and is not a data-state transition lasting more than 2 seconds. **Why:** This guideline is scoped only to long-running, looping, or long transition animations.

## Costs of playback controls <!-- role: costs -->

**Sacrifice:** You must add extra playback controls and support their control states.
**Risk:** If you add the same controls to brief motion that does not meet the duration or looping trigger, you add unnecessary interface overhead.
**Mitigation:** Reserve these controls for animations longer than 2 seconds, looping animations, and long data-state transitions.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Let a long or looping animation auto-run without pause, stop, or replay controls. **Why it fails:** Users stay locked to the animation's pace, and long data-state transitions cannot be restarted.

## How to review it <!-- role: check -->

**Failure Sign:** An animation runs longer than 2 seconds or loops, but no control lets the user pause or stop it, or a long data-state transition cannot be replayed.
**Quick Check:** Trigger every animation and watch for more than 2 seconds. Confirm that long or looping animations expose pause or stop controls and that long state transitions expose a way to start over.
**Stronger Test:** Run each long or looping animation end to end and verify that you can pause it mid-stream, stop it, and restart the sequence without waiting for it to finish naturally.

## How to fix it <!-- role: fix -->

- Add a visible pause control to any chart animation that lasts more than 2 seconds.
- Add a stop control to any looping or explanatory animation.
- Add a start or replay control so the user can begin the animation again.
- Add a restart control to any data-state transition animation that lasts more than 2 seconds.
