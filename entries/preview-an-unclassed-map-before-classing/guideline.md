---
id: preview-an-unclassed-map-before-classing
title: Preview an unclassed map before choosing classes
bibliography: references.bib
description: For workflow decisions on continuous choropleth data, use an unclassed
  preview on a quantitative map to improve fidelity and mitigate unconscious oversimplification
  before finalizing a classed color scale.
labels:
- purpose:refine
- basis:heuristic
- chart:choropleth
- data:quantitative
- quality:fidelity
- lever:encoding
- communication:workflow
---

## Preview the unclassed version first <!-- role: advice -->

Start the design process with an unclassed map before deciding whether to class continuous values. For example, render the full gradient first, inspect subtle differences and transitions between neighboring areas, and only then decide which distinctions to simplify into color bins.

## Make simplification deliberate <!-- role: reason -->

Classification is a simplification step. Seeing the continuous version first reveals what that simplification will hide, so the final classes can be chosen consciously.

**Mechanism:** An unclassed preview exposes subtle differences, local contrasts, and transition shapes before class boundaries collapse them.

**Evidence:** The article recommends starting with an unclassed map even if the final result will be classed, because it helps designers see subtle differences and make a conscious decision about how to simplify them [@muth_classed_vs_unclassed_2021].

## Use during the classification decision <!-- role: context -->

- **User Goal:** Decide whether a continuous map should stay unclassed or be simplified into classes.
- **Data:** Continuous quantitative values that could be shown either as a gradient or as bins.
- **Chart Setting:** Choropleth design workflow before the final color scale is locked.
- **Success Criterion:** The final classing decision reflects visible patterns in the data rather than arbitrary simplification.

## Do not use when the data is already discrete <!-- role: exceptions -->

**Break it when:** The data is already classed or ordinal. **Why:** An unclassed scale would imply intermediate values that are not valid data states.

## Accept the extra review step <!-- role: costs -->

**Sacrifice:** You add one more draft to the process.
**Risk:** Stopping at the preview can leave threshold-based messages underemphasized.
**Mitigation:** Compare the unclassed preview against the communication goal before finalizing the published version.

## Avoid classing blind <!-- role: mistakes -->

**Mistake:** Choosing class boundaries before ever inspecting the continuous version. **Why it fails:** You cannot see which subtle differences or transitions the classes will erase.

## Check whether a preview exists <!-- role: check -->

**Failure Sign:** The final classed map has no unclassed draft behind it.
**Quick Check:** Generate an unclassed preview and note which visible differences vanish once classes are applied.
**Stronger Test:** Compare each final class boundary against the preview and confirm that each simplification is intentional.

## Add the preview step <!-- role: fix -->

- Render an unclassed draft before setting class boundaries.
- Inspect subtle regional differences and transition shapes on that draft.
- Rework the class breaks if the preview shows distinctions you do not want to hide.
