# Carbon Reduction Input Fields

## Reduction and Reuse

#### Reduction in building Area

A reduction to the overall floor area, distributed evenly across the building's floors.

#### Building structure reuse

The reuse of a pre-existing structural system for a given percentage of the building's floor area.

#### Envelope reuse

The reuse of opaque envelope for a given percentage of the building’s total envelope.

#### Glazing reuse

The reuse of glazing units for a given percentage of the building’s total envelope.

## Embodied Carbon Measures - Structure

#### New primary structural system

Specification of a structural system other than the system modeled in the base case. Note that this is not strictly a carbon _reduction_ measure, as the substitution of some structural systems with some others can lead to an increase in embodied emissions.&#x20;

<details>

<summary>Structural Systems included in EPIC</summary>

* _Steel frame_. A structural system comprised of columns, beams, girders, and decking constructed from steel structural members connected with rigid or pin joints.

<!---->

* _Reinforced concrete_. A structural system comprised of columns, beams, and slabs of concrete reinforced with steel that provides tensile strength.

<!---->

* _Hybrid concrete/steel (high-rise)_. A structural system that combines rigid steel frames with concrete columns, beams, and slabs. These hybrid structures are more materially intensive and may be used when there are significant seismic loads, in high-rise buildings, or for programs with very high live or environmental loads.

<!---->

* _Wood frame_. A structural system comprised of dimensional lumber, plywood sheathing, and reinforced concrete cores and podiums.

<!---->

* _Comprehensive mass timber_. A structural system comprised of massive beams, panels, and columns, often assembled by aggregating many smaller timber elements. This approach assumes that timber elements are aggressively substituted for other structural materials.

</details>

#### Concrete specification

