---
id: avoid-hard-boundaries-for-continuous-uncertainty
title: Avoid hard boundaries when encoding continuous uncertainty
bibliography: references.bib
description: For uncertainty judgments on continuous data, avoid hard boundary encodings
  on maps or interval displays to improve fidelity and mitigate containment and deterministic
  reading errors for viewers interpreting probabilistic information.
labels:
- purpose:refine
- basis:empirical
- operator:uncertainty
- quality:fidelity:use
- lever:encoding
- channel:line-style:avoid
---

## Boundary treatment <!-- role: advice -->

Avoid enclosing continuous or probabilistic ranges with hard boundaries when readers should interpret gradual uncertainty. For example, replace a bounded uncertainty region with a graded fade or an ensemble of possible paths, and avoid interval displays that look like discrete high and low endpoints when the message is probabilistic spread.

## Why hard boundaries mislead <!-- role: reason -->

A hard outline implies categorical inside-versus-outside status. Readers then treat nearby values across the boundary as more different than they really are, or read the bounded region as a deterministic forecast rather than a probability distribution.

**Mechanism:** Boundary marks trigger a containment heuristic and make the enclosed area feel semantically distinct, which distorts judgments about continuity and likelihood.

**Evidence:** The review synthesizes evidence that bounded circles, cones, and interval-like displays can produce containment and deterministic construal errors, while graded or ensemble-style displays can better support probabilistic interpretation [@padillaDecisionMakingVisualizations2018].

**Notes:** Summarizing continuous data into bins can simplify a display, but the boundary itself can become the dominant message.

## Use when the message is probabilistic <!-- role: context -->

- **User Goal:** Judge uncertainty, likelihood, or probable location/path.
- **Task:** Compare nearby positions or values within a continuous or probabilistic range.
- **Data:** Continuous, uncertain, or distributional information.
- **Chart Setting:** Maps or interval-like displays that could be drawn with enclosing outlines or bounded regions.
- **Audience:** Nonexperts or mixed audiences interpreting probability visually.
- **Success Criterion:** Readers treat the data as gradual or probabilistic rather than categorical.

## Do not use when the boundary is the message <!-- role: exceptions -->

**Break it when:** The display intentionally defines discrete bins or a true cutoff where inside and outside should be treated differently. **Why:** In that case the boundary is not an artifact; it is the intended classification.

## Costs of removing hard boundaries <!-- role: costs -->

**Sacrifice:** You lose a crisp categorical edge.
**Risk:** Some readers may find graded uncertainty less immediate than a simple enclosed region.

## Common boundary failure <!-- role: mistakes -->

**Mistake:** Draw a bold enclosing region around continuous uncertainty and expect readers to infer gradual probability from it. **Why it fails:** The outline encourages an inside/outside reading and hides variation within the region.

## How to test for containment bias <!-- role: check -->

**Failure Sign:** Readers treat points just across a boundary as categorically different, or they describe the display as a sure path or fixed range.
**Quick Check:** Ask whether two nearby positions on opposite sides of the boundary are judged more differently than two equally close positions within the same region.
**Stronger Test:** Compare the bounded version against a graded or ensemble version and see whether judgments become less categorical.

## How to repair boundary-driven misreadings <!-- role: fix -->

- Remove or soften enclosing outlines around continuous uncertainty.
- Replace a single bounded summary region with a graded fade when the message is gradual likelihood.
- Replace a bounded path region with an ensemble of possible paths when the message is spread across alternatives.
- Redesign interval-like uncertainty displays so they do not read as discrete endpoints.
