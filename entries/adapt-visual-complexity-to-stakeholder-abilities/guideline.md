---
id: adapt-visual-complexity-to-stakeholder-abilities
title: Adapt visual complexity to stakeholder abilities and interests
bibliography: references.bib
description: For policy design workflows with heterogeneous stakeholders, use adaptive
  visual structure on user-facing interfaces to improve readability and mitigate one-size-fits-all
  complexity for mixed-knowledge participants.
labels:
- purpose:refine
- basis:empirical
- quality:readability:use
- lever:layout-structure
- communication:workflow
- knowledge:mixed
---

## Adapt the visible structure and level of detail <!-- role: advice -->

Adjust visual structure, visual complexity, and displayed data to the stakeholder's abilities and interests instead of showing the same view to every participant. For example, change the amount of information shown and adapt workflow guidance and available functionality from observed usage patterns during policy creation.

## Match the interface to heterogeneous participants <!-- role: reason -->

Policy work involves stakeholders with different skills, knowledge, preferences, and positions in the process, so a fixed level of detail and a fixed workflow interface will not communicate equally well to everyone.

**Mechanism:** Adapting what is shown and how the workflow is guided makes the same policy process more usable for people with different abilities and interests.

**Evidence:** The paper describes political decision-making as involving stakeholders with heterogeneous skills, knowledge, and preferences, and it presents Fupol's plan to automatically adapt visual structure, visual complexity, displayed data, functionalities, and user guidance to stakeholders' abilities, interests, and observed usage behavior [@kohlhammerVisualizationPolicyModeling2012].

## Use when one workflow serves different stakeholder profiles <!-- role: context -->

- **User Goal:** Communicate policy information and guide policy creation across different participants.
- **Data:** Heterogeneous viewpoints, opinions, and possibilities with different relevance to different stakeholders.
- **Chart Setting:** An interactive policy-design workflow that can observe usage behavior.
- **Audience:** Mixed-knowledge stakeholders participating in the same policy process.
- **Success Criterion:** Users receive a level of detail and guidance that matches their ability and interest.

## Do not use when the stakeholder group is uniform <!-- role: exceptions -->

**Break it when:** The interface is for a single stakeholder group with the same role, ability level, and information needs. **Why:** The paper motivates adaptation specifically from heterogeneity in stakeholder skills, knowledge, preferences, and interests.

## Accept less uniformity across users <!-- role: costs -->

**Sacrifice:** One fixed interface for every stakeholder.
**Risk:** Different users may see different levels of detail or guidance across the workflow.
**Mitigation:** Base the adaptation on observed usage patterns and stakeholder interests.

## Avoid one-size-fits-all complexity <!-- role: mistakes -->

**Mistake:** Keep one fixed visual complexity and one fixed set of functions for all stakeholders in the workflow. **Why it fails:** Heterogeneous participants do not share the same communication needs or level of detail.

## Verify that the interface actually changes by user profile <!-- role: check -->

**Failure Sign:** Novice and expert participants receive the same amount of detail and the same guidance even when their behavior differs.
**Quick Check:** Compare two stakeholder profiles or two different usage patterns and see whether the visible structure, amount of displayed data, or guidance changes.
**Stronger Test:** Confirm that both the shown information and the workflow guidance adapt after usage behavior is observed.

## Change detail, data, and guidance together <!-- role: fix -->

- Reduce visible information for users who need an overview.
- Expand detail and available functionality for users who show stronger interest or expertise.
- Change workflow guidance when observed usage patterns show different needs.
