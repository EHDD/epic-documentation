---
description: '[ARCHIVE] EPIC v1 Documentation'
---

# Calculations

### Embodied Carbon Emissions

For each contributor i, embodied emissions assessed by EPIC are evaluated with the following expression:

$$
{Assessed\ emissions}_i=\ A\ast x_i\ast c_i
$$

Where A is the total building area, $$x_i$$ is the quantity of the contributor $$i$$ per building area, and $$c_i$$ is the carbon intensity per unit of the contributor $$i$$.

For example, a 10,000 square foot building may use 4 pounds of reinforcing steel per square foot of floor area, and the reinforcing steel may have a carbon intensity of 500 grams (0.5 kilograms) of carbon dioxide-equivalent emissions per pound of steel (values for illustrative purposes only). Taking the product of these three hypothetical quantities yields the contribution of reinforcing steel to that building’s embodied carbon emission:

$$
10,000\ sf\ast4\ \frac{lbs\ rebar}{sf}\ast0.5\ \frac{kg\ CO_2e}{lb\ rebar}=20,000\ kg\ CO_2e
$$

In each section of its model, EPIC sums the assessed emission of many individual contributors. While simple summation is acceptable in some cases, some materials will be replaced before the target date. For these materials, the emissions are assigned to the year(s) in which they’re replaced, and a multiplier is added to the total summation. The total embodied emissions assessed by EPIC are represented by this expression:

$$
Total\ embodied\ carbon\ emissions=\ \sum_{i=1}^{n}\ A\ast x_i\ast c_i\ast(1+r_i)\
$$

For n number of contributors to the embodied emissions, where A is the total building area, $$x_i$$ is the quantity of the contributor $$i$$ per building area, $$c_i$$ is the carbon intensity per unit of the contributor $$i$$, and $$r_i$$ is the number of replacements of the contributor $$i$$ before the target date.

### Operational Carbon Emissions

The operational emissions of the project are assessed annually and summed across all years before the target date. The equation is similar to the equation for embodied emissions, with two key differences: first, the quantity x is substituted for the energy use intensity (EUI) e; second, the equation is a double summation, once across all the fuel types in the building and again across all years between the building’s completion and the target year. The total operational emissions assessed by EPIC are represented by this expression:

$$
Operational\ carbon\ emissions=\ \sum_{t=1}^{m}\ \sum_{j=1}^{o}\ A\ast e_{tj}\ast c_j
$$

For m total years between the building’s completion and the target year and across o fuel types, where A is the total building area, $$e_{tj}$$ is the energy use per building area (EUI) in year $$t$$ of fuel $$j$$, and $$c_{tj}$$ is the carbon intensity per energy unit in year $$t$$ of fuel $$j$$.

Carbon emissions associated with electricity are derived from NREL's Cambium model. Onsite fossil fuel use is assumed to be natural gas. The carbon emissions of natural gas are assessed with a 2.4% leakage rate. Fuel oil emissions account for N20 and CH4 emissions. Characterization of non-CO2 emissions is determined with the GWP100 factors published in IPCC AR5.

### Total Landscape Emissions

Landscape emissions assessed by EPIC are evaluated with the following expression:

$$
Landscape\ carbon\ emissions=\ \sum_{t=1}^{m}\ \sum_{k=1}^{p}\ A_k\ast c_{tk}
$$

For $$p$$ number of contributors to the embodied emissions, where $$A$$ is the total planted area of landscaping type$$k$$ and $$c_k$$ is the carbon intensity of maintenance of landscape in year $$t$$ per area of planting $$k$$.

### Total Carbon Emissions

The total carbon emissions assessed by EPIC can be represented by this expression:

$$
{Total \atop Emissions} =\ \sum_{i=1}^{n}\ A\ast x_i\ast c_i\ast\left(1+r_i\right)+\ \sum_{t=1}^{m}\ \sum_{j=1}^{o}\ A\ast e_{tj}\ast c_j+\ \sum_{t=1}^{m}\ \sum_{k=1}^{p}\ A_k\ast c_{tk}
$$

With variables as defined in the preceding sections.

### Biogenic Carbon Sequestration

In EPIC, landscaping and the use of structural timber contribute to biogenic carbon sequestration. Carbon sequestration in structural materials is assessed once at the beginning of the project, and landscape sequestration is assessed each year. Biogenic carbon sequestration is evaluated with the following expression:

$$
Carbon\ Sequestration=x_i\ast C_i+\sum_{t=1}^{m}\ \sum_{t=1}^{m}\ A_k\ast C_k
$$

Where $$x_i$$ is the amount of carbon-sequestering timber structural material $$i$$, $$C_i$$ is the carbon sequestration per unit $$i$$,$$A_k$$ is the area A of carbon-sequestering planting type k, and $$C_k$$ is the carbon sequestration in year $$t$$ per area of planting $$k$$.

For more information on how biogenic carbon sequestration is treated within EPIC, refer to the appendix on [Biogenic Carbon](../appendices/biogenic-carbon.md).
