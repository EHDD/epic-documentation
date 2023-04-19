---
description: Customize Scenario Parameters
---

# Refine Data

This modal allows a user to customize the data used to calculate the current scenario. This can be useful when a project team has specific information about material quantities or carbon intensities, or to set goTals in regard to either.&#x20;

Entering data in this panel will only affect the current scenario. No other scenarios will be affected.

### Embodied Carbon | Structure

In this section of the panel, a user can override EPIC's calculations for either the quantity or carbon intensity of structural materials. In all fields where no user data is entered, the value is inferred by EPIC (in some cases, this value is zero). EPIC assumes that the density of concrete is 2400 kg/m3 and timber is 450 kg/m3. If there is a material not currently included that you would like to see in our model, [please reach out](mailto:epic@ehdd.com).

| Material            | Quantity Unit | Carbon Intensity Unit |
| ------------------- | ------------- | --------------------- |
| Concrete (3-4 kSI)  | m3            | kgCO2e/m3             |
| Concrete (5-6 kSI)  | m3            | kgCO2e/m3             |
| Concrete (7-10 kSI) | m3            | kgCO2e/m3             |
| Reinforcing Steel   | kg            | kgCO2e/kg             |
| Structural Steel    | kg            | kgCO2e/kg             |
| Steel Deck          | kg            | kgCO2e/kg             |
| Engineered Timber   | m3            | kgCO2e/m3             |
| Lumber              | m3            | kgCO2e/m3             |
| Plywood             | m3            | kgCO2e/m3             |

### Embodied Carbon | Assemblies

Scopes other than structure can be customized on a per-area basis. The calculations for determining the area takeoffs used in each calculation is detailed in the embodied carbon methodology.&#x20;

Entering in data in any field (even if a zero is entered) will override the corresponding calculation in EPIC. If a field is left blank, EPIC will calculate the field.&#x20;

_Note that while a user can override EPIC's calculation of A4-A5 emissions on a per-area basis, EPIC's default calculation of A4-A5 emissions is as a proportion of A1-A3 emission._&#x20;
