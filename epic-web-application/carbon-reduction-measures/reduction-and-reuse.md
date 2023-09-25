# Carbon Reduction Input Fields

##

## Sufficiency and Reuse

Sufficiency strategies are, as defined by the [IPCC](https://www.ipcc.ch/), that "measures and daily practices that avoid demand for energy, materials, land and water while delivering human well-being." Examples of sufficiency include building less, and reusing existing buildings instead of building new.

### **Reduction in building area**

A reduction to the overall floor area, distributed evenly across the building's floors. Typically, this can be achieved on projects by maximizing use of existing assets and through clever program design.&#x20;

### Building Reuse

<details>

<summary>Building Reuse Parameters</summary>

_Note that these measure only affects upfront emissions; refurbishments are counted normally._&#x20;

**Structure Reuse**

The reuse of a preexisting structural system for a given percentage of the building's floor area.

**Roofing Reuse**

The reuse of the roofing assembly for a given percentage of the building’s total roof area.&#x20;

**Cladding Reuse**

The reuse of opaque envelope for a given percentage of the building’s total envelope. Note that this measure only affects upfront emissions; refurbishments are counted normally.&#x20;

**Glazing Reuse**

The reuse of transparency envelope for a given percentage of the building’s total envelope. Note that this measure only affects upfront emissions; refurbishments are counted normally.&#x20;

**Fitout Reuse**

The reuse of interior fitout materials as a percentage of the total fitout.

**MEP Reuse**

The reuse of MEP systems as a percentage of the total system.





</details>



## Embodied Carbon | Structure

### New primary structural system

Specification of a structural system other than the system modeled in the base case. Note that this is not strictly a carbon _reduction_ measure, as the substitution of some structural systems with some others can lead to an increase in embodied emissions.&#x20;

<details>

<summary>Structural Systems included in EPIC</summary>

* _Composite_ s_teel frame_. A structural system comprised of steel columns, beams, and girders connected with rigid or pin joints. Floors are steel decking with a concrete topping slab.&#x20;

<!---->

* _Reinforced concrete_. A structural system comprised of columns, beams, and slabs of concrete reinforced with steel that provides tensile strength.

<!---->

* _Hybrid concrete/steel (high-rise)_. A structural system that combines rigid steel frames with concrete columns, beams, and slabs. These hybrid structures are more materially intensive and may be used when there are significant seismic loads, in high-rise buildings, or for programs with very high live or environmental loads.

<!---->

* _Wood frame_. A structural system comprised of dimensional lumber, plywood sheathing, and reinforced concrete cores and podiums.

<!---->

* _Comprehensive mass timber_. A structural system comprised of massive beams, panels, and columns, often assembled by aggregating many smaller timber elements. This approach assumes that timber elements are aggressively substituted for other structural materials.

</details>

### Concrete specification

The specification of concrete with lower embodied carbon emissions. Choices are described in narrative form below, and the underlying data is listed in the [embodied carbon methodology](../../c.scale-tm-data-model/methodology/embodied-carbon.md#carbon-intensities-of-structural-materials). Narrative descriptions are approximate; there are many options that can yield similar carbon intensities.

* **Conservative.** GWP in the 80th percentile of locally available concrete. Typical concrete mix, no effort made to lower carbon emissions.&#x20;
* **Best practices.** GWP in the 50th percentile of locally available concrete. Concrete with 30-50% replacement of cement by supplementary cementitious materials (SCM) and careful sizing of concrete structural elements to reduce overspecification.&#x20;
* **Low-carbon.** GWP in the 20th percentile of locally available concrete. Concrete with >50% replacement of cement by SCM, lower carbon aggregate, and careful sizing of concrete structural elements to reduce overspecification.&#x20;

<table><thead><tr><th width="199">Structural Material</th><th>Low Carbon</th><th width="174">Best Practices</th><th>Conservative</th></tr></thead><tbody><tr><td><strong>Concrete, 3-4 kSI</strong></td><td><em>Location-specific</em></td><td><em>Location-specific</em></td><td><em>Location-specific</em></td></tr><tr><td><strong>Concrete, 5-6 kSI</strong></td><td><em>Location-specific</em></td><td><em>Location-specific</em></td><td><em>Location-specific</em></td></tr><tr><td><strong>Concrete, 7-10 kSI</strong></td><td>0.16 kgCO2e/kg</td><td>0.18 kgCO2e/kg</td><td>0.19 kgCO2e/kg</td></tr></tbody></table>

### Steel specification

The specification of structural steel, steel deck, and reinforcing bar with lower embodied carbon emissions. Choices are described in narrative form below, and the underlying data is listed in the [embodied carbon methodology](../../c.scale-tm-data-model/methodology/embodied-carbon.md#carbon-intensities-of-structural-materials). Narrative descriptions are approximate; there are many options that can yield similar carbon intensities.

* **Conservative.** GWP in the 80th percentile of nationally available steel. Typical steel with a typical recycled content, from a mix of blast and electric arc furnaces.&#x20;
* **Best practices.** GWP in the 50th percentile of nationally available steel. Steel from electric arc furnaces or blast furnaces with gas recovery, with high recycled content, and structural design to minimize overspecification. &#x20;
* **Low-carbon.** GWP in the 20th percentile of nationally available steel. Steel from electric arc furnaces powered with renewable energy sources, potentially with biomass reductants, with high-recycled content, and structural design to minimize overspecification and maximize reusability.&#x20;

<table><thead><tr><th width="199">Structural Material</th><th>Low Carbon</th><th width="174">Best Practices</th><th>Conservative</th></tr></thead><tbody><tr><td><strong>Reinforcing Steel</strong></td><td>0.9 kgCO2e/kg</td><td>1.1 kgCO2e/kg</td><td>0.16 kgCO2e/kg</td></tr><tr><td><strong>Structural Steel</strong></td><td>0.9 kgCO2e/kg</td><td>1.1 kgCO2e/kg</td><td>1.2 kgCO2e/kg</td></tr><tr><td><strong>Steel Deck</strong></td><td>1.7 kgCO2e/kg</td><td>2.2 kgCO2e/kg</td><td>2.4 kgCO2e/kg</td></tr></tbody></table>

### Timber specification

The specification of lumber, plywood/OSB, and engineered timber elements with lower embodied carbon emissions. Choices are described in narrative form below, and the underlying data is listed in the [embodied carbon methodology](../../c.scale-tm-data-model/methodology/embodied-carbon.md#carbon-intensities-of-structural-materials). Narrative descriptions are approximate; there are many options that can yield similar carbon intensities.

* **Conservative.** GWP in the 80th percentile of nationally available timber. The highest GWP forest products may come from value chains where fossil gas is used for process heat at the mill, forestry and nursery practices require high levels of chemical inputs, forestry practices utilize intensive short-rotation harvest regimes, and transportation is over long distances by truck.
* **Best practices.** GWP in the 50th percentile of nationally available timber. Lowering the GWP of wood products can be achieved by using wood waste instead of natural gas for process heat at the mill, limiting chemical inputs such as fertilizer, practicing forestry that increases or at minimum maintains forest carbon stocks over time and provides protection for older forests, and transportation by efficient means such as rail.
* **Low-carbon.** GWP in the 20th percentile of locally available timber . Wood products with the lowest GWP may come from value chains where wood waste is reused to make durable goods, electricity or biomass is used for process heat where possible, chemical inputs such as fertilizer are mostly avoided, climate-smart forestry practices increase forest carbon stocks over time and promotes the growth of complex older forest conditions, and the forest is near the mill and construction sites.

<table><thead><tr><th width="199">Structural Material</th><th>Low Carbon</th><th width="174">Best Practices</th><th>Conservative</th></tr></thead><tbody><tr><td><strong>Lumber</strong></td><td>0.09 kgCO2e/kg</td><td>0.16 kgCO2e/kg</td><td>0.21 kgCO2e/kg</td></tr><tr><td><strong>Plywood/OSB</strong></td><td>0.36 kgCO2e/kg</td><td>0.51 kgCO2e/kg</td><td>0.73 kgCO2e/kg</td></tr><tr><td><strong>Engineered Wood</strong> </td><td>0.19 kgCO2e/kg</td><td>0.25 kgCO2e/kg</td><td>0.36 kgCO2e/kg</td></tr></tbody></table>

### Responsibly sourced timber

In accordance with ISO 21930, the carbon content of biogenic materials can only be counted as carbon-storing if the timber comes from a forest managed with sustainable practices. An example of this is timber from an FSC-certified forest. For more information, please refer to our methodology for [stored and avoided carbon](../../c.scale-tm-data-model/methodology/stored-avoided-carbon.md) or the procurement guidance from the [Climate Smart Wood Group](https://www.climatesmartwood.net/procurement/).

In EPIC, we identify three criteria contributing to the claim that wood products are responsibly sourced. While EPIC does not prevent the user from counting the carbon storage benefits on other terms (as the list below is nonexhaustive), we recommend meeting at least two out of the three criteria below in order to claim climate benefits from carbon storage:&#x20;

* **Transparency and traceability in the supply chain (required)**. Claims can be made about the environmental attributes of timber are impossible to verify without transparency and traceability in the supply chain. This means that a project team should be able to identify:
  1. The source forest(s) or supply area(s)
     * _This is the area from which a primary manufacturer sources most or all of its logs, typically a circle drawn around the location of the site of the mill, with the size being dictated by the maximum hauling distance of the logs._
  2. The primary manufacturer mill(s)
     * _E.g., sawmill, veneer mill, chip mill, etc._
  3. The fabrication shop (for engineered timber).
* **Increasing forest carbon stocks (optional)**. Carbon storage in wood products can only be claimed if the carbon stock of the source forest is maintained or increasing. This means that the forest area is managed and regenerates in a way that either preserves or increases the average level of carbon stored in vegetation and soils, or that high conservation value or high carbon stock forests are not replaced by less ecological valuable and carbon rich production forests.
* **Certified, recycled, or reclaimed wood (optional)**. The use of recycled or reclaimed wood prolongs its storage of carbon and can displace the use of virgin timber. Certification by the Forest Stewardship Council (FSC) ensures that sound forestry, audit, and reporting practices are used.

## Embodied Carbon | Assemblies <a href="#embodied-carbon-measures-nonstructure" id="embodied-carbon-measures-nonstructure"></a>

### Envelope specification

The specification of the roofing, glazing, and opaque envelope assemblies. These specification levels do not describe specific assemblies. Instead, they approximate the 80th, 50th, and 20th percentile of the distribution of all envelope options. The three options for this measure and their general description:

* **Conservative.** 80th percentile of GWP for envelope assemblies. Standard materials and assemblies, no effort made to lower carbon emissions.
* **Best practices.** 50th percentile of GWP for envelope assemblies. Reduce redundancies and select low-carbon materials with high levels of recycled content.
* **Low-carbon.** 20th percentile of GWP for envelope assemblies. Maximize biogenic materials, innovate efficient assemblies, and reduce material use.

| Envelope Assembly                                                       | Low Carbon     | Best Practices | Conservative   |
| ----------------------------------------------------------------------- | -------------- | -------------- | -------------- |
| <p><strong>Cladding</strong> <br><strong>(opaque envelope)</strong></p> | 3.0 kgCO2e/sf  | 8.8 kgCO2e/sf  | 14.3 kgCO2e/sf |
| **Glazing (transparent envelope)**                                      | 11.4 kgCO2e/sf | 13.6 kgCO2e/sf | 19.0 kgCO2e/sf |
| **Roofing**                                                             | 5.3 kgCO2e/sf  | 7.7 kgCO2e/sf  | 14.0 kgCO2e/sf |

### Interior Fit Out specification

The specification of the fittings, furniture, and fixtures required for the use of the building by its tenants. These specification levels do not describe specific fit-outs or materials. Instead, they approximate the 80th, 50th, and 20th percentile of the distribution of all available data on tenant fit-outs. The three options for this measure and their general description:

* **Conservative.** 80th percentile of GWP for interior fitouts. Standard fittings, furniture, and fixtures, no effort made to lower carbon emissions.
* **Best practices.** 50th percentile of GWP for interior fitouts. Address "hot spots" (flooring, acoustic panels, casework, etc.).
* **Low-carbon.** 20th percentile of GWP for interior fitouts. Comprehensive low-carbon design and specification of tenant fit-out.

| Assembly             | Low Carbon    | Best Practices | Conservative   |
| -------------------- | ------------- | -------------- | -------------- |
| **Interior Fit Out** | 4.0 kgCO2e/sf | 7.6 kgCO2e/sf  | 13.3 kgCO2e/sf |

### Hardscape specification

The specification of the pervious and impervious surfaces on the building site (outside the building envelope. These specification levels do not describe specific materials or assemblies. Instead, they approximate the 80th, 50th, and 20th percentile of the distribution of all hardscape assemblies based on a set of standard details. The three options for this measure and their general description:

* **Conservative.** 80th percentile of GWP for hardscape assemblies.&#x20;
* **Best practices.** 50th percentile of GWP for hardscape assemblies.&#x20;
* **Low-carbon.** 20th percentile of GWP for hardscape assemblies.&#x20;

| Assembly      | Low Carbon    | Best Practices | Conservative  |
| ------------- | ------------- | -------------- | ------------- |
| **Hardscape** | 4.4 kgCO2e/sf | 5.9 kgCO2e/sf  | 7.2 kgCO2e/sf |

### Envelope refurbishment period

The length of time over which a majority of the exterior envelope will be replaced.

### Interior fit-out refurbishment period

The length of time over which a majority of the interior fit-out will be replaced.

### MEP and PV refurbishment period

The length of time over which a majority of the building systems will be replaced.

### Hardscape refurbishment period

The length of time over which a majority of the site's hardscape will be replaced.

## Operational Carbon

### All Electric Building

The elimination of all onsite combustion and provision of 100% of the project’s energy use from electric sources.

### EUI reduction

The reduction of the building’s EUI by any of a number of strategies.

### Solar photovoltaic (PV) array

The construction of a solar PV array on the project site. The size of this array can be input in three forms:

* **Area.** The solar PV area size is input by its total area in square feet.
* **Capacity.** The solar PV area size is input by its nameplate capacity in kW.
* **% of load.** The solar PV area size is calculated to account for the input percentage of building energy load.

### Solar PV orientation

The ability of solar PV arrays to produce electricity is related to their geometry and siting. Not all projects sites, such as partially shaded sites, will have an optimal solar orientation. This toggle has two options:

* **Optimal.** There is no impediment on the site to maximum solar exposure.
* **Suboptimal.** There is solar potential on the site, but it is partly compromised. A 20% penalty on solar energy production will be assessed.

### Clean power purchase

The purchase of clean power through Direct Ownership, Green Retail Tariffs, Power Purchase Agreements (PPAs), Community Renewables or Utility Renewable Contracts (the five categories of renewables for which credit can be claimed in AIA 2030 commitment reporting) equivalent to the selected percentage of total energy use. _The purchase of unbundled RECs should not be counted as a clean power purchase in EPIC._

Some operational emissions (20%) will persist after the clean power purchase to account for the real emissions that are still generated on an electrical grid with both intermittent renewable and carbon-emitting energy sources. There are three options for this measure:

* **None.** No purchase of clean power or RECs.
* **Low: 50% of electricity purchased from clean sources.** Purchase of clean power to cover 50% of building energy use.&#x20;
* **High: 100% of electricity purchased from clean sources.** Purchase of clean power to cover 100% of building energy use.&#x20;
* **24/7 Clean: 100% time-matched clean power purchase**. Time matched purchase of zero-carbon power to ensure that building emissions are totally offset. Because they are not time-matched, the clean power purchase is not subject to the 20% discounting.

## Refrigerant Emissions

_\*\*\*coming soon\*\*\*_

## Site and Landscape

This set of measures describes potential carbon storage in the landscape as well as annual emissions associated with the landscape's upkeep.

### Convert hardscape area to planted area

Converts hardscape area to planted area, up to the maximum of site area less building footprint.&#x20;

### Carbon Storing Landscape

Definition of the proportion of total planted area that is low, moderate, or high carbon storage.

* **Low carbon storage planted area.** Example of a low carbon storage landscape is no-mow turfgrass or other herbaceous perennials. This is the assumption for all planted areas in the base case.
* **High carbon storage planted area.** An example of a high carbon storage landscape is one composed of dense broadleaf shrubs and trees in a matrix of no-mow turfgrass or herbaceous perennials.

## Planted Roof

### Planted roof area

The percentage of roof area planted.

### Planted roof specification

There are two levels of specification available in EPIC for green roofs.&#x20;

* **Low Carbon Storage (extensive).** An extensive green roof has a thin layer of soil that can only support shallowly rooted plants. An example of an extensive green roof is sedum mat or low turfgrass.
* **High Carbon Storage (intensive).** An intensive green roof has a deeper layer of soil that can support plants such as larger perennial grasses and small shrubs.

