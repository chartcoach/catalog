---
id: use-line-charts-to-foreground-x-y-interactions
title: "Use line charts to foreground x\u2013y interactions"
bibliography: references.bib
description: "For open-ended interpretation of grouped three-variable data, use a\
  \ line chart instead of a bar chart on multivariate quantitative graphs to improve\
  \ insight into x\u2013y interactions and mitigate unintended focus on legend-variable\
  \ contrasts for viewers identifying the main point."
labels:
- purpose:select
- basis:empirical
- task:relate
- chart:line:use
- chart:bar:avoid
- quality:insight
- lever:chart-family
- measure:multi
---

## Use connected lines for the intended interaction <!-- role: advice -->

Choose a line chart when the main message is the x–y relationship and the legend variable should read as the moderator. For example, use connected lines instead of grouped bars for three-variable data when you want viewers to say how y changes across x for each legend-coded group.

## Why the line chart works here <!-- role: reason -->

Connected lines make the x-axis relationship the dominant visual chunk, so viewers tend to read change across x first and treat the legend variable as the condition on that relationship.

**Mechanism:** Good continuity groups points into lines, which makes the x–y relationship visually salient and encourages interaction descriptions framed around the x-axis variable.

**Evidence:** In written descriptions of multivariate graphs, viewers described x–y interactions more often from line graphs than from bar graphs, and this x–y emphasis was strongest when the content was unfamiliar. [@shahBarLineGraph2011]

**Notes:** The line chart created a stronger directional bias than the bar chart.

## When to use this contrast <!-- role: context -->

- **User Goal:** The reader should state the x–y interaction as the main point.
- **Task:** Open-ended explanation of what matters most in a three-variable graph.
- **Data:** Two ordered independent variables and one quantitative dependent variable.
- **Chart Setting:** One variable is on the x-axis and the other grouping variable is shown in the legend as separate lines.
- **Audience:** Topic familiarity may be low; the line-chart emphasis on x–y interactions was strongest for unfamiliar content.
- **Success Criterion:** Readers spontaneously describe how y changes across x, qualified by the legend-coded groups.

## When not to use this contrast <!-- role: exceptions -->

**Break it when:** The intended message is a comparison among legend categories within each x-axis group, or a main effect that ignores one variable. **Why:** Line charts steered viewers away from those readings and toward x–y interaction descriptions.

## Tradeoffs of the line chart choice <!-- role: costs -->

**Sacrifice:** You give up emphasis on within-group legend-category comparisons and on main-effect summaries.\
**Risk:** Readers may overlook alternative summaries of the same data because the connected lines strongly cue one interpretation.\
**Mitigation:** If those alternative summaries are the message, switch to a grouped bar chart instead of trying to force them out of the line chart.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Using a line chart when the key message is the legend-variable comparison inside each x-axis group. **Why it fails:** The line chart encourages readers to describe change across x instead of the intended grouped comparison.

## How to test the choice <!-- role: check -->

**Failure Sign:** Reviewers lead with a different summary than the intended x–y interaction.\
**Quick Check:** Show matched line and bar versions and ask, “What is the main point?” Choose the line chart only if the x–y interaction is mentioned more readily from the line version.\
**Stronger Test:** Run the same prompt with viewers unfamiliar with the topic, since reliance on the line chart’s x–y cue was strongest there.

## What to change <!-- role: fix -->

- Replot the grouped bars as connected lines while keeping the same variables on the x-axis and in the legend.
- Retest with an open-ended “main point” prompt and keep the line chart only if readers now lead with the intended x–y interaction.
- If readers still need to notice grouped legend-category comparisons or main effects instead, replace the line chart with a grouped bar chart.
