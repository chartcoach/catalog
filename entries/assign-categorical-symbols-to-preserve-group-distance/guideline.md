---
id: assign-categorical-symbols-to-preserve-group-distance
title: Assign categorical symbols so perceptual differences match group differences
bibliography: references.bib
description: For cluster-oriented reading of categorical group relations, use distance-preserving
  shape or color assignments on categorical encodings to improve fidelity and mitigate
  arbitrary similarity cues for viewers interpreting how groups relate.
labels:
- purpose:refine
- basis:empirical
- task:cluster
- data:categorical
- quality:fidelity:use
- lever:encoding
- operator:association
---

## Distance-preserving assignment <!-- role: advice -->

Assign category colors or shapes so perceptual distances mirror the distances between the groups they encode. For example, when group-to-group connection strengths or other pairwise distances are known, give closely related groups more similar symbols and distant groups more distinct ones instead of mapping categories to the palette arbitrarily.

## Why matched assignments help <!-- role: reason -->

Distance-preserving assignments turn visual similarity into a usable cue about data similarity. Viewers can then read group relations from the encoded symbols, not just group identity.

**Mechanism:** When perceptual similarity tracks group similarity, the encoding preserves more of the underlying structure and makes relational patterns easier to interpret.

**Evidence:** The paper presents visual embedding with perceptual kernels and shows color and shape assignments chosen to reflect distances among community clusters, so visually similar symbols represent more closely related groups. A later review collates this paper as empirical evidence on nominal shape, color-hue, and area encodings for cluster-oriented visualization design [@zengReviewCollationGraphical2023; @demiralpLearningPerceptualKernels2014].

## Use when group relations matter <!-- role: context -->

- **User Goal:** Show not just which group an item belongs to, but also how groups relate.
- **Task:** Read relative closeness or separation between groups from categorical encodings.
- **Data:** Categories or clusters with a known pairwise distance, similarity, or connection-strength structure.
- **Chart Setting:** Color or shape already encodes group membership.
- **Audience:** Viewers need to interpret relations among groups from the same display.
- **Success Criterion:** Visually similar symbols correspond to closer groups, and visually distinct symbols correspond to farther groups.

## Do not use when there is no group-distance structure to preserve <!-- role: exceptions -->

**Break it when:** The categories do not have a meaningful pairwise similarity or distance structure. **Why:** The assignment rule depends on preserving an existing structure; without one, there is nothing for perceptual similarity to represent.

## Costs of matched assignment <!-- role: costs -->

**Sacrifice:** You need both a group-distance model and a perceptual kernel.
**Risk:** Preserving one chosen structure can leave other possible structures unrepresented.
**Mitigation:** Decide which group relation is most important before optimizing the assignments.

## Common assignment mistakes <!-- role: mistakes -->

**Mistake:** Map categories to colors or shapes in arbitrary order when the groups have known similarities or distances. **Why it fails:** Visual similarity then carries accidental meaning instead of reflecting the intended group structure.

## Check whether the mapping preserves structure <!-- role: check -->

**Failure Sign:** Two close groups get very different symbols, or two distant groups get very similar ones.
**Quick Check:** Compare a few nearest and farthest group pairs against their assigned colors or shapes.
**Stronger Test:** Compare the group-distance matrix to the perceptual distances induced by the final assignments and check whether the ordering broadly agrees.

## Fix the category mapping <!-- role: fix -->

- Derive the pairwise distance or similarity matrix for the groups you want to relate.
- Choose the perceptual kernel for the encoding channel you will use.
- Optimize the category-to-symbol assignment against those two distance structures instead of using arbitrary category order.
- Revise the legend mapping so the final color or shape assignments preserve the intended group relations.
