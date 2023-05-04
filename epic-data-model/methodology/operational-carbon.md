# Operational Carbon

The overview of how c.scale calculated operational carbon is detailed on the [model structure](model-structure.md#calculating-operational-carbon) page. Below, we give additional detail about how c.scale calculates emissions from all the sources contributing to a proejct's operational carbon.

### Energy Use

EPIC uses energy use intensity (EUI) in kBtu/sf/yr as its metric for energy use in buildings. EPIC is designed to give accurate feedback on the carbon emissions associated with a declared energy use, but is not an energy modeling tool for determining how a declared energy use can be achieved.

Baseline EUIs are set in c.scale using a direct API connection with Architecture 2030's [Zero Tool](https://zerotool.org/zerotool/), with a failover to a subset of cached Zero Tool results. Zero Tool estimates are used to set baselines for AIA 2030 reporting, but should not be construed as representing "code minimum" design. To set a code minimum EUI, enter a custom value in the "Benchmark EUI" [override](../../users-guide/base-case/overrides.md) in EPIC's Base Case tab.&#x20;

### Fuel Mix

Benchmark buildings are assumed to be "mixed fuel," using energy from both electricity and onsite combustion. The fuel mix of buildings is calculated to align with assumptions in Architecture 2030's [Zero Tool](https://zerotool.org/zerotool/). Zero Tool estimates are used to set baselines for AIA 2030 reporting, but should not be construed as representing "code minimum" design. To set a code minimum fossil fuel use, enter a custom value in the "% Onsite Fossil Fuel Combustion" [override](../../users-guide/base-case/overrides.md) in EPIC's Base Case tab.&#x20;

c.scale assumes a 2.4% upstream leakage rate for all fossil fuel combusted in a building. The carbon intensity of this leakage is calculated with characterization factors from the IPCC's AR6.&#x20;

### Carbon Intensity of Electricity

c.scale includes estimates of carbon emissions from demand for electricity from now until 2110. These estimates are based on NREL's Cambium capacity expansion model. If you are curious about the underlying data, you can explore Cambium data in NREL's [online scenario viewer](https://scenarioviewer.nrel.gov/). Cambium data is not available annually, but annual data is necessary in c.scale. To annualize Cambium data, we use the following method:

* **Fill temporal gaps in Cambium data from 2024-2050** with geometric interpolation for all years between two years reported in Cambium.
  * I.e. for 2025 between the reported values in 2024 and 2026, or for 2041-2044 between the reported values in 2040 and 2045.&#x20;
* **Extend data to 2110** assuming the electricity grid continue to decarbonize at the same average rate that it decarbonized from 2024-2050. Note that the end date of 2110 has no basis in the data; 2110 is only chosen so that c.scale can model a 60 year reference period for buildings completed up to the year 2050.&#x20;
* **Fill geographic gaps** to give wall-to-wall coverage of United States.&#x20;
  * c.scale assumes the average emission rate in Washington, DC, is the same as in Virginia (highly interconnected grids, both PJM).&#x20;
  * For Alaska and Hawaii, we assume exponential reductions that allow them to meet their climate goals (in the mid-case scenario) or get to 95% decarb by 2045. We don’t make an assumption to approximate a scenario like High Cost of Renewable Energy for either of these two states.

#### Electrical grid emission metrics

c.scale includes two metrics for grid emissions.

* **Average Emission Rate (AER)**. By default, c.scale measures annual emission factors by summing the total generation of all resources in a given year and putting them on a MWh basis. This average emission rate also includes 'precombustion emissions from the leakage of fossil gas in the energy supply chain. This metric is described in NREL's Cambium model as "AER Load: Combustion + Precombustion."&#x20;
* **Long-Run Marginal Emission Rates (LRMER)**. LRMER emissions are described by NREL as emission rates for “of the next unit of electricity considering the grid’s structure as variable.” This emission metric is preferable to a simple average emission rate because buildings are long-lived assets whose demand for energy has a marginal influence on the evolution of the energy grid. This metric is described in NREL's Cambium model as "LRMER: Combustion + Precombustion."&#x20;

#### Electrical grid projections

The future of the electrical grid is uncertain. To account for this uncertainty, c.scale includes three NREL Cambium scenarios for the future evolution of the electrical grid. Portions of the text below are quoted from the description of these scenarios and their derivation published by NREL [here](https://www.nrel.gov/docs/fy23osti/84916.pdf) (pdf).

* **Expected decarbonization**. Average estimates for inputs such as technology costs, fuel prices, and demand growth. No inclusion of nascent technologies. Electric sector policies as they existed in September 2022, with the assumption that the Inflation Reduction Act’s Production and Investment Tax Credits do not phase out. This metric is described in NREL's Cambium model as "Midcase."
* **Slow Decarbonization**. Average estimates as in the mid-case scenario, but with an assumption that battery and renewable energy costs are high. This scenario assumes that the thresholds set by the Inflation Reduction Act’s Production and Investment Tax Credits are not met and, as such, they do not phase out. This metric is described in NREL's Cambium model as "High Cost of Renewable Energy."
* **Rapid Decarbonization**. Average estimates for inputs such as technology costs, fuel prices, and demand growth. Nascent technologies are included. Electric sector policies as they existed in September 2022, with the assumption that the Inflation Reduction Act’s Production and Investment Tax Credits do not phase out. High-level assumption that the national electricity grid's carbon emissions in 2050 are 5% of their 2005 level. This metric is described in NREL's Cambium model as "95% decarbonization by 2050."

c.scale evaluates energy use on an annual basis. The carbon emissions from electricity, however, vary hour by hour. Depending on the use type and location, this can lead to a difference of as much as +/- 20% between annual (modeled) and hourly (measured) estimates of operational emissions.&#x20;

<figure><img src="../../.gitbook/assets/EPIC - LRMER and AER.png" alt=""><figcaption><p>Carbon emissions from electricity demand from 2023-2110 for two metrics and three scenarios.</p></figcaption></figure>

### Energy Generation from Onsite Renewables

c.scale calculates energy generation from onsite solar photovoltaic arrays using an API connection to Version 8 of NREL's [PVWatts](https://pvwatts.nrel.gov/) tool. This energy is assumed to displace an equivalent amount of energy demand from the electrical grid and, by doing so, displace a corresponding quantity of emissions (calculated using the Cambium data detailed above).&#x20;

The  array area returned by the c.scale is the total area of the array (i.e., inclusive of the space between the panels). The ratio of solar panels to total array area is the Ground Coverage Ratio (GCR). This ratio can be adjusted in the [Overrides](../../users-guide/base-case/overrides.md#solar-ground-coverage-ratio) panel of the Base Case tab.&#x20;

