---
id: omit-point-labels-when-scatterplot-details-are-not-required
title: Omit point labels when item details are not required in a scatter plot
bibliography: references.bib
description: For relationship reading in item-based scatter plots, avoid per-point
  labels on the plotted marks to improve readability and mitigate obscured positions
  for viewers who do not need item-level lookup.
labels:
- purpose:refine
- basis:empirical
- task:relate
- chart:scatter
- scope:record-list
- quality:readability:use
- lever:text-annotation
- component:label:avoid
- reading-mode:overview
---

## Remove per-point labels from overview scatter plots <!-- role: advice -->

Remove point labels from a scatter plot when the item identities can be left in the background. For example, use an unlabeled scatter plot for two quantitative relations instead of labeling every point, because the unlabeled version keeps point positions visible and the overall relationship easier to see.

## Why labels hurt the overview <!-- role: reason -->

Point labels compete with the marks that actually encode the values. Once labels pile onto the marks, readers lose the clean positional pattern and also have trouble locating any one label.

**Mechanism:** Removing labels preserves the visibility of point positions, which is the main cue in a scatter plot, and prevents the search burden of scanning many item names.

**Evidence:** The paper shows that a scatter plot expresses the data when item details may be omitted and identifies two problems with the labeled version: labels obscure point positions and make individual items difficult to find [@mackinlayAutomatingDesignGraphical1986].

## Use when the scatter plot is for relationships, not item lookup <!-- role: context -->

- **User Goal:** See the general relationship between two quantitative variables.
- **Task:** Read the positional pattern rather than identify every individual item.
- **Data:** Records are plotted as individual points.
- **Chart Setting:** A scatter plot could include one label per point, but the item details are optional.
- **Success Criterion:** The point pattern remains easy to perceive without text covering the marks.

## Keep the labels only when item identity is required <!-- role: exceptions -->

**Break it when:** The presentation must include the details of the individual items. **Why:** Then omitting the labels would leave out required information.

## Tradeoffs of removing labels <!-- role: costs -->

**Sacrifice:** Readers lose direct item identification from the plot itself.
**Risk:** Someone who needs one item's name or values cannot get that detail from the unlabeled scatter plot alone.
**Mitigation:** Switch to a different chart structure when item-level detail is required.

## Common labeling failure in scatter plots <!-- role: mistakes -->

**Mistake:** Keep a label on every plotted point even though the chart's job is to show the overall relation. **Why it fails:** The labels hide the positional encoding and add a hard visual search task.

## Check whether labels are undermining the scatter plot <!-- role: check -->

**Failure Sign:** Text overlaps marks or makes the point cloud hard to read as positions.
**Quick Check:** Remove the labels temporarily; if the relationship becomes easier to see immediately, keep the unlabeled version.
**Stronger Test:** Ask whether a reader can still see the point positions clearly and find a single item quickly with all labels present.

## Fix the cluttered scatter plot <!-- role: fix -->

- Delete the per-point labels when item details are optional.
- Keep the points as the only marks carrying the quantitative values.
- Replace the scatter plot with a detail-oriented structure such as aligned bar charts if item identities must be shown.
