# Embodied Carbon

The overview of how EPIC calculated embodied carbon is detailed on the [model structure](carbon-reduction-measures.md) page. Below, we give additional detail about how EPIC calculates emissions from all the assemblies and processes counted as part of a project's embodied carbon.&#x20;

Every attempt has been made to ensure that EPIC's results describe a typical building (i.e. a building similar to those in our database) whose characteristics match those you enter in the tool. However, unreported characteristics may make a particular building atypical in ways that it is beyond the scope of EPIC to describe. For instance, the use of particularly high-carbon and high-cost finish materials (e.g., a building where all the millwork is in gold leaf) is not covered by EPIC. It is impossible to pre-emptively describe all cases where EPIC might deviate from a particular building (the possibilities are literally endless) but, as your project progresses, we recommend that your project team stay aware of potential whole carbon implication of a project's idiosyncrasies.

### Embodied Carbon in Building Structure

Embodied carbon in building structure is calculated in two stages: a bill of structural materials is estimated and carbon intensities are applied to those materials.&#x20;

EPIC's estimation of embodied carbon in a building's structure is modeled based on statistical analysis of completed buildings. This approach is preferable to a first-principles approach—i.e. assuming an optimized structural grid for a given geometry—because it greatly reduces truncation error and better describes the variation present in real buildings.&#x20;

#### Calculating a Bill of Materials

EPIC uses a set of statistical regression models to estimate quantities of major structural materials in typical buildings. These models were trained from an EHDD database of structural quantities in completed buildings assembled from internal and public sources.&#x20;

Input data was weighted by trustworthiness to minimize incomplete or spurious data from having too large an affect on our models. Validated data was given a full weight, incomplete data weighted at 50%, and poorly documented or partially modeled data at 30%.&#x20;

There are nine materials currently modeled in EPIC:

* Concrete, 3-4 kSI
* Concrete, 5-6 kSI
* Concrete, 7-10 kSI
* Reinforcing Steel
  * Reinforcing steel is modeled in proportion to concrete quantity (kg steel / m3 concrete).
* Structural Steel
* Steel Deck
* Lumber
* Plywood
* Engineered Wood Products

A statistical model is trained for each structural material in each structural system. These models are trained on four predictors:

* Use category (one-hot encoded)
* Total GFA
* Number of floors
* GFA/floor

Where the model explains more than 70% of variation in the underlying data, it is included in EPIC and the model-specific uncertainty value is included in the uncertainty calculation. Where the model explains less than 70% of the variation in the underlying data, a per-area measure of center is included in EPIC and the uncertainty is the standard error of the sample. When the model uncertainty is large but the predicted quantities very small (i.e. engineered wood in a steel building), the quantity is assumed to be zero.&#x20;

These methods for calculating a structural bill of materials have been reviewed by colleagues at [MKA](https://www.mka.com/) and [Carbon Leadership Forum](https://carbonleadershipforum.org/), with additional comment from collaborators at [Arup](https://www.arup.com/). If you are a structural engineer interested in providing further review of our models, [please reach out](mailto:epic@ehdd.com?subject=Review).&#x20;

#### Carbon Intensities of Structural Materials

**Carbon intensity is the amount of CO2-equivalent emissions per unit of material**. For structural materials, carbon intensity information is drawn from a variety of sources. These sources are documented in the [Reference Data Sources](../backmatter/data-sources.md) section of this guide.&#x20;

The three specifications available in EPIC—low carbon, best practices, and conservative—correspond to the 20th, 50th, and 80th percentile of emissions for that material. These estimates _do not_ correspond to a specific EPD, as there are many options for achieving a certain level of performance. Most carbon intensities for structural materials in EPIC are national averages, as material supply chains for major structural materials are typically national (or global) in coverage.&#x20;

Concrete emissions, on the other hand, as assessed at the zip code level. Concrete is a regional material, rarely traveling more than 25 miles between production and use. Additionally, the relatively large number of concrete EPDs available in the United States ([80,000+](https://buildingtransparency.org/ec3) at time of writing) supports a regional approach to measuring concrete emissions.&#x20;

Where concrete EPDs are not available, the specification levels in EPIC are set using NRMCA published minimum, average, and maximum values in line with the method outlined in the CLF's [2021 Material Baseline Report](https://carbonleadershipforum.org/2021-material-baseline-report/), included the use of the uncertainty method put forward by Building Transparency.

In locations where concrete EPDs are available, EPIC sets the specification levels for concrete by sampling the distribution of GWP values from available concrete EPDs at the 20th, 50th, and 80th percentile. Data on concrete are queried via the [OpenEPD API](https://openepd.buildingtransparency.org/) and compiled in a GIS.&#x20;

<figure><img src="../.gitbook/assets/concrete regionalization-01.png" alt=""><figcaption><p>EPD regionalization. Note that EPDs are typically concentrated in metro areas, and the background NRMCA data for that region may have either a higher or a lower carbon intensity. </p></figcaption></figure>

### Embodied Carbon in Building Assembles

Building assemblies in EPIC are evaluated on a per-area basis.&#x20;

#### Embodied Carbon in the Building Envelope

The building envelope in divided into three components: opaque cladding, glazing, and roofing. The area of each is calculated based on user inputs for building floor area, number of floors, floor-to-floor height window-to-wall ratio (WWR), and building perimeter. EPIC makes a preliminary estimate of floor-to-floor height, WWR, and building perimeter (assuming a square building) which the user can refine in the "overrides" panel in the base case tab.&#x20;

$$
Envelope  \ area = Perimeter \ * \ Floor  \ Height \ * \ Number  \ of \ floors
$$

$$
Glazing  \ area = WWR \ * \ Perimeter \ * \ Floor  \ Height \ * \ Number  \ of \ floors
$$

$$
Cladding  \ area = (1-WWR) \ * \ Perimeter \ * \ Floor  \ Height \ * \ Number  \ of \ floors
$$

$$
Roof  \ area = Above \ Ground \ Floor \ Area
$$

For each of the three envelope categories, the carbon intensity is determined by sampling the distribution of GWP values from typical assemblies at the 20th, 50th, and 80th percentile.&#x20;

#### Embodied Carbon in Interior Fit Out



#### Embodied Carbon in MEP



#### Embodied Carbon in Solar Photovoltaic Arrays



#### Embodied Carbon in Hardscape



#### Emissions from Landscape Maintenance





