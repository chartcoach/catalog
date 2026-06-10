---
id: use-neutral-open-ended-titles-when-a-chart-supports-opposing-interpretations
title: Use a neutral open-ended title when a chart supports opposing interpretations
bibliography: references.bib
description: For explanation of controversial single-view visualizations, use neutral
  open-ended titles on multi-measure charts to improve fidelity and mitigate unnoticed
  one-sided interpretation for viewers who may assume statistical displays are impartial.
labels:
- purpose:refine
- basis:empirical
- quality:fidelity
- lever:text-annotation
- component:title:use
- measure:multi
- communication:framing
---

## Neutral title framing <!-- role: advice -->

Use a neutral open-ended title instead of an advocacy title when one chart contains measures that can support opposite sides of a controversial issue. For example, state the chart's topic or name both displayed measures rather than titling the chart with only the percentage, absolute value, or comparison that favors one side.

## Title slant becomes the chart's message cue <!-- role: reason -->

Readers often take the title as the chart's main message before they inspect the rest of the display. On controversial charts, that first cue can steer recall toward one interpretation even when the same marks also support another reading.

**Mechanism:** A neutral open-ended title reduces the chance that viewers will anchor on one side of the issue and overlook the other displayed measure.

**Evidence:** Experiment 2 found a significant association between title slant and the slant of the recalled main message, with most slanted recalled messages matching the slant of the title shown. Experiment 1 also found that default and neutral titles were most often open-ended, while many viewers in Experiment 2 still judged titled visualizations as neutral even when their recalled message reflected the title's slant [@kongFramesSlantsTitles2018].

**Notes:** The paper highlights statistics-framed titles as especially easy to mistake for neutral even when they steer attention to one side.

## Use when the chart is about a contested issue <!-- role: context -->

- **User Goal:** Present a controversial issue without steering readers to one side through the title alone.
- **Task:** Compose a title that supports interpretation rather than argument.
- **Data:** One visualization shows multiple displayed measures that support different interpretations.
- **Chart Setting:** A standalone chart where the title is visible during reading.
- **Audience:** Viewers who may treat statistical displays as inherently neutral.
- **Success Criterion:** Viewers can describe the issue without simply repeating a one-sided title as the chart's main message.

## Do not rely on this outside the tested setting <!-- role: exceptions -->

**Break it when:** The chart is read together with substantial accompanying text or covers a less controversial topic. **Why:** The paper only tested standalone visualizations on controversial issues and notes that transfer beyond those settings is uncertain.

## You give up directional messaging <!-- role: costs -->

**Sacrifice:** You give up a strong argumentative takeaway in the title.
**Risk:** The title will do less to steer readers toward one preferred interpretation.
**Mitigation:** If the title still needs to summarize data, name both displayed measures rather than only the one that supports one side.

## A statistical title can still be slanted <!-- role: mistakes -->

**Mistake:** Use a statistics-sounding title that mentions only one favorable measure and assume it reads as neutral. **Why it fails:** Readers often treat statistical titles as impartial while still taking that one-sided cue as the chart's main message.

## Test whether the title already argues a side <!-- role: check -->

**Failure Sign:** Reviewers can tell which side of the issue the title supports before they inspect the chart.
**Quick Check:** Read the title alone and label which side of the issue it supports; if that is possible, the title is not neutral.
**Stronger Test:** Ask a reviewer to write the chart's main message after viewing it; if the answer repeats the title's slant and ignores the other displayed measure, the title is steering interpretation.

## Replace one-sided title language <!-- role: fix -->

- Replace a one-sided comparison title with a topic-level title.
- Rewrite a one-sided statistics title to name both displayed measures instead of only one.
- Remove title language that explicitly supports or opposes one side of the issue.