The specification of concrete with lower embodied carbon emissions. Choices are described in narrative form below, and the underlying data is listed in the [embodied carbon methodology](../../methodology/calculations.md#carbon-intensities-of-structural-materials). Narrative descriptions are approximate; there are many options that can yield similar carbon intensities.

* **Conservative.** GWP in the 80th percentile of locally available concrete. Typical concrete mix, no effort made to lower carbon emissions.&#x20;
* **Best practices.** GWP in the 50th percentile of locally available concrete. Concrete with 30-50% replacement of cement by supplementary cementitious materials (SCM) and careful sizing of concrete structural elements to reduce overspecification.&#x20;
* **Low-carbon.** GWP in the 20th percentile of locally available concrete. Concrete with >50% replacement of cement by SCM, lower carbon aggregate, and careful sizing of concrete structural elements to reduce overspecification.&#x20;

#### Steel specification

The specification of structural steel, steel deck, and reinforcing bar with lower embodied carbon emissions. Choices are described in narrative form below, and the underlying data is listed in the [embodied carbon methodology](../../methodology/calculations.md#carbon-intensities-of-structural-materials). Narrative descriptions are approximate; there are many options that can yield similar carbon intensities.

* **Conservative.** GWP in the 80th percentile of nationally available steel. Typical steel with a typical recycled content, from a mix of blast and electric arc furnaces.&#x20;
* **Best practices.** GWP in the 50th percentile of nationally available steel. Steel from electric arc furnaces or blast furnaces with gas recovery, with high recycled content, and structural design to minimize overspecification. &#x20;
* **Low-carbon.** GWP in the 20th percentile of nationally available steel. Steel from electric arc furnaces powered with renewable energy sources, potentially with biomass reductants, with high-recycled content, and structural design to minimize overspecification and maximize reusability.&#x20;

#### Timber specification

The specification of lumber, plywood/OSB, and engineered timber elements with lower embodied carbon emissions. Choices are described in narrative form below, and the underlying data is listed in the [embodied carbon methodology](../../methodology/calculations.md#carbon-intensities-of-structural-materials). Narrative descriptions are approximate; there are many options that can yield similar carbon intensities.

* **Conservative.** GWP in the 80th percentile of nationally available timber. The highest GWP forest products may come from value chains where fossil gas is used for process heat at the mill, forestry and nursery practices require high levels of chemical inputs, and transportation is over long distances by truck. Typically, forest products from forests in the American Southeast have higher GWP than those from the Northeast or Northwest.&#x20;
* **Best practices.** GWP in the 50th percentile of nationally available timber. Lowering the GWP of wood products can be achieved by using wood waste instead of natural gas for process heat at the mill, limiting chemical inputs such as fertilizer, and transportation by efficient means such as rail. Typically, forest products from forests in the American Northwest have GWP values lower than those from the Southeast and higher than those in th Northeast.&#x20;
* **Low-carbon.** GWP in the 20th percentile of locally available concrete. Wood products with the lowest GWP may come from value chains where wood waste is reused to make durable goods, electricity is used for process heat where possible, chemical inputs such as fertilizer are mostly avoided, and the forest is near the mill and construction sites. Typically, forest products from forests in the American Northeast have lower GWP than those from the Southeast or Northwest.&#x20;

#### Responsibly sourced timber

In accordance with ISO 21930, the carbon content of biogenic materials can only be counted as carbon-storing if the timber comes from a forest managed with sustainable practices. An example of this is timber from an FSC-certified forest. For more information, please refer to the appendix on [Biogenic Carbon](https://epic-documentation.gitbook.io/epic/appendices/biogenic-carbon) or the procurement guidance from the [Climate Smart Wood Group](https://www.climatesmartwood.net/procurement/).

## Embodied Carbon Measures - Non-structure <a href="#embodied-carbon-measures-nonstructure" id="embodied-carbon-measures-nonstructure"></a>

#### Envelope specification

The specification of the roofing, glazing, and opaque envelope assemblies. These specification levels do not describe specific assemblies. Instead, they approximate the 80th, 50th, and 20th percentile of the distribution of all envelope options. The three options for this measure and their general description:

* **Conservative.** 80th percentile of GWP for envelope assemblies. Standard materials and assemblies, no effort made to lower carbon emissions.
* **Best practices.** 50th percentile of GWP for envelope assemblies. Reduce redundancies and select low-carbon materials with high levels of recycled content.
* **Low-carbon.** 20th percentile of GWP for envelope assemblies. Maximize biogenic materials, innovate efficient assemblies, and reduce material use.

#### Envelope refurbishment period

The length of time over which a majority of the exterior envelope will be replaced.

#### Interior fit-out specification

The specification of the fittings, furniture, and fixtures required for tenants by tenants who inhabit and use the building. These specification levels do not describe specific fit-outs or materials. Instead, they approximate the 80th, 50th, and 20th percentile of the distribution of all available data on tenant fit-outs. The three options for this measure and their general description:

* **Conservative.** Standard fittings, furniture, and fixtures, no effort made to lower carbon emissions.
* **Best practices.** Address "hot spots" (flooring, acoustic panels, casework, etc.).
* **Low-carbon.** Comprehensive low-carbon design and specification of tenant fit-out.

#### Interior fit-out refurbishment period

The length of time over which a majority of the interior fit-out will be replaced.

#### Systems refurbishment period

The length of time over which a majority of the building systems (MEP and solar PV) will be replaced.

## Operational Carbon

#### All Electric Building

The elimination of all onsite combustion and provision of 100% of the project’s energy use from electric sources.

#### EUI reduction

The reduction of the building’s EUI by any of a number of strategies.

#### Solar photovoltaic (PV) array

The construction of a solar PV array on the project site. The size of this array can be input in three forms:

* **Area.** The solar PV area size is input by its total area in square feet.
* **Capacity.** The solar PV area size is input by its nameplate capacity in kW.
* **% of load.** The solar PV area size is calculated to account for the input percentage of building energy load.

#### Solar PV orientation

The ability of solar PV arrays to produce electricity is related to their geometry and siting. Not all projects sites, such as partially shaded sites, will have an optimal solar orientation. This toggle has two options:

* **Optimal.** There is no impediment on the site to maximum solar exposure.
* **Suboptimal.** There is solar potential on the site, but it is partly compromised. A 20% penalty on solar energy production will be assessed.

#### Clean power purchase

The purchase of clean power through Direct Ownership, Green Retail Tariffs, Power Purchase Agreements (PPAs), Community Renewables or Utility Renewable Contracts (the five categories of renewables for which credit can be claimed in AIA 2030 commitment reporting) equivalent to the selected percentage of total energy use. _The purchase of unbundled RECs should not be counted here._

Some operational emissions (20%) will persist after the clean power purchase to account for the real emissions that are still generated on an electrical grid with both intermittent renewable and carbon-emitting energy sources. There are three options for this measure:

* **None.** No purchase of clean power or RECs.
* **Low: 50% of electricity purchased from clean sources.** Purchase of clean power to cover 50% of building energy use.&#x20;
* **High: 100% of electricity purchased from clean sources.** Purchase of clean power to cover 100% of building energy use.&#x20;
* **24/7 Clean: 100% time-matched clean power purchase**. Time matched purchase of zero-carbon power to ensure that building emissions are totally offset. Because they are not time-matched, the clean power purchase is not subject to the 20% discounting.

## Site and Landscape

This set of measures describes potential carbon storage in the landscape as well as annual emissions associated with the landscape's upkeep.

#### Reduced hardscape area

Converts hardscape area to planted area, up to the maximum of site area less building footprint.&#x20;

#### Carbon Storing Landscape

Definition of the proportion of total planted area that is low, moderate, or high carbon storage.

* **Low carbon storage planted area.** Example of a low carbon storage landscape is no-mow turfgrass or other herbaceous perennials. This is the assumption for all planted areas in the base case.
* **Moderate carbon storage planted area.** An example of a moderate carbon storage landscape is low shrubs and small trees in a matrix of no-mow turfgrass or herbaceous perennials.
* **High carbon storage planted area.** An example of a high carbon storage landscape is one composed of dense broadleaf shrubs and trees in a matrix of no-mow turfgrass or herbaceous perennials.

#### Hardscape specification

Text

* **Conservative.** Text
* **Best practices.** Text
* **Low-carbon.** Text

#### Hardscape refurbishment period

The length of time over which a majority of the interior fit-out will be replaced.

#### Planted roof area

The length of time over which a majority of the interior fit-out will be replaced.

#### Planted roof specification

Text

* **Conservative.** Text
* **Best practices.** Text
* **Low-carbon.** Text

