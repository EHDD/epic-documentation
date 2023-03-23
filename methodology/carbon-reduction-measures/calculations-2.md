# Stored and Avoided Carbon

The overview of how EPIC calculated stored and avoided carbon is detailed on the [model structure](../carbon-reduction-measures.md#calculating-operational-carbon) page. Below, we give additional detail about how EPIC calculates emissions from all the sources contributing to a project's stored and avoided carbon.

## Biogenic Carbon

Living systems present a particular challenge for carbon emission accounting. Static emission factors are sufficient for manmade or mineral materials, but biogenic materials—those materials, such as forest products, originating from living systems—can’t be as easily summarized. Through photosynthesis, living materials remove carbon from the atmosphere as they grow; the removal of carbon dioxide from the atmosphere and its storage in biogenic materials is called referred to in EPIC as "carbon storage." But there are also emissions associated with the processing and maintenance of biogenic materials. And, eventually, biogenic materials are stored in landfills where they continue to store carbon, are recycled, or are combusted for energy and release their stored carbon back into the atmosphere.

### Carbon storage in timber

To account for the life cycle emissions of biogenic materials including carbon storage, EPIC follows the recent guidance of the American Center for Life Cycle Assessment (ACLCA) in accounting for their carbon emissions (see citation in Data and References). This guidance is applied to accounting for the biogenic carbon in forest products (lumber, plywood, and mass timber assemblies) as well as to biogenic carbon stored in the landscape. To understand the tradeoffs in biogenic materials, life cycle stages for the end-of-life of biogenic materials are counted upfront, even if they aren’t included for other products.

Once calculated, the emissions and carbon storage associated with biogenic structural materials are accounted for at the beginning of the project.&#x20;

In EPIC, this has a few ramifications:

* **The carbon emitted in the production of biogenic materials is accounted separately from stored biogenic carbon**. The carbon emissions related to material production (arising from processes such as the use of machinery and transportation) are counted as embodied carbon.
* **Carbon storage in lumber, plywood, and mass timber assemblies can only be counted if those materials are sourced from responsibly managed forests**. Practically, this can mean a number of things. In the rule's widest interpretation, timber from any forest whose area is expanding can contribute to carbon storage—a definition that leaves many important questions unresolved. One way to determine whether a forest is responsibly managed is to determine if it has a third-party certification for sustainable forestry practices, such as that offered by the Forest Stewardship Council (FSC).
* **EPIC assumes that lumber, plywood, and mass timber assemblies are landfilled, recycled, or combusted for energy at the end of their useful life**. The mix of landfilling, combustion, and recycling is determined by the EPA analysis of US disposal in 2018. The emissions from these three activities are calculated with the EPA’s Waste Reduction Model (v15).

### Carbon storage in landscapes and green roofs

EPIC measures the annual carbon storage of in living and growing landscape. We assume that all plantings will achieve maturity across the building project's reference period. Carbon storage in the landscape is accrued year over year by amortizing the total carbon storage in mature landscapes over the model's reference period.&#x20;

Globally, the storage of carbon in plants is a major carbon sink. There are a number of imperatives for greening our built environment—such as [addressing a history of racist redlining](https://ehp.niehs.nih.gov/doi/full/10.1289/EHP7495), [reducing urban heat island](https://www.sciencedirect.com/science/article/abs/pii/S1618866718306411), or [contributing to mental wellness](https://www.sciencedirect.com/science/article/abs/pii/S0033350613002862)—that add positive co-benefits to the carbon storage potential of green space.&#x20;

In EPIC, landscaped area is assumed to approach its maximum storage potential over a 30 year period. The amount of carbon that a landscape can store is location-dependent (i.e., a landscape in Miami can store more carbon than one of a similar size in Arizona). Maintaining carbon storage in landscape requires maintenance. Emissions from the maintenance of carbon-storing landscape are assessed as embodied emissions. The storage potential of a landscape or green roof depends on its area, its specification (low, moderate, or high storage), and the location of the project.&#x20;

Note that there is no option in EPIC to describe turfgrass, as turfgrass is a net emitter.

## Avoided carbon from surplus energy generation

Once production from an onsite solar array has zero'ed out annual electricity use, EPIC assumes all additional energy generated by the array displaces generation of electricity by the electrical grid. The avoided emissions from surplus onsite energy generation are calculated as the emissions that this displaced energy would have incurred.&#x20;

This method assumes that there is no curtailment of PV production, and that the carbon emissions of grid electricity when solar energy is produced is substantially similar to the annual average emissions. In locations with a high proportion of solar on the grid, _these assumptions will not hold_ and skepticism of EPIC's calculation of avoided emissions is warranted. Read more about curtailment in [this publication ](https://www.nrel.gov/docs/fy14osti/60983.pdf)(pdf) from there National Renewable Energy Laboratory.&#x20;

The assumption of displacement generation will not hold true in all locations, and some skepticism of this estimate is encouraged. Two interrelated situations where EPIC's assumptions of displaced generation will not hold are when:

* Daytime (i.e., when solar is available) emissions from the electrical grid are significantly lower than the national average.
* Surplus energy generation is expected to be curtailed by the utility.  For an overview of curtailment in the United States, we recommend [this report from NREL](https://www.nrel.gov/docs/fy14osti/60983.pdf) (pdf).

If you are interested in further analysis of hourly emissions, [please reach out](mailto:epic@ehddd.com).&#x20;
