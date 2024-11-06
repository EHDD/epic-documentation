# Carbon Reduction Measures

<mark style="background-color:red;">Carbon reduction measures in EPIC are generally divided into the following categories:</mark>

* [<mark style="background-color:red;">**Reuse**</mark>](reduction-and-reuse.md#reduction-and-reuse)<mark style="background-color:red;">. These measures deal with the savings from reuse of existing building assemblies.</mark>
* <mark style="background-color:red;">**Form and Massing**</mark><mark style="background-color:red;">. These measures pertain to the impact the form of the building has on the amount of materials used in the structure and enclosure.</mark>&#x20;
* <mark style="background-color:red;">**Energy Use**</mark><mark style="background-color:red;">. These measures pertain to reducing the use of energy in the building, and selecting clean sources of energy.</mark>
* <mark style="background-color:red;">**Structure**</mark><mark style="background-color:red;">. These measures pertain to selecting low carbon alternatives for the substructure and superstructure, including both lateral and gravity systems.</mark>
* <mark style="background-color:red;">**Enclosure**</mark><mark style="background-color:red;">. These measures pertain to selecting low carbon alternatives for the opaque enclosure, transparent enclosure, and roofing, and their replacement periods.</mark>
* <mark style="background-color:red;">**Interior**</mark><mark style="background-color:red;">. These measures pertain to selecting low carbon alternatives for the interior construction and fit-out, and their replacement periods.</mark>
* <mark style="background-color:red;">**Services**</mark><mark style="background-color:red;">.</mark> <mark style="background-color:red;">These measures pertain to selecting low carbon alternatives for the mechanical, electrical, and plumbing (MEP) services and PV Array, and their replacement periods.</mark>
* <mark style="background-color:red;">**Refrigerants**</mark><mark style="background-color:red;">. These measures pertain to selecting low carbon alternatives for the refrigerants used in building services (e.g., HVAC+R).</mark>
* [<mark style="background-color:red;">**Sitework**</mark>](reduction-and-reuse.md#site-and-landscape)<mark style="background-color:red;">.</mark> <mark style="background-color:red;">These measures pertain to the hardscape and landscape surrounding the building, and assess their respective potential to add or sequester carbon.</mark>
* <mark style="background-color:red;">**Jobsite**</mark><mark style="background-color:red;">. These measures pertain to the construction-related (A5) emissions.</mark>

## Reuse

### Building Reuse

The percentage of existing building materials to remain on-site and be used in the project, reducing the demand for new materials.

<details>

<summary>Building Reuse Parameters</summary>

_Note that these measures only affect upfront emissions; refurbishments are counted normally._&#x20;

**Structure Reuse**

The reuse of a pre-existing structural system for a given percentage of the building's floor area.

**Opaque Enclosure Reuse**

The reuse of opaque enclosure for a given percentage of the building’s total enclosure. Note that this measure only affects upfront emissions; refurbishments are counted normally.&#x20;

**Transparent Enclosure Reuse**

The reuse of transparent enclosure for a given percentage of the building’s total enclosure. Note that this measure only affects upfront emissions; refurbishments are counted normally.&#x20;

**Roofing Reuse**

The reuse of the roofing assembly for a given percentage of the building’s total roof area.&#x20;

**Interior Reuse**

The reuse of interior fitout materials as a percentage of the total fitout.

**Services Reuse**

The reuse of MEP systems as a percentage of the total system.

</details>

## Form and Massing

### **Building Perimeter**

The user-declared perimeter of the building. In the absence of a user input, EPIC assumes the building is an extruded square.

### **Floor-to-Floor Height**

The vertical distance between building floors in feet. The default value is 13’.

### Window-to-Wall Ratio (WWR)

The ratio of windows to total wall area. The default value is .45.

## Energy Use

### All Electric Building

The elimination of all onsite combustion and provision of 100% of the project’s energy use from electric sources.

### EUI Target

The reduction of the building’s EUI by any of a number of strategies. If the you have not entered a custom EUI, the EUI is estimated via [ZeroTool](https://zerotool.org/).&#x20;

### Clean Power Purchase

The purchase of clean power through Direct Ownership, Green Retail Tariffs, Power Purchase Agreements (PPAs), Community Renewables or Utility Renewable Contracts (the five categories of renewables for which credit can be claimed in AIA 2030 commitment reporting) equivalent to the selected percentage of total energy use. _The purchase of unbundled RECs should not be counted as a clean power purchase in EPIC._

<details>

<summary>Clean Power Purchase Thresholds</summary>

* **0%.** No purchase of clean power or RECs.

<!---->

* **50%.** Purchase of clean power to cover 50% of building energy use. This option assumes that these RECs are not time-matched, and discounts their effectiveness by 20% as they don't follow patterns of emissions on the electrical grid.&#x20;

<!---->

* **100%.** Purchase of clean power to cover 100% of building energy use. This option assumes that these RECs are not time-matched, and discounts their effectiveness by 20% as they don't follow patterns of emissions on the electrical grid.&#x20;

</details>

### Solar photovoltaic (PV) array

The addition of a solar PV array on the project site. The size of this array can be input in three forms:

* **Percentage of Load.** The solar PV area size is calculated to account for the input percentage of building energy load.
* **Nameplate Capacity.** The solar PV area size is input by its nameplate capacity in kW.
* **Area.** The solar PV area size is input by its total area in square feet.

#### Solar PV orientation

The ability of solar PV arrays to produce electricity is related to their geometry and siting. Not all projects sites, such as partially shaded sites, will have an optimal solar orientation. This toggle has two options:

* **Optimal.** There is no impediment on the site to maximum solar exposure.
* **Suboptimal.** There is solar potential on the site, but it is partly compromised. A 20% penalty on solar energy production will be assessed.

## Structure

### Primary Structural System

Specification of a structural system other than the system modeled in the base case. Note that this is not strictly a carbon _reduction_ measure, as the substitution of some structural systems with some others can lead to an increase in embodied emissions.&#x20;

<details>

<summary>Structural Systems Included in EPIC</summary>

* **Reinforced Concrete**. A structural system comprised of columns, beams, and slabs of concrete reinforced with steel that provides tensile strength.

<!---->

* **Mass Timber**. A structural system comprised of massive beams, panels, and columns, often assembled by aggregating many smaller timber elements. This approach assumes that timber elements are aggressively substituted for other structural materials.

<!---->

* **Wood Frame**. A structural system comprised of dimensional lumber, plywood sheathing, and reinforced concrete cores and podiums.

<!---->

* **Steel Frame**. A structural system comprised of steel columns, beams, and girders connected with rigid or pin joints. Floors are steel decking with a concrete topping slab.&#x20;

<!---->

* **Hybrid Concrete-Steel**. A structural system that combines rigid steel frames with concrete columns, beams, and slabs. These hybrid structures are more materially intensive and may be used when there are significant seismic loads, in high-rise buildings, or for programs with very high live or environmental loads.

</details>

### Secondary Structural System

Specification of a secondary structural system, and its associated percentage of the overall building structure.&#x20;

### Concrete Specification

The specification of concrete with lower embodied carbon emissions. Choices are described in narrative form below, and the underlying data is listed in [C.Scale's whole life carbon methodology](https://docs.cscale.io/the-c.scale-tm-data-model/embodied-carbon). Narrative descriptions are approximate; there are many options that can yield similar carbon intensities.

<details>

<summary>Concrete Specification Choices (Carbon Intensity)</summary>

* **High (80th percentile).** GWP in the 80th percentile of locally available concrete. Typical concrete mix, no effort made to lower carbon emissions.&#x20;

<!---->

* **Medium (50th percentile).** GWP in the 50th percentile of locally available concrete. Concrete with 30-50% replacement of cement by supplementary cementitious materials (SCM) and careful sizing of concrete structural elements to reduce overspecification.&#x20;

<!---->

* **Low (20th percentile).** GWP in the 20th percentile of locally available concrete. Concrete with >50% replacement of cement by SCM, lower carbon aggregate, and careful sizing of concrete structural elements to reduce overspecification.&#x20;

</details>

<table><thead><tr><th width="199">Structural Material</th><th>Low Carbon</th><th width="174">Best Practices</th><th>Conservative</th></tr></thead><tbody><tr><td><strong>Concrete, 3-4 kSI</strong></td><td><em>Location-specific</em></td><td><em>Location-specific</em></td><td><em>Location-specific</em></td></tr><tr><td><strong>Concrete, 5-6 kSI</strong></td><td><em>Location-specific</em></td><td><em>Location-specific</em></td><td><em>Location-specific</em></td></tr><tr><td><strong>Concrete, 7-10 kSI</strong></td><td>0.16 kgCO2e/kg</td><td>0.18 kgCO2e/kg</td><td>0.19 kgCO2e/kg</td></tr></tbody></table>

### Steel Specification

The specification of structural steel, steel deck, and reinforcing bar with lower embodied carbon emissions. Choices are described in narrative form below, and the underlying data is described in [C.Scale's whole life carbon methodology](https://docs.cscale.io/the-c.scale-tm-data-model/embodied-carbon). Narrative descriptions are approximate; there are many options that can yield similar carbon intensities.

<details>

<summary>Steel Specification Choices (Carbon Intensity)</summary>

* **High (80th percentile).** GWP in the 80th percentile of locally available concrete. Typical concrete mix, no effort made to lower carbon emissions.&#x20;

<!---->

* **Medium (50th percentile).** GWP in the 50th percentile of locally available concrete. Concrete with 30-50% replacement of cement by supplementary cementitious materials (SCM) and careful sizing of concrete structural elements to reduce overspecification.&#x20;

<!---->

* **Low (20th percentile).** GWP in the 20th percentile of locally available concrete. Concrete with >50% replacement of cement by SCM, lower carbon aggregate, and careful sizing of concrete structural elements to reduce overspecification.&#x20;

</details>

<table><thead><tr><th width="199">Structural Material</th><th>Low Carbon</th><th width="174">Best Practices</th><th>Conservative</th></tr></thead><tbody><tr><td><strong>Reinforcing Steel</strong></td><td>0.9 kgCO2e/kg</td><td>1.1 kgCO2e/kg</td><td>0.16 kgCO2e/kg</td></tr><tr><td><strong>Structural Steel</strong></td><td>0.9 kgCO2e/kg</td><td>1.1 kgCO2e/kg</td><td>1.2 kgCO2e/kg</td></tr><tr><td><strong>Steel Deck</strong></td><td>1.7 kgCO2e/kg</td><td>2.2 kgCO2e/kg</td><td>2.4 kgCO2e/kg</td></tr></tbody></table>

### Timber Specification

The specification of lumber, plywood/OSB, and engineered timber elements with lower embodied carbon emissions. Choices are described in narrative form below. Narrative descriptions are approximate; there are many options that can yield similar carbon intensities.

<details>

<summary>Timber Specification Choices (Carbon Intensity)</summary>

* **High (80th percentile).** GWP in the 80th percentile of nationally available timber. The highest GWP forest products may come from value chains where fossil gas is used for process heat at the mill, forestry and nursery practices require high levels of chemical inputs, forestry practices utilize intensive short-rotation harvest regimes, and transportation is over long distances by truck.

<!---->

* **Medium (50th percentile).** GWP in the 50th percentile of nationally available timber. Lowering the GWP of wood products can be achieved by using wood waste instead of natural gas for process heat at the mill, limiting chemical inputs such as fertilizer, practicing forestry that increases or at minimum maintains forest carbon stocks over time and provides protection for older forests, and transportation by efficient means such as rail.

<!---->

* **Low (20th percentile)** GWP in the 20th percentile of locally available timber . Wood products with the lowest GWP may come from value chains where wood waste is reused to make durable goods, electricity or biomass is used for process heat where possible, chemical inputs such as fertilizer are mostly avoided, climate-smart forestry practices increase forest carbon stocks over time and promotes the growth of complex older forest conditions, and the forest is near the mill and construction sites.

</details>

<table><thead><tr><th width="199">Structural Material</th><th>Low Carbon</th><th width="174">Best Practices</th><th>Conservative</th></tr></thead><tbody><tr><td><strong>Lumber</strong></td><td>0.09 kgCO2e/kg</td><td>0.16 kgCO2e/kg</td><td>0.21 kgCO2e/kg</td></tr><tr><td><strong>Plywood/OSB</strong></td><td>0.36 kgCO2e/kg</td><td>0.51 kgCO2e/kg</td><td>0.73 kgCO2e/kg</td></tr><tr><td><strong>Engineered Wood</strong> </td><td>0.19 kgCO2e/kg</td><td>0.25 kgCO2e/kg</td><td>0.36 kgCO2e/kg</td></tr></tbody></table>

### Responsibly-Sourced Timber

In accordance with ISO 21930, the carbon content of biogenic materials can only be counted as carbon-storing if the timber comes from a forest managed with sustainable practices. An example of this is timber from an FSC-certified forest. For more information, please refer to C.Scale methodology for [stored and avoided carbon emissions](https://docs.cscale.io/the-c.scale-tm-data-model/embodied-carbon/stored-avoided-carbon) or the procurement guidance from the [Climate Smart Wood Group](https://www.climatesmartwood.net/procurement/).

In EPIC, we identify three criteria contributing to the claim that wood products are responsibly sourced. While EPIC does not prevent the user from counting the carbon storage benefits on other terms (as the list is nonexhaustive), we recommend meeting at least two out of the three criteria below in order to claim climate benefits from carbon storage.

<details>

<summary>Criteria for "Responsibly-Sourced Timber"</summary>

* **Transparent & traceable supply chain (required)**. Claims can be made about the environmental attributes of timber are impossible to verify without transparency and traceability in the supply chain. This means that a project team should be able to identify:
  1. The source forest(s) or supply area(s)
     * _This is the area from which a primary manufacturer sources most or all of its logs, typically a circle drawn around the location of the site of the mill, with the size being dictated by the maximum hauling distance of the logs._
  2. The primary manufacturer mill(s)
     * _E.g., sawmill, veneer mill, chip mill, etc._
  3. The fabrication shop (for engineered timber).

<!---->

* **Source forest has a growing carbon stock (optional)**. Carbon storage in wood products can only be claimed if the carbon stock of the source forest is maintained or increasing. This means that the forest area is managed and regenerates in a way that either preserves or increases the average level of carbon stored in vegetation and soils, or that high conservation value or high carbon stock forests are not replaced by less ecological valuable and carbon rich production forests.

<!---->

* **Timber is certified, recycled, or reclaimed (optional)**. The use of recycled or reclaimed wood prolongs its storage of carbon and can displace the use of virgin timber. Certification by the Forest Stewardship Council (FSC) ensures that sound forestry, audit, and reporting practices are used.

</details>

## Enclosure&#x20;

### Opaque Enclosure Specification

The specification of the opaque envelope assemblies. These specification levels do not describe specific assemblies. Instead, they approximate the 80th, 50th, and 20th percentile of the distribution of all opaque enclosure options.&#x20;

<details>

<summary>Opaque Enclosure Specification Choices (Carbon Intensity)</summary>

* **High (80th percentile).** 80th percentile of GWP for envelope assemblies. Standard materials and assemblies, no effort made to lower carbon emissions.

<!---->

* **Medium (50th percentile).** 50th percentile of GWP for envelope assemblies. Reduce redundancies and select low-carbon materials with high levels of recycled content.

<!---->

* **Low (20th percentile).** 20th percentile of GWP for envelope assemblies. Maximize biogenic materials, innovate efficient assemblies, and reduce material use.

</details>

<table><thead><tr><th width="203">Envelope Assembly</th><th>Low Carbon</th><th>Best Practices</th><th>Conservative</th></tr></thead><tbody><tr><td><strong>Opaque Enclosure</strong></td><td>3.0 kgCO2e/sf</td><td>8.8 kgCO2e/sf</td><td>14.3 kgCO2e/sf</td></tr></tbody></table>

### Opaque Enclosure Refresh Rate

The length of time over which a majority of the opaque enclosure will be replaced.

### Transparent Enclosure Specification

The specification of the transparent enclosure assemblies. These specification levels do not describe specific assemblies. Instead, they approximate the 80th, 50th, and 20th percentile of the distribution of all transparent enclosure options.&#x20;

<details>

<summary>Transparent Enclosure Specification Choices (Carbon Intensity)</summary>

* **High (80th percentile).** 80th percentile of GWP for envelope assemblies. Standard materials and assemblies, no effort made to lower carbon emissions.

<!---->

* **Medium (50th percentile).** 50th percentile of GWP for envelope assemblies. Reduce redundancies and select low-carbon materials with high levels of recycled content.

<!---->

* **Low (20th percentile).** 20th percentile of GWP for envelope assemblies. Maximize biogenic materials, innovate efficient assemblies, and reduce material use.

</details>

<table><thead><tr><th width="203">Envelope Assembly</th><th>Low Carbon</th><th>Best Practices</th><th>Conservative</th></tr></thead><tbody><tr><td><strong>Transparent Enclosure</strong></td><td>11.4 kgCO2e/sf</td><td>13.6 kgCO2e/sf</td><td>19.0 kgCO2e/sf</td></tr></tbody></table>

### Transparent Enclosure Refresh Rate

The length of time over which a majority of the transparent enclosure will be replaced.

### Roofing Specification

The specification of the roofing assemblies. These specification levels do not describe specific assemblies. Instead, they approximate the 80th, 50th, and 20th percentile of the distribution of all roofing options.&#x20;

<details>

<summary>Roofing Specification Choices (Carbon Intensity)</summary>

* **High (80th percentile).** 80th percentile of GWP for envelope assemblies. Standard materials and assemblies, no effort made to lower carbon emissions.

<!---->

* **Medium (50th percentile).** 50th percentile of GWP for envelope assemblies. Reduce redundancies and select low-carbon materials with high levels of recycled content.

<!---->

* **Low (20th percentile).** 20th percentile of GWP for envelope assemblies. Maximize biogenic materials, innovate efficient assemblies, and reduce material use.

</details>

<table><thead><tr><th width="203">Envelope Assembly</th><th>Low Carbon</th><th>Best Practices</th><th>Conservative</th></tr></thead><tbody><tr><td><strong>Roofing</strong></td><td>5.3 kgCO2e/sf</td><td>7.7 kgCO2e/sf</td><td>14.0 kgCO2e/sf</td></tr></tbody></table>

### Roofing Refresh Rate

The length of time over which a majority of the roofing will be replaced.

## Interior

### Interior Fit Out specification

The specification of the fittings, furniture, and fixtures required for the use of the building by its tenants. These specification levels do not describe specific fit-outs or materials. Instead, they approximate the 80th, 50th, and 20th percentile of the distribution of all available data on tenant fit-outs.&#x20;

<details>

<summary>Interior Fit Out Specification Options</summary>

* **Conservative.** 80th percentile of GWP for interior fitouts. Standard fittings, furniture, and fixtures, no effort made to lower carbon emissions.

<!---->

* **Best practices.** 50th percentile of GWP for interior fitouts. Address "hot spots" (flooring, acoustic panels, casework, etc.).

<!---->

* **Low-carbon.** 20th percentile of GWP for interior fitouts. Comprehensive low-carbon design and specification of tenant fit-out.

</details>

| Assembly             | Low Carbon    | Best Practices | Conservative   |
| -------------------- | ------------- | -------------- | -------------- |
| **Interior Fit Out** | 4.0 kgCO2e/sf | 7.6 kgCO2e/sf  | 13.3 kgCO2e/sf |

#### Interior fit-out refurbishment period

The length of time over which a majority of the interior fit out will be replaced.

### Hardscape specification

The specification of the pervious and impervious surfaces on the building site (outside the building envelope. These specification levels do not describe specific materials or assemblies. Instead, they approximate the 80th, 50th, and 20th percentile of the distribution of all hardscape assemblies based on a set of standard details.&#x20;

<details>

<summary>Hardscape Specification Options</summary>

* **Conservative.** 80th percentile of GWP for hardscape assemblies.&#x20;

<!---->

* **Best practices.** 50th percentile of GWP for hardscape assemblies.&#x20;

<!---->

* **Low-carbon.** 20th percentile of GWP for hardscape assemblies.&#x20;

</details>

| Assembly      | Low Carbon    | Best Practices | Conservative  |
| ------------- | ------------- | -------------- | ------------- |
| **Hardscape** | 4.4 kgCO2e/sf | 5.9 kgCO2e/sf  | 7.2 kgCO2e/sf |

#### Hardscape refurbishment period

The length of time over which a majority of the site's hardscape will be replaced.

### MEP and PV Specification

Embodied carbon in mechanical systems in evaluated at two specification levels—standard performance and high performance—and is dependent of the total square footage of the building. This approach, and the data used in EPIC, follow from the CLF study on building mechanical systems.&#x20;

Base case buildings in EPIC are always assumed to have a standard performance system. Scenarios that achieve an EUI reduction of more than 50% the benchmark are assumed to have a high performance system. The EUI reduction threshold is not directly editable in the public-facing web app, but can be redefined in the API.&#x20;

_Embodied carbon in MEP is a data-scarce category, and we cannot confidently describe the potential to reduce embodied carbon in MEP systems through specification. Accordingly, only a "conservative" option is available._&#x20;

#### MEP and PV Refurbishment Period

The length of time over which a majority of the building systems will be replaced.

##

## Refrigerant Emissions

#### Refrigerant Charge

The reduction of the total quantity of refrigerants used in the buildings HVAC+R system.&#x20;

<table><thead><tr><th width="469">Specification Level</th><th>kg refrigerants per 1000 sf</th></tr></thead><tbody><tr><td>Conservative</td><td>8.36</td></tr><tr><td>Best Practices </td><td>4.66</td></tr><tr><td>Low Carbon</td><td>1.86</td></tr></tbody></table>

#### Refrigerant Specification

The  average global warming potential (GWP) of refrigerants used in the buildings HVAC+R system.

| Specification Level | Reference Refrigerant(s) | GWP Value |
| ------------------- | ------------------------ | --------- |
| Standard            | 60% R-410a; 40% R-134    | **1675**  |
| Lower Carbon        | R-513                    | **573**   |
| Lowest Carbon       | R-123                    | **79**    |

## Site and Landscape

This set of measures describes potential carbon storage in the landscape as well as annual emissions associated with the landscape's upkeep.

#### Convert hardscape area to planted area

Converts hardscape area to planted area, up to the maximum of site area less building footprint.&#x20;

#### Carbon Storing Landscape

Definition of the proportion of total planted area that is low, moderate, or high carbon storage.

* **Low carbon storage planted area.** Example of a low carbon storage landscape is no-mow turfgrass or other herbaceous perennials. This is the assumption for all planted areas in the base case.
* **High carbon storage planted area.** An example of a high carbon storage landscape is one composed of dense broadleaf shrubs and trees in a matrix of no-mow turfgrass or herbaceous perennials.

## Planted Roof

#### Planted roof area

The percentage of roof area planted.

#### Planted roof specification

There are two levels of specification available in EPIC for green roofs.&#x20;

* **Low Carbon Storage (extensive).** An extensive green roof has a thin layer of soil that can only support shallowly rooted plants. An example of an extensive green roof is sedum mat or low turfgrass.
* **High Carbon Storage (intensive).** An intensive green roof has a deeper layer of soil that can support plants such as larger perennial grasses and small shrubs.

