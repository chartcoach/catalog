---
id: provide-controls-when-extremes-compress-chart-space
title: Provide controls when data extremes compress chart space
bibliography: references.bib
description: For dynamic comparison tasks, use interaction access on quantitative
  charts where extreme values or near-equal values compress mark spacing to improve
  accessibility and mitigate unreadable chart space for users changing parameters
  or filters.
labels:
- purpose:refine
- basis:accessibility
- task:compare
- data:quantitative
- quality:accessibility
- lever:interaction-access
- temporal-pattern:dynamic
- polish:spacing
---

## Add separation controls <!-- role: advice -->

Add user controls that separate data when outliers or near-equal values compress chart space. For example, when a parameter-driven chart pushes marks into the margins or packs lines so tightly that differences are hard to see, let users sort, divide, or filter the view.

## Why separation controls help <!-- role: reason -->

Compressed marks force readers to do extra comparison work in space that no longer supports readable differences. Separation controls reduce that labor by letting the reader reallocate or isolate chart space before interpreting the data.

**Mechanism:** Sorting, dividing, or filtering gives the reader a direct way to separate values that are competing for the same visual space, instead of forcing them to infer tiny or margin-squeezed differences.

**Evidence:** Chartability defines this as an Assistive failure when extreme quantitative differences or similarities make a chart unreadable and specifies that dynamic charts should let the user sort, divide, or filter chart space when automatic handling or automatic annotations are not possible [@elavskyHowAccessibleMy2022]. The linked white-space guidance also treats space as a critical readability resource rather than wasted area [@towardsdatascience_data_visualisation_2].

**Notes:** The same failure can come from very large outliers or from values that are so similar that they visually collapse together.

## Use when chart space collapses <!-- role: context -->

- **User Goal:** Compare values after changing filters or parameters.
- **Data:** Quantitative values with extreme outliers or many near-equal values.
- **Chart Setting:** An analytical or parameter-driven chart where marks get pushed into the margins or packed tightly together.
- **Audience:** Users who need lower cognitive and functional effort during chart reading.
- **Success Criterion:** Users can separate or isolate the crowded values without guessing what the compressed spacing means.

## Skip when the chart already adapts or explains itself <!-- role: exceptions -->

**Break it when:** The chart already automatically handles the extremes or already makes the compression clear with annotations. **Why:** The source makes user controls the fallback when automatic handling or automatic annotations are not feasible.

## Costs of adding separation controls <!-- role: costs -->

**Sacrifice:** Users may need one extra action before the compressed values become readable.\
**Risk:** Adding controls without tying them to visible compression leaves the spacing problem unexplained.\
**Mitigation:** Expose the controls when marks are visibly pushed into margins or packed together by similarity.

## Common failure with separation controls <!-- role: mistakes -->

**Mistake:** Leaving a dynamic chart static after filters create outliers or near-identical values. **Why it fails:** The reader must do the separation work mentally, and the chart stays unreadable when marks compete for the same space.

## Check for compressed chart space <!-- role: check -->

**Failure Sign:** Marks are squished into the margins, or multiple lines or marks sit so close together that the difference is almost impossible to see.\
**Quick Check:** Change the chart's parameters or filters to produce an outlier or a cluster of near-equal values and see whether the view offers sort, divide, or filter controls.\
**Stronger Test:** If the chart cannot automatically adapt or automatically annotate the compression, verify that at least one user control can separate the crowded data into more readable space.

## Fix compressed chart space <!-- role: fix -->

- Add a sort control that reorders the crowded values after filters or parameter changes.
- Add a divide or split control that separates data competing for the same space.
- Add a filter control that isolates the outlier or the near-equal subset when one shared view stays unreadable.
- If the chart can handle the extremes automatically instead, annotate the compressed region so users know what is happening.
