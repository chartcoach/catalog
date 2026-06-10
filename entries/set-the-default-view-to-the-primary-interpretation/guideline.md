---
id: set-the-default-view-to-the-primary-interpretation
title: Set the default view to the primary interpretation
bibliography: references.bib
description: For interactive narrative visualization with multiple views, use interaction
  access on default states and menu order to improve insight and mitigate unguided
  first impressions for readers entering a focused story.
labels:
- purpose:refine
- basis:empirical
- quality:insight:use
- lever:interaction-access
- structure:multi-view
- communication:framing
---

## Default view and menu order <!-- role: advice -->

Set the default view and the first-listed control to the view you want readers to interpret first. For example, open on the overview or priority variable and list that same view first in the menu instead of making readers reach it through secondary options.

## Why default views and menu order work <!-- role: reason -->

The first state of an interactive visualization is not neutral. It becomes the anchor for later exploration and makes some interpretations more likely than others before any user choice occurs.

**Mechanism:** Default views and first-listed options direct attention early, so users start from the framed comparison or dimension the design wants them to notice.

**Evidence:** The paper identifies default views, fixed comparisons, spatial ordering, menu choices, and suggested goals as procedural rhetoric that anchors interpretation in interactive narrative visualization. Its case analysis shows how a default overview and first-listed menu option privilege one data dimension over others and make that reading more likely through common navigational conventions [@hullmanVisualizationRhetoricFraming2011].

**Notes:** The paper explicitly notes that designers could choose different defaults when the goal is not a single intended interpretation.

## Use when the story has a focused first read <!-- role: context -->

- **User Goal:** Enter the story through the intended first comparison or dimension.
- **Task:** Explore an interactive narrative with more than one possible view.
- **Data:** Several variables or map views are available, but one is meant to anchor the story.
- **Chart Setting:** Interactive visualization with a default state and a menu, button, or other view selector.
- **Audience:** Readers who are likely to begin with the first visible and first listed option.
- **Success Criterion:** Most first-time readers begin from the intended view without extra interaction.

## Do not force one default when the story is not single-path <!-- role: exceptions -->

**Break it when:** The visualization goal is not specifically focused on a single intended interpretation. **Why:** The paper notes that a single default view for all users is not a given in that case, and dynamic defaults are a plausible alternative.

## Costs of anchoring the default view <!-- role: costs -->

**Sacrifice:** You give up equal exposure of all views at entry.
**Risk:** Over-anchoring can make other valid interpretations less likely to be explored.
**Mitigation:** Keep additional views available through clear controls after the primary entry view.

## Common default-view mistake <!-- role: mistakes -->

**Mistake:** Placing the priority view behind secondary controls while another view loads first. **Why it fails:** The first visible state frames interpretation before users decide what else to inspect.

## Check the entry-state frame <!-- role: check -->

**Failure Sign:** On first load, the visualization highlights a secondary view or variable.
**Quick Check:** Reload the visualization and record the first visible view and first-listed menu item.
**Stronger Test:** Ask a reviewer what the chart seems to be "about" after the first screen only.

## Fix weak default framing <!-- role: fix -->

- Make the primary overview or priority variable the default state.
- Move the primary view to the first position in the menu or selector.
- Keep secondary views accessible, but do not let them define the first reading by default.
