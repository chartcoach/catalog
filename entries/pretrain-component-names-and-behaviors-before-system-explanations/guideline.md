---
id: pretrain-component-names-and-behaviors-before-system-explanations
title: Teach component names and basic behaviors before the full system explanation
bibliography: references.bib
description: For explanatory viewing of a causal system, use brief pretraining on
  component names and behaviors before the full system graphic to improve insight
  and address overload from learning parts and relations at the same time for viewers
  with low prior knowledge.
labels:
- purpose:refine
- basis:empirical
- quality:insight
- lever:text-annotation
- communication:workflow
- knowledge:low
---

## Add a component primer before the main explanation <!-- role: advice -->

Add a short pretraining step that names each visible component and states its basic behavior before the full system explanation begins. For example, show a lead-in screen or mini-sequence that labels each part and describes what it does before the narrated animation explains how the parts interact.

## Why pretraining works here <!-- role: reason -->

Without pretraining, viewers must learn what each part is and how the parts interact at the same time. Pretraining handles the component models first so working memory can focus on the causal model during the main explanation.

**Mechanism:** Knowing part names and behaviors in advance reduces the essential processing load during the full explanation because viewers no longer have to build component models and the causal model simultaneously.

**Evidence:** Across three studies, learners showed better problem-solving transfer when a multimedia system explanation was preceded by short pretraining on the names and behaviors of the components [@mayerNineWaysReduce2003].

## Use when viewers do not yet know the parts <!-- role: context -->

- **User Goal:** Understand how a system works.
- **Task:** Integrate part behavior with causal relations across the full display.
- **Data:** A system with named components and causal links among them.
- **Chart Setting:** A full narrated animation or diagram explains how the system operates, and a short introductory step can be added.
- **Audience:** Viewers with low prior knowledge of the system components.
- **Success Criterion:** Viewers can apply the explanation to new problems, not just recall the parts.

## Do not use when the audience already knows the components <!-- role: exceptions -->

**Break it when:** Viewers already know the names and behaviors of the visible components. **Why:** The supported overload scenario comes from learning the parts and the causal relations at the same time.

## Tradeoffs of adding pretraining <!-- role: costs -->

**Sacrifice:** The explanation gains a separate introductory step before the main view.\
**Risk:** If the primer does not cover both names and basic behaviors, the core overload remains.\
**Mitigation:** Keep the primer focused on component names and what each component does.

## Common failure mode <!-- role: mistakes -->

**Mistake:** Starting with the full causal explanation before viewers know what each part is. **Why it fails:** Viewers must learn the component models and the causal model at once.

## Check whether the primer is sufficient <!-- role: check -->

**Failure Sign:** Viewers cannot name key parts or say what they do before the main explanation starts.\
**Quick Check:** Ask whether each visible component can be identified and briefly described from the primer alone.\
**Stronger Test:** Compare understanding after a version with the primer and a version without it.

## Fix missing prior knowledge <!-- role: fix -->

- Add a short labeled primer for each component.
- State or show each component's basic behavior in the primer.
- Start the full system explanation only after the component primer.
