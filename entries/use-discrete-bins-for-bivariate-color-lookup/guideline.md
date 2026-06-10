---
id: use-discrete-bins-for-bivariate-color-lookup
title: Use discrete bins for bivariate color lookup
bibliography: references.bib
description: For exact lookup tasks on bivariate color maps, prefer discrete encoding
  on value-and-uncertainty charts to improve identification accuracy and mitigate
  perceptual color-decoding errors for readers matching marks to a legend.
labels:
- purpose:refine
- basis:empirical
- task:retrieve
- quality:fidelity:use
- lever:encoding
- operator:uncertainty
- reading-mode:exact
---

## Discretize the bivariate color scale <!-- role: advice -->

Quantize the value-and-uncertainty scale into explicit color bins when readers must identify exact pairs from a legend. For example, use a stepped 2D color matrix instead of a smooth bivariate gradient when a reader must locate a cell with a specific value and uncertainty.

## Why discrete bins beat continuous bivariate color for lookup <!-- role: reason -->

A continuous bivariate color field asks readers to estimate two integrated color dimensions precisely at once. Discrete bins trade some quantization error for easier matching between the map and the legend.

**Mechanism:** Discrete outputs reduce perceptual decoding error because readers compare a small set of distinct colors instead of estimating exact positions in a smooth 2D color blend.

**Evidence:** In the paper's identification experiment, discrete bivariate maps were significantly more accurate than continuous bivariate maps for finding target value-uncertainty combinations [@correllValueSuppressingUncertaintyPalettes2018].

## Use when exact legend matching matters <!-- role: context -->

- **User Goal:** Identify or verify a specific value-uncertainty combination.
- **Task:** Exact lookup from a bivariate legend.
- **Data:** Two quantitative variables encoded together in color, with one variable representing uncertainty.
- **Chart Setting:** A superimposed bivariate color map with a legend that readers must decode directly.
- **Audience:** Readers performing precise read-off rather than broad visual impression.
- **Success Criterion:** Higher accuracy in matching map colors to legend entries.

## Do not use when continuous appearance is the higher priority <!-- role: exceptions -->

**Break it when:** The main goal is preserving class-less continuous appearance rather than exact pair lookup. **Why:** The paper notes that discretization introduces quantization error even though it improves lookup performance.

## What you give up with discretization <!-- role: costs -->

**Sacrifice:** You lose continuous, class-less representation.
**Risk:** Bins can hide small within-bin differences.
**Mitigation:** Use discrete bins specifically for tasks that require exact matching from the legend.

## Common failure in bivariate color maps <!-- role: mistakes -->

**Mistake:** Use a smooth bivariate gradient and expect readers to recover precise value-uncertainty pairs from color alone. **Why it fails:** Precise estimation from integrated color channels is error-prone.

## Test whether readers can actually match the colors <!-- role: check -->

**Failure Sign:** Readers hesitate between neighboring colors or repeatedly miss exact target pairs.
**Quick Check:** Ask a reviewer to find a specific value-uncertainty pair in the continuous version and in a discretized version of the same map.
**Stronger Test:** Compare accuracy on a short identification task that uses the same legend and data in both versions.

## Revise the scale for exact reading <!-- role: fix -->

- Replace the smooth bivariate gradient with a stepped set of color bins.
- Turn the legend into explicit discrete categories rather than continuous interpolation.
- If exact lookup is not the chart's job, keep the continuous scale out of tasks that ask for precise value-uncertainty identification.
