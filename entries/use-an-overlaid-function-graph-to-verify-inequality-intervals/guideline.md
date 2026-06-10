---
id: use-an-overlaid-function-graph-to-verify-inequality-intervals
title: Use an overlaid function graph to verify interval solutions
bibliography: references.bib
description: For compare tasks on non-temporal quantitative functions, use a line
  chart instead of text-only checking on paired function displays to improve fidelity
  and mitigate missed extra-intersection mistakes for learners verifying inequality
  intervals.
labels:
- purpose:select
- basis:empirical
- task:compare
- chart:line:use
- chart:text:avoid
- data:quantitative
- quality:fidelity:use
- lever:chart-family
- operator:difference
---

## Overlay the functions for interval checks <!-- role: advice -->

Plot both functions on the same axes when you need to verify where one expression is above, equal to, or below the other. For example, use the graph to confirm the full solution interval of an inequality and to catch extra crossings outside the expected endpoints instead of checking only symbolic substitutions at a few values.

## Why the overlaid graph works <!-- role: reason -->

An overlaid graph turns an interval check into a whole-range comparison instead of a few sampled algebraic checks. That makes missed intersections visible and shows the exact regions where one function is above, equal to, or below the other.

**Mechanism:** The graph externalizes the sign comparison across the x-range, so users can inspect intervals directly rather than infer them from separate substitutions.

**Evidence:** In the study, students who connected symbolic and graphical forms could produce candidate solutions, and graphical verification exposed an extra third intersection that had been missed by an endpoint-based solution; the paper states that the graphical representation simplified verification by showing where one graph is above, coincides with, or is below the other [@mesaSolvingProblemsFunctions2008].

**Notes:** The study also showed that widening the plotted range mattered: the extra intersection became clear only after the viewing window was extended.

## Use when all of these are true <!-- role: context -->

- **User Goal:** Verify that a proposed interval really is the full solution to an inequality between two functions.
- **Task:** Compare two continuous functions across an x-range, not just at named endpoints.
- **Data:** Quantitative function data with candidate expressions already available.
- **Chart Setting:** Both functions can be plotted together, and the view can be extended beyond the expected interval.
- **Audience:** Learners or problem solvers checking a candidate answer.
- **Success Criterion:** All intersections and above/below regions are found, including any outside the expected interval.

## Do not use when this condition holds <!-- role: exceptions -->

**Break it when:** The task is still to derive the expressions from scratch and users do not yet have a candidate pair of functions to plot. **Why:** In the study, students who treated the unknown parameters as a reason not to graph could not use the display productively.

## Costs of this choice <!-- role: costs -->

**Sacrifice:** The graph verifies a candidate answer but does not itself provide the algebraic derivation.
**Risk:** A narrow viewing window or a quick visual match can hide an additional intersection.
**Mitigation:** Extend the displayed x-range beyond the target interval before accepting the result.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Verify only the named endpoints or only the visible local part of the plot. **Why it fails:** A third intersection can lie outside the expected interval even when the endpoints look correct.

## Review check <!-- role: check -->

**Failure Sign:** The candidate answer matches the target endpoints, but the graph has not been checked outside that local range.
**Quick Check:** Ask whether checking a few substituted x-values could still miss another crossing; if yes, prefer the overlaid graph to text-only checking.
**Stronger Test:** Widen the plotting window and confirm that the overlaid graph shows exactly the intended intersections and above/below regions.

## Fix the problem <!-- role: fix -->

- Plot both candidate functions on the same axes before finalizing the interval.
- Extend the x-range beyond the expected solution interval to look for extra crossings.
- Use the graph to inspect where one curve is above, equal to, and below the other across the whole visible range.
- If the graph reveals an unintended extra intersection, revise the function parameters and re-plot before accepting the answer.
