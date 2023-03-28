# Overrides

Overrides affect the assumptions in the base case and all scenarios within a project.

#### **Base case EUI override**

If the EUI required for a project will be significantly different from Zero Tool's EUI estimate, your preferred EUI can be entered here.&#x20;

#### **% onsite fossil fuel combustion**

The percentage of building energy use resulting from the combustion of fossil fuel at the building site. Default values via Zero Tool.&#x20;

#### Perimeter

The user-declared perimeter of the building. In the absence of a user input, EPIC assumes the building is an extruded square.

#### Window-to-wall ratio (WWR)

The ratio of windows to total wall area. The default value is .45.

#### Floor-to-floor height

The vertical distance between building floors in feet. The default value is 13’.

#### Interior fit-out percentage

The percentage of floor space that will be fitted out for occupation by building tenants. The default value is 70%. If tenant fit-out is outside the project scope, this field can be set to 0%.

#### Solar ground coverage ratio

For any solar array entered as a decarbonization measure, this ratio describes the ratio of active solar cells to total array area. EPIC's assumption is 0.7, representing an efficient solar layout.&#x20;

#### Electricity grid, future scenario

The future of the electric grid is uncertain. EPIC gives the user the choice between three future scenarios modeled by NREL as part of their [CAMBIUM model](https://www.nrel.gov/analysis/cambium.html).&#x20;

* **Expected Decarbonization (Midcase)**. By default, EPIC uses a mid-case assumption of how the electrical grid will evolve over time. This scenario reflects policy and economic models through 2022 (i.e. the passage of the IRA, the continued operation of Diablo Canyon Nuclear Power Plant). This scenario is constructed from the "Midcase" scenario in NREL Cambium.&#x20;
* **Slow Decarbonization**. This scenario is based on the same model and assumptions as the 'expected decarbonization' scenario, except it assumes that the cost of renewable energy will remain high. This assumption slows progress toward a decarbonized electricity grid. This scenario is constructed from the "High Cost of Renewable Energy" scenario in NREL Cambium.&#x20;
* **Rapid Decarbonization**. This scenario is based on the same model and assumptions as the 'expected decarbonization' scenario, except for an additional constraint that the grid decarbonized by 95% by 2050 (against a 2005 baseline).  This scenario is constructed from the "Mid-case with 95% Decarbonization by 2050 (without tax credit phaseout)" scenario in NREL Cambium.&#x20;

#### Electricity grid, emission metric

text
