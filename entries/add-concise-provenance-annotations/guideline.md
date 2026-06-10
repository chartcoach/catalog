---
id: add-concise-provenance-annotations
title: Add concise provenance annotations
bibliography: references.bib
description: For explanatory narrative visualization, use text annotation on the presentation
  to improve trust and mitigate hidden editorial choices for readers interpreting
  a guided story.
labels:
- purpose:refine
- basis:empirical
- quality:trust:use
- lever:text-annotation
- communication:credibility
- component:annotation:use
---

## Provenance annotations <!-- role: advice -->

Add concise provenance annotations that disclose the data source, method, and important exceptions or corrections. For example, cite the source dataset, link to methodological notes, and mark exceptional cases or corrections directly in or beside the visualization.

## Why provenance annotations work <!-- role: reason -->

Provenance notes make editorial decisions visible at the moment of reading. That shifts the chart from an unexplained claim to a documented presentation and helps readers judge how much to trust the story.

**Mechanism:** Source, method, and correction notes signal transparency and trustworthiness without requiring readers to infer where the data came from or how the graphic was prepared.

**Evidence:** A qualitative analysis of 51 professionally produced narrative visualizations identified data source citations, methodology references, and exception or correction notes as recurring techniques that signal transparency and trustworthiness to end-users. The paper also notes that exhaustive provenance for every design manipulation is often impossible and can burden a concise visual representation, which is why concise provenance is the actionable form [@hullmanVisualizationRhetoricFraming2011].

**Notes:** The rule is about selective disclosure of key provenance, not exhaustive disclosure of every design choice.

## Use when concise provenance matters <!-- role: context -->

- **User Goal:** Understand and trust the chart's story.
- **Task:** Interpret a guided explanation rather than inspect raw data independently.
- **Data:** Data source, method, exceptions, or corrections materially affect how the story should be read.
- **Chart Setting:** Narrative visualization with surrounding text, caption space, or linked notes.
- **Audience:** Readers who are not expected to reconstruct provenance on their own.
- **Success Criterion:** A reader can identify where the data came from and what major caveats apply.

## Do not overextend provenance disclosure <!-- role: exceptions -->

**Break it when:** Following the rule would require exhaustive disclosure of every design manipulation or implicit author intention. **Why:** The paper argues that full provenance may be impossible and can reduce the value of a concise visual representation.

## Costs of concise provenance annotations <!-- role: costs -->

**Sacrifice:** You give up some visual space and brevity.
**Risk:** Long provenance text can compete with the chart's main message.
**Mitigation:** Keep the on-chart note short and move detail into linked methodological notes.

## Common provenance annotation mistake <!-- role: mistakes -->

**Mistake:** Omitting source and method notes from the presentation. **Why it fails:** Readers cannot easily detect those omissions, so the chart hides key editorial choices instead of signaling transparency.

## Check provenance visibility <!-- role: check -->

**Failure Sign:** The visualization makes claims without any visible source, method, or correction note.
**Quick Check:** Can a reviewer identify the data source and the main method note from the chart area or one linked note?
**Stronger Test:** Ask a reviewer to state the data source and one caveat before they interpret the chart's conclusion.

## Fix missing provenance <!-- role: fix -->

- Add a visible data source citation near the chart.
- Add a short methodology note or link to a method page.
- Annotate any exceptions, corrections, or unusual cases directly on the visualization.
