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

The future of the electric grid is uncertain. EPIC gives the user the choice between three future scenarios, each derived from NREL's [CAMBIUM model](https://www.nrel.gov/analysis/cambium.html).&#x20;

* **Expected decarbonization**. Average estimates for inputs such as technology costs, fuel prices, and demand growth. No inclusion of nascent technologies. Electric sector policies as they existed in September 2022, with the assumption that the Inflation Reduction Act’s Production and Investment Tax Credits do not phase out. This metric is described in NREL's Cambium model as "Midcase."
* **Slow Decarbonization**. Average estimates as in the mid-case scenario, but with an assumption that battery and renewable energy costs are high. This scenario assumes that the thresholds set by the Inflation Reduction Act’s Production and Investment Tax Credits are not met and, as such, they do not phase out. This metric is described in NREL's Cambium model as "High Cost of Renewable Energy."
* **Rapid Decarbonization**. Average estimates for inputs such as technology costs, fuel prices, and demand growth. Nascent technologies are included. Electric sector policies as they existed in September 2022, with the assumption that the Inflation Reduction Act’s Production and Investment Tax Credits do not phase out. High-level assumption that the national electricity grid's carbon emissions in 2050 are 5% of their 2005 level. This metric is described in NREL's Cambium model as "95% decarbonization by 2050."

#### Electricity grid, emission metric

For a given scenario, there are multiple methods to account for the emissions associated with a building. Two metrics are provided in EPIC, both derived from NREL's [CAMBIUM model](https://www.nrel.gov/analysis/cambium.html). Both metrics use GWP-100 characterization factors.&#x20;

* **Average Emission Rate (AER)**. By default, EPIC measures annual emission factors by summing the total generation of all resources in a given year and putting them on a MWh basis. This average emission rate also includes 'precombustion emissions from the leakage of fossil gas in the energy supply chain. This metric is described in NREL's Cambium model as "AER Load: Combustion + Precombustion."&#x20;
* **Long-Run Marginal Emission Rates (LRMER)**. LRMER emissions are described by NREL as emission rates for “of the next unit of electricity considering the grid’s structure as variable.” This emission metric is preferable to a simple average emission rate because buildings are long-lived assets whose demand for energy has a marginal influence on the evolution of the energy grid. This metric is described in NREL's Cambium model as "LRMER: Combustion + Precombustion."&#x20;

#### Refrigerant Leakage

Annual and end-of-life refrigerant leakage rates are typically a model assumption, not a carbon reduction measures. In c.scale, there are two options for leakage assumptions.&#x20;

| Reporting Scheme    | Annual Leakage | End-of-Life Leakage |
| ------------------- | -------------- | ------------------- |
| LEED                | 2%             | 10%                 |
| CIBSE TM65 (Type 2) | 4%             | 2%                  |

#### Percent conditioned area

The percentage of total floor area that is heated or cooled.&#x20;
