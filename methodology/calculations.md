# Embodied Carbon

The overview of how EPIC calculated embodied carbon is detailed on the [model structure](carbon-reduction-measures.md) page. Below, we give additional detail about how EPIC calculates emissions from all the assemblies and processes counted as part of a project's embodied carbon.&#x20;

Every attempt has been made to ensure that EPIC's results describe a typical building (i.e. a building similar to those in our database) whose characteristics match those you enter in the tool. However, unreported characteristics may make a particular building atypical in ways that it is beyond the scope of EPIC to describe. For instance, the use of particularly high-carbon and high-cost finish materials (e.g., a building where all the millwork is in gold leaf) is not covered by EPIC. It is impossible to pre-emptively describe all cases where EPIC might deviate from a particular building (the possibilities are literally endless) but, as your project progresses, we recommend that your project team stay aware of potential whole carbon implication of a project's idiosyncrasies.

### Embodied Carbon in Building Structure

Embodied carbon in building structure is calculated in two stages: a bill of structural materials is estimated and carbon intensities are applied to those materials.&#x20;

#### Calculating a Bill of Materials

EPIC uses a set of statistical regression models to estimate quantities of major structural materials in typical buildings. These models were trained from an EHDD database of data from multiple sources. Input data was weighted by trustworthiness to prevent incomplete or spurious data from having too large an affect on our models.&#x20;

A model is trained for each structural material in each structural system. These models are trained on four predictors:

* Use category (one-hot encoded)
* Total GFA
* Number of floors
* GFA/floor

Where the model explains more than 70% of variation in the underlying data, it is included in EPIC and the model-specific uncertainty value is included in the uncertainty calculation. Where the model explains less than 70% of the variation in the underlying data, a per-area measure of center is included in EPIC and the uncertainty is the standard error of the sample.&#x20;

These methods for calculating a structural bill of materials have been reviewed by colleagues at [MKA](https://www.mka.com/) and [Carbon Leadership Forum](https://carbonleadershipforum.org/), with additional comment from collaborators at [Arup](https://www.arup.com/). If you are a structural engineer interested in providing further review of our models, [please reach out](mailto:epic@ehdd.com?subject=Review).&#x20;

#### Carbon Intensities of Structural Materials



### Embodied Carbon in the Envelope



### Embodied Carbon in Interior Fit Out



### Embodied Carbon in MEP



### Embodied Carbon in Solar Photovoltaic Arrays



### Embodied Carbon in Hardscape



### Emissions from Landscape Maintenance





