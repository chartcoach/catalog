---
id: preserve-user-style-overrides
title: Preserve user style overrides in chart styling
bibliography: references.bib
description: For accessibility implementation and review, use chart styling that preserves
  user-agent overrides on charts and dashboards to improve accessibility and mitigate
  fixed-presentation failures for users who rely on browser, operating-system, or
  application style changes.
labels:
- purpose:refine
- basis:accessibility
- quality:accessibility
- lever:interaction-access
- needs:low-vision
- access:contrast:use
---

## Preserve user style overrides <!-- role: advice -->

Let chart styling inherit and respond to user-agent style changes instead of forcing a fixed presentation. For example, verify that a chart still works when a browser or application applies a custom stylesheet and when an operating system high-contrast mode changes chart text, fills, and other elements.

## Respecting user settings keeps the chart usable after style changes <!-- role: reason -->

When a chart blocks user styling, people who depend on system or browser presentation changes can lose access to the chart or its controls. When the chart respects those changes, users keep their own presentation settings while the chart remains perceivable and operable.

**Mechanism:** User-applied styles can change contrast, text appearance, and other presentation traits that some readers need; preserving those overrides keeps the chart compatible with the user's broader technical environment instead of locking them into the author's default styling.

**Evidence:** Chartability defines this as a critical Flexible heuristic and states that styling changed by the user must be respected; the chart must not interfere with custom stylesheets or system settings, and the audit procedure explicitly tests this by changing system settings such as high-contrast modes to see whether the data experience respects them [@elavskyHowAccessibleMy2022].

## Use when user-controlled presentation can affect the chart <!-- role: context -->

- **User Goal:** Read or operate the chart using personal browser, operating-system, or application style settings.
- **Chart Setting:** The chart is rendered in a context where user styles or system display modes can change presentation.
- **Audience:** People who rely on user-controlled presentation changes, including high-contrast settings.
- **Success Criterion:** User-applied styling remains in effect and the chart stays usable after the change.

## Do not apply outside a user-agent styling context <!-- role: exceptions -->

**Break it when:** The chart is not rendered in a browser, operating-system, or application context that can apply user style changes. **Why:** This guideline is specifically about preserving user-agent styling changes, so the check is not applicable when no such override can act on the chart.

## Cost of preserving user style overrides <!-- role: costs -->

**Sacrifice:** You give up some control over the exact authored appearance of the chart.
**Risk:** Meanings that depend too heavily on one fixed visual treatment can weaken after user styles change the presentation.
**Mitigation:** Test the chart after style changes and revise any text or marks that disappear, merge, or lose distinction.

## Common failures when chart styling ignores user settings <!-- role: mistakes -->

- **Mistake:** Hard-code chart styles so author styling overrides browser, operating-system, or application styling changes. **Why it fails:** Users cannot apply the presentation changes they need.
- **Mistake:** Review the chart only in its default presentation. **Why it fails:** Style-override failures may appear only after a user setting such as high-contrast mode is turned on.

## Check whether user style changes are preserved <!-- role: check -->

**Failure Sign:** Changing user settings does not alter the chart, or the changed chart becomes hard to read or distinguish.
**Quick Check:** Toggle a system setting such as high-contrast mode, or load a custom stylesheet, and inspect whether chart text and marks follow the new styling.
**Stronger Test:** Compare the default and user-styled renderings and confirm that the user-styled chart still leaves text readable and chart elements distinguishable.

## Fix chart styling that blocks user overrides <!-- role: fix -->

- Remove or loosen authored styles that block browser, operating-system, or application overrides on chart text and marks.
- Revise chart elements that disappear or merge after a user style change so the chart remains distinguishable under the new styling.
- Re-test the chart with a custom stylesheet and with a system setting such as high-contrast mode until the user-applied styling is preserved.
