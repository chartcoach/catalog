---
id: repeat-the-same-local-transition-pattern-across-matched-story-segments
title: Repeat the same local transition pattern across matched story segments
bibliography: references.bib
description: For grouped linear narrative sequencing, use repeated local transition
  patterns on multi-view visualization presentations to improve readability and mitigate
  harder-to-explain reversed sections for audiences following a guided presentation.
labels:
- purpose:refine
- basis:empirical
- task:compose
- scope:grouped-result
- structure:multi-view
- quality:readability
- lever:layout-structure
---

## Keep repeated sections in the same order <!-- role: advice -->

Repeat the same local transition pattern for each matched section of the presentation. For example, if one group is shown as overview then two more specific views, keep that same order for the next group instead of reversing it, and if you interleave matched views from two groups, keep the same interleaving pattern across the whole sequence.

## Why repeated transition patterns help <!-- role: reason -->

A repeated sequence pattern gives viewers a stable structural cue for how the story is organized. Reversing that pattern breaks the cue and makes the overall order harder to remember.

**Mechanism:** Parallel local patterns help viewers encode the presentation as repeated units instead of unrelated steps, which supports recall of the sequence.

**Evidence:** The paper's qualitative analysis identified transition parallelism as a recurring global sequencing strategy in professional narrative visualizations. In a between-subjects study of full presentations, non-reversed sequences with perfect parallelism produced significantly better memory for the original order than reversed variants, and ratings for ease of explaining the sequence were marginally better for the non-reversed versions [@hullmanDeeperUnderstandingSequence2013].

**Notes:** The study did not find clear treatment differences for comparison-question accuracy.

## Use when the presentation has matched grouped sections <!-- role: context -->

- **User Goal:** Make the structure of a slideshow memorable and explainable.
- **Task:** Order a full presentation, not just one local transition.
- **Data:** Two or more high-level groups are present, and each visualization in one group has a matched counterpart in another group.
- **Chart Setting:** A guided multi-view presentation where similar sections repeat.
- **Audience:** Viewers following the full sequence.
- **Success Criterion:** Viewers can recall the original order and explain the organizational pattern.

## Do not force parallelism when there is no repeatable counterpart structure <!-- role: exceptions -->

**Break it when:** The visualization set does not contain matched counterpart views across repeated groups. **Why:** Parallelism depends on having a repeatable local pattern to reuse.

## Costs of repeating the same pattern <!-- role: costs -->

**Sacrifice:** You give up some freedom to locally reorder one section for a one-off shortcut.\
**Risk:** A locally cheaper reversed section can still hurt memory for the whole sequence.\
**Mitigation:** Prioritize repeated structure when sequence memorability matters more than shaving local transition cost in one section.

## Common parallelism mistake <!-- role: mistakes -->

**Mistake:** Reverse the order of matched slides in a later section of the story. **Why it fails:** The section no longer matches the earlier pattern, which weakens viewers' memory for the overall sequence.

## Check pattern consistency across sections <!-- role: check -->

**Failure Sign:** One high-level section follows a different local order than its matched section.\
**Quick Check:** Write the local transition pattern for each repeated section and verify that the pattern repeats exactly.\
**Stronger Test:** After viewers watch the presentation, ask them to reconstruct the original slide order and compare the repeated-pattern version with a reversed version.

## Fix broken parallelism <!-- role: fix -->

- Rewrite each matched section to use the same sequence of local transition types.
- Remove local reversals that swap the order of counterpart views in later sections.
- If you interleave groups, keep the interleaving rule identical across the whole presentation.
