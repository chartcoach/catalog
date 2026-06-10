---
id: limit-necessary-animation-to-grouped-build
title: Restrict unavoidable animation to one-at-a-time building on grouped icons
bibliography: references.bib
description: For compare tasks on animated icon-array risk graphics, use one-at-a-time
  building on grouped arrays to prevent accuracy losses and mitigate the distraction
  of more complex motion for mixed-numeracy audiences.
labels:
- purpose:refine
- basis:empirical
- task:compare
- quality:fidelity
- lever:interaction-access
- temporal-pattern:dynamic
- knowledge:mixed
---

## Use grouped build as the only animation <!-- role: advice -->

If the display must animate, reveal event icons one at a time on an already grouped array. For example, start with an empty grouped matrix and add colored event icons sequentially instead of combining the build with scattered layouts, shuffles, or extra settle effects.

## Why grouped build is the safest animated option here <!-- role: reason -->

Sequential building on a grouped arrangement adds only one simple motion cue while preserving the final grouped magnitude view. It avoids the extra attentional load introduced by scattered or shuffling motion.

**Mechanism:** Readers can still rely on the same grouped magnitude structure as the static display, while the one-at-a-time appearance lightly signals accumulation and can make the larger risk finish later.

**Evidence:** The grouped-build condition performed as well as the static grouped control on all outcomes and was the only animation that showed even slight promise, while the more complex animated variants generally underperformed [@zikmund-fisherAnimatedGraphicsComparing2012].

## Use when animation cannot be removed <!-- role: context -->

- **User Goal:** Preserve an animated presentation while still supporting accurate comparison.
- **Task:** Compare two risks in a computer-delivered icon-array display.
- **Data:** Quantitative risk counts shown as event icons in paired arrays.
- **Chart Setting:** Animation is required, but the designer can choose which motion cue to use.
- **Audience:** Adults with mixed numeracy.
- **Success Criterion:** Match the static grouped baseline on choice accuracy, gist knowledge, and graph ratings.

## Do not use this when animation is optional <!-- role: exceptions -->

**Break it when:** You can show the risks without animation. **Why:** Static grouped displays already performed very well, and no animation significantly improved results.

## Costs of keeping even simple animation <!-- role: costs -->

**Sacrifice:** The display still takes time to play through.
**Risk:** Adding any extra motion beyond the sequential build can erase the advantage of this restrained approach.
**Mitigation:** Keep the icons grouped from start to finish and remove all shuffle effects.

## Common over-animated build failure <!-- role: mistakes -->

**Mistake:** Treating one-at-a-time building as permission to also scatter, shuffle, or re-randomize the event icons. **Why it fails:** The more complex animated versions generally performed worse than both the static grouped display and the grouped-build display.

## Compare grouped-build against the static baseline <!-- role: check -->

**Failure Sign:** The animated version includes motion beyond one-at-a-time appearance on a grouped arrangement.
**Quick Check:** Put the grouped-build version next to the static grouped baseline on the same task and keep grouped-build only if performance is at least comparable.
**Stronger Test:** Check both correct choice and gist knowledge, not just whether the animation looks appealing.

## Strip the animation back to the minimal safe form <!-- role: fix -->

- Remove shuffle behavior from any animated risk array.
- Keep the event icons grouped throughout the animation.
- Use only one-at-a-time appearance as the motion cue.
- Fall back to a static grouped display if the animation is not necessary.
