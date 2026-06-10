---
id: define-metrics-variables-calculations-and-source-near-chart
title: Define every metric, variable, calculation, and data source next to the chart
bibliography: references.bib
description: For chart reading and interpretation, use nearby explanatory text on
  charts and data interfaces that introduce named or derived measures to improve accessibility
  and address misleading or undefined metrics, variables, calculations, and sources
  for readers who need definitions ready and convenient.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility:use
- lever:text-annotation
- communication:context
---

## Add adjacent definitions for measures and source <!-- role: advice -->

Add chart-adjacent explanatory text that defines every variable, metric, calculation, and data source used in the view. For example, move a metric definition out of surrounding article paragraphs and into text immediately next to the chart so a reader can identify what the measure means, how it is calculated, and where the data comes from.

## Undefined measures force readers to infer meaning <!-- role: reason -->

Undefined measure names make readers stop interpreting the chart and start searching for missing context. Keeping definitions and source information next to the chart reduces ambiguity and makes the needed context available at the point of reading.

**Mechanism:** Nearby definitions let readers resolve what each variable or metric means without leaving the chart, which lowers interpretation effort and reduces the chance of being misled by undefined or unexplained measures.

**Evidence:** Chartability treats undefined metrics and variables as an Understandable failure and states that data, source, metadata, metrics, calculations, and variables must be defined, with that information kept as close to the chart or data interface as possible [@elavskyHowAccessibleMy2022]. Guidance for accessible description of scientific graphics likewise emphasizes defining variables, units, and metrics so complex visuals remain understandable to blind readers [@wgbh_effective_practices].

## Use when the chart introduces terms a reader must decode <!-- role: context -->

- **User Goal:** Understand what each measure in the chart means without searching elsewhere.
- **Data:** The chart uses named variables, derived metrics, calculations, metadata fields, or source-dependent claims.
- **Chart Setting:** Definitions are absent from the chart or appear only in surrounding article text instead of adjacent chart text.
- **Audience:** Readers who need the information ready and convenient at the chart.
- **Success Criterion:** A reader can explain each measure and identify the data source from the chart and its immediately adjacent text.

## Do not add more when the definitions are already adjacent <!-- role: exceptions -->

**Break it when:** The chart and its immediately adjacent text already define every variable, metric, calculation, and data source used in the view. **Why:** This rule addresses missing or distant definitions.

## Extra context takes space near the chart <!-- role: costs -->

**Sacrifice:** The chart needs extra adjacent text for definitions and source information.\
**Risk:** If the added definitions are incomplete or scattered away from the chart, readers still have to search for missing context.\
**Mitigation:** Keep the variable, metric, calculation, and source definitions together in one nearby text block.

## Common ways this still fails <!-- role: mistakes -->

- **Mistake:** Leaving variable or metric definitions only in surrounding body text. **Why it fails:** Readers must leave the chart to recover information that should be ready and convenient.
- **Mistake:** Naming a calculated measure without explaining how it is derived or where the data came from. **Why it fails:** The chart remains misleading because key terms are still undefined.

## Check whether the chart can be read without hunting for definitions <!-- role: check -->

**Failure Sign:** A variable name, metric, calculation, or source cannot be explained from the chart and the text immediately next to it.\
**Quick Check:** Read only the chart and its adjacent text; if you cannot define each measure and identify the data source, it fails.\
**Stronger Test:** Ask a reviewer to explain the variables and calculations without searching the wider article or interface.

## Move missing definitions into chart-adjacent text <!-- role: fix -->

- Add adjacent text that defines each variable and metric used in the chart.
- State how any calculated measure is computed.
- Identify the data source in the same nearby text.
- Move definitions out of surrounding paragraphs and place them immediately next to the chart or data interface.
