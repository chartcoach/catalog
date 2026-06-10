---
id: keep-multiple-temporal-states-visible-for-analytical-comparison
title: Keep multiple temporal states visible for analytical comparison
bibliography: references.bib
description: For analytical tasks on ordered-time data, avoid substitutive animation
  in temporal views to improve fidelity and mitigate recall burden for users comparing
  changing states.
labels:
- purpose:refine
- basis:empirical
- task:trend
- time:ordered-time
- temporal-pattern:dynamic
- quality:fidelity:use
- lever:interaction-access
---

## Show temporal states simultaneously <!-- role: advice -->

Keep relevant time states visible during analytical comparison instead of replacing one state with the next in animation. For example, do not make viewers infer trends from a sequence of changing frames in a multivariate time view; keep multiple states or facets on screen so earlier states do not have to be recalled from memory.

## Reduce recall load during time comparison <!-- role: reason -->

Substitutive animation makes one state disappear as the next appears. That forces the viewer to remember earlier frames while judging later ones, which is especially costly when the data is large or multifaceted.

**Mechanism:** Simultaneous visibility supports direct comparison across time states, while frame-by-frame replacement turns comparison into a memory task.

**Evidence:** The paper says animated visualizations may help narrative tasks but are not always effective for analytical tasks because each representation replaces the previous one in time, overloading short-term memory, and it notes that as data increases this approach can produce inaccurate understanding of trends [@olaSimpleChartsDesign2016].

## Use when the task is analytical time comparison <!-- role: context -->

- **User Goal:** Compare earlier and later states accurately.
- **Task:** Analyze temporal trends rather than watch a narrated sequence.
- **Data:** Ordered-time data with multiple facets or changing states.
- **Chart Setting:** The current design reveals change by replacing one frame with another.
- **Success Criterion:** The viewer can compare time states without replaying or remembering prior frames.

## Do not use when the task is narrative presentation <!-- role: exceptions -->

**Break it when:** The main goal is narrative communication rather than analytical comparison. **Why:** The paper explicitly says animation may be beneficial for narrative tasks.

## Trade off storytelling motion against analytical comparison <!-- role: costs -->

**Sacrifice:** You give up some of the compact, story-like pacing of animation.
**Risk:** Keeping multiple states visible can increase on-screen density.
**Mitigation:** Use simultaneous visibility when accurate comparison matters more than narrative flow.

## Avoid frame replacement for analytic trend reading <!-- role: mistakes -->

**Mistake:** Using animation to reveal successive analytical states that viewers must compare. **Why it fails:** Each new frame replaces the old one, so the comparison depends on memory instead of direct inspection.

## Test whether the viewer must remember earlier frames <!-- role: check -->

**Failure Sign:** Reviewers replay or scrub the animation to compare two states.
**Quick Check:** Pause the display on one state and ask whether a reviewer can still compare it to the previous state without replay.
**Stronger Test:** Compare the animated version with a simultaneous version and see which one supports a direct explanation of the trend.

## Replace substitution with simultaneous visibility <!-- role: fix -->

- Replace frame-by-frame substitution with a view that keeps multiple relevant states visible.
- Keep earlier and later states available in the same analytical workspace.
- Reduce the use of animation when the viewer's main task is to compare trends accurately.
