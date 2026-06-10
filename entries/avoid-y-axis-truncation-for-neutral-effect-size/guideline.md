---
id: avoid-y-axis-truncation-for-neutral-effect-size
title: Avoid truncating the y-axis when neutral effect size matters
bibliography: references.bib
description: For compare or trend judgments, avoid y-axis truncation on quantitative
  charts to improve fidelity and mitigate exaggerated effect-size judgments for viewers
  making overview assessments.
labels:
- purpose:refine
- basis:empirical
- data:quantitative
- quality:fidelity:use
- lever:scale-order
- component:axis
- reading-mode:overview
---

## Y-axis range <!-- role: advice -->

Use a wider y-axis range when readers need an unbiased read of how large a difference or trend is. For example, avoid raising the y-axis start from 0 to 25% or 50% on bar charts or line charts when the same data need a neutral read of severity.

## Why a wider range changes interpretation <!-- role: reason -->

A tighter y-axis makes the visible vertical gap larger, so the same numbers look like a stronger difference. Readers carry that stronger visual impression into qualitative judgments even when they can still read the chart correctly.

**Mechanism:** Truncation magnifies the apparent height or slope of the data, which increases judged severity without changing the underlying values.

**Evidence:** Across repeated-measures experiments, higher y-axis starts produced higher perceived severity ratings, and this effect appeared for both bar charts and line charts. The bias persisted even when participants could estimate the underlying values accurately in a separate value-reading task [@correllTruncatingYAxisThreat2020].

**Notes:** The paper argues against a strict honest-versus-dishonest split and instead treats y-axis range as a deliberate choice that changes how strong the effect feels.

## When this applies <!-- role: context -->

- **User Goal:** Show how large a difference or change should feel without overstating it.
- **Task:** Readers compare endpoints or judge how quickly values are changing.
- **Data:** Quantitative values occupy a narrow range, so truncation is tempting.
- **Chart Setting:** A static chart with a quantitative y-axis, including bar charts and line charts.
- **Audience:** Readers are making quick qualitative judgments from the visual shape of the chart.
- **Success Criterion:** Perceived severity stays driven by the data rather than by axis cropping.

## When to break it <!-- role: exceptions -->

**Break it when:** The task is specifically to show deviations from a non-zero reference or small but meaningful changes that disappear on a zero baseline. **Why:** The paper explicitly notes cases such as anomaly, index, process, and stock-style charts where zero is not always the meaningful reference point.

## Costs of a wider range <!-- role: costs -->

**Sacrifice:** Small differences can look flatter and less salient.
**Risk:** A zero baseline or similarly wide range can hide narrow but important variation.
**Mitigation:** Choose the range by the meaningful effect size you need to communicate rather than treating either zero or strong truncation as an automatic default.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Keep the truncated range and expect a line chart to solve the exaggeration that appeared in a bar chart. **Why it fails:** The paper found similar inflation in perceived severity for truncated bar charts and truncated line charts.

## How to test it <!-- role: check -->

**Failure Sign:** The same data look much more dramatic after you raise the y-axis start.
**Quick Check:** Render the same chart with the current start value and with a wider y-axis range, then compare how severe the change feels.
**Stronger Test:** Ask a reviewer to rate the effect size on both versions; a large shift in ratings shows that the axis choice is driving interpretation.

## What to change <!-- role: fix -->

- Lower the y-axis start or widen the plotted range.
- Compare the truncated version against a wider-range version before finalizing the chart.
- Keep a truncated view only when you intentionally want to emphasize small deviations and have decided that emphasis fits the task.
