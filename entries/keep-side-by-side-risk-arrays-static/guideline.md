---
id: keep-side-by-side-risk-arrays-static
title: Keep side-by-side risk arrays static during comparison
bibliography: references.bib
description: For compare tasks in multi-view risk displays, avoid animation on icon-array
  risk graphics to improve choice and gist accuracy and mitigate distraction for mixed-numeracy
  audiences.
labels:
- purpose:refine
- basis:empirical
- task:compare
- structure:multi-view
- quality:fidelity
- lever:interaction-access
- temporal-pattern:dynamic
- knowledge:mixed
---

## Keep the comparison view static <!-- role: advice -->

Keep paired risk arrays static when readers must choose the lower-risk option. For example, use a static grouped icon array instead of built, shuffled, or settle animations when two options are shown side by side and differ by a small amount.

## Why static comparison works better here <!-- role: reason -->

Simultaneous motion in two side-by-side risk displays competes with the reader's job of comparing magnitudes. Extra motion can pull attention away from the simple count or gist judgment needed to identify which option is safer.

**Mechanism:** Static grouped arrays preserve a stable part-whole view, so readers can compare the two risk magnitudes directly instead of tracking motion in both panels.

**Evidence:** In this experiment, no animated display improved treatment choice, gist knowledge, or graph ratings over the static grouped control, and most animations reduced performance or preference; the static grouped version consistently produced the strongest overall results [@zikmund-fisherAnimatedGraphicsComparing2012].

**Notes:** The paper tested two risks shown side by side, so this rule is strongest for simultaneous risk comparisons.

## Use when the display is a paired risk decision <!-- role: context -->

- **User Goal:** Choose between two options based on which has the lower risk profile.
- **Task:** Compare two risk displays at the same time and identify the better option.
- **Data:** Two close quantitative risk values, often with one equal risk and one differing risk.
- **Chart Setting:** Computer-administered icon arrays shown in parallel, with animation available as a design option.
- **Audience:** Adults with mixed numeracy.
- **Success Criterion:** Higher choice accuracy, better gist knowledge, and better graph evaluation ratings.

## Do not generalize past this tested comparison setup <!-- role: exceptions -->

**Break it when:** The display is not a side-by-side comparison of two risks, such as a single-risk display or a one-risk-at-a-time presentation. **Why:** The paper identifies those cases as untested and notes animation could behave differently there.

## Costs of removing motion <!-- role: costs -->

**Sacrifice:** You give up motion cues that might signal buildup or randomness.
**Risk:** A fully static view may not convey that events occur randomly across individuals.
**Mitigation:** If you must preserve a randomness cue, use a scattered introduction only if it resolves to a grouped comparison view.

## Common motion-heavy failure <!-- role: mistakes -->

**Mistake:** Replacing a static grouped risk array with a more complex animated version to make the display look more engaging. **Why it fails:** The added motion often reduced knowledge and preference instead of improving them.

## Test static against animated directly <!-- role: check -->

**Failure Sign:** Viewers miss the lower-risk option or misread which risks are equal.
**Quick Check:** Run the same two-risk comparison once with a static grouped array and once with the animated alternative; keep the version with higher correct choice and knowledge rates.
**Stronger Test:** Also compare graph evaluation ratings, since the most complex animations were often least liked.

## Remove unnecessary motion cues <!-- role: fix -->

- Replace the animated comparison view with a static grouped icon array.
- Remove shuffle effects from any scattered version used for decision-making.
- Remove settle effects if the display does not need an initial randomness cue.
- If animation is unavoidable, reduce it to one-at-a-time building on a grouped array.
