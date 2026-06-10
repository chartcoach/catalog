---
id: state-data-source-collection-processing-and-omissions
title: State the data source, collection method, processing, and omissions
bibliography: references.bib
description: For explanatory communication, use provenance and methodology text on
  visualization captions or notes to improve trust and address credibility doubts
  from unexplained sources, processing, and omissions for viewers assessing whether
  the visualization is reliable.
labels:
- purpose:refine
- basis:rhetorical
- quality:trust
- lever:text-annotation
- communication:credibility
- component:caption:use
---

## Provenance note <!-- role: advice -->

Add a provenance note that states where the data came from, how it was collected, how it was processed, and what was omitted. For example, put this information in the caption or note, say which part of the visualization uses which source when you combine datasets, and explain blank regions or missing values instead of leaving them unexplained.

## Why provenance details increase trust <!-- role: reason -->

Readers judge credibility from the information around the chart as well as from the marks themselves. When the source and method are visible, viewers have less reason to infer that the display is unsupported, incomplete, or hiding missing information.

**Mechanism:** Provenance text makes the evidence trail visible, so readers can connect what they see to a source, a collection process, any processing steps, and any deliberate omissions.

**Evidence:** Viewers tended to trust visualizations more when they found the data source reputable, and methodological details in captions were appreciated because they helped people produce more complete and accurate messages [@knoll_gulf_2025; @koesten_what_2023]. Viewers expressed distrust when blank parts of maps were left unexplained, and published science graphics commonly specified data sources, distinguished source types, mapped combined sources to specific parts of the visualization, and credited contributors [@koesten_encountering_2025; @gregory_data_2024].

**Notes:** When multiple datasets appear in one visualization, the provenance note needs to distinguish which source supports which part of the display.

## Use when credibility depends on chart context <!-- role: context -->

- **User Goal:** Build trust in an explanatory visualization.
- **Task:** Show what data is used and what was done to it before plotting.
- **Data:** The visualization uses external data, combines multiple sources, includes processing steps, or contains omitted or unavailable values.
- **Chart Setting:** A caption or note can carry methodological detail, and some chart parts may come from different sources or appear blank.
- **Audience:** Viewers may question credibility if the evidence trail is incomplete.
- **Success Criterion:** A viewer can identify the source, collection method, processing, and explanation for any blank or omitted parts from the chart text.

## Do not treat a generic source line as sufficient <!-- role: exceptions -->

**Break it when:** the visualization combines sources or shows blank or missing parts, but the note gives only one undifferentiated source line. **Why:** viewers still cannot tell which source supports which part of the display or whether blanks reflect omission, unavailability, or missing explanation.

## Tradeoffs of provenance detail <!-- role: costs -->

**Sacrifice:** The caption or note becomes longer because it carries methodological context.
**Risk:** A short generic source line can look complete while still leaving credibility gaps.
**Mitigation:** Keep the note focused on source, collection, processing, source-to-chart mapping, and explained omissions.

## Common provenance failures <!-- role: mistakes -->

- **Mistake:** Naming only the source. **Why it fails:** Readers still do not know how the data was collected, how it was processed, or whether anything was omitted.
- **Mistake:** Listing several sources without mapping them to specific chart parts. **Why it fails:** Readers cannot tell what evidence underlies each region, layer, or component.
- **Mistake:** Leaving blank regions or missing values unexplained. **Why it fails:** Viewers can read the gaps as a credibility problem rather than as documented missing or omitted data.

## Check provenance coverage <!-- role: check -->

**Failure Sign:** A reviewer cannot tell where the data came from, how it was collected, how it was processed, or why visible gaps or missing values exist.
**Quick Check:** Read only the chart caption or note and answer four questions: source, collection, processing, and omissions.
**Stronger Test:** In a multi-source or partially blank visualization, ask a reviewer to point to each visible part and say which source supports it and why any empty region is empty.

## Fix incomplete provenance <!-- role: fix -->

- Add a caption or note that names the data source and states how the data was collected.
- Add one sentence that states the main processing or transformation applied before plotting.
- When multiple datasets are combined, state which chart part uses which source.
- Add an explicit explanation for blank regions, omitted values, or unavailable data.
