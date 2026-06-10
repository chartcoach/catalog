---
id: provide-an-alternative-view-for-difficult-charts
title: Provide an alternative view for difficult charts
bibliography: references.bib
description: For interpretation tasks on difficult or complex charts, use an adjustable
  alternative presentation on high-risk chart types to improve accessibility and mitigate
  misinterpretation for readers with cognitive accessibility needs.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:interaction-access
- needs:cognitive
---

## Add an alternative view <!-- role: advice -->

Add a companion or switchable alternative view when a chart type is difficult or complex. For example, let users switch a pie chart to a stacked bar, add discrete marks to a line chart, and divide a bar into countable isotypes when those edits preserve the same analytical task.

## Alternative views reduce cognitive difficulty <!-- role: reason -->

Alternative views lower the amount of interpretation work the reader must do when a chart type is hard to parse. Keeping the same task available in a more accessible presentation lets the reader continue the analysis without losing the question the chart is meant to answer.

**Mechanism:** An alternative presentation changes the form of the data display, not the analytical goal, so readers can move to a chart or mark treatment that is easier for them to interpret.

**Evidence:** Chartability recommends that difficult or complex charts be adjustable into more accessible alternatives that still accomplish the same analytical task, and it identifies pie charts, line charts without discrete marks, and bar charts without countable isotypes as cognitive risks [@elavskyHowAccessibleMy2022]. Research on accessible data visualization for people with intellectual and developmental disabilities supports avoiding pie charts, using discrete marks or countable pictograms, and allowing readers to switch between representations that match their cognitive needs [@wu_understanding_data_2021; @cu-visualab_state_states].

**Notes:** The alternative can be shown alongside the original chart or exposed through a user control.

## Use when the chart form is itself a barrier <!-- role: context -->

- **User Goal:** Interpret a chart that may be difficult to read accurately.
- **Task:** Keep the same analytical task available after the presentation changes.
- **Chart Setting:** The chart is difficult or complex, or it uses a high-risk form such as a pie chart, a line without discrete marks, or a bar without countable isotypes.
- **Audience:** Readers with cognitive accessibility needs.
- **Success Criterion:** The reader can move to an easier-to-interpret view without losing the intended task.

## Do not use when the alternative changes the task <!-- role: exceptions -->

**Break it when:** the chart is not high risk for cognitive difficulty, or the alternative presentation no longer supports the same analytical task. **Why:** the source limits this guidance to difficult charts and requires the alternative to preserve the task.

## Costs of adding an alternative view <!-- role: costs -->

**Sacrifice:** You add another presentation or a control for switching views.
**Risk:** The alternative can fail if it changes the chart's question instead of only changing the presentation.
**Mitigation:** Keep the data and analytical task constant across views.

## Common failures when adding an alternative view <!-- role: mistakes -->

- **Mistake:** Leave a difficult chart type as the only available view. **Why it fails:** Readers who struggle with that form have no accessible way to perform the task.
- **Mistake:** Add a second chart that changes what the reader is supposed to analyze. **Why it fails:** The source requires the alternative to accomplish the same analytical task.

## Check for a preserved-task alternative <!-- role: check -->

**Failure Sign:** A pie chart, a line without discrete marks, or a bar without countable isotypes is shown with no companion view or switchable alternative.
**Quick Check:** Verify that the user can open or view a different presentation of the same data for the same task.
**Stronger Test:** Try to answer the same analytic question in the alternative view; if the task changes or no alternative exists, fail.

## Fix the chart by adding an alternative presentation <!-- role: fix -->

- Add a switch that changes a pie chart into a stacked bar while keeping the same comparison.
- Add discrete marks to a line chart so intervals are shown as distinct positions.
- Divide a bar into countable isotypes when counting units helps interpretation.
- If switching is not available, place the alternative chart alongside the difficult chart.
