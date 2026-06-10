---
id: name-the-measure-in-a-trend-title-when-a-chart-shows-multiple-measures
title: Name the measure in a trend title when a chart shows multiple measures
bibliography: references.bib
description: For trend explanation in controversial single-view visualizations, use
  measure-specific trend titles on multi-measure charts to improve fidelity and mitigate
  ambiguous trend interpretation for viewers who may not detect title framing.
labels:
- purpose:refine
- basis:empirical
- task:trend
- quality:fidelity
- lever:text-annotation
- component:title:use
- measure:multi
- communication:framing
---

## Measure-specific trend titles <!-- role: advice -->

Include the referenced measure directly in any trend title when the chart shows more than one displayed measure. For example, attach the measure to the trend claim with wording such as a percentage basis or constant-value basis instead of saying a quantity simply rises or falls when another displayed measure moves differently.

## Unqualified trend words invite the wrong reading <!-- role: reason -->

A trend title can be factually true for one displayed measure and false for another measure in the same chart. When the title omits the measure name, readers can map the claim to the wrong line, section, or scale.

**Mechanism:** Naming the measure tells readers exactly which displayed trend the title summarizes and prevents them from generalizing the claim to the whole chart.

**Evidence:** Experiment 2 showed that slanted titles changed the perceived main message of the same visualization. In the discussion, the paper identifies trend titles that omit the referenced measure as a misleading form of statistics frame on multi-measure charts because viewers can infer that the trend applies to the wrong displayed measure [@kongFramesSlantsTitles2018].

**Notes:** The paper describes this as a subtle form of framing because the title can sound statistical and neutral while still steering interpretation.

## Use when one chart contains competing trends <!-- role: context -->

- **User Goal:** Summarize a trend accurately in the title.
- **Task:** Communicate which displayed trend matters.
- **Data:** One chart shows multiple displayed measures that move differently or support opposite sides of an issue.
- **Chart Setting:** A title summarizes a line, series, or chart section in a standalone visualization.
- **Audience:** Viewers who may not inspect every displayed measure before forming a takeaway.
- **Success Criterion:** Readers can identify exactly which displayed measure the trend statement refers to.

## Skip this when no trend ambiguity exists <!-- role: exceptions -->

**Break it when:** The chart shows only one displayed measure or the title is intentionally topic-only rather than trend-based. **Why:** The ambiguity comes from unqualified trend claims on charts with multiple displayed measures.

## Precision costs title brevity <!-- role: costs -->

**Sacrifice:** The title becomes longer.
**Risk:** A vague noun can still imply the wrong measure even after you add a trend word.
**Mitigation:** Use the exact displayed measure name, not a broad umbrella term.

## Generic rise-fall wording is the failure mode <!-- role: mistakes -->

**Mistake:** Write a trend title that says a quantity increases or decreases without naming the measure. **Why it fails:** Readers can attach the claim to the wrong displayed measure when the chart contains more than one metric.

## Check whether the trend claim answers “of what?” <!-- role: check -->

**Failure Sign:** The title contains increase, decrease, higher, or lower language but reviewers cannot say which displayed measure it refers to.
**Quick Check:** If the chart has multiple displayed measures, scan the title for the explicit measure name next to the trend claim; if it is missing, revise.
**Stronger Test:** Ask a reviewer which displayed measure the title refers to; if answers vary or point to different lines or sections, the title is ambiguous.

## Edit the trend claim to bind it to one measure <!-- role: fix -->

- Insert the exact measure name directly into the trend statement.
- Replace broad nouns that could refer to multiple displayed measures with the specific displayed metric.
- If concise disambiguation is not possible, replace the trend title with a neutral topic title.
