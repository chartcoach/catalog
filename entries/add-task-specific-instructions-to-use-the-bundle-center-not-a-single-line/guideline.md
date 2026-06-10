---
id: add-task-specific-instructions-to-use-the-bundle-center-not-a-single-line
title: Add task-specific instructions to use the bundle center, not a single line
bibliography: references.bib
description: For point-location judgments in static uncertainty forecasts, use task-specific
  instructions on ensemble path maps to improve fidelity and mitigate line-overlap
  bias for novice viewers.
labels:
- purpose:refine
- basis:empirical
- chart:map
- data:geospatial
- quality:fidelity
- lever:text-annotation
- operator:uncertainty
- literacy:novice
---

## Add task-specific debiasing instructions <!-- role: advice -->

Add task-specific instructions that tell viewers to judge location risk from the center of the path grouping rather than from any single visible path. For example, explicitly say that one overlapping path is not meaningful, identify the center of the grouping as the most likely path, and include brief practice questions where the correct choice is the location nearer the bundle center even when another location touches a line.

## Why task-specific instructions work better <!-- role: reason -->

Viewers can consciously use the wrong rule when they see a line crossing the target. Instructions that name the specific error and rehearse the correct readout give viewers a better chance to override the pull of the visible overlap.

**Mechanism:** Explicitly warning against single-line reasoning and practicing center-of-bundle judgments supports top-down correction of a bottom-up visual bias.

**Evidence:** Task-specific instructions reduced the overlap bias more than general visualization instructions and cut the original 9-path bias by about 61%. They also sharply improved correct responses to the question about whether line-touching locations are more likely than equally distant non-touching locations [@padillaPowerfulInfluenceMarks2020].

**Notes:** Even these explicit instructions did not eliminate the bias completely.

## Use when all are true <!-- role: context -->

- **User Goal:** Make a decision about one specific location from an ensemble path display.
- **Task:** Compare likely damage or risk between locations using a static uncertainty image.
- **Data:** Geospatial path uncertainty shown as sampled lines.
- **Chart Setting:** The display can be paired with a short tutorial, briefing, or practice step before use.
- **Audience:** Novice viewers who may otherwise rely on the visible overlap of a single path.
- **Success Criterion:** Smaller differences between equal-distance locations that vary only in whether one touches a visible path.

## Do not use when any are true <!-- role: exceptions -->

**Break it when:** The display must work with no accompanying tutorial or when the goal is to eliminate overlap bias entirely. **Why:** The tested improvement came from explicit pre-use instruction and still left a residual bias.

## Tradeoffs of task-specific instruction <!-- role: costs -->

**Sacrifice:** You add time and cognitive effort before the viewer can use the display.\
**Risk:** Viewers may become more confident without becoming fully unbiased.\
**Mitigation:** Keep the instruction narrowly focused on the single-line-overlap error and the center-of-bundle rule.

## Common failure modes <!-- role: mistakes -->

**Mistake:** Explaining only how the forecast was generated and stopping there. **Why it fails:** General explanation helped less than instructions that explicitly named the overlap error and practiced the correct judgment rule.

## How to test it <!-- role: check -->

**Failure Sign:** Viewers still choose the line-touching location over an equally distant location nearer the bundle center.\
**Quick Check:** Use one or two practice items where a visible line crosses the wrong answer and see whether viewers still pick it.\
**Stronger Test:** Measure the on-line minus off-line judgment gap after the instruction and compare it with a version that uses only generic explanation.

## What to change <!-- role: fix -->

- Add an explicit sentence telling viewers not to base judgments on an individual visible path.
- Point viewers to the center of the grouping as the most likely path.
- Add short practice items that require choosing the nearer-center location over the line-touching alternative.
