---
id: add-visible-explanatory-text-for-chart-purpose
title: "Add visible explanatory text that states the chart\u2019s purpose and takeaway"
bibliography: references.bib
description: For visual interpretation of a chart, use visible explanatory text on
  the chart to improve accessibility and mitigate generic titles and unstated takeaways
  for readers who may struggle to infer purpose from the display alone.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:text-annotation
- communication:framing
- component:title:use
- needs:cognitive
---

## Add a takeaway title and visible summary text <!-- role: advice -->

Add visible explanatory text that tells readers what the chart is for and what to notice. For example, replace a generic subject title with a takeaway title, add a short visible description of what the chart measures, and add a textual callout for a non-obvious feature in a complex chart.

## Why visible explanation improves interpretation <!-- role: reason -->

Visible explanatory text gives readers an interpretation frame before they have to infer meaning from marks alone. That reduces ambiguity, supports recall, and helps readers notice the intended conclusion or important feature instead of guessing.

**Mechanism:** A descriptive title and supporting text state the chart’s purpose and outcome up front, while a local callout anchors interpretation at a specific complex feature.

**Evidence:** Chartability treats missing visible textual description and takeaway as a critical failure and presents descriptive titles, summaries, and textual callouts as the concrete repair for charts and complex features [@elavskyHowAccessibleMy2022]. Charts with descriptive titles and supporting text were more likely to be correctly recalled in a recognition and recall study of 393 visualizations [@xiong_curse_of_2020].

**Notes:** Even simple charts can be hard to interpret without this visible explanation.

## Use when the chart needs an explicit reading frame <!-- role: context -->

- **User Goal:** Understand what the chart is about and what conclusion to take from it.
- **Task:** Interpret or recall the message of the chart.
- **Chart Setting:** A chart is presented visually and readers must otherwise infer meaning from the display itself.
- **Audience:** Readers may have trouble interpreting even simple charts, or may miss the intended point in a complex chart.
- **Success Criterion:** The chart’s visible text states its purpose and takeaway, and any important complex feature is explicitly called out.

## Do not stop at the title when a complex feature still needs explanation <!-- role: exceptions -->

**Break it when:** The chart already has a visible title and summary that state the main takeaway, but a specific complex feature inside the plot is still only implied visually. **Why:** The needed repair is a localized textual callout on that feature, not another generic title revision.

## Tradeoffs of adding explanatory text <!-- role: costs -->

**Sacrifice:** The chart needs explicit supporting text in addition to the visual.
**Risk:** A single summary line can still leave a complex feature open to misinterpretation.
**Mitigation:** Add a textual annotation or callout at the specific feature that needs explanation.

## Common failures in chart purpose text <!-- role: mistakes -->

- **Mistake:** Using a generic subject title that names the topic but not the takeaway. **Why it fails:** Readers still have to infer the chart’s purpose and conclusion from the marks alone.
- **Mistake:** Leaving an assumedly obvious visual feature without a textual callout in a complex chart. **Why it fails:** Readers can miss or misread the intended interpretation.

## Check whether the visible text explains the chart <!-- role: check -->

**Failure Sign:** The visible text only names the subject, or it does not say what the reader should conclude or notice.
**Quick Check:** Read only the chart’s visible text. If it does not tell a reviewer what the chart is for and what to take away, fail it.
**Stronger Test:** In a complex chart, inspect the main visually salient feature. If that feature has no visible summary cue or textual callout, fail it.

## Fix missing purpose and reading cues <!-- role: fix -->

- Replace a generic subject title with a descriptive title that states the chart’s takeaway.
- Add a short visible description that says what the chart measures or why it is shown.
- Add a textual annotation or callout for any complex feature whose meaning would otherwise be inferred only from the visual.
