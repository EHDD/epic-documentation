---
description: Customize Scenario Parameters
---

# Refine Data

This modal allows a user to customize the data used to calculate the current scenario. This can be useful when a project team has specific information about material quantities or carbon intensities, or to set goals in regard to either. Entering data in this panel will only affect the current scenario. No other scenarios will be affected.

These quantities are entered on an area basis in units of kgCO2e/sf values. The area baseline for each quantity is as follows:

<table><thead><tr><th width="212.33333333333331">Scope</th><th width="267">Area Baseline</th><th>Inputs Affecting Area Baseline</th></tr></thead><tbody><tr><td>Structure</td><td>Total Floor Area</td><td>Floor area </td></tr><tr><td>Envelope | Cladding</td><td>Opaque Envelope Area</td><td>WWR, floor-to-floor height, perimeter, and floor area. </td></tr><tr><td>Envelope | Glazing</td><td>Transparent Envelope Area</td><td>WWR, floor-to-floor height, perimeter, and floor area. </td></tr><tr><td>Envelope | Roofing</td><td>Roof Area</td><td>Floor area per above ground floor</td></tr><tr><td>Tenant Fit Out</td><td>Tenant Fit Out Area</td><td>Floor area, % floor area with tenant fit out</td></tr><tr><td>MEP</td><td>Total Floor Area</td><td>Floor area</td></tr><tr><td>Hardscape</td><td>Hardscape Area</td><td>Scenario hardscape area</td></tr><tr><td>A4-A5: Construction</td><td>Total Floor Area</td><td>Floor area</td></tr></tbody></table>



The calculations for determining the area takeoffs used in each calculation is detailed in the embodied carbon methodology. A summary of input fields used in each is outlined above. Entering in data in any field (even if a zero is entered) will override the corresponding calculation in EPIC. If a field is left blank, EPIC will calculate the field.&#x20;

_Note that while a user can override EPIC's calculation of A4-A5 emissions on a per-area basis, EPIC's default calculation of A4-A5 emissions is as a proportion of A1-A3 emission._&#x20;
