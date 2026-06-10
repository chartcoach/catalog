---
id: prefer-filled-point-shapes-for-color-comparisons
title: Prefer filled point shapes when color differences must be read
bibliography: references.bib
description: For point-to-point color comparison, prefer filled point shapes on scatterplots
  that encode information with both shape and color to improve fidelity and mitigate
  missed color differences for viewers reading multiclass points.
labels:
- purpose:refine
- basis:empirical
- task:compare
- chart:scatter
- quality:fidelity:use
- lever:encoding
- channel:shape:use
- channel:color-hue
---

## Filled shape markers <!-- role: advice -->

Use filled point shapes when readers must compare color differences in a scatterplot. For example, replace outline circles, squares, or triangles with filled versions when the points also carry color, and only keep open shapes such as `+` or `⊤` after checking that their color differences remain easy to see.

## Why filled shapes help color reading <!-- role: reason -->

Point color is read through the mark geometry. Filled shapes give the color more visible surface, so equal color steps are less likely to disappear on one shape while remaining visible on another.

**Mechanism:** Filled marks support more reliable color-difference judgments than outline marks, which reduces shape-driven interference when readers compare colored points.

**Evidence:** Filled squares and triangles significantly outperformed their unfilled counterparts for color-difference discrimination across the tested color axes, while some open shapes such as `+` and `⊤` performed comparably better than other open forms. The review collated this study as evidence that shape interferes with color reading in scatterplots [@smartMeasuringSeparabilityShape2019; @zengReviewCollationGraphical2023].

**Notes:** The paper did not find a simple density rule for all open shapes, so the safest portable move is to prefer filled shapes over outline counterparts rather than assuming every dense-looking open shape will work equally well.

## Use when color and shape are read together <!-- role: context -->

- **User Goal:** Compare color differences between points.
- **Task:** Decide whether point colors are the same or different across categories.
- **Data:** Multiclass scatterplot data where shape and color are both used on the same points.
- **Chart Setting:** A scatterplot with shaped point symbols at practical viewing sizes.
- **Audience:** Readers interpreting multivariate point encodings.
- **Success Criterion:** Color differences stay easy to discriminate across the full shape set.

## Do not use when outlines are needed for overlap handling <!-- role: exceptions -->

**Break it when:** Point overlap or overdraw must be disambiguated with outline shapes. **Why:** The paper notes that unfilled shapes can help distinguish overlapping marks, so color discrimination is not the only design constraint in that setting.

## Tradeoffs of switching to filled shapes <!-- role: costs -->

**Sacrifice:** You give up some of the overlap-separating benefit of outline marks.
**Risk:** Blindly filling every shape can make crowded regions harder to untangle.
**Mitigation:** If outlines are necessary, test specific open shapes that preserved color discrimination better than other outline forms.

## Common failure with color-on-shape encoding <!-- role: mistakes -->

**Mistake:** Mixing filled and outline versions of shapes and expecting the same color steps to read equally well on all of them. **Why it fails:** Unfilled shapes required larger color differences for readers to perceive a difference accurately.

## How to review the shape choice <!-- role: check -->

**Failure Sign:** The same color step looks obvious on one shape and weak on another.
**Quick Check:** Render the same two colors on filled and outline versions of each candidate shape at the intended sizes and ask which pair looks more different.
**Stronger Test:** A/B compare a filled-shape version and an outline-shape version of the same scatterplot and keep the version with fewer missed same/different judgments.

## What to change <!-- role: fix -->

- Replace outline circles, squares, and triangles with filled versions when those shapes carry color.
- If open shapes must remain, test `+` or `⊤` against outline polygons before finalizing the shape set.
- Recheck the intended color steps at the smallest planned mark size, because color discrimination also changed with size.
