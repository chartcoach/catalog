---
id: review-chart-against-applicable-accessibility-standards
title: Review the chart against all applicable accessibility standards
bibliography: references.bib
description: For accessibility review of an implemented chart, use standards-based
  conformance checks on chart structure and interaction to improve assistive-technology
  compatibility and address unchecked standards failures for users of compliant assistive
  technologies.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:interaction-access
- communication:workflow
---

## Standards conformance review <!-- role: advice -->

Review the chart against every applicable accessibility requirement before treating it as accessible. For example, check the chart against relevant WCAG 2.1, Section 508, or equivalent criteria, then run automated checks and manually inspect whether the chart's semantics and parsing can be interpreted consistently by assistive technologies.

## Why standards conformance matters <!-- role: reason -->

Accessibility standards provide a baseline for whether a chart's implemented structure can be parsed and exposed consistently to assistive technologies. Treating missing conformance as a failure prevents a chart from being accepted on appearance alone before its structure and semantics have actually been verified.

**Mechanism:** Standards conformance makes the chart's structure and interaction more reliable for compliant assistive technologies, and an automatic-failure stance prevents incomplete review from being mistaken for accessibility.

**Evidence:** Chartability defines lack of conformance to relevant WCAG 2.1, Section 508, or equivalent requirements as a robustness failure and says to treat the chart as an automatic failure until it can be fully evaluated. W3C guidance for compatible parsing explains that content should be unambiguously parsed so assistive technologies can interpret it consistently and reliably [@elavskyHowAccessibleMy2022; @w3c_understanding_ensure].

## When to apply this review <!-- role: context -->

- **User Goal:** Confirm that the chart works with compliant assistive technologies.
- **Task:** Audit a built chart or data interface for accessibility conformance.
- **Chart Setting:** An implemented digital chart with structure, semantics, or interaction that can be checked against WCAG 2.1, Section 508, or an equivalent standard.
- **Audience:** People using compliant assistive technologies.
- **Success Criterion:** All relevant applicable standards checks pass, and the chart no longer counts as an automatic failure.

## When not to force a requirement <!-- role: exceptions -->

**Break it when:** A specific standards requirement does not apply to the chart or interface. **Why:** This guideline requires passing relevant requirements where applicable, not irrelevant ones.

## What this review step costs <!-- role: costs -->

**Sacrifice:** The chart cannot be treated as passing until standards review is complete.\
**Risk:** A partial review can leave failures in place while the chart appears finished.\
**Mitigation:** Keep the chart in automatic-failure status until all applicable standards checks have been completed and repaired.

## Common ways this fails <!-- role: mistakes -->

- **Mistake:** Using Chartability as a substitute for WCAG, Section 508, or equivalent standards review. **Why it fails:** Chartability is intended to work alongside existing standards and guidelines, not replace them.
- **Mistake:** Treating the chart as passed before the applicable standards review is complete. **Why it fails:** This heuristic is an automatic failure until the chart can be fully evaluated.

## How to verify conformance <!-- role: check -->

**Failure Sign:** The chart has unchecked or failing applicable WCAG 2.1, Section 508, or equivalent requirements.\
**Quick Check:** If you cannot point to a completed review of all relevant applicable standards criteria, record a failure.\
**Stronger Test:** Run an automated standards evaluation, then manually inspect whether the chart's semantics and parsing are exposed in a form assistive technologies can interpret consistently.

## What to change when it fails <!-- role: fix -->

- Review the chart against every relevant WCAG 2.1, Section 508, or equivalent requirement that applies to it.
- Repair semantic or parsing failures so assistive technologies can interpret the chart consistently.
- Re-run the automated and manual checks after repair.
- Keep the chart marked as failed until the applicable standards review passes.
