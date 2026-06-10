---
id: define-potentially-overlapping-variables-explicitly
title: Define potentially overlapping variables explicitly
bibliography: references.bib
description: For multi-variable narrative visualization, use text annotation on labels
  or legends to improve fidelity and mitigate ambiguous readings for readers comparing
  potentially overlapping groups.
labels:
- purpose:refine
- basis:empirical
- quality:fidelity:use
- lever:text-annotation
- data:categorical
- communication:context
- component:label:use
---

## Variable definitions <!-- role: advice -->

Define category membership rules when variables could overlap or be read in more than one way. For example, add a note that clarifies whether two named groups can share members and what counts for inclusion in each group.

## Why explicit variable definitions work <!-- role: reason -->

Ambiguous category names let readers fill in definitions for themselves. That can produce several plausible readings, including ones the data does not actually support.

**Mechanism:** Explicit definitions close off guesswork about category overlap and membership, so readers do not have to rely on unstated assumptions to interpret the chart.

**Evidence:** The paper's case analysis shows that unclear definitions for potentially overlapping categories create ambiguity about how variables relate and whether groups overlap. It also argues that ambiguity omits more specific information and prevents readers from knowing whether their interpretation is actually supported [@hullmanVisualizationRhetoricFraming2011].

**Notes:** The paper also notes that ambiguity can be used strategically to permit several interpretations.

## Use when category labels can be read more than one way <!-- role: context -->

- **User Goal:** Compare groups or variables without guessing what each label includes.
- **Task:** Read a chart with several named categories or mapped variables.
- **Data:** Category membership may overlap, or the label alone does not make inclusion rules obvious.
- **Chart Setting:** Visualization with labels, legend space, or short explanatory notes.
- **Audience:** Readers who may bring different assumptions to the category names.
- **Success Criterion:** Independent readers describe the category boundaries the same way.

## Do not remove ambiguity when ambiguity is the intended rhetorical move <!-- role: exceptions -->

**Break it when:** Deliberate ambiguity is part of the intended rhetorical effect. **Why:** The paper notes that ambiguity can preserve multiple interpretations and sometimes sustain an engaging reading that full specificity would eliminate.

## Costs of explicit definitions <!-- role: costs -->

**Sacrifice:** You give up some brevity and rhetorical openness.
**Risk:** Long definitions can clutter labels and slow scanning.
**Mitigation:** Move the definition into smaller type near the label or legend rather than forcing it into the main title.

## Common variable-definition mistake <!-- role: mistakes -->

**Mistake:** Naming categories without clarifying whether they overlap or how membership is assigned. **Why it fails:** Readers may apply different private definitions and reach incompatible interpretations.

## Check category-definition clarity <!-- role: check -->

**Failure Sign:** A reviewer cannot tell from the chart whether two categories can share members.
**Quick Check:** Ask two reviewers to explain who belongs in each category.
**Stronger Test:** If their explanations differ, the category definition is still ambiguous.

## Fix ambiguous category labels <!-- role: fix -->

- Add a short definition for each potentially overlapping category.
- State explicitly whether categories can share members.
- Move longer definitions into smaller type near the legend or label if the main view becomes crowded.
