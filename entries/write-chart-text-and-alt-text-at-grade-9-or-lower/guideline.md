---
id: write-chart-text-and-alt-text-at-grade-9-or-lower
title: Write chart text and alternative text at grade 9 or lower
bibliography: references.bib
description: For accessibility review of a data visualization, use plain-language
  text annotation on chart text and alternative text to improve accessibility and
  mitigate comprehension barriers for readers with cognitive disabilities.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:text-annotation
- needs:cognitive
- access:plain-language:use
---

## Simplify chart text <!-- role: advice -->

Write every visible chart text element and every alternative text element to a ninth-grade reading level or lower. For example, shorten complex sentences, replace jargon with simpler wording, and if a technical term must remain, add a short plain-language explanation written at grade 9 or lower.

## Why lower reading level helps <!-- role: reason -->

Lower-complexity wording reduces ambiguity and cognitive load in the text that people use to understand a visualization. Defining unavoidable specialized terms lets readers keep needed precision without making the chart text harder to process.

**Mechanism:** Simpler wording makes chart text easier to read directly, and plain-language explanations prevent unfamiliar terms from blocking understanding.

**Evidence:** Chartability marks inappropriate reading level as a critical understandable accessibility issue and requires all text and alternative text to target a reading grade level of 9 or lower, with analytical tools used to estimate readability [@elavskyHowAccessibleMy2022]. W3C guidance says complex or unfamiliar terms should be supported with definitions or supplementary explanation, and the Hemingway Editor is described as a tool that flags complex sentences and estimates readability grade level [@w3c_understanding_meaningful; @hemingwayapp_hemingway_editor].

**Notes:** This rule applies to both visible text and alternative text.

## Use when chart text must be understood directly <!-- role: context -->

- **User Goal:** Understand the visualization's text support without extra interpretation.
- **Chart Setting:** The visualization includes visible text or alternative text that explains, supplements, or accompanies the data.
- **Audience:** Readers include people with cognitive disabilities or readers who may not know specialized terms.
- **Success Criterion:** Each text block reads at grade 9 or lower, and any required technical term is explained in simpler language.

## Keep required terms only when they must stay <!-- role: exceptions -->

**Break it when:** A specialized term is required for accuracy and cannot be removed. **Why:** The term may stay, but it must be explained with supplementary text written at grade 9 or lower.

## Tradeoffs of simplifying chart text <!-- role: costs -->

**Sacrifice:** You may need extra explanatory text when a required technical term cannot be replaced.
**Risk:** Simplifying blindly can remove terminology that is necessary for accuracy.
**Mitigation:** Keep the required term and add a short plain-language definition beside it or in supplementary text.

## Common failure modes <!-- role: mistakes -->

- **Mistake:** Simplify only visible text and leave alternative text dense or jargon-heavy. **Why it fails:** The requirement covers all provided text, including alternative text.
- **Mistake:** Leave complex terminology unexplained. **Why it fails:** Complex terms are only acceptable when they are explained in simpler language.

## Check reading level directly <!-- role: check -->

**Failure Sign:** A readability tool scores any chart text or alternative text above grade 9, or the text contains unexplained specialized terms.
**Quick Check:** Run a reading-level tool on every visible text block and every alternative text block.
**Stronger Test:** Verify that each unavoidable technical term has a plain-language explanation written at grade 9 or lower.

## Fix the text <!-- role: fix -->

- Rewrite long or complex sentences in visible text and alternative text until they read at grade 9 or lower.
- Replace jargon with simpler words where accuracy allows.
- Add a short plain-language definition for any technical term that must remain.
