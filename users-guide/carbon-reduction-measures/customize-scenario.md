---
description: Customize Scenario Parameters
---

# Refine Data

This modal allows a user to customize the data used to calculate the current scenario. This can be useful when a project team has specific information about material quantities or carbon intensities, or to set goals in regard to either. Entering data in this panel will only affect the current scenario. No other scenarios will be affected.

These quantities are entered on an area basis in units of kgCO2e/sf values. The area baseline for each quantity is as follows:

| Scope                | Area Baseline             | Inputs affecting area baseline                          |
| -------------------- | ------------------------- | ------------------------------------------------------- |
| Structure            | Total Floor Area          | Floor area                                              |
| Envelope \| Cladding | Opaque Envelope Area      | WWR, floor-to-floor height, perimeter, and floor area.  |
| Envelope \| Glazing  | Transparent Envelope Area | WWR, floor-to-floor height, perimeter, and floor area.  |
| Envelope \| Roofing  | Roof Area                 | Floor area per above ground floor                       |
| Tenant Fit Out       | Tenant Fit Out Area       | Floor area, % floor area with tenant fit out            |
| MEP                  | Total Floor Area          | Floor area                                              |
| Hardscape            | Hardscape Area            | Scenario hardscape area                                 |
| A4-A5: Construction  | Total Floor Area          | Floor area                                              |



The calculations for determining the area takeoffs used in each calculation is detailed in the embodied carbon methodology. A summary of input fields used in each is outlined above. Entering in data in any field (even if a zero is entered) will override the corresponding calculation in EPIC. If a field is left blank, EPIC will calculate the field.&#x20;

_Note that while a user can override EPIC's calculation of A4-A5 emissions on a per-area basis, EPIC's default calculation of A4-A5 emissions is as a proportion of A1-A3 emission._&#x20;
