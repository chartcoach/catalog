---
id: label-axes-clearly-and-mark-truncation
title: Label axes clearly and mark any truncation
bibliography: references.bib
description: For chart reading and interpretation, use clear axis labels and explicit
  truncation labels on charts with axes to improve accessibility and mitigate ambiguous
  or misleading scale reading for readers with cognitive accessibility needs.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:text-annotation
- component:axis:use
- needs:cognitive
---

## Clarify axis labeling <!-- role: advice -->

Label each visible axis clearly and mark any truncation directly on the axis. For example, add an explicit measure label to each axis, keep abbreviated axis text clear and consistent, and visibly label a shortened scale instead of leaving truncation implicit.

## Why explicit axis labels reduce ambiguity <!-- role: reason -->

Clear axis labels tell readers what each direction on the chart means and reduce the need to infer scale meaning from context. Explicit truncation labels also prevent readers from misreading a shortened scale as a full one.

**Mechanism:** Clear axis text lowers cognitive load during chart reading, while explicit truncation cues prevent incorrect interpretation of the plotted values.

**Evidence:** Chartability classifies unclear or missing axis labels as an Understandable accessibility issue and states that axes should be present and clear, that truncated axes must have a clear label, and that abbreviations must follow a clear and consistent convention; it also allows axis removal only in rare cases with adequate text explanation or annotation. The linked axis-practice reference likewise recommends axis titles and clear labelling and warns against truncating axes without clear disclosure because that can lead to misinterpretation [@elavskyHowAccessibleMy2022; @yellowfinbi_chart_axis].

## When this applies <!-- role: context -->

- **User Goal:** Read and interpret values from a chart correctly.
- **Data:** Values are plotted against one or more axes.
- **Chart Setting:** The chart shows axes, uses abbreviated axis text, or shortens an axis range.
- **Audience:** Readers need low-ambiguity chart text and reduced cognitive load.
- **Success Criterion:** Readers can tell what each axis measures and can detect any truncation without guessing.

## When text can replace an axis <!-- role: exceptions -->

**Break it when:** the chart intentionally removes an axis and already provides adequate text explanation or annotation for how to read the values. **Why:** the explanatory text supplies the missing reading guidance that the axis would otherwise provide.

## Tradeoffs of fuller axis labeling <!-- role: costs -->

**Sacrifice:** Clearer axis labeling can require extra layout and engineering effort.
**Risk:** Shortened or abbreviated axis text can stay unclear if the convention is not explained consistently.
**Mitigation:** Keep abbreviations consistent, and move essential reading guidance into nearby text or annotation when an axis cannot carry it clearly.

## Common axis-label failures <!-- role: mistakes -->

- **Mistake:** Showing an axis without a clear label. **Why it fails:** readers must infer what the scale represents.
- **Mistake:** Truncating an axis without marking the truncation. **Why it fails:** readers can misread the scale.
- **Mistake:** Abbreviating axis labels inconsistently. **Why it fails:** the label text stops being predictable and easy to interpret.

## How to audit axis labeling <!-- role: check -->

**Failure Sign:** An axis is unlabeled, ambiguously labeled, inconsistently abbreviated, or visually shortened without a clear truncation label.
**Quick Check:** Look only at the chart text and ask whether each axis can be identified and whether any truncation is obvious.
**Stronger Test:** If an axis is removed, verify that nearby text explanation or annotation gives the missing reading guidance.

## What to change <!-- role: fix -->

- Add a clear label to each visible axis.
- Add a clear label wherever an axis is truncated.
- Rewrite abbreviated axis text so the convention is clear and used consistently.
- If you remove an axis, add adequate text explanation or annotation that tells readers how to interpret the chart.
