---
id: separate-baseline-and-treatment-added-risk-in-risk-pictographs
title: Separate baseline cases from treatment-added cases in risk pictographs
bibliography: references.bib
description: For comparing treatment side effects against preexisting risk at a single
  time point, use separate visual encoding for baseline and incremental cases on a
  risk display to improve fidelity and mitigate the mistake of attributing the full
  treated-group risk to the treatment for patient decision-makers with low numeracy.
labels:
- purpose:refine
- basis:empirical
- task:compare
- time:timepoint
- quality:fidelity
- lever:encoding
- operator:difference
- audience:decision-maker
---

## Incremental risk encoding <!-- role: advice -->

Show baseline cases and treatment-added cases as separate visual groups within the same denominator. For example, in a pictograph, color the cases that would occur anyway in one color and only the extra cases caused by treatment in a second color instead of showing only the total treated-group risk.

## Why incremental risk encoding works <!-- role: reason -->

A total-risk-only display encourages readers to blame the whole treated-group risk on the treatment. Separating baseline from added risk makes the treatment-caused increment visible and reduces over-attribution.

**Mechanism:** Readers can see which cases are part of the preexisting baseline and which cases are added by treatment, so they judge the treatment's contribution more accurately.

**Evidence:** The paper describes studies showing that separating baseline and incremental risk within pictographs reduced worry about side effects and reduced perceived likelihood of experiencing a side effect; it also notes that the knowledge benefit of the incremental format required pictographs [@fagerlinHelpingPatientsDecide2011].

**Notes:** The paper illustrates this move with one color for baseline cases and another color for the additional treated cases.

## Use when treatment changes an existing baseline risk <!-- role: context -->

- **User Goal:** Judge how much extra risk a treatment adds.
- **Task:** Compare baseline risk with treatment-caused incremental risk.
- **Data:** A side effect or complication that can occur both without treatment and with treatment.
- **Chart Setting:** A static risk graphic that explains side effects for a treatment decision.
- **Audience:** Patients weighing risks and benefits of an intervention.
- **Success Criterion:** Readers can distinguish what would happen anyway from what is added by treatment.

## Do not use the incremental format without a pictograph <!-- role: exceptions -->

**Break it when:** The incremental risk framing is shown without a pictograph. **Why:** The paper reports that the knowledge advantage of the incremental approach depended on combining it with pictographs.

## Tradeoffs of incremental risk encoding <!-- role: costs -->

**Sacrifice:** You give up some visual simplicity by adding another visual group.
**Risk:** If the added cases are not clearly separated from baseline cases, the treatment effect can still be missed.
**Mitigation:** Keep the same denominator visible and add only the extra treatment-caused cases in a distinct visual encoding.

## Common failure mode in side-effect graphics <!-- role: mistakes -->

**Mistake:** Show only the total complication rate in the treatment group. **Why it fails:** Readers may treat the entire displayed risk as if it were caused by the treatment alone.

## How to check the encoding <!-- role: check -->

**Failure Sign:** A reviewer cannot tell which cases belong to baseline risk and which cases are added by treatment.
**Quick Check:** Ask whether each highlighted case would still be present without the treatment.
**Stronger Test:** Compare the display with a total-risk-only version and check which one makes the treatment-caused increment directly visible.

## How to fix the display <!-- role: fix -->

- Start with the baseline risk in the full denominator.
- Add a second visual encoding for only the extra cases caused by treatment.
- Avoid a treated-group total that does not distinguish baseline from added risk.
