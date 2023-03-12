# Operational Carbon

The overview of how EPIC calculated operational carbon is detailed on the [model structure](carbon-reduction-measures.md#calculating-operational-carbon) page. Below, we give additional detail about how EPIC calculates emissions from all the sources contributing to a proejct's operational carbon.

### Energy Use

EPIC uses energy use intensity (EUI) in kBtu/sf/yr as a metric to describe energy use in buildings. EPIC is designed to give accurated feedback on the carbon emissions associated with energy use, but is not an energy modeling tool for determining how a particular EUI can be achieved.

Baseline EUIs are set in EPIC using a direct API connection with Architecture 2030's [Zero Tool](https://zerotool.org/zerotool/), with a failover to a subset of cached Zero Tool results. Zero Tool estimates are used to set baselines for AIA 2030 reporting, but should not be construed as representing "code minimum" design. To set a code minimum EUI, enter a custom value in the "Benchmark EUI" [override](../users-guide/base-case/overrides.md) in EPIC's Base Case tab.&#x20;

### Fuel Mix

Benchmark buildings are assumed to be "mixed fuel," using energy from both electricity and onsite combustion. The fuel mix of buildings is calculated to align with assumptions in Architecture 2030's [Zero Tool](https://zerotool.org/zerotool/). Zero Tool estimates are used to set baselines for AIA 2030 reporting, but should not be construed as representing "code minimum" design. To set a code minimum fossil fuel use, enter a custom value in the "% Onsite Fossil Fuel Combustion" [override](../users-guide/base-case/overrides.md) in EPIC's Base Case tab.&#x20;

EPIC assumes a 2.4% upstream leakage rate for all fossil fuel combusted in a building. The carbon intensity of this leakage is calculated with characterization factors from the IPCC's AR6.&#x20;

### Carbon Intensity of Electricity

EPIC includes estimates of carbon emissions from demand for electricity from now until 2110. These estimates are based on NREL's Cambium capacity expansion model. If you are curious about the underlying data, you can explore Cambium data in NREL's [online scenario viewer](https://scenarioviewer.nrel.gov/). Cambium data is not available annually, but annual data is necessary in EPIC. To annualize Cambium data, we use the following method:

* **Fill temporal gaps in Cambium data from 2024-2050** with geometric interpolation for all years between two years reported in Cambium.
  * I.e. for 2025 between the reported values in 2024 and 2026, or for 2041-2044 between the reported values in 2040 and 2045.&#x20;
* **Extend data to 2110**, assuming the electricity grid continue to decarbonize at the same average rate that it decarbonized from 2024-2050. Note that the end date of 2110 has no basis in the data; 2110 is only chosen so that EPIC can model a 60 year reference period for buildings completed up to the year 2050.&#x20;
* **Fill geographic gaps** to give wall-to-wall coverage of United States.&#x20;
  * EPIC assumes the average emission rate in Washington, DC, is the same as in Virginia (highly interconnected grids, both PJM).&#x20;
  * For Alaska and Hawaii, we assume exponential reductions that allow them to meet their climate goals (in the mid-case scenario) or get to 95% decarb by 2045. We don’t make an assumption to approximate a scenario like High Cost of Renewable Energy for either of these two states.

EPIC includes two metrics for grid emissions.

* **Average emission rates (AER)**. The average emission rate of the generation mix in the selected location in the selected year.&#x20;
* **Long run marginal emission rates (LRMER)**. The emissions rate that would be induced by a long-term change in electrical demand. An example of a long-term change in electrical demand is the demand incurred by a building.&#x20;

The future of the electrical grid is uncertain. To account for this uncertainty, EPIC includes three NREL Cambium scenarios for the future evolution of the electrical grid.&#x20;

* **Midcase**.
* **95% decarbonization by 2045**.
* **High Cost of Renewable Energy**.&#x20;



