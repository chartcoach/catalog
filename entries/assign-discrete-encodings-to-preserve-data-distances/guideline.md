---
id: assign-discrete-encodings-to-preserve-data-distances
title: Assign discrete encodings to preserve data-space distances
bibliography: references.bib
description: For grouped categorical encoding with known pairwise relations, use perceptual-distance-preserving
  assignment on discrete color or shape palettes to improve fidelity and mitigate
  arbitrary category mapping for viewers relating groups.
labels:
- purpose:refine
- basis:empirical
- task:relate
- scope:grouped-result
- quality:fidelity
- lever:encoding
---

## Optimize the category-to-palette mapping <!-- role: advice -->

Assign discrete colors or shapes by optimizing the mapping so perceptual distances in the palette reflect distances in the data. For example, use a perceptual kernel for a color or shape palette and choose the assignment that best preserves cluster-to-cluster or model-to-model distances, so related groups get more similar symbols and distant groups get more distinct ones.

## Why distance-preserving assignment works <!-- role: reason -->

Arbitrary category mappings throw away useful structure when categories themselves have meaningful similarities or dissimilarities. A distance-preserving assignment lets the encoding communicate relationships among groups, not just group identity.

**Mechanism:** Viewers can read similarity and difference directly from the assigned symbols because perceptual spacing in the palette is aligned with spacing in the underlying data.

**Evidence:** The paper applies perceptual kernels to visual embedding, first assigning shapes to reflect distances among color models and then assigning colors and shapes to community clusters so the resulting encodings perceptually reflect correlations and inter-cluster relations [@demiralpLearningPerceptualKernels2014].

## Use when group relationships matter <!-- role: context -->

- **User Goal:** Show not only group identity but also which groups are more or less related.
- **Task:** Encode groups, clusters, or models that have a pairwise distance or similarity structure.
- **Data:** Grouped results with a defined relation matrix or distance matrix.
- **Chart Setting:** Any chart or network view where groups receive discrete colors or shapes.
- **Audience:** Viewers comparing relations among groups.
- **Success Criterion:** Similar groups receive perceptually similar encodings and dissimilar groups receive more separated encodings.

## Do not use when categories have no meaningful distance structure <!-- role: exceptions -->

**Break it when:** The categories only need distinct labels and there is no meaningful pairwise distance or similarity to preserve. **Why:** The method depends on a data-space distance structure; without one, the optimization target is undefined.

## Tradeoffs of distance-preserving assignment <!-- role: costs -->

**Sacrifice:** You give up a simple arbitrary or default-order category mapping.
**Risk:** A poor distance definition in the data will produce a misleading visual similarity structure.
**Mitigation:** Define and normalize the group-distance measure before optimizing the assignment.

## Common mapping failure <!-- role: mistakes -->

**Mistake:** Map categories to colors or shapes in palette order or at random when the categories have known relations. **Why it fails:** The visual similarities then reflect the palette order rather than the actual structure in the data.

## Check whether the mapping preserves relations <!-- role: check -->

**Failure Sign:** Closely related groups are encoded with very different symbols, or unrelated groups look unusually similar.
**Quick Check:** Rank the group-to-group distances in the data and check whether the assigned palette distances follow a similar rank order.
**Stronger Test:** Compare the chosen mapping against a default-order or random mapping and keep the one with lower mismatch between data distances and perceptual distances.

## Fix the category-to-palette mapping <!-- role: fix -->

- Build a distance matrix that captures the relations you want viewers to see among groups.
- Choose a discrete palette with a known perceptual kernel.
- Optimize the assignment from groups to palette items against that kernel instead of using palette order.
- Recompute the assignment when the set of groups or the target distance structure changes.
