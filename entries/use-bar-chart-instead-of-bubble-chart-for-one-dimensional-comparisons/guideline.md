---
id: use-bar-chart-instead-of-bubble-chart-for-one-dimensional-comparisons
title: Use a bar chart instead of a bubble-style scatter chart for one-dimensional
  comparisons
bibliography: references.bib
description: For one-dimensional comparison tasks, use a bar chart instead of a bubble-style
  scatter chart on simple comparison displays to improve readability and address interpretation
  difficulty for general audiences.
labels:
- purpose:select
- basis:rhetorical
- task:compare
- chart:bar:use
- chart:scatter:avoid
- audience:general-public
- quality:readability
- lever:chart-family
---

## Choose a familiar chart family <!-- role: advice -->

Choose a chart family your audience already recognizes for simple comparisons. For example, use a bar chart instead of a bubble chart when viewers need to compare one-dimensional values.

## Familiar forms reduce decoding effort <!-- role: reason -->

Recognizing the chart family reduces the effort spent figuring out how the display works. That leaves more attention for reading the values and making the comparison.

**Mechanism:** Familiar chart types help viewers interpret the display faster, while unfamiliar or more artful forms make readers spend effort decoding the form before they can compare the data.

**Evidence:** Workshop participants said that recognizing a chart type helped them understand it, and some preferred several simple charts over one complex multi-dimensional visualization. In direct testing for one-dimensional data, bar charts were perceived as easier to interpret than bubble charts, and practitioners reported that familiar chart types are usually more understandable than artful ones [@knoll_gulf_2025; @prantl_studying_forthcoming; @schuster_who_2023].

**Notes:** Practitioners reported that audiences may actively ask for a simpler depiction when a chart form feels too elaborate.

## Use when simple comparison is the main job <!-- role: context -->

- **User Goal:** Compare values across categories.
- **Task:** Read a one-dimensional comparison without first learning a novel chart form.
- **Data:** One-dimensional values.
- **Chart Setting:** A single comparison is being shown, or the current design feels visually complex.
- **Audience:** Lay viewers or other audiences who benefit from familiar chart forms.
- **Success Criterion:** Viewers say the chart is easy to interpret and can compare values without hesitation.

## Do not use when the situation no longer matches the tested case <!-- role: exceptions -->

- **Break it when:** the display is not a one-dimensional comparison. **Why:** the direct tested advantage is specific to one-dimensional data.
- **Break it when:** your audience already recognizes and routinely uses the alternative chart type. **Why:** the benefit here comes from chart-type familiarity.

## Simplicity trades away form novelty <!-- role: costs -->

**Sacrifice:** You give up a more decorative or visually novel form.
**Risk:** Applying the rule blindly can flatten a display that is trying to show several dimensions in one view.
**Mitigation:** If the current view combines several simple comparisons in one complex display, separate them into several simple charts instead of keeping one unfamiliar multi-dimensional view.

## A common failure is choosing a richer-looking form for a simple task <!-- role: mistakes -->

**Mistake:** Use a bubble-style scatter chart for a simple one-dimensional comparison because it looks more expressive. **Why it fails:** viewers must decode the chart form before they can make the comparison, so the chart feels harder to interpret than a bar chart.

## Test bar versus bubble directly <!-- role: check -->

**Failure Sign:** Viewers hesitate, ask how to read the marks, or say the chart feels harder than the question it is answering.
**Quick Check:** Put a bar-chart version and a bubble-chart version of the same one-dimensional data side by side and ask representative viewers which one is easier to interpret.
**Stronger Test:** Ask viewers to answer the same comparison question from both versions and keep the version they recognize and explain more readily.

## Replace the unfamiliar form with a simpler one <!-- role: fix -->

- Replace the bubble-style scatter chart with a bar chart when the data are one-dimensional and the main job is comparison.
- If one complex visualization is carrying several simple comparisons, split it into several simple charts.
- Re-test the revised chart against the original and keep the version viewers say is easier to interpret.
