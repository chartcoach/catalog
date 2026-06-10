---
id: use-triplet-matching-to-learn-perceptual-kernels
title: Use triplet matching to learn perceptual kernels for encoding design
bibliography: references.bib
description: For perceptual similarity collection in visualization design, prefer
  triplet matching on encoding palettes to improve kernel fidelity and mitigate high-variance
  or underexpressive estimates for designers building perceptual models.
labels:
- purpose:refine
- basis:empirical
- quality:fidelity
- lever:interaction-access
- communication:workflow
- audience:designer
---

## Collect similarity with triplet matching <!-- role: advice -->

Use triplet matching with a designated reference item when collecting perceptual judgments for palette design. For example, show three symbols and ask which of two candidates is more similar to the reference, rather than asking for a Likert similarity rating or asking people to arrange items in a plane.

## Why triplet matching works better <!-- role: reason -->

Triplet matching asks for a simple forced choice while still eliciting fine-grained distinctions among similar items. That combination makes the resulting perceptual kernels more stable and more useful for later design steps.

**Mechanism:** The reference-based match turns each judgment into a direct perceptual comparison, which lowers ambiguity and preserves distinctions that broader ratings or 2D arrangements can blur.

**Evidence:** Across univariate and bivariate palettes, triplet matching produced the lowest cross-subject variance, the greatest robustness to subject removal, and the best prediction of bivariate distances from univariate kernels; the paper therefore recommends triplet matching unless time or cost prohibit it [@demiralpLearningPerceptualKernels2014].

**Notes:** Triplet discrimination was weaker than triplet matching because matching elicited finer distinctions with the same total number of judgments.

## Use when building a perceptual model for design <!-- role: context -->

- **User Goal:** Learn a perceptual kernel that can guide palette design or automated assignment.
- **Task:** Collect similarity judgments over discrete visual stimuli such as shape, color, size, or their combinations.
- **Data:** A finite palette of candidate encoding values.
- **Chart Setting:** Offline judgment collection for visualization evaluation or automated design.
- **Audience:** Designers or researchers building reusable perceptual models.
- **Success Criterion:** Low-variance kernels that remain stable across subjects and support later prediction or optimization.

## Do not use when collection time or budget is the binding constraint <!-- role: exceptions -->

**Break it when:** The available time or budget cannot support the larger total number of triplet judgments. **Why:** The paper reports that exhaustive triplet comparison costs more total experiment time and compensation than pairwise ratings or spatial arrangement.

## Tradeoffs of triplet matching <!-- role: costs -->

**Sacrifice:** You spend more total collection time and money than with pairwise ratings or spatial arrangement.
**Risk:** Large palettes become expensive because the number of possible triplets grows quickly.
**Mitigation:** Subdivide the stimulus set or use adaptive sampling when the palette is too large for exhaustive triplet collection.

## Common judgment-task failure <!-- role: mistakes -->

**Mistake:** Use spatial arrangement as a drop-in substitute for learning perceptual structure in color or multidimensional palettes. **Why it fails:** The paper found higher variance for spatial arrangement and notes that a 2D arrangement cannot accurately express higher-dimensional structures.

## Check whether the elicitation task is stable enough <!-- role: check -->

**Failure Sign:** Different subject subsets produce noticeably different kernels, or the learned kernel poorly supports later prediction of combined encodings.
**Quick Check:** Run a small pilot and compare cross-subject variance or rank-correlation stability for triplet matching against your current elicitation task.
**Stronger Test:** Fit bivariate distances from univariate kernels and verify that the triplet-matching kernel yields the best predictive fit.

## Fix the elicitation procedure <!-- role: fix -->

- Replace rating-based or spatial-arrangement collection with reference-based triplet matching.
- Use matching rather than triplet discrimination when you need finer distinctions among similar items.
- If the palette is too large, partition the stimuli across subjects instead of abandoning triplet matching outright.
- Add adaptive triplet sampling when exhaustive collection is impractical.
